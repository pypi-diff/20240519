# Comparing `tmp/patchworklib-0.6.3-py3-none-any.whl.zip` & `tmp/patchworklib-0.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 48251 bytes, number of entries: 9
--rw-r--r--  2.0 unx       50 b- defN 23-Oct-23 11:25 patchworklib/__init__.py
--rw-r--r--  2.0 unx    19093 b- defN 23-Oct-23 11:03 patchworklib/modified_grid.py
--rw-r--r--  2.0 unx     2677 b- defN 23-May-16 06:03 patchworklib/modified_plotnine.py
--rw-r--r--  2.0 unx   135804 b- defN 23-Oct-23 11:56 patchworklib/patchworklib.py
--rw-r--r--  2.0 unx    35147 b- defN 23-Oct-23 11:56 patchworklib-0.6.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    24536 b- defN 23-Oct-23 11:56 patchworklib-0.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-23 11:56 patchworklib-0.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Oct-23 11:56 patchworklib-0.6.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      756 b- defN 23-Oct-23 11:56 patchworklib-0.6.3.dist-info/RECORD
-9 files, 218168 bytes uncompressed, 46949 bytes compressed:  78.5%
+Zip file size: 48543 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       50 b- defN 23-Dec-07 16:44 patchworklib/__init__.py
+-rw-r--r--  2.0 unx    19093 b- defN 23-Dec-07 16:20 patchworklib/modified_grid.py
+-rw-r--r--  2.0 unx     2904 b- defN 23-Dec-07 16:30 patchworklib/modified_plotnine.py
+-rw-r--r--  2.0 unx   136143 b- defN 24-May-19 14:09 patchworklib/patchworklib.py
+-rw-r--r--  2.0 unx    35147 b- defN 24-May-19 14:21 patchworklib-0.6.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    24844 b- defN 24-May-19 14:21 patchworklib-0.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-19 14:21 patchworklib-0.6.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-19 14:21 patchworklib-0.6.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      756 b- defN 24-May-19 14:21 patchworklib-0.6.4.dist-info/RECORD
+9 files, 219042 bytes uncompressed, 47241 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: patchworklib/modified_plotnine.py
 Comment: 
 
 Filename: patchworklib/patchworklib.py
 Comment: 
 
-Filename: patchworklib-0.6.3.dist-info/LICENSE
+Filename: patchworklib-0.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: patchworklib-0.6.3.dist-info/METADATA
+Filename: patchworklib-0.6.4.dist-info/METADATA
 Comment: 
 
-Filename: patchworklib-0.6.3.dist-info/WHEEL
+Filename: patchworklib-0.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: patchworklib-0.6.3.dist-info/top_level.txt
+Filename: patchworklib-0.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: patchworklib-0.6.3.dist-info/RECORD
+Filename: patchworklib-0.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## patchworklib/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .patchworklib import *
-__version__ = "0.6.3"
+__version__ = "0.6.4"
```

## patchworklib/modified_plotnine.py

```diff
@@ -30,15 +30,22 @@
     # assign a default theme
     self = deepcopy(self)
     
     with plot_context(self, show=show):
         self._build()
 
         # setup
-        figure, axs = self._create_figure()
+        #figure, axs = self._create_figure()
+        import matplotlib.pyplot as plt
+        figure = plt.figure()
+        axs = self.facet.make_axes(
+            figure, self.layout.layout, self.coordinates
+        )
+        self.figure = figure 
+        self.axs = axs
         self._setup_parameters()
         self.theme.setup()
         self.facet.strips.generate()
 
         # Drawing
         self._draw_layers()
         self._draw_breaks_and_labels()
```

## patchworklib/patchworklib.py

```diff
@@ -17,26 +17,25 @@
 import plotnine
 
 from contextlib import suppress
 from types import SimpleNamespace as NS
 from matplotlib.offsetbox import AnchoredOffsetbox
 from matplotlib.transforms import Bbox, TransformedBbox, Affine2D
 
-
 try:
     import patchworklib.modified_plotnine as mp9
     import patchworklib.modified_grid as mg
     import seaborn as sns
 except Exception as e:
     print(e) 
 
 #warnings.simplefilter('ignore', SettingWithCopyWarning)
 warnings.simplefilter('ignore')
 
-__version__     = "0.6.3" 
+__version__     = "0.6.4" 
 _basefigure     = plt.figure(figsize=(1,1))
 _render         = _basefigure.canvas.get_renderer()
 _scale          = Affine2D().scale(1./_basefigure.dpi)
 _axes_dict      = {}
 _removed_axes   = {}
 _bricks_list    = [] 
 basefigure      = _basefigure
@@ -207,15 +206,14 @@
             del bricks._seaborn_legend[0]["bbox_to_anchor"] 
         bricks._case.legend(handles, labels, **bricks._seaborn_legend[0], title=title, bbox_to_anchor=bricks._seaborn_legend[1])
 
     else:
         pass
 
 def overwrite_plotnine():
-    import plotnine
     plotnine.ggplot.draw = mp9.draw
 
 def load_ggplot(ggplot=None, figsize=None):  
     """
 
     Convert a plotnine plot object to a patchworklib.Bricks object.
 
@@ -397,30 +395,30 @@
         try:
             fontsize = get_property('plot_title', 'size')
         except KeyError:
             fontsize = float(rcParams.get('font.size', 12))
         
         try:
             ha = get_property('plot_title', 'ha')
-            mx0, mx1, my0, my1 = bricks.get_middle_corner() 
+            mx0, mx1, my0, my1 = bricks.get_outer_corner() 
             ix0, ix1, iy0, iy1 = bricks.get_inner_corner() 
 
             if ha == "left":
                 x = (ix0-mx0)/abs(mx1-mx0) 
                 
             elif ha == "right": 
                 x = (ix1-mx0)/abs(mx1-mx0) 
             
             elif ha == "center":
                 x = (((ix0-mx0) + (ix1-mx0))/2)/abs(mx1-mx0) 
 
             else:
                 x  = ha      
                 ha = "center"
-
+        
         except KeyError:
             ha = 0.5
         
         try:
             va = get_property('plot_title', 'va')
         except KeyError:
             va = "center" 
@@ -449,19 +447,16 @@
                 gori.theme.themeables['plot_title'].apply_ax(ax)
         else:
             gori.figure._themeable['plot_title'] = text
             gori.theme.themeables['plot_title'].apply_figure(gori.figure)
             for ax in gori.axs:
                 gori.theme.themeables['plot_title'].apply(ax)
         
-    import plotnine
     plotnine_version = plotnine.__version__
-    if StrictVersion(plotnine_version) >= StrictVersion("0.12"):
-        overwrite_plotnine()
-
+    
     #save_original_position
     global _basefigure
     global _axes_dict
     position_dict = {} 
     tmp_axes_keys = [key for key in list(_axes_dict.keys()) if type(_axes_dict[key]) == axes.Axes or _axes_dict[key]._type == "Brick"]
     for key in tmp_axes_keys:
         axtmp = _axes_dict[key] 
@@ -580,15 +575,15 @@
     else:
         raise ValueError("patchworklib does not support plotnine {}".format(plotnine_version))
 
     if len(ggplot.axs) == 1: 
         ax = Brick(ax=ggplot.axs[0])
         if "_ggplot_legend" in ax.__dict__:
             ax._ggplot_legend = None #For Google colab... 
-        ax.change_aspectratio((figsize[0], figsize[1])) 
+        ax.change_plotsize((figsize[0], figsize[1])) 
         
         if StrictVersion(plotnine_version) >= StrictVersion("0.9"):
             xl, yl = draw_labels(ax, ggplot, gcp, figsize) 
             draw_legend(ax, ggplot, gcp, figsize)
             draw_title(ax,  ggplot, gcp, figsize)
 
         elif StrictVersion("0.8") <= StrictVersion(plotnine_version) < StrictVersion("0.9"):
@@ -1546,15 +1541,14 @@
     for caselabel in brick2._case_labels:
         caselabel = caselabel[5:] 
         _reset_ggplot_legend(_axes_dict[caselabel])
 
     bricks_dict = {}
     for key in brick1_bricks_dict:
         if "outline:" == key[:len("outline:")]:
-
             pass 
         else:
             bricks_dict[key] = brick1_bricks_dict[key] 
     
     for key in brick2.bricks_dict:
         if "outline:" == key[:len("outline:")]:
             pass 
@@ -1839,15 +1833,15 @@
             fig.add_axes(ax)
         _removed_axes = {}
         
     def set_originalpositions(self):
         self._originalpositions = {}
         labels_all = set(self._labels) | set(self._case_labels)
         for label in labels_all:
-            if type(_axes_dict[label]) == Brick:
+            if type(_axes_dict[label]) == Brick: #or type(_axes_dict[label]) == axes.Axes:
                 self._originalpositions[label] = _axes_dict[label].get_inner_corner()
             else:
                 pass 
 
     def reset_label(self, name):
         """
 
@@ -1886,18 +1880,19 @@
         Parameters
         ----------
         new_size : tuple (float, float) 
 
         """
         self._comeback() 
         outers = self.get_outer_corner()  
-        expand(self, new_size[0]/abs(outers[0]-outers[1]), new_size[1]/abs(outers[3]-outers[2])) 
-        
+        expand(self.outline, new_size[0]/abs(outers[0]-outers[1]), new_size[1]/abs(outers[3]-outers[2]))  
         x0, x1, y0, y1     = self.get_outer_corner() 
         self._originalsize = (abs(x1-x0), abs(y0-y1))
+        self.set_originalpositions() 
+        self.case
 
     def align_xlabels(self, keys=None):
         global _basefigure
         global _axes_dict
         renderer = _basefigure.canvas.get_renderer()
         
         if keys is None:
@@ -2323,15 +2318,20 @@
         new_lock : str or int
             Location argument, as in matplotlib.axes.Axes.legend().
         kws : dict
             Other keyword arguments can be used in matplotlib.axes.Axes.legend().
 
         """
         old_legend = self._case.legend_
-        handles    = old_legend.legendHandles
+        
+        if (matplotlib.__version__) >= StrictVersion("3.8"):
+            handles = old_legend.legend_handles
+        else:
+            handles = old_legend.legendHandles
+
         labels     = [t.get_text() for t in old_legend.get_texts()]
         title      = old_legend.get_title().get_text()
         self._seaborn_legend[0]["loc"] = new_loc
         for key in kws:
             self._seaborn_legend[0][key] = kws[key]  
         if "bbox_to_anchor" in kws:
             self._seaborn_legend = (self._seaborn_legend[0], kws["bbox_to_anchor"])
@@ -2463,15 +2463,14 @@
         2. If the Bricks object is composed of more than a few dozens of Brick objects, 
         the methods consume a lot of times for saving the figure..., please take a coffe break.
 
         """
         for label in self._originalpositions:
             x0, x1, y0, y1 = self._originalpositions[label]
             _axes_dict[label].set_position([x0, y0, x1-x0, y1-y0])
-        
         for case_label in self._case_labels:
             _axes_dict[":".join(case_label.split(":")[1:])].case 
 
         global param
         global _basefigure
         global _removed_axes
         if quick == False:
@@ -2966,14 +2965,15 @@
         if type(new_size) ==  tuple or type(new_size) == list:
             self.set_position([0, 0, new_size[0], new_size[1]])
             self._originalsize = new_size 
         else:
             self.set_position([0, 0, 1, new_size])
             self._originalsize = (1, new_size) 
         _reset_ggplot_legend(self)
+        self.case 
     
     def change_aspectratio(self, new_size):  
         """
         
         Change figsize
         This function is deprecated.
         
@@ -2993,15 +2993,20 @@
         kws : dict
             Other keyword arguments can be used in matplotlib.axes.Axes.legend().
 
         """
         
         self._comeback()
         old_legend = self.legend_
-        handles = old_legend.legendHandles
+        
+        if (matplotlib.__version__) >= StrictVersion("3.8"):
+            handles = old_legend.legend_handles
+        else:
+            handles = old_legend.legendHandles
+
         labels = [t.get_text() for t in old_legend.get_texts()]
         title = old_legend.get_title().get_text()
         self._middle_flag = False
         self._outer_flag  = False
         self.legend(handles, labels, loc=new_loc, title=title, **kws)
     
     def __or__(self, other):
@@ -3507,8 +3512,11 @@
 
     ax12345 = (ax1 | ax2 | ax3) / (ax4 | ax5) 
     ax12345.savefig("test1.pdf")
     
     #bricks2 = (brick2 | (brick5 / brick4)) / (brick1 | brick3) 
     ax21543 = (ax2 / ax1) | (ax5 / ax4 / ax3) 
     ax21543.savefig("test2.pdf") 
-    
+ 
+if StrictVersion(plotnine.__version__) >= StrictVersion("0.12"):
+    overwrite_plotnine()
+
```

## Comparing `patchworklib-0.6.3.dist-info/LICENSE` & `patchworklib-0.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `patchworklib-0.6.3.dist-info/METADATA` & `patchworklib-0.6.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7061 7463  : 2.1.Name: patc
 00000020: 6877 6f72 6b6c 6962 0a56 6572 7369 6f6e  hworklib.Version
-00000030: 3a20 302e 362e 330a 5375 6d6d 6172 793a  : 0.6.3.Summary:
+00000030: 3a20 302e 362e 340a 5375 6d6d 6172 793a  : 0.6.4.Summary:
 00000040: 2070 6174 6368 776f 726b 2066 6f72 206d   patchwork for m
 00000050: 6174 706c 6f74 6c69 620a 486f 6d65 2d70  atplotlib.Home-p
 00000060: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000070: 6875 622e 636f 6d2f 706f 6e6e 6869 6465  hub.com/ponnhide
 00000080: 2f70 6174 6368 776f 726b 6c69 620a 446f  /patchworklib.Do
 00000090: 776e 6c6f 6164 2d55 524c 3a20 6874 7470  wnload-URL: http
 000000a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
@@ -43,1492 +43,1511 @@
 000002a0: 3320 2847 504c 7633 290a 5265 7175 6972  3 (GPLv3).Requir
 000002b0: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
 000002c0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 000002d0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 000002e0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
 000002f0: 2d46 696c 653a 204c 4943 454e 5345 0a52  -File: LICENSE.R
 00000300: 6571 7569 7265 732d 4469 7374 3a20 6d61  equires-Dist: ma
-00000310: 7470 6c6f 746c 6962 203e 3d33 2e34 0a52  tplotlib >=3.4.R
-00000320: 6571 7569 7265 732d 4469 7374 3a20 7061  equires-Dist: pa
-00000330: 6e64 6173 203e 3d30 2e32 340a 5265 7175  ndas >=0.24.Requ
-00000340: 6972 6573 2d44 6973 743a 206e 756d 7079  ires-Dist: numpy
-00000350: 203e 3d31 2e31 360a 5265 7175 6972 6573   >=1.16.Requires
-00000360: 2d44 6973 743a 2064 696c 6c0a 5265 7175  -Dist: dill.Requ
-00000370: 6972 6573 2d44 6973 743a 2073 6561 626f  ires-Dist: seabo
-00000380: 726e 0a52 6571 7569 7265 732d 4469 7374  rn.Requires-Dist
-00000390: 3a20 706c 6f74 6e69 6e65 0a0a 2320 7061  : plotnine..# pa
-000003a0: 7463 6877 6f72 6b6c 6962 0a5b 5061 7463  tchworklib.[Patc
-000003b0: 6877 6f72 6b6c 6962 5d28 6874 7470 733a  hworklib](https:
-000003c0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6f6e  //github.com/pon
-000003d0: 6e68 6964 652f 7061 7463 6877 6f72 6b6c  nhide/patchworkl
-000003e0: 6962 2920 6973 2061 2075 6e69 7665 7273  ib) is a univers
-000003f0: 616c 2063 6f6d 706f 7365 7220 6f66 206d  al composer of m
-00000400: 6174 706c 6f74 6c69 622d 7265 6c61 7465  atplotlib-relate
-00000410: 6420 706c 6f74 7320 2873 696d 706c 6520  d plots (simple 
-00000420: 6d61 7470 6c6f 746c 6962 2070 6c6f 7473  matplotlib plots
-00000430: 2c20 5365 6162 6f72 6e20 706c 6f74 7320  , Seaborn plots 
-00000440: 2862 6f74 6820 6178 6973 2d6c 6576 656c  (both axis-level
-00000450: 2061 6e64 2066 6967 7572 652d 6c65 7665   and figure-leve
-00000460: 6c29 2c20 616e 6420 706c 6f74 6e69 6e65  l), and plotnine
-00000470: 2070 6c6f 7473 292e 2054 6869 7320 6c69   plots). This li
-00000480: 6272 6172 7920 6973 2069 6e73 7069 7265  brary is inspire
-00000490: 6420 6279 205b 7061 7463 6877 6f72 6b5d  d by [patchwork]
-000004a0: 2868 7474 7073 3a2f 2f70 6174 6368 776f  (https://patchwo
-000004b0: 726b 2e64 6174 612d 696d 6167 696e 6973  rk.data-imaginis
-000004c0: 742e 636f 6d2f 2920 666f 7220 6767 706c  t.com/) for ggpl
-000004d0: 6f74 322e 2041 6363 6f72 6469 6e67 6c79  ot2. Accordingly
-000004e0: 2c20 6173 206f 7269 6769 6e61 6c20 7061  , as original pa
-000004f0: 7463 6877 6f72 6b2c 2075 7365 7273 2063  tchwork, users c
-00000500: 616e 2065 6173 696c 7920 616c 6967 6e20  an easily align 
-00000510: 6d61 7470 6c6f 746c 6962 2070 6c6f 7473  matplotlib plots
-00000520: 2077 6974 6820 6f6e 6c79 2022 2f22 2061   with only "/" a
-00000530: 6e64 2022 7c22 206f 7065 7261 746f 7273  nd "|" operators
-00000540: 2e20 416c 7468 6f75 6768 2061 2067 6f6f  . Although a goo
-00000550: 6420 7375 6270 6c6f 7420 636f 6d70 6f73  d subplot compos
-00000560: 6572 2c20 2273 7562 706c 6f74 5f6d 6f73  er, "subplot_mos
-00000570: 6169 6322 2069 7320 7072 6f76 6964 6564  aic" is provided
-00000580: 2066 726f 6d20 6d61 7470 6c6f 746c 6962   from matplotlib
-00000590: 2066 6f72 6d61 6c6c 792c 2049 2062 656c   formally, I bel
-000005a0: 6965 7665 2074 6865 2077 6179 206f 6620  ieve the way of 
-000005b0: 7061 7463 6877 6f72 6b6c 6962 2069 7320  patchworklib is 
-000005c0: 6d6f 7265 2073 7472 6169 6768 7466 6f72  more straightfor
-000005d0: 7761 7264 2061 6e64 206d 6f72 6520 666c  ward and more fl
-000005e0: 6578 6962 6c65 2e0a 0a41 6464 6974 696f  exible...Additio
-000005f0: 6e61 6c6c 792c 2073 6576 6572 616c 2074  nally, several t
-00000600: 6869 7264 2d70 6172 7479 206c 6962 7261  hird-party libra
-00000610: 7269 6573 2062 6173 6564 206f 6e20 6d61  ries based on ma
-00000620: 7470 6c6f 746c 6962 2c20 7375 6368 2061  tplotlib, such a
-00000630: 7320 706c 6f74 6e69 6e65 2061 6e64 2073  s plotnine and s
-00000640: 6561 626f 726e 2c20 7072 6f76 6964 6520  eaborn, provide 
-00000650: 6675 6e63 7469 6f6e 7320 746f 2067 656e  functions to gen
-00000660: 6572 6174 6520 6265 6175 7469 6675 6c20  erate beautiful 
-00000670: 706c 6f74 7320 7769 7468 2073 696d 706c  plots with simpl
-00000680: 6520 7079 7468 6f6e 2063 6f64 6573 2c20  e python codes, 
-00000690: 6275 7420 6d61 6e79 206f 6620 7468 6f73  but many of thos
-000006a0: 6520 706c 6f74 7320 6361 6e6e 6f74 2062  e plots cannot b
-000006b0: 6520 6861 6e64 6c65 6420 6173 206d 6174  e handled as mat
-000006c0: 706c 6f74 6c69 6220 7375 6270 6c6f 7473  plotlib subplots
-000006d0: 2e20 5468 6572 6566 6f72 652c 2074 6865  . Therefore, the
-000006e0: 6972 2070 6c61 6365 6d65 6e74 206d 7573  ir placement mus
-000006f0: 7420 6265 2061 646a 7573 7465 6420 6d61  t be adjusted ma
-00000700: 6e75 616c 6c79 2e20 4e6f 772c 2073 6369  nually. Now, sci
-00000710: 656e 7469 7374 7320 7370 656e 6420 7468  entists spend th
-00000720: 6569 7220 7661 6c75 6162 6c65 2074 696d  eir valuable tim
-00000730: 6520 6172 7261 6e67 696e 6720 6669 6775  e arranging figu
-00000740: 7265 732e 0a0a 5061 7463 6877 6f72 6b6c  res...Patchworkl
-00000750: 6962 2070 726f 7669 6465 7320 6120 736f  ib provides a so
-00000760: 6c75 7469 6f6e 2066 6f72 2074 6865 2070  lution for the p
-00000770: 726f 626c 656d 2e20 4279 2075 7369 6e67  roblem. By using
-00000780: 2070 6174 6368 776f 726b 6c69 622c 2061   patchworklib, a
-00000790: 6e79 206b 696e 6420 6f66 2073 6561 626f  ny kind of seabo
-000007a0: 726e 2061 6e64 2070 6c6f 746e 696e 6520  rn and plotnine 
-000007b0: 706c 6f74 7320 6361 6e20 6265 2068 616e  plots can be han
-000007c0: 646c 6564 2061 7320 6d61 7470 6c6f 746c  dled as matplotl
-000007d0: 6962 2073 7562 706c 6f74 732e 0a0a 2323  ib subplots...##
-000007e0: 2049 6e73 7461 6c6c 6174 696f 6e0a 466f   Installation.Fo
-000007f0: 7220 6e6f 726d 616c 2075 7365 7273 2c20  r normal users, 
-00000800: 7765 2072 6563 6f6d 6d65 6e64 6564 2079  we recommended y
-00000810: 6f75 2074 6f20 696e 7374 616c 6c20 7468  ou to install th
-00000820: 6520 6f66 6669 6369 616c 2072 656c 6561  e official relea
-00000830: 7365 2061 7320 666f 6c6c 6f77 732e 2020  se as follows.  
-00000840: 0a60 7069 7020 696e 7374 616c 6c20 7061  .`pip install pa
-00000850: 7463 6877 6f72 6b6c 6962 600a 0a49 6620  tchworklib`..If 
-00000860: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
-00000870: 6465 7665 6c6f 706d 656e 7461 6c20 7665  developmental ve
-00000880: 7273 696f 6e2c 2069 7420 6361 6e20 6265  rsion, it can be
-00000890: 2069 6e73 7461 6c6c 6564 2075 7369 6e67   installed using
-000008a0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
-000008b0: 696e 676c 6520 636f 6d6d 616e 643a 2020  ingle command:  
-000008c0: 0a60 7069 7020 696e 7374 616c 6c20 6769  .`pip install gi
-000008d0: 742b 6874 7470 733a 2f2f 6769 7468 7562  t+https://github
-000008e0: 2e63 6f6d 2f70 6f6e 6e68 6964 652f 7061  .com/ponnhide/pa
-000008f0: 7463 6877 6f72 6b6c 6962 2e67 6974 600a  tchworklib.git`.
-00000900: 0a23 2320 4e65 7773 0a23 2323 2320 3130  .## News.#### 10
-00000910: 3233 3230 3233 3a20 7665 7273 696f 6e20  232023: version 
-00000920: 302e 362e 3320 6973 2072 656c 6561 7365  0.6.3 is release
-00000930: 642e 200a 2d20 5365 6162 6f72 6e20 7630  d. .- Seaborn v0
-00000940: 2e31 332e 3020 6973 206e 6f77 2073 7570  .13.0 is now sup
-00000950: 706f 7274 6564 2e0a 2d20 4920 6861 7665  ported..- I have
-00000960: 2063 6f6e 6669 726d 6564 2070 6174 6368   confirmed patch
-00000970: 776f 726b 6c69 6220 7374 696c 6c20 776f  worklib still wo
-00000980: 726b 7320 666f 7270 6c6f 746e 696e 6520  rks forplotnine 
-00000990: 7630 2e31 322e 332e 200a 0a23 2323 2320  v0.12.3. ..#### 
-000009a0: 3035 3136 3230 3233 3a20 7665 7273 696f  05162023: versio
-000009b0: 6e20 302e 362e 3120 7761 7320 7265 6c65  n 0.6.1 was rele
-000009c0: 6173 6564 2e0a 2d20 4920 636f 756c 6420  ased..- I could 
-000009d0: 6e6f 7420 6675 6c6c 7920 7375 7070 6f72  not fully suppor
-000009e0: 7420 706c 6f74 6e69 6e65 2076 6572 7369  t plotnine versi
-000009f0: 6f6e 2030 2e31 322e 3120 2849 7420 776f  on 0.12.1 (It wo
-00000a00: 726b 732c 2062 7574 2070 6174 6368 776f  rks, but patchwo
-00000a10: 726b 6c69 6220 6172 7261 6e67 656d 656e  rklib arrangemen
-00000a20: 7420 7265 7375 6c74 7320 6172 6520 6e6f  t results are no
-00000a30: 7420 6173 2065 7870 6563 7465 6429 2e20  t as expected). 
-00000a40: 4d61 7962 652c 2049 2077 696c 6c20 646f  Maybe, I will do
-00000a50: 206e 6f74 2073 7570 706f 7274 2070 6c6f   not support plo
-00000a60: 746e 696e 6520 696e 2074 6865 2066 7574  tnine in the fut
-00000a70: 7572 652e 200a 2d20 4272 6963 6b73 206f  ure. .- Bricks o
-00000a80: 626a 6563 7420 6761 696e 6564 2074 6865  bject gained the
-00000a90: 206e 6577 206d 6574 686f 6473 2060 616c   new methods `al
-00000aa0: 6967 6e5f 786c 6162 656c 7360 2061 6e64  ign_xlabels` and
-00000ab0: 2020 6061 6c69 676e 5f79 6c61 6265 6c73    `align_ylabels
-00000ac0: 602c 2077 6869 6368 2068 656c 7020 7573  `, which help us
-00000ad0: 6572 7320 616c 6967 6e20 782f 7920 6c61  ers align x/y la
-00000ae0: 6265 6c73 206f 6620 7468 6520 6769 7665  bels of the give
-00000af0: 6e20 4272 6963 6b20 6f62 6a65 6374 2e0a  n Brick object..
-00000b00: 2d20 5468 6520 6e65 7720 6172 6775 6d65  - The new argume
-00000b10: 6e74 2060 6571 7561 6c5f 7370 6163 696e  nt `equal_spacin
-00000b20: 6760 2077 6173 2061 6464 6564 2074 6f20  g` was added to 
-00000b30: 7468 6520 7374 6163 6b20 6675 6e63 7469  the stack functi
-00000b40: 6f6e 2e20 4966 2074 6869 7320 7661 6c75  on. If this valu
-00000b50: 6520 6973 2060 5472 7565 602c 2061 7865  e is `True`, axe
-00000b60: 7320 626f 756e 6469 6e67 2d62 6f78 6573  s bounding-boxes
-00000b70: 2073 686f 756c 6420 6265 2070 6c61 6365   should be place
-00000b80: 6420 7769 7468 2065 7175 616c 2073 7061  d with equal spa
-00000b90: 6369 6e67 2062 6574 7765 656e 2074 6865  cing between the
-00000ba0: 6d2e 204f 7468 6572 7769 7365 2c20 6465  m. Otherwise, de
-00000bb0: 7065 6e64 696e 6720 6f6e 2074 6865 2074  pending on the t
-00000bc0: 6578 7420 7661 6c75 6573 206f 6620 782f  ext values of x/
-00000bd0: 7920 7469 636b 206c 6162 656c 7320 616e  y tick labels an
-00000be0: 6420 782f 7920 6c61 6265 6c73 2c20 7468  d x/y labels, th
-00000bf0: 6579 206d 6179 206e 6f74 2061 6c77 6179  ey may not alway
-00000c00: 7320 6265 2065 7175 616c 6c79 2073 7061  s be equally spa
-00000c10: 6365 642e 0a2d 2043 6c6f 7365 6420 616e  ced..- Closed an
-00000c20: 6420 6d61 7962 6520 736f 6c76 6564 2074  d maybe solved t
-00000c30: 6865 2069 7373 7565 205b 2241 6c69 676e  he issue ["Align
-00000c40: 206c 6162 656c 7320 6f66 2042 7269 636b   labels of Brick
-00000c50: 7320 7768 656e 2073 7562 706c 6f74 2061  s when subplot a
-00000c60: 7865 7320 6172 6520 616c 6967 6e65 642e  xes are aligned.
-00000c70: 2023 3430 225d 2868 7474 7073 3a2f 2f67   #40"](https://g
-00000c80: 6974 6875 622e 636f 6d2f 706f 6e6e 6869  ithub.com/ponnhi
-00000c90: 6465 2f70 6174 6368 776f 726b 6c69 622f  de/patchworklib/
-00000ca0: 6973 7375 6573 2f34 3029 200a 2d20 436c  issues/40) .- Cl
-00000cb0: 6f73 6564 2061 6e64 206d 6179 6265 2073  osed and maybe s
-00000cc0: 6f6c 7665 6420 7468 6520 6973 7375 6520  olved the issue 
-00000cd0: 5b22 446f 6573 6e27 7420 776f 726b 2077  ["Doesn't work w
-00000ce0: 6974 6820 506c 6f74 6e69 6e65 2053 6561  ith Plotnine Sea
-00000cf0: 626f 726e 2054 6865 6d65 2e20 2333 3722  born Theme. #37"
-00000d00: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000d10: 2e63 6f6d 2f70 6f6e 6e68 6964 652f 7061  .com/ponnhide/pa
-00000d20: 7463 6877 6f72 6b6c 6962 2f69 7373 7565  tchworklib/issue
-00000d30: 732f 3337 290a 2d20 436c 6f73 6564 2061  s/37).- Closed a
-00000d40: 6e64 206d 6179 6265 2073 6f6c 7665 6420  nd maybe solved 
-00000d50: 7468 6520 6973 7375 6520 5b22 5468 6520  the issue ["The 
-00000d60: 706f 7369 7469 6f6e 206f 6620 7468 6520  position of the 
-00000d70: 7469 746c 6520 6361 6e6e 6f74 2062 6520  title cannot be 
-00000d80: 7365 7420 696e 2070 6c6f 746e 696e 652e  set in plotnine.
-00000d90: 2023 3336 225d 2868 7474 7073 3a2f 2f67   #36"](https://g
-00000da0: 6974 6875 622e 636f 6d2f 706f 6e6e 6869  ithub.com/ponnhi
-00000db0: 6465 2f70 6174 6368 776f 726b 6c69 622f  de/patchworklib/
-00000dc0: 6973 7375 6573 2f33 3629 0a0a 3c64 6574  issues/36)..<det
-00000dd0: 6169 6c73 3e20 0a0a 3c73 756d 6d61 7279  ails> ..<summary
-00000de0: 3e20 3c68 323e 2043 6861 6e67 6520 6c6f  > <h2> Change lo
-00000df0: 6720 3c2f 6832 3e20 3c2f 7375 6d6d 6172  g </h2> </summar
-00000e00: 793e 0a23 2323 2320 3132 3038 3230 3232  y>.#### 12082022
-00000e10: 3a20 7665 7273 696f 6e20 302e 352e 3020  : version 0.5.0 
-00000e20: 7761 7320 7265 6c65 6173 6564 2e0a 2d20  was released..- 
-00000e30: 4e65 7720 6f70 6572 6174 6f72 732c 2022  New operators, "
-00000e40: 2b22 2061 6e64 2022 2d22 2c20 7765 7265  +" and "-", were
-00000e50: 2061 6464 6564 2e20 0a2d 2070 6c6f 746e   added. .- plotn
-00000e60: 696e 6520 3e20 7630 2e31 302e 7820 6973  ine > v0.10.x is
-00000e70: 206e 6f77 2073 7570 706f 7274 6564 2e0a   now supported..
-00000e80: 2d20 506c 6f74 7320 6765 6e65 7261 7465  - Plots generate
-00000e90: 6420 6279 206f 626a 6563 742d 6f72 6965  d by object-orie
-00000ea0: 6e74 6564 2073 6561 626f 726e 2069 6e74  nted seaborn int
-00000eb0: 6572 6661 6365 2063 616e 206e 6f77 2062  erface can now b
-00000ec0: 6520 6861 6e64 6c65 6420 6279 2070 6174  e handled by pat
-00000ed0: 6368 776f 726b 6c69 622e 0a2d 2044 6573  chworklib..- Des
-00000ee0: 6372 6970 7469 6f6e 7320 6f66 2065 6163  criptions of eac
-00000ef0: 6820 6675 6e63 7469 6f6e 2061 6e64 2063  h function and c
-00000f00: 6c61 7373 2070 726f 7669 6465 6420 696e  lass provided in
-00000f10: 2070 6174 6368 776f 726b 6c69 6220 7761   patchworklib wa
-00000f20: 7320 6164 6465 6420 746f 2074 6869 7320  s added to this 
-00000f30: 7265 706f 7369 746f 7279 2e20 4966 2079  repository. If y
-00000f40: 6f75 2077 616e 7420 746f 206b 6e6f 7720  ou want to know 
-00000f50: 686f 7720 746f 2075 7365 2070 6174 6368  how to use patch
-00000f60: 776f 726b 6c69 6220 696e 2064 6574 6169  worklib in detai
-00000f70: 6c2c 2070 6c65 6173 6520 7365 6520 5b41  l, please see [A
-00000f80: 5049 2e6d 645d 2868 7474 7073 3a2f 2f67  PI.md](https://g
-00000f90: 6974 6875 622e 636f 6d2f 706f 6e6e 6869  ithub.com/ponnhi
-00000fa0: 6465 2f70 6174 6368 776f 726b 6c69 622f  de/patchworklib/
-00000fb0: 626c 6f62 2f6d 6169 6e2f 4150 492e 6d64  blob/main/API.md
-00000fc0: 292e 0a2d 2055 7064 6174 6564 205b 7061  )..- Updated [pa
-00000fd0: 7463 6877 6f72 6b6c 6962 2d65 7861 6d70  tchworklib-examp
-00000fe0: 6c65 735d 2868 7474 7073 3a2f 2f67 6974  les](https://git
-00000ff0: 6875 622e 636f 6d2f 706f 6e6e 6869 6465  hub.com/ponnhide
-00001000: 2f70 6174 6368 776f 726b 6c69 622d 6578  /patchworklib-ex
-00001010: 616d 706c 6573 290a 0a23 2323 2320 3038  amples)..#### 08
-00001020: 3135 3230 3232 3a20 5665 7273 696f 6e20  152022: Version 
-00001030: 302e 342e 3720 7761 7320 7265 6c65 6173  0.4.7 was releas
-00001040: 6564 2e20 0a2d 2041 2066 6577 2062 7567  ed. .- A few bug
-00001050: 7320 7765 7265 2066 6978 6564 2e0a 2d20  s were fixed..- 
-00001060: 4164 6420 696e 7365 7420 6675 6e63 7469  Add inset functi
-00001070: 6f6e 2e20 706c 6561 7365 2073 6565 2074  on. please see t
-00001080: 6865 2066 6f6c 6c6f 7769 6e67 2065 7861  he following exa
-00001090: 6d70 6c65 2e20 0a2d 2041 6464 2060 6b65  mple. .- Add `ke
-000010a0: 6570 5f61 7370 6563 7460 2070 6172 616d  ep_aspect` param
-000010b0: 6574 6572 2074 6f20 6068 7374 6163 6b60  eter to `hstack`
-000010c0: 2061 6e64 2060 7673 7461 636b 6020 6675   and `vstack` fu
-000010d0: 6e63 6974 6f6e 2e0a 2d20 4578 616d 706c  nciton..- Exampl
-000010e0: 6520 636f 6465 7320 7765 7265 206d 6f76  e codes were mov
-000010f0: 6564 2074 6f20 5b70 6174 6368 776f 726b  ed to [patchwork
-00001100: 6c69 622d 6578 616d 706c 6573 5d28 6874  lib-examples](ht
-00001110: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001120: 2f70 6f6e 6e68 6964 652f 7061 7463 6877  /ponnhide/patchw
-00001130: 6f72 6b6c 6962 2d65 7861 6d70 6c65 7329  orklib-examples)
-00001140: 0a0a 3c64 6574 6169 6c73 3e20 0a3c 7375  ..<details> .<su
-00001150: 6d6d 6172 793e 2043 7265 6174 6520 616e  mmary> Create an
-00001160: 2069 6e73 6574 2065 6c65 6d65 6e74 203c   inset element <
-00001170: 2f73 756d 6d61 7279 3e0a 0a60 6060 7079  /summary>..```py
-00001180: 7468 6f6e 0a69 6d70 6f72 7420 7061 7463  thon.import patc
-00001190: 6877 6f72 6b6c 6962 2061 7320 7077 0a66  hworklib as pw.f
-000011a0: 726f 6d20 706c 6f74 6e69 6e65 2069 6d70  rom plotnine imp
-000011b0: 6f72 7420 2a0a 6672 6f6d 2070 6c6f 746e  ort *.from plotn
-000011c0: 696e 652e 6461 7461 2069 6d70 6f72 7420  ine.data import 
-000011d0: 2a0a 0a67 3120 203d 2070 772e 6c6f 6164  *..g1  = pw.load
-000011e0: 5f67 6770 6c6f 7428 6767 706c 6f74 286d  _ggplot(ggplot(m
-000011f0: 7463 6172 7329 202b 2067 656f 6d5f 706f  tcars) + geom_po
-00001200: 696e 7428 6165 7328 226d 7067 222c 2022  int(aes("mpg", "
-00001210: 6469 7370 2229 292c 6669 6773 697a 653d  disp")),figsize=
-00001220: 2834 2c20 3229 290a 6732 2020 3d20 7077  (4, 2)).g2  = pw
-00001230: 2e6c 6f61 645f 6767 706c 6f74 2867 6770  .load_ggplot(ggp
-00001240: 6c6f 7428 6d74 6361 7273 2920 2b20 6765  lot(mtcars) + ge
-00001250: 6f6d 5f62 6f78 706c 6f74 2861 6573 2822  om_boxplot(aes("
-00001260: 6765 6172 222c 2022 6469 7370 222c 2067  gear", "disp", g
-00001270: 726f 7570 203d 2022 6765 6172 2229 2920  roup = "gear")) 
-00001280: 2b20 7468 656d 655f 636c 6173 7369 6328  + theme_classic(
-00001290: 2929 0a67 3132 203d 2070 772e 696e 7365  )).g12 = pw.inse
-000012a0: 7428 6731 2c67 3229 0a67 3132 2e73 6176  t(g1,g2).g12.sav
-000012b0: 6566 6967 2829 0a60 6060 0a3c 696d 6720  efig().```.<img 
-000012c0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-000012d0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-000012e0: 6e74 2e63 6f6d 2f70 6f6e 6e68 6964 652f  nt.com/ponnhide/
-000012f0: 7061 7463 6877 6f72 6b6c 6962 2f6d 6169  patchworklib/mai
-00001300: 6e2f 696d 672f 696e 7365 745f 706c 6f74  n/img/inset_plot
-00001310: 6e69 6e65 2e70 6e67 2220 7769 6474 683d  nine.png" width=
-00001320: 2236 3030 7836 3030 223e 0a0a 6060 6070  "600x600">..```p
-00001330: 7974 686f 6e0a 6731 3220 3d20 7077 2e69  ython.g12 = pw.i
-00001340: 6e73 6574 2867 312c 6732 2c20 6c6f 633d  nset(g1,g2, loc=
-00001350: 226c 6f77 6572 206c 6566 7422 2c20 6872  "lower left", hr
-00001360: 6174 696f 3d30 2e34 2c20 7772 6174 696f  atio=0.4, wratio
-00001370: 3d30 2e32 290a 6731 322e 7361 7665 6669  =0.2).g12.savefi
-00001380: 6728 2269 6e73 6574 5f70 6c6f 746e 696e  g("inset_plotnin
-00001390: 6532 2e70 6e67 2229 0a60 6060 0a3c 696d  e2.png").```.<im
-000013a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-000013b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000013c0: 7465 6e74 2e63 6f6d 2f70 6f6e 6e68 6964  tent.com/ponnhid
-000013d0: 652f 7061 7463 6877 6f72 6b6c 6962 2f6d  e/patchworklib/m
-000013e0: 6169 6e2f 696d 672f 696e 7365 745f 706c  ain/img/inset_pl
-000013f0: 6f74 6e69 6e65 322e 706e 6722 2077 6964  otnine2.png" wid
-00001400: 7468 3d22 3630 3078 3630 3022 3e0a 0a3c  th="600x600">..<
-00001410: 2f64 6574 6169 6c73 3e0a 0a23 2323 2320  /details>..#### 
-00001420: 3038 3039 3230 3232 3a20 5665 7273 696f  08092022: Versio
-00001430: 6e20 302e 342e 3620 7761 7320 7265 6c65  n 0.4.6 was rele
-00001440: 6173 6564 2e20 0a2d 2041 2066 6577 2062  ased. .- A few b
-00001450: 7567 7320 7765 7265 2066 6978 6564 2028  ugs were fixed (
-00001460: 5365 6520 6973 7375 6520 5b23 3138 5d28  See issue [#18](
-00001470: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001480: 6f6d 2f70 6f6e 6e68 6964 652f 7061 7463  om/ponnhide/patc
-00001490: 6877 6f72 6b6c 6962 2f69 7373 7565 732f  hworklib/issues/
-000014a0: 3138 2929 2e20 2020 0a2d 2050 6c6f 7474  18)).   .- Plott
-000014b0: 696e 6720 7370 6565 6420 7761 7320 696d  ing speed was im
-000014c0: 7072 6f76 6564 2e0a 0a23 2323 2320 3037  proved...#### 07
-000014d0: 3230 3230 3232 3a20 5665 7273 696f 6e20  202022: Version 
-000014e0: 302e 342e 3520 7761 7320 7265 6c65 6173  0.4.5 was releas
-000014f0: 6564 2e20 0a2d 2041 2066 6577 2062 7567  ed. .- A few bug
-00001500: 7320 7765 7265 2066 6978 6564 2e0a 2d20  s were fixed..- 
-00001510: 4d6f 6469 6669 6564 2066 756e 6374 696f  Modified functio
-00001520: 6e73 2072 656c 6174 696e 6720 746f 2074  ns relating to t
-00001530: 6865 2069 6e68 6572 6974 616e 6365 206f  he inheritance o
-00001540: 6620 7468 6520 6767 706c 6f74 2074 6865  f the ggplot the
-00001550: 6d65 2e20 4966 2079 6f75 2075 7365 2070  me. If you use p
-00001560: 6174 6368 776f 726b 6c69 6220 666f 7220  atchworklib for 
-00001570: 6861 6e64 6c69 6e67 2070 6c6f 746e 696e  handling plotnin
-00001580: 6520 706c 6f74 732c 2070 6c65 6173 6520  e plots, please 
-00001590: 646f 2075 7064 6174 652e 0a2d 2057 6865  do update..- Whe
-000015a0: 6e20 7370 6563 6966 7969 6e67 2061 2070  n specifying a p
-000015b0: 6c6f 7420 2842 7269 636b 206f 626a 6563  lot (Brick objec
-000015c0: 7429 2069 6e20 4272 6963 6b73 206f 626a  t) in Bricks obj
-000015d0: 6563 742c 2079 6f75 2063 616e 2073 7065  ect, you can spe
-000015e0: 6369 6679 2074 6865 2042 7269 636b 206f  cify the Brick o
-000015f0: 626a 6563 7420 6469 7265 6374 6c79 2069  bject directly i
-00001600: 6e73 7465 6164 206f 6620 7468 6520 6c61  nstead of the la
-00001610: 6265 6c20 6e61 6d65 206f 6620 7468 6520  bel name of the 
-00001620: 4272 6963 6b20 6f62 6a65 6374 2e20 506c  Brick object. Pl
-00001630: 6561 7365 2073 6565 2074 6865 2066 6f6c  ease see the fol
-00001640: 6c6f 7769 6e67 2065 7861 6d70 6c65 2e20  lowing example. 
-00001650: 0a3c 6465 7461 696c 733e 200a 3c73 756d  .<details> .<sum
-00001660: 6d61 7279 3e20 416c 6967 6e6d 656e 7420  mary> Alignment 
-00001670: 6f66 2061 2070 6c6f 7469 6e65 2070 6c6f  of a plotine plo
-00001680: 7420 6279 2073 7065 6369 6679 696e 6720  t by specifying 
-00001690: 6120 4272 6963 6b20 6f62 6a65 6374 2069  a Brick object i
-000016a0: 6e20 7468 6520 4272 6963 6b73 206f 626a  n the Bricks obj
-000016b0: 6563 742e 203c 2f73 756d 6d61 7279 3e0a  ect. </summary>.
-000016c0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-000016d0: 7420 7061 7463 6877 6f72 6b6c 6962 2061  t patchworklib a
-000016e0: 7320 7077 0a66 726f 6d20 706c 6f74 6e69  s pw.from plotni
-000016f0: 6e65 2069 6d70 6f72 7420 2a0a 6672 6f6d  ne import *.from
-00001700: 2070 6c6f 746e 696e 652e 6461 7461 2069   plotnine.data i
-00001710: 6d70 6f72 7420 2a0a 0a67 3120 3d20 7077  mport *..g1 = pw
-00001720: 2e6c 6f61 645f 6767 706c 6f74 2867 6770  .load_ggplot(ggp
-00001730: 6c6f 7428 6d70 672c 2061 6573 2878 3d27  lot(mpg, aes(x='
-00001740: 6374 7927 2c20 636f 6c6f 723d 2764 7276  cty', color='drv
-00001750: 272c 2066 696c 6c3d 2764 7276 2729 2920  ', fill='drv')) 
-00001760: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
-00001770: 2020 2020 2020 6765 6f6d 5f64 656e 7369        geom_densi
-00001780: 7479 2861 6573 2879 3d61 6674 6572 5f73  ty(aes(y=after_s
-00001790: 7461 7428 2763 6f75 6e74 2729 292c 2061  tat('count')), a
-000017a0: 6c70 6861 3d30 2e31 2920 2b0a 2020 2020  lpha=0.1) +.    
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 7363 616c 655f 636f 6c6f 725f 6469 7363  scale_color_disc
-000017d0: 7265 7465 2867 7569 6465 3d46 616c 7365  rete(guide=False
-000017e0: 2920 2b0a 2020 2020 2020 2020 2020 2020  ) +.            
-000017f0: 2020 2020 2020 2020 7468 656d 6528 6178          theme(ax
-00001800: 6973 5f74 6963 6b73 5f6d 616a 6f72 5f78  is_ticks_major_x
-00001810: 3d65 6c65 6d65 6e74 5f62 6c61 6e6b 2829  =element_blank()
-00001820: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001830: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-00001840: 5f74 6578 745f 7820 3d65 6c65 6d65 6e74  _text_x =element
-00001850: 5f62 6c61 6e6b 2829 2c0a 2020 2020 2020  _blank(),.      
-00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001870: 2020 2020 6178 6973 5f74 6974 6c65 5f78      axis_title_x
-00001880: 3d65 6c65 6d65 6e74 5f62 6c61 6e6b 2829  =element_blank()
-00001890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000018a0: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-000018b0: 5f74 6578 745f 7920 3d65 6c65 6d65 6e74  _text_y =element
-000018c0: 5f74 6578 7428 7369 7a65 3d31 3229 2c0a  _text(size=12),.
-000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018e0: 2020 2020 2020 2020 2020 6178 6973 5f74            axis_t
-000018f0: 6974 6c65 5f79 3d65 6c65 6d65 6e74 5f74  itle_y=element_t
-00001900: 6578 7428 7369 7a65 3d31 3429 2c0a 2020  ext(size=14),.  
-00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001920: 2020 2020 2020 2020 6c65 6765 6e64 5f70          legend_p
-00001930: 6f73 6974 696f 6e3d 226e 6f6e 6522 292c  osition="none"),
-00001940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001950: 2020 2020 2066 6967 7369 7a65 3d28 342c       figsize=(4,
-00001960: 3129 290a 0a67 3220 3d20 7077 2e6c 6f61  1))..g2 = pw.loa
-00001970: 645f 6767 706c 6f74 2867 6770 6c6f 7428  d_ggplot(ggplot(
-00001980: 6d70 672c 2061 6573 2878 3d27 6877 7927  mpg, aes(x='hwy'
-00001990: 2c20 636f 6c6f 723d 2764 7276 272c 2066  , color='drv', f
-000019a0: 696c 6c3d 2764 7276 2729 2920 2b0a 2020  ill='drv')) +.  
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 6765 6f6d 5f64 656e 7369 7479 2861    geom_density(a
-000019d0: 6573 2879 3d61 6674 6572 5f73 7461 7428  es(y=after_stat(
-000019e0: 2763 6f75 6e74 2729 292c 2061 6c70 6861  'count')), alpha
-000019f0: 3d30 2e31 2920 2b0a 2020 2020 2020 2020  =0.1) +.        
-00001a00: 2020 2020 2020 2020 2020 2020 636f 6f72              coor
-00001a10: 645f 666c 6970 2829 202b 0a20 2020 2020  d_flip() +.     
-00001a20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001a30: 6865 6d65 2861 7869 735f 7469 636b 735f  heme(axis_ticks_
-00001a40: 6d61 6a6f 725f 793d 656c 656d 656e 745f  major_y=element_
-00001a50: 626c 616e 6b28 292c 0a20 2020 2020 2020  blank(),.       
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2061 7869 735f 7465 7874 5f79 203d     axis_text_y =
-00001a80: 656c 656d 656e 745f 626c 616e 6b28 292c  element_blank(),
-00001a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001aa0: 2020 2020 2020 2020 2020 2061 7869 735f             axis_
-00001ab0: 7469 746c 655f 793d 656c 656d 656e 745f  title_y=element_
-00001ac0: 626c 616e 6b28 292c 0a20 2020 2020 2020  blank(),.       
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 2020 2061 7869 735f 7465 7874 5f78 203d     axis_text_x =
-00001af0: 656c 656d 656e 745f 7465 7874 2873 697a  element_text(siz
-00001b00: 653d 3132 292c 0a20 2020 2020 2020 2020  e=12),.         
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2061 7869 735f 7469 746c 655f 783d 656c   axis_title_x=el
-00001b30: 656d 656e 745f 7465 7874 2873 697a 653d  ement_text(size=
-00001b40: 3134 290a 2020 2020 2020 2020 2020 2020  14).            
-00001b50: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b70: 2020 2020 6669 6773 697a 653d 2831 2c34      figsize=(1,4
-00001b80: 2929 0a0a 6733 203d 2070 772e 6c6f 6164  ))..g3 = pw.load
-00001b90: 5f67 6770 6c6f 7428 6767 706c 6f74 286d  _ggplot(ggplot(m
-00001ba0: 7067 2920 2b0a 2020 2020 2020 2020 2020  pg) +.          
-00001bb0: 2020 2020 2020 2020 2020 6765 6f6d 5f70            geom_p
-00001bc0: 6f69 6e74 2861 6573 2878 3d22 6374 7922  oint(aes(x="cty"
-00001bd0: 2c20 793d 2268 7779 222c 2063 6f6c 6f72  , y="hwy", color
-00001be0: 3d22 6472 7622 2929 202b 0a20 2020 2020  ="drv")) +.     
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001c00: 6361 6c65 5f63 6f6c 6f72 5f64 6973 6372  cale_color_discr
-00001c10: 6574 6528 6775 6964 653d 4661 6c73 6529  ete(guide=False)
-00001c20: 202b 0a20 2020 2020 2020 2020 2020 2020   +.             
-00001c30: 2020 2020 2020 2074 6865 6d65 2861 7869         theme(axi
-00001c40: 735f 7465 7874 203d 656c 656d 656e 745f  s_text =element_
-00001c50: 7465 7874 2873 697a 653d 3132 292c 0a20  text(size=12),. 
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 2020 2020 2020 2020 2061 7869 735f 7469           axis_ti
-00001c80: 746c 653d 656c 656d 656e 745f 7465 7874  tle=element_text
-00001c90: 2873 697a 653d 3134 290a 2020 2020 2020  (size=14).      
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00001cc0: 2020 2020 2020 2020 2020 6669 6773 697a            figsiz
-00001cd0: 653d 2834 2c34 2929 0a0a 7077 2e70 6172  e=(4,4))..pw.par
-00001ce0: 616d 5b22 6d61 7267 696e 225d 203d 2030  am["margin"] = 0
-00001cf0: 2e32 0a28 6731 2f28 6733 7c67 3229 5b67  .2.(g1/(g3|g2)[g
-00001d00: 335d 292e 7361 7665 6669 6728 2920 2342  3]).savefig() #B
-00001d10: 7920 7370 6563 6966 7969 6e67 2067 3320  y specifying g3 
-00001d20: 696e 2028 6733 7c67 3229 2c20 6731 2069  in (g3|g2), g1 i
-00001d30: 7320 706f 7369 7469 6f6e 6564 2065 7861  s positioned exa
-00001d40: 6374 6c79 206f 6e20 6733 2e20 0a0a 6060  ctly on g3. ..``
-00001d50: 600a 0a3c 696d 6720 7372 633d 2268 7474  `..<img src="htt
-00001d60: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00001d70: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f70  sercontent.com/p
-00001d80: 6f6e 6e68 6964 652f 7061 7463 6877 6f72  onnhide/patchwor
-00001d90: 6b6c 6962 2f6d 6169 6e2f 696d 672f 6a6f  klib/main/img/jo
-00001da0: 696e 745f 706c 6f74 5f70 6c6f 746e 696e  int_plot_plotnin
-00001db0: 652e 706e 6722 2077 6964 7468 3d22 3830  e.png" width="80
-00001dc0: 3078 3830 3022 3e0a 0a3c 2f64 6574 6169  0x800">..</detai
-00001dd0: 6c73 3e0a 0a23 2323 2320 3037 3139 3230  ls>..#### 071920
-00001de0: 3232 3a20 5665 7273 696f 6e20 302e 342e  22: Version 0.4.
-00001df0: 3320 7761 7320 7265 6c65 6173 6564 2e20  3 was released. 
-00001e00: 0a2d 2041 2066 6577 2062 7567 7320 7765  .- A few bugs we
-00001e10: 7265 2066 6978 6564 2e20 200a 2d20 6062  re fixed.  .- `b
-00001e20: 6173 6566 6967 7572 6560 2070 6172 616d  asefigure` param
-00001e30: 6574 6572 2077 6173 2061 6464 6564 2e20  eter was added. 
-00001e40: 596f 7520 6361 6e20 6163 6365 7373 2074  You can access t
-00001e50: 6865 2062 6173 6520 6669 6775 7265 206f  he base figure o
-00001e60: 6620 7061 7463 6877 6f72 6b6c 6962 2062  f patchworklib b
-00001e70: 7920 6070 6174 6368 776f 726b 6c69 622e  y `patchworklib.
-00001e80: 6261 7365 6669 6775 7265 600a 2d20 706c  basefigure`.- pl
-00001e90: 6f74 6e69 6e65 2076 302e 392e 3020 7761  otnine v0.9.0 wa
-00001ea0: 7320 6e6f 7720 7375 7070 6f72 7465 642e  s now supported.
-00001eb0: 2050 726f 6261 626c 792c 2069 7420 7374   Probably, it st
-00001ec0: 696c 6c20 6861 7665 2073 6f6d 6520 6275  ill have some bu
-00001ed0: 6773 2e20 4966 2079 6f75 2066 696e 6420  gs. If you find 
-00001ee0: 6275 6773 2c20 706c 6561 7365 206c 6574  bugs, please let
-00001ef0: 206d 6520 6b6e 6f77 206f 6e20 7468 6520   me know on the 
-00001f00: 6973 7375 652e 0a0a 2323 2323 2030 3432  issue...#### 042
-00001f10: 3232 3032 323a 2056 6572 7369 6f6e 2030  22022: Version 0
-00001f20: 2e34 2e32 2077 6173 2072 656c 6561 7365  .4.2 was release
-00001f30: 642e 200a 2d20 4120 6665 7720 6275 6773  d. .- A few bugs
-00001f40: 2077 6572 6520 6669 7865 642e 2020 0a0a   were fixed.  ..
-00001f50: 2323 2323 2030 3431 3832 3032 323a 2056  #### 04182022: V
-00001f60: 6572 7369 6f6e 2030 2e34 2e31 2077 6173  ersion 0.4.1 was
-00001f70: 2072 656c 6561 7365 642e 200a 2d20 606c   released. .- `l
-00001f80: 6f61 645f 7365 6162 6f72 6e67 7269 6460  oad_seaborngrid`
-00001f90: 2063 616e 2061 6363 6570 7473 2061 2060   can accepts a `
-00001fa0: 7365 6162 6f72 6e2e 636c 7573 7465 726d  seaborn.clusterm
-00001fb0: 6170 6020 706c 6f74 2e20 466f 7220 6465  ap` plot. For de
-00001fc0: 7461 696c 732c 2073 6565 2065 7861 6d70  tails, see examp
-00001fd0: 6c65 2063 6f64 6520 6f6e 205b 476f 6f67  le code on [Goog
-00001fe0: 6c65 2063 6f6c 6162 5d28 6874 7470 733a  le colab](https:
-00001ff0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00002000: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
-00002010: 652f 3177 5151 7942 484c 4e58 4a35 4b73  e/1wQQyBHLNXJ5Ks
-00002020: 3665 7638 3849 6a58 6847 6654 3938 5347  6ev88IjXhGfT98SG
-00002030: 4a75 4d3f 7573 703d 7368 6172 696e 6729  JuM?usp=sharing)
-00002040: 0a2d 2041 2066 6577 2062 7567 7320 7765  .- A few bugs we
-00002050: 7265 2066 6978 6564 2e20 200a 0a23 2323  re fixed.  ..###
-00002060: 2320 3033 3237 3230 3232 3a20 5665 7273  # 03272022: Vers
-00002070: 696f 6e20 302e 342e 3020 7761 7320 7265  ion 0.4.0 was re
-00002080: 6c65 6173 6564 2e20 0a2d 2041 6464 2064  leased. .- Add d
-00002090: 6f63 7374 7269 6e67 2066 6f72 2065 6163  ocstring for eac
-000020a0: 6820 6d65 7468 6f64 2061 6e64 2063 6c61  h method and cla
-000020b0: 7373 2e20 200a 2d20 4164 6420 7365 7665  ss.  .- Add seve
-000020c0: 7261 6c20 6e65 7720 6d65 7468 6f64 7320  ral new methods 
-000020d0: 6f66 2060 7061 7463 6877 6f72 6b6c 6962  of `patchworklib
-000020e0: 2e42 7269 636b 7360 2063 6c61 7373 2074  .Bricks` class t
-000020f0: 6f20 7365 7420 636f 6d6d 6f6e 206c 6162  o set common lab
-00002100: 656c 2c20 7469 746c 652c 2073 7069 6e65  el, title, spine
-00002110: 2061 6e64 2063 6f6c 6f72 6261 7220 666f   and colorbar fo
-00002120: 7220 6042 7269 636b 6020 6f62 6a65 7473  r `Brick` objets
-00002130: 2069 6e20 7468 6520 6042 7269 636b 7360   in the `Bricks`
-00002140: 206f 626a 6563 742e 2020 0ae3 8080 466f   object.  ....Fo
-00002150: 7220 7573 6167 652c 2070 6c65 6173 6520  r usage, please 
-00002160: 7265 6665 7220 746f 2074 6865 2064 6f63  refer to the doc
-00002170: 7374 7269 6e67 206f 7220 7468 6520 6578  string or the ex
-00002180: 616d 706c 6520 636f 6465 7320 6f6e 205b  ample codes on [
-00002190: 476f 6f67 6c65 2063 6f6c 6162 5d28 6874  Google colab](ht
-000021a0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
-000021b0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
-000021c0: 6472 6976 652f 3166 3036 4151 4f71 4e6e  drive/1f06AQOqNn
-000021d0: 5359 506a 6339 456b 7765 4333 5f48 6d79  SYPjc9EkweC3_Hmy
-000021e0: 3461 6272 2d67 6f3f 7573 703d 7368 6172  4abr-go?usp=shar
-000021f0: 696e 6729 2e0a 0a23 2323 2320 3032 3034  ing)...#### 0204
-00002200: 3230 3232 3a20 5665 7273 696f 6e20 302e  2022: Version 0.
-00002210: 332e 3620 7761 7320 7265 6c65 6173 6564  3.6 was released
-00002220: 2e20 0a2d 2041 2066 6577 2062 7567 7320  . .- A few bugs 
-00002230: 7265 6c61 7469 6e67 2077 6974 6820 7468  relating with th
-00002240: 6520 6675 6e63 7469 6f6e 2074 6f20 6172  e function to ar
-00002250: 7261 6e67 6520 6d75 6c74 6970 6c65 2070  range multiple p
-00002260: 6f6c 6172 2070 6c6f 7420 6f62 6a65 6374  olar plot object
-00002270: 732e 0a0a 2323 2323 2030 3230 3432 3032  s...#### 0204202
-00002280: 323a 2056 6572 7369 6f6e 2030 2e33 2e35  2: Version 0.3.5
-00002290: 2077 6173 2072 656c 6561 7365 642e 0a2d   was released..-
-000022a0: 2041 2066 6577 2062 7567 7320 696e 2060   A few bugs in `
-000022b0: 6d6f 7665 5f6c 6567 656e 6460 2077 6572  move_legend` wer
-000022c0: 6520 6669 7865 642e 2028 5468 6520 606d  e fixed. (The `m
-000022d0: 6f76 655f 6c65 6765 6e64 6020 666f 7220  ove_legend` for 
-000022e0: 7365 6162 6f72 6e20 6772 6964 6564 2070  seaborn grided p
-000022f0: 6c6f 7420 7761 7320 6e6f 7420 776f 726b  lot was not work
-00002300: 696e 6720 7072 6f70 6572 6c79 2e29 0a2d  ing properly.).-
-00002310: 2049 6d70 726f 7665 6420 7468 6520 7370   Improved the sp
-00002320: 6565 6420 6f66 2060 7361 7665 6669 6760  eed of `savefig`
-00002330: 206f 7065 7261 7469 6f6e 2e0a 0a23 2323   operation...###
-00002340: 2320 3031 3234 3230 3232 3a20 5665 7273  # 01242022: Vers
-00002350: 696f 6e20 302e 332e 3320 7761 7320 7265  ion 0.3.3 was re
-00002360: 6c65 6173 6564 2e20 0a2d 2041 2066 6577  leased. .- A few
-00002370: 2062 7567 7320 7765 7265 2066 6978 6564   bugs were fixed
-00002380: 2e0a 090a 2323 2323 2030 3132 3232 3032  ....#### 0122202
-00002390: 323a 2056 6572 7369 6f6e 2030 2e33 2e30  2: Version 0.3.0
-000023a0: 2077 6173 2072 656c 6561 7365 642e 0a3c   was released..<
-000023b0: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
-000023c0: 793e 2050 6174 6368 776f 726b 6c69 6220  y> Patchworklib 
-000023d0: 6e6f 7720 7375 7070 6f72 7473 2074 6865  now supports the
-000023e0: 2066 756e 6374 696f 6e20 746f 2061 7272   function to arr
-000023f0: 616e 6765 206d 6174 706c 6f74 6c69 622e  ange matplotlib.
-00002400: 7072 6f6a 6563 7469 6f6e 732e 706f 6c61  projections.pola
-00002410: 722e 506f 6c61 7241 7865 7320 6f6a 6265  r.PolarAxes ojbe
-00002420: 6374 732e 2020 3c2f 7375 6d6d 6172 793e  cts.  </summary>
-00002430: 0a0a 5768 656e 2079 6f75 206c 6f61 6420  ..When you load 
-00002440: 6120 6d61 7470 6c6f 746c 6962 2e70 726f  a matplotlib.pro
-00002450: 6a65 6374 696f 6e73 2e70 6f6c 6172 2e50  jections.polar.P
-00002460: 6f6c 6172 4178 6573 206f 626a 6563 7420  olarAxes object 
-00002470: 6173 2061 2042 7269 636b 2063 6c61 7373  as a Brick class
-00002480: 206f 626a 6563 742c 2070 6c65 6173 6520   object, please 
-00002490: 7573 6520 2763 4272 6963 6b27 2069 6e73  use 'cBrick' ins
-000024a0: 7465 6164 206f 6620 2742 7269 636b 272e  tead of 'Brick'.
-000024b0: 0a4e 6f77 2c20 796f 7520 6361 6e20 6172  .Now, you can ar
-000024c0: 7261 6e67 6520 6d75 6c74 6970 6c65 2063  range multiple c
-000024d0: 6972 636f 7320 706c 6f74 7320 7573 696e  ircos plots usin
-000024e0: 6720 5b70 7963 6972 636f 735d 2868 7474  g [pycircos](htt
-000024f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002500: 706f 6e6e 6869 6465 2f70 7943 6972 636f  ponnhide/pyCirco
-00002510: 7329 2061 6e64 2070 6174 6368 776f 726b  s) and patchwork
-00002520: 6c69 622e 2050 6c65 6173 6520 7365 6520  lib. Please see 
-00002530: 7468 6520 666f 6c6c 6f77 696e 6720 6578  the following ex
-00002540: 616d 706c 6520 636f 6465 2e20 200a 6874  ample code.  .ht
-00002550: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
-00002560: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
-00002570: 6472 6976 652f 3174 6b6e 3770 7852 7168  drive/1tkn7pxRqh
-00002580: 3942 7935 7254 4671 5262 564e 4456 7773  9By5rTFqRbVNDVws
-00002590: 2d6f 2d79 537a 393f 7573 703d 7368 6172  -o-ySz9?usp=shar
-000025a0: 696e 670a 0a3c 2f64 6574 6169 6c73 3e0a  ing..</details>.
-000025b0: 0a23 2323 2320 3031 3231 3230 3232 3a20  .#### 01212022: 
-000025c0: 5665 7273 696f 6e20 302e 322e 3120 7761  Version 0.2.1 wa
-000025d0: 7320 7265 6c65 6173 6564 2e20 200a 2d20  s released.  .- 
-000025e0: 4120 6665 7720 6275 6773 2066 6f72 2027  A few bugs for '
-000025f0: 6c6f 6164 5f73 6561 626f 726e 6772 6964  load_seaborngrid
-00002600: 2720 7765 7265 2066 6978 6564 2e0a 0a23  ' were fixed...#
-00002610: 2323 2320 3031 3230 3230 3232 3a20 5665  ### 01202022: Ve
-00002620: 7273 696f 6e20 302e 322e 3020 7761 7320  rsion 0.2.0 was 
-00002630: 7265 6c65 6173 6564 2e0a 3c64 6574 6169  released..<detai
-00002640: 6c73 3e0a 3c73 756d 6d61 7279 3e20 5061  ls>.<summary> Pa
-00002650: 7463 6877 6f72 6b6c 6962 2069 7320 6e6f  tchworklib is no
-00002660: 7720 706f 7373 6962 6c65 2074 6f20 6172  w possible to ar
-00002670: 7261 6e67 6520 5365 6162 726f 6e20 6772  range Seabron gr
-00002680: 6964 6465 6420 706c 6f74 732e 2054 6865  idded plots. The
-00002690: 2022 7374 6163 6b22 2066 756e 6374 696f   "stack" functio
-000026a0: 6e20 6973 2061 6464 6564 2e20 4120 6665  n is added. A fe
-000026b0: 7720 6275 6773 2077 6572 6520 6669 7865  w bugs were fixe
-000026c0: 642e 203c 2f73 756d 6d61 7279 3e0a 090a  d. </summary>...
-000026d0: 2323 2323 2041 7272 616e 6769 6e67 2073  #### Arranging s
-000026e0: 6561 626f 726e 2067 7269 6464 6564 2070  eaborn gridded p
-000026f0: 6c6f 7473 200a 5061 7463 6877 6f72 6b6c  lots .Patchworkl
-00002700: 6962 2073 7570 706f 7274 6564 2074 6865  ib supported the
-00002710: 2066 756e 6374 696f 6e20 746f 2061 7261   function to ara
-00002720: 6e67 6520 6d75 6c74 6970 6c65 2073 6562  nge multiple seb
-00002730: 6f72 6e20 706c 6f74 7320 6765 6e65 7261  orn plots genera
-00002740: 7465 6420 6261 7365 6420 6f6e 2061 7869  ted based on axi
-00002750: 7367 7269 6420 2846 6163 6574 4772 6964  sgrid (FacetGrid
-00002760: 2c20 5061 6972 4772 6964 2c20 616e 6420  , PairGrid, and 
-00002770: 4a6f 696e 7447 7269 6429 2e0a 4c65 7427  JointGrid)..Let'
-00002780: 7320 7365 6520 7468 6520 666f 6c6c 776f  s see the follwo
-00002790: 696e 6720 6578 616d 706c 652e 0a0a 6060  ing example...``
-000027a0: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
-000027b0: 730a 696d 706f 7274 2073 6561 626f 726e  s.import seaborn
-000027c0: 2061 7320 736e 730a 696d 706f 7274 2070   as sns.import p
-000027d0: 6174 6368 776f 726b 6c69 6220 6173 2070  atchworklib as p
-000027e0: 770a 6672 6f6d 2066 756e 6374 6f6f 6c73  w.from functools
-000027f0: 2069 6d70 6f72 7420 7265 6475 6365 0a70   import reduce.p
-00002800: 772e 6f76 6572 7772 6974 655f 6178 6973  w.overwrite_axis
-00002810: 6772 6964 2829 2023 5768 656e 2079 6f75  grid() #When you
-00002820: 2075 7365 2070 772e 6c6f 6164 5f73 6561   use pw.load_sea
-00002830: 676f 726e 6772 6964 2c20 276f 7665 7277  gorngrid, 'overw
-00002840: 7269 7465 5f61 7869 7367 7269 6427 2073  rite_axisgrid' s
-00002850: 686f 756c 6420 6265 2065 7865 6375 7465  hould be execute
-00002860: 642e 0a0a 6466 203d 2073 6e73 2e6c 6f61  d...df = sns.loa
-00002870: 645f 6461 7461 7365 7428 2270 656e 6775  d_dataset("pengu
-00002880: 696e 7322 290a 6731 2020 3d20 736e 732e  ins").g1  = sns.
-00002890: 7061 6972 706c 6f74 2864 662c 2068 7565  pairplot(df, hue
-000028a0: 3d22 7370 6563 6965 7322 290a 6731 2020  ="species").g1  
-000028b0: 3d20 7077 2e6c 6f61 645f 7365 6162 6f72  = pw.load_seabor
-000028c0: 6e67 7269 6428 6731 290a 6731 2e6d 6f76  ngrid(g1).g1.mov
-000028d0: 655f 6c65 6765 6e64 2822 7570 7065 7220  e_legend("upper 
-000028e0: 6c65 6674 222c 2062 626f 785f 746f 5f61  left", bbox_to_a
-000028f0: 6e63 686f 723d 2830 2e30 382c 312e 3031  nchor=(0.08,1.01
-00002900: 2929 0a0a 706c 616e 6574 7320 3d20 736e  ))..planets = sn
-00002910: 732e 6c6f 6164 5f64 6174 6173 6574 2822  s.load_dataset("
-00002920: 706c 616e 6574 7322 290a 636d 6170 203d  planets").cmap =
-00002930: 2073 6e73 2e63 7562 6568 656c 6978 5f70   sns.cubehelix_p
-00002940: 616c 6574 7465 2872 6f74 3d2d 2e32 2c20  alette(rot=-.2, 
-00002950: 6173 5f63 6d61 703d 5472 7565 290a 6732  as_cmap=True).g2
-00002960: 203d 2073 6e73 2e72 656c 706c 6f74 280a   = sns.relplot(.
-00002970: 2020 2020 6461 7461 3d70 6c61 6e65 7473      data=planets
-00002980: 2c0a 2020 2020 783d 2264 6973 7461 6e63  ,.    x="distanc
-00002990: 6522 2c20 793d 226f 7262 6974 616c 5f70  e", y="orbital_p
-000029a0: 6572 696f 6422 2c0a 2020 2020 6875 653d  eriod",.    hue=
-000029b0: 2279 6561 7222 2c20 7369 7a65 3d22 6d61  "year", size="ma
-000029c0: 7373 222c 0a20 2020 2070 616c 6574 7465  ss",.    palette
-000029d0: 3d63 6d61 702c 2073 697a 6573 3d28 3130  =cmap, sizes=(10
-000029e0: 2c20 3230 3029 2c0a 290a 6732 2e73 6574  , 200),.).g2.set
-000029f0: 2878 7363 616c 653d 226c 6f67 222c 2079  (xscale="log", y
-00002a00: 7363 616c 653d 226c 6f67 2229 0a67 322e  scale="log").g2.
-00002a10: 6178 2e78 6178 6973 2e67 7269 6428 5472  ax.xaxis.grid(Tr
-00002a20: 7565 2c20 226d 696e 6f72 222c 206c 696e  ue, "minor", lin
-00002a30: 6577 6964 7468 3d2e 3235 290a 6732 2e61  ewidth=.25).g2.a
-00002a40: 782e 7961 7869 732e 6772 6964 2854 7275  x.yaxis.grid(Tru
-00002a50: 652c 2022 6d69 6e6f 7222 2c20 6c69 6e65  e, "minor", line
-00002a60: 7769 6474 683d 2e32 3529 0a67 322e 6465  width=.25).g2.de
-00002a70: 7370 696e 6528 6c65 6674 3d54 7275 652c  spine(left=True,
-00002a80: 2062 6f74 746f 6d3d 5472 7565 290a 6732   bottom=True).g2
-00002a90: 203d 2070 772e 6c6f 6164 5f73 6561 626f   = pw.load_seabo
-00002aa0: 726e 6772 6964 2867 3229 0a0a 7065 6e67  rngrid(g2)..peng
-00002ab0: 7569 6e73 203d 2073 6e73 2e6c 6f61 645f  uins = sns.load_
-00002ac0: 6461 7461 7365 7428 2270 656e 6775 696e  dataset("penguin
-00002ad0: 7322 290a 6733 203d 2073 6e73 2e6a 6f69  s").g3 = sns.joi
-00002ae0: 6e74 706c 6f74 280a 2020 2020 6461 7461  ntplot(.    data
-00002af0: 3d70 656e 6775 696e 732c 0a20 2020 2078  =penguins,.    x
-00002b00: 3d22 6269 6c6c 5f6c 656e 6774 685f 6d6d  ="bill_length_mm
-00002b10: 222c 2079 3d22 6269 6c6c 5f64 6570 7468  ", y="bill_depth
-00002b20: 5f6d 6d22 2c20 6875 653d 2273 7065 6369  _mm", hue="speci
-00002b30: 6573 222c 0a20 2020 206b 696e 643d 226b  es",.    kind="k
-00002b40: 6465 222c 0a29 0a67 3320 3d20 7077 2e6c  de",.).g3 = pw.l
-00002b50: 6f61 645f 7365 6162 6f72 6e67 7269 6428  oad_seaborngrid(
-00002b60: 6733 2c20 6c61 6265 6c73 3d5b 226a 6f69  g3, labels=["joi
-00002b70: 6e74 222c 226d 6172 675f 7822 2c22 6d61  nt","marg_x","ma
-00002b80: 7267 5f79 225d 290a 2828 6732 2f67 335b  rg_y"]).((g2/g3[
-00002b90: 226d 6172 675f 7822 5d29 7c67 3129 2e73  "marg_x"])|g1).s
-00002ba0: 6176 6566 6967 2829 0a60 6060 0a3c 696d  avefig().```.<im
-00002bb0: 6720 7372 633d 2269 6d67 2f73 6561 626f  g src="img/seabo
-00002bc0: 726e 5f67 7269 6473 2e70 6e67 2220 7769  rn_grids.png" wi
-00002bd0: 6474 683d 2238 3030 7838 3030 223e 0a0a  dth="800x800">..
-00002be0: 416c 736f 2c20 736f 6d65 2065 7861 6d70  Also, some examp
-00002bf0: 6c65 2063 6f64 6573 2061 7265 206d 6164  le codes are mad
-00002c00: 6520 6578 6563 7574 6162 6c65 2069 6e20  e executable in 
-00002c10: 476f 6f67 6c65 2043 6f6c 6162 6f72 6174  Google Colaborat
-00002c20: 6f72 792e 0a2d 205b 7365 6162 6f72 6e20  ory..- [seaborn 
-00002c30: 6772 6964 5d28 6874 7470 733a 2f2f 636f  grid](https://co
-00002c40: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00002c50: 676c 652e 636f 6d2f 6472 6976 652f 317a  gle.com/drive/1z
-00002c60: 3030 334c 6162 5077 6f66 6273 4e38 3778  003LabPwofbsN87x
-00002c70: 7333 3646 4271 4b63 4d67 5473 774f 343f  s36FBqKcMgTswO4?
-00002c80: 7573 703d 7368 6172 696e 6729 0a2d 205b  usp=sharing).- [
-00002c90: 7365 6162 6f72 6e5f 6767 706c 6f74 5d28  seaborn_ggplot](
-00002ca0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00002cb0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00002cc0: 6d2f 6472 6976 652f 3153 5049 316a 536f  m/drive/1SPI1jSo
-00002cd0: 4837 4c30 6866 5837 346e 7551 7434 4277  H7L0hfX74nuQt4Bw
-00002ce0: 5935 524b 7772 5857 573f 7573 703d 7368  Y5RKwrXWW?usp=sh
-00002cf0: 6172 696e 6729 0a0a 2323 2323 2022 7374  aring)..#### "st
-00002d00: 6163 6b22 2066 7563 6e74 696f 6e0a 4920  ack" fucntion.I 
-00002d10: 696d 706c 656d 656e 7465 6420 7468 6520  implemented the 
-00002d20: 6073 7461 636b 6020 6675 6e63 7469 6f6e  `stack` function
-00002d30: 2e20 5468 6973 2066 756e 6374 696f 6e20  . This function 
-00002d40: 616c 6c6f 7773 2075 7365 7273 2074 6f20  allows users to 
-00002d50: 6172 7261 6e67 6520 6d75 6c74 6970 6c65  arrange multiple
-00002d60: 2028 6d6f 7265 2074 6861 6e20 7477 6f29   (more than two)
-00002d70: 2042 7269 636b 206f 7220 4272 6963 6b73   Brick or Bricks
-00002d80: 206f 626a 6563 7473 2061 6c6f 6e67 2074   objects along t
-00002d90: 6865 2073 7065 6369 6669 6564 2064 6972  he specified dir
-00002da0: 6563 7469 6f6e 2061 7320 666f 6c6c 6f77  ection as follow
-00002db0: 732e 0a0a 6060 6070 7974 686f 6e0a 696d  s...```python.im
-00002dc0: 706f 7274 2070 6174 6368 776f 726b 6c69  port patchworkli
-00002dd0: 6220 6173 2070 770a 6178 5f6c 6973 7420  b as pw.ax_list 
-00002de0: 3d20 5b5d 0a66 6f72 2069 2069 6e20 7261  = [].for i in ra
-00002df0: 6e67 6528 3130 293a 0a20 2020 2061 785f  nge(10):.    ax_
-00002e00: 6c69 7374 2e61 7070 656e 6428 7077 2e42  list.append(pw.B
-00002e10: 7269 636b 2866 6967 7369 7a65 3d28 322c  rick(figsize=(2,
-00002e20: 3229 2c20 6c61 6265 6c3d 2261 787b 7d22  2), label="ax{}"
-00002e30: 2e66 6f72 6d61 7428 6929 2929 0a73 7461  .format(i))).sta
-00002e40: 636b 6564 5f61 7865 7320 3d20 7077 2e73  cked_axes = pw.s
-00002e50: 7461 636b 2861 785f 6c69 7374 2c20 6f70  tack(ax_list, op
-00002e60: 6572 6174 6f72 3d22 7c22 2c20 6d61 7267  erator="|", marg
-00002e70: 696e 3d30 2e32 290a 7374 6163 6b65 645f  in=0.2).stacked_
-00002e80: 6178 6573 2e73 6176 6566 6967 2829 0a60  axes.savefig().`
-00002e90: 6060 0a3c 696d 6720 7372 633d 2269 6d67  ``.<img src="img
-00002ea0: 2f73 7461 636b 5f65 7861 6d70 6c65 2e70  /stack_example.p
-00002eb0: 6e67 2220 7769 6474 683d 2238 3030 7838  ng" width="800x8
-00002ec0: 3030 223e 0a0a 0a3c 2f64 6574 6169 6c73  00">...</details
-00002ed0: 3e0a 090a 2323 2323 2030 3131 3432 3032  >...#### 0114202
-00002ee0: 323a 2056 6572 7369 6f6e 2030 2e31 2e30  2: Version 0.1.0
-00002ef0: 2077 6173 2072 656c 6561 7365 642e 2020   was released.  
-00002f00: 0a2d 2050 6174 6368 776f 726b 6c69 6220  .- Patchworklib 
-00002f10: 7761 7320 6e6f 7720 6176 6961 6c61 626c  was now avialabl
-00002f20: 6520 7468 726f 7567 6820 7069 702e 0a0a  e through pip...
-00002f30: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
-00002f40: 7279 3e20 3c62 3e30 3131 3332 3032 323a  ry> <b>01132022:
-00002f50: 2022 7370 6163 6572 2220 636c 6173 7320   "spacer" class 
-00002f60: 7761 7320 696d 706c 656d 656e 7465 6420  was implemented 
-00002f70: 616e 6420 2263 6173 6522 2070 6172 616d  and "case" param
-00002f80: 6574 6572 2077 6173 2061 6464 6564 2074  eter was added t
-00002f90: 6f20 4272 6963 6b73 2063 6c61 7373 2e3c  o Bricks class.<
-00002fa0: 2f62 3e20 3c2f 7375 6d6d 6172 793e 0a0a  /b> </summary>..
-00002fb0: 2a2a 4164 6420 656d 7074 7920 7370 6163  **Add empty spac
-00002fc0: 6573 2061 726f 756e 6420 6120 706c 6f74  es around a plot
-00002fd0: 2a2a 200a 6060 6070 7974 686f 6e0a 2370  ** .```python.#p
-00002fe0: 7265 7061 7261 7469 6f6e 206f 6620 706c  reparation of pl
-00002ff0: 6f74 2064 6174 610a 696d 706f 7274 206e  ot data.import n
-00003000: 756d 7079 2061 7320 6e70 200a 696d 706f  umpy as np .impo
-00003010: 7274 206d 6174 706c 6f74 6c69 6220 6173  rt matplotlib as
-00003020: 206d 706c 0a69 6d70 6f72 7420 7061 7463   mpl.import patc
-00003030: 6877 6f72 6b6c 6962 2061 7320 7077 0a0a  hworklib as pw..
-00003040: 6461 7461 3120 3d20 3230 202a 206e 702e  data1 = 20 * np.
-00003050: 7261 6e64 6f6d 2e72 616e 6428 3130 302c  random.rand(100,
-00003060: 3130 3029 202d 2031 300a 6461 7461 3220  100) - 10.data2 
-00003070: 3d20 3230 202a 206e 702e 7261 6e64 6f6d  = 20 * np.random
-00003080: 2e72 616e 6428 3130 302c 3130 3029 202d  .rand(100,100) -
-00003090: 2031 300a 636d 6170 203d 206d 706c 2e63   10.cmap = mpl.c
-000030a0: 6d2e 5265 6473 0a6e 6f72 6d20 3d20 6d70  m.Reds.norm = mp
-000030b0: 6c2e 636f 6c6f 7273 2e4e 6f72 6d61 6c69  l.colors.Normali
-000030c0: 7a65 2876 6d69 6e3d 2d31 302c 2076 6d61  ze(vmin=-10, vma
-000030d0: 783d 3130 290a 6178 3120 3d20 7077 2e42  x=10).ax1 = pw.B
-000030e0: 7269 636b 2822 6178 7822 2c20 6669 6773  rick("axx", figs
-000030f0: 697a 653d 2833 2c33 2929 0a61 7832 203d  ize=(3,3)).ax2 =
-00003100: 2070 772e 4272 6963 6b28 2261 7879 222c   pw.Brick("axy",
-00003110: 2066 6967 7369 7a65 3d28 332c 3329 290a   figsize=(3,3)).
-00003120: 6178 312e 696d 7368 6f77 2864 6174 6131  ax1.imshow(data1
-00003130: 2c20 696e 7465 7270 6f6c 6174 696f 6e3d  , interpolation=
-00003140: 276e 6561 7265 7374 272c 2063 6d61 703d  'nearest', cmap=
-00003150: 636d 6170 2c20 6173 7065 6374 3d22 6175  cmap, aspect="au
-00003160: 746f 2229 0a61 7832 2e69 6d73 686f 7728  to").ax2.imshow(
-00003170: 6461 7461 322c 2069 6e74 6572 706f 6c61  data2, interpola
-00003180: 7469 6f6e 3d27 6e65 6172 6573 7427 2c20  tion='nearest', 
-00003190: 636d 6170 3d63 6d61 702c 2061 7370 6563  cmap=cmap, aspec
-000031a0: 743d 2261 7574 6f22 290a 6060 600a 0a77  t="auto").```..w
-000031b0: 2f6f 2073 7061 6365 720a 6060 6070 7974  /o spacer.```pyt
-000031c0: 686f 6e0a 6178 5f63 6220 2020 203d 2070  hon.ax_cb    = p
-000031d0: 772e 4272 6963 6b28 2261 785f 6362 222c  w.Brick("ax_cb",
-000031e0: 2066 6967 7369 7a65 3d28 302e 312c 3329   figsize=(0.1,3)
-000031f0: 290a 6362 2020 2020 2020 203d 206d 706c  ).cb       = mpl
-00003200: 2e63 6f6c 6f72 6261 722e 436f 6c6f 7262  .colorbar.Colorb
-00003210: 6172 4261 7365 2861 785f 6362 2c20 636d  arBase(ax_cb, cm
-00003220: 6170 3d63 6d61 702c 206e 6f72 6d3d 6e6f  ap=cmap, norm=no
-00003230: 726d 290a 6178 3132 2020 2020 203d 2061  rm).ax12     = a
-00003240: 7831 7c61 7832 0a68 6561 746d 6170 3220  x1|ax2.heatmap2 
-00003250: 3d20 6178 3132 207c 2061 785f 6362 0a68  = ax12 | ax_cb.h
-00003260: 6561 746d 6170 322e 7361 7665 6669 6728  eatmap2.savefig(
-00003270: 290a 6060 600a 3c69 6d67 2073 7263 3d22  ).```.<img src="
-00003280: 696d 672f 6865 6174 6d61 702d 312e 706e  img/heatmap-1.pn
-00003290: 6722 2077 6964 7468 3d22 3430 3078 3430  g" width="400x40
-000032a0: 3022 3e0a 0a77 2f20 7370 6163 6572 0a60  0">..w/ spacer.`
-000032b0: 6060 7079 7468 6f6e 0a61 785f 6362 3220  ``python.ax_cb2 
-000032c0: 2020 3d20 7077 2e42 7269 636b 2822 6178    = pw.Brick("ax
-000032d0: 5f63 6232 222c 2066 6967 7369 7a65 3d28  _cb2", figsize=(
-000032e0: 302e 312c 312e 3529 290a 6362 3220 2020  0.1,1.5)).cb2   
-000032f0: 2020 203d 206d 706c 2e63 6f6c 6f72 6261     = mpl.colorba
-00003300: 722e 436f 6c6f 7262 6172 4261 7365 2861  r.ColorbarBase(a
-00003310: 785f 6362 322c 2063 6d61 703d 636d 6170  x_cb2, cmap=cmap
-00003320: 2c20 6e6f 726d 3d6e 6f72 6d29 0a68 6561  , norm=norm).hea
-00003330: 746d 6170 3220 3d20 6178 3132 207c 2028  tmap2 = ax12 | (
-00003340: 7077 2e73 7061 6365 7228 6178 5f63 6232  pw.spacer(ax_cb2
-00003350: 2c30 2e35 292f 6178 5f63 6232 2f70 772e  ,0.5)/ax_cb2/pw.
-00003360: 7370 6163 6572 2861 785f 6362 322c 302e  spacer(ax_cb2,0.
-00003370: 3529 290a 6865 6174 6d61 7032 2e73 6176  5)).heatmap2.sav
-00003380: 6566 6967 2829 0a60 6060 0a3c 696d 6720  efig().```.<img 
-00003390: 7372 633d 2269 6d67 2f68 6561 746d 6170  src="img/heatmap
-000033a0: 2d32 2e70 6e67 2220 7769 6474 683d 2234  -2.png" width="4
-000033b0: 3030 7834 3030 223e 0a0a 2a2a 5375 7065  00x400">..**Supe
-000033c0: 7220 7469 7469 6c65 2066 6f72 206d 756c  r titile for mul
-000033d0: 7469 706c 6520 706c 6f74 732a 2a20 200a  tiple plots**  .
-000033e0: 536f 6d65 7469 6d65 732c 2061 6c6c 2074  Sometimes, all t
-000033f0: 6861 7420 6973 206e 6565 6465 6420 746f  hat is needed to
-00003400: 2068 6176 6520 636f 6d6d 6f6e 206c 6162   have common lab
-00003410: 656c 7320 616e 6420 7469 746c 6520 666f  els and title fo
-00003420: 7220 6d75 6c74 6970 6c65 2070 6c6f 7473  r multiple plots
-00003430: 2e20 2020 0a42 7920 7370 6563 6966 7969  .   .By specifyi
-00003440: 6e67 2060 6361 7365 6020 7061 7261 6d65  ng `case` parame
-00003450: 7465 7220 6f66 2061 2042 7269 636b 7320  ter of a Bricks 
-00003460: 636c 6173 7320 6f62 6a65 6374 2c20 636f  class object, co
-00003470: 6d6d 6f6e 206d 6174 706c 6f74 6c69 6220  mmon matplotlib 
-00003480: 6172 7469 7374 206f 6a62 6563 7473 2066  artist ojbects f
-00003490: 6f72 206d 756c 7469 706c 6520 706c 6f74  or multiple plot
-000034a0: 7320 6361 6e20 6265 2068 616e 646c 6564  s can be handled
-000034b0: 2e0a 6060 6070 7974 686f 6e0a 6178 3132  ..```python.ax12
-000034c0: 2e63 6173 652e 7365 745f 7469 746c 6528  .case.set_title(
-000034d0: 2241 2067 6c6f 6261 6c20 7469 746c 6520  "A global title 
-000034e0: 666f 7220 6d75 6c74 6970 6c65 2070 6c6f  for multiple plo
-000034f0: 7473 222c 2070 6164 3d31 3029 0a68 6561  ts", pad=10).hea
-00003500: 746d 6170 3220 3d20 6178 3132 7c28 7077  tmap2 = ax12|(pw
-00003510: 2e73 7061 6365 7228 6178 5f63 622c 302e  .spacer(ax_cb,0.
-00003520: 3529 2f61 785f 6362 2f70 772e 7370 6163  5)/ax_cb/pw.spac
-00003530: 6572 2861 785f 6362 2c30 2e35 2929 0a68  er(ax_cb,0.5)).h
-00003540: 6561 746d 6170 322e 7361 7665 6669 6728  eatmap2.savefig(
-00003550: 2222 290a 6060 600a 3c69 6d67 2073 7263  "").```.<img src
-00003560: 3d22 696d 672f 6865 6174 6d61 702d 332e  ="img/heatmap-3.
-00003570: 706e 6722 2077 6964 7468 3d22 3430 3078  png" width="400x
-00003580: 3430 3022 3e0a 0a3c 2f64 6574 6169 6c73  400">..</details
-00003590: 3e0a 0a0a 3c64 6574 6169 6c73 3e0a 3c73  >...<details>.<s
-000035a0: 756d 6d61 7279 3e20 3c62 3e30 3130 3732  ummary> <b>01072
-000035b0: 3032 323a 2050 6174 6368 776f 726b 6c69  022: Patchworkli
-000035c0: 6220 7761 7320 7570 6461 7465 6420 746f  b was updated to
-000035d0: 2061 6c6c 6f77 2061 7272 616e 6769 6e67   allow arranging
-000035e0: 206d 756c 7469 706c 6520 706c 6f74 7320   multiple plots 
-000035f0: 6765 6e65 7261 7465 6420 6279 203c 6120  generated by <a 
-00003600: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00003610: 7468 7562 2e63 6f6d 2f68 6173 326b 312f  thub.com/has2k1/
-00003620: 706c 6f74 6e69 6e65 223e 706c 6f74 6e69  plotnine">plotni
-00003630: 6e65 3c2f 613e 2e3c 2f62 3e20 3c2f 7375  ne</a>.</b> </su
-00003640: 6d6d 6172 793e 0a0a 6060 6070 7974 686f  mmary>..```pytho
-00003650: 6e0a 696d 706f 7274 2070 6174 6368 776f  n.import patchwo
-00003660: 726b 6c69 6220 6173 2070 770a 6672 6f6d  rklib as pw.from
-00003670: 2070 6c6f 746e 696e 6520 696d 706f 7274   plotnine import
-00003680: 202a 0a66 726f 6d20 706c 6f74 6e69 6e65   *.from plotnine
-00003690: 2e64 6174 6120 696d 706f 7274 202a 0a67  .data import *.g
-000036a0: 3120 3d20 7077 2e6c 6f61 645f 6767 706c  1 = pw.load_ggpl
-000036b0: 6f74 2867 6770 6c6f 7428 6d74 6361 7273  ot(ggplot(mtcars
-000036c0: 2920 2b20 6765 6f6d 5f70 6f69 6e74 2861  ) + geom_point(a
-000036d0: 6573 2822 6d70 6722 2c20 2264 6973 7022  es("mpg", "disp"
-000036e0: 2929 202b 2074 6865 6d65 2866 6967 7572  )) + theme(figur
-000036f0: 655f 7369 7a65 3d28 322c 2033 2929 290a  e_size=(2, 3))).
-00003700: 6732 203d 2070 772e 6c6f 6164 5f67 6770  g2 = pw.load_ggp
-00003710: 6c6f 7428 6767 706c 6f74 286d 7463 6172  lot(ggplot(mtcar
-00003720: 7329 202b 2067 656f 6d5f 626f 7870 6c6f  s) + geom_boxplo
-00003730: 7428 6165 7328 2267 6561 7222 2c20 2264  t(aes("gear", "d
-00003740: 6973 7022 2c20 6772 6f75 7020 3d20 2267  isp", group = "g
-00003750: 6561 7222 2929 202b 2074 6865 6d65 2866  ear")) + theme(f
-00003760: 6967 7572 655f 7369 7a65 3d28 322c 2033  igure_size=(2, 3
-00003770: 2929 290a 6731 3220 3d20 6731 207c 2067  ))).g12 = g1 | g
-00003780: 320a 6731 322e 7361 7665 6669 6728 290a  2.g12.savefig().
-00003790: 6060 600a 0a3c 696d 6720 7372 633d 2269  ```..<img src="i
-000037a0: 6d67 2f67 3132 2e70 6e67 2220 7769 6474  mg/g12.png" widt
-000037b0: 683d 2234 3030 7834 3030 223e 0a0a 6060  h="400x400">..``
-000037c0: 6070 7974 686f 6e0a 6733 203d 2070 772e  `python.g3 = pw.
-000037d0: 6c6f 6164 5f67 6770 6c6f 7428 6767 706c  load_ggplot(ggpl
-000037e0: 6f74 286d 7067 2c20 6165 7328 783d 2764  ot(mpg, aes(x='d
-000037f0: 6973 706c 272c 2079 3d27 6877 7927 2929  ispl', y='hwy'))
-00003800: 202b 2067 656f 6d5f 706f 696e 7428 2920   + geom_point() 
-00003810: 2b20 6765 6f6d 5f73 6d6f 6f74 6828 7370  + geom_smooth(sp
-00003820: 616e 3d2e 3329 202b 2074 6865 6d65 2866  an=.3) + theme(f
-00003830: 6967 7572 655f 7369 7a65 3d28 322c 2033  igure_size=(2, 3
-00003840: 2929 290a 6734 203d 2070 772e 6c6f 6164  ))).g4 = pw.load
-00003850: 5f67 6770 6c6f 7428 6767 706c 6f74 286d  _ggplot(ggplot(m
-00003860: 7463 6172 7329 202b 2067 656f 6d5f 6261  tcars) + geom_ba
-00003870: 7228 6165 7328 2263 6172 6222 2929 202b  r(aes("carb")) +
-00003880: 2074 6865 6d65 2866 6967 7572 655f 7369   theme(figure_si
-00003890: 7a65 3d28 372c 2032 2929 290a 6731 3233  ze=(7, 2))).g123
-000038a0: 3420 3d20 2867 317c 6732 7c67 3329 2f67  4 = (g1|g2|g3)/g
-000038b0: 340a 6731 3233 342e 7361 7665 6669 6728  4.g1234.savefig(
-000038c0: 290a 6060 600a 3c69 6d67 2073 7263 3d22  ).```.<img src="
-000038d0: 696d 672f 6731 3233 342e 706e 6722 2077  img/g1234.png" w
-000038e0: 6964 7468 3d22 3630 3078 3630 3022 3e0a  idth="600x600">.
-000038f0: 0a3c 2f64 6574 6169 6c73 3e0a 3c2f 6465  .</details>.</de
-00003900: 7461 696c 733e 200a 0a23 2320 5573 6167  tails> ..## Usag
-00003910: 650a 3e20 5f49 6620 796f 7520 7761 6e74  e.> _If you want
-00003920: 2074 6f20 6b6e 6f77 2068 6f77 2074 6f20   to know how to 
-00003930: 7573 6520 7061 7463 6877 6f72 6b6c 6962  use patchworklib
-00003940: 2069 6e20 6465 7461 696c 2c20 706c 6561   in detail, plea
-00003950: 7365 2073 6565 205b 4150 492e 6d64 5d28  se see [API.md](
-00003960: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003970: 6f6d 2f70 6f6e 6e68 6964 652f 7061 7463  om/ponnhide/patc
-00003980: 6877 6f72 6b6c 6962 2f62 6c6f 622f 6d61  hworklib/blob/ma
-00003990: 696e 2f41 5049 2e6d 6429 2e5f 2020 0a3e  in/API.md)._  .>
-000039a0: 0a55 7369 6e67 2060 7061 7463 6877 6f72  .Using `patchwor
-000039b0: 6b6c 6962 602c 2079 6f75 2063 616e 2071  klib`, you can q
-000039c0: 7569 636b 6c79 2061 6e64 2066 7265 656c  uickly and freel
-000039d0: 7920 6172 7261 6e67 6520 6d61 7470 6c6f  y arrange matplo
-000039e0: 746c 6962 2070 6c6f 7473 2077 6974 6820  tlib plots with 
-000039f0: 6f6e 6c79 2060 7c60 2061 6e64 2060 2f60  only `|` and `/`
-00003a00: 206f 7061 7261 746f 7273 2061 7320 666f   oparators as fo
-00003a10: 6c6c 6f77 732e 0a0a 6060 6070 7974 686f  llows...```pytho
-00003a20: 6e0a 696d 706f 7274 2070 6174 6368 776f  n.import patchwo
-00003a30: 726b 6c69 6220 6173 2070 770a 696d 706f  rklib as pw.impo
-00003a40: 7274 2073 6561 626f 726e 2061 7320 736e  rt seaborn as sn
-00003a50: 7320 0a0a 666d 7269 203d 2073 6e73 2e6c  s ..fmri = sns.l
-00003a60: 6f61 645f 6461 7461 7365 7428 2266 6d72  oad_dataset("fmr
-00003a70: 6922 290a 6178 3120 3d20 7077 2e42 7269  i").ax1 = pw.Bri
-00003a80: 636b 2866 6967 7369 7a65 3d28 332c 3229  ck(figsize=(3,2)
-00003a90: 290a 736e 732e 6c69 6e65 706c 6f74 2878  ).sns.lineplot(x
-00003aa0: 3d22 7469 6d65 706f 696e 7422 2c20 793d  ="timepoint", y=
-00003ab0: 2273 6967 6e61 6c22 2c20 6875 653d 2272  "signal", hue="r
-00003ac0: 6567 696f 6e22 2c20 7374 796c 653d 2265  egion", style="e
-00003ad0: 7665 6e74 222c 2064 6174 613d 666d 7269  vent", data=fmri
-00003ae0: 2c20 6178 3d61 7831 290a 6178 312e 6c65  , ax=ax1).ax1.le
-00003af0: 6765 6e64 2862 626f 785f 746f 5f61 6e63  gend(bbox_to_anc
-00003b00: 686f 723d 2831 2e30 352c 2031 2e30 292c  hor=(1.05, 1.0),
-00003b10: 206c 6f63 3d27 7570 7065 7220 6c65 6674   loc='upper left
-00003b20: 2729 0a61 7831 2e73 6574 5f74 6974 6c65  ').ax1.set_title
-00003b30: 2822 6178 3122 290a 200a 7469 7461 6e69  ("ax1"). .titani
-00003b40: 6320 3d20 736e 732e 6c6f 6164 5f64 6174  c = sns.load_dat
-00003b50: 6173 6574 2822 7469 7461 6e69 6322 290a  aset("titanic").
-00003b60: 6178 3220 3d20 7077 2e42 7269 636b 2866  ax2 = pw.Brick(f
-00003b70: 6967 7369 7a65 3d28 312c 3229 290a 736e  igsize=(1,2)).sn
-00003b80: 732e 6261 7270 6c6f 7428 783d 2273 6578  s.barplot(x="sex
-00003b90: 222c 2079 3d22 7375 7276 6976 6564 222c  ", y="survived",
-00003ba0: 2068 7565 3d22 636c 6173 7322 2c20 6461   hue="class", da
-00003bb0: 7461 3d74 6974 616e 6963 2c20 6178 3d61  ta=titanic, ax=a
-00003bc0: 7832 290a 6178 322e 6d6f 7665 5f6c 6567  x2).ax2.move_leg
-00003bd0: 656e 6428 6e65 775f 6c6f 633d 2775 7070  end(new_loc='upp
-00003be0: 6572 206c 6566 7427 2c20 6262 6f78 5f74  er left', bbox_t
-00003bf0: 6f5f 616e 6368 6f72 3d28 312e 3035 2c20  o_anchor=(1.05, 
-00003c00: 312e 3029 290a 6178 322e 7365 745f 7469  1.0)).ax2.set_ti
-00003c10: 746c 6528 2261 7832 2229 0a0a 6178 3132  tle("ax2")..ax12
-00003c20: 203d 2061 7831 7c61 7832 0a61 7831 322e   = ax1|ax2.ax12.
-00003c30: 7361 7665 6669 6728 2261 7831 322e 706e  savefig("ax12.pn
-00003c40: 6722 290a 6060 600a 0a3c 696d 6720 7372  g").```..<img sr
-00003c50: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00003c60: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00003c70: 2e63 6f6d 2f70 6f6e 6e68 6964 652f 7061  .com/ponnhide/pa
-00003c80: 7463 6877 6f72 6b6c 6962 2f6d 6169 6e2f  tchworklib/main/
-00003c90: 696d 672f 6178 3132 2e70 6e67 2220 7769  img/ax12.png" wi
-00003ca0: 6474 683d 2236 3030 7836 3030 223e 0a0a  dth="600x600">..
-00003cb0: 4a75 7079 7465 7220 4e6f 7465 626f 6f6b  Jupyter Notebook
-00003cc0: 2066 696c 6573 2066 6f72 2061 6c6c 206f   files for all o
-00003cd0: 6620 7468 6520 6578 616d 706c 6520 636f  f the example co
-00003ce0: 6465 7320 6172 6520 7072 6f76 6964 6564  des are provided
-00003cf0: 2069 6e20 5b70 6174 6368 776f 726b 6c69   in [patchworkli
-00003d00: 622d 6578 616d 706c 6573 5d28 6874 7470  b-examples](http
-00003d10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00003d20: 6f6e 6e68 6964 652f 7061 7463 6877 6f72  onnhide/patchwor
-00003d30: 6b6c 6962 2d65 7861 6d70 6c65 7329 2061  klib-examples) a
-00003d40: 6e64 2061 6c73 6f20 6d61 6465 2065 7865  nd also made exe
-00003d50: 6375 7461 626c 6520 696e 2047 6f6f 676c  cutable in Googl
-00003d60: 6520 436f 6c61 626f 7261 746f 7279 2e0a  e Colaboratory..
-00003d70: 2d20 5b74 7574 6f72 6961 6c5d 2868 7474  - [tutorial](htt
-00003d80: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-00003d90: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
-00003da0: 7269 7665 2f31 4e66 6a79 754b 5039 6e71  rive/1NfjyuKP9nq
-00003db0: 414d 3068 616e 7652 4851 502d 6b44 3167  AM0hanvRHQP-kD1g
-00003dc0: 626d 5039 517a 3f75 7370 3d73 6861 7269  bmP9Qz?usp=shari
-00003dd0: 6e67 293a 2042 6173 6963 2065 7861 6d70  ng): Basic examp
-00003de0: 6c65 2063 6f64 6573 206f 6620 7061 7463  le codes of patc
-00003df0: 6877 6f72 6b6c 6962 200a 2d20 5b73 7562  hworklib .- [sub
-00003e00: 706c 6f74 7320 666f 7220 706c 6f74 6e69  plots for plotni
-00003e10: 6e65 5d28 6874 7470 733a 2f2f 636f 6c61  ne](https://cola
-00003e20: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-00003e30: 652e 636f 6d2f 6472 6976 652f 3137 6f74  e.com/drive/17ot
-00003e40: 5870 7668 2d6a 4c6e 306a 6f49 324d 7764  Xpvh-jLn0joI2Mwd
-00003e50: 7954 3652 4b4a 7a78 3641 6e77 703f 7573  yT6RKJzx6Anwp?us
-00003e60: 703d 7368 6172 696e 6729 3a20 4172 7261  p=sharing): Arra
-00003e70: 6e67 696e 6720 706c 6f74 6e69 6e65 2070  nging plotnine p
-00003e80: 6c6f 7473 2075 7369 6e67 2070 6174 6368  lots using patch
-00003e90: 776f 726b 6c69 620a 2d20 5b73 7562 706c  worklib.- [subpl
-00003ea0: 6f74 7320 666f 7220 7365 6162 6f72 6e67  ots for seaborng
-00003eb0: 7269 645d 2868 7474 7073 3a2f 2f63 6f6c  rid](https://col
-00003ec0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
-00003ed0: 6c65 2e63 6f6d 2f64 7269 7665 2f31 4331  le.com/drive/1C1
-00003ee0: 454e 312d 354c 3251 6a6e 4141 566f 3476  EN1-5L2QjnAAVo4v
-00003ef0: 7078 5f69 396b 6e44 527a 5834 6a79 3f75  px_i9knDRzX4jy?u
-00003f00: 7370 3d73 6861 7269 6e67 293a 2041 7272  sp=sharing): Arr
-00003f10: 616e 6769 6e67 2066 6967 7572 652d 6c65  anging figure-le
-00003f20: 7665 6c20 7365 6162 6f72 6e20 706c 6f74  vel seaborn plot
-00003f30: 7320 7573 696e 6720 7061 7463 6877 6f72  s using patchwor
-00003f40: 6b6c 6962 0a2d 205b 706c 6163 696e 675f  klib.- [placing_
-00003f50: 7375 7065 725f 656c 656d 656e 7473 5d28  super_elements](
-00003f60: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00003f70: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00003f80: 6d2f 6472 6976 652f 3166 3036 4151 4f71  m/drive/1f06AQOq
-00003f90: 4e6e 5359 506a 6339 456b 7765 4333 5f48  NnSYPjc9EkweC3_H
-00003fa0: 6d79 3461 6272 2d67 6f3f 7573 703d 7368  my4abr-go?usp=sh
-00003fb0: 6172 696e 6729 3a20 506c 6163 696e 6720  aring): Placing 
-00003fc0: 7375 7065 7220 6c61 6265 6c73 2061 6e64  super labels and
-00003fd0: 2073 7069 6e65 7320 666f 7220 6120 7365   spines for a se
-00003fe0: 7420 6f66 206d 756c 7469 706c 6520 7375  t of multiple su
-00003ff0: 6270 6c6f 7473 2e20 200a 416c 736f 2c20  bplots.  .Also, 
-00004000: 706c 6561 7365 2073 6565 2068 7474 7073  please see https
-00004010: 3a2f 2f70 7974 686f 6e2e 706c 6169 6e65  ://python.plaine
-00004020: 6e67 6c69 7368 2e69 6f2f 612d 7375 6270  nglish.io/a-subp
-00004030: 6c6f 742d 6d61 6e61 6765 722d 666f 722d  lot-manager-for-
-00004040: 696e 7475 6974 6976 652d 6c61 796f 7574  intuitive-layout
-00004050: 2d69 6e2d 6d61 7470 6c6f 746c 6962 2d62  -in-matplotlib-b
-00004060: 6430 3337 6665 3936 3766 340a 2323 2047  d037fe967f4.## G
-00004070: 616c 6c65 7279 0a0a 2a2a 4172 7261 6e67  allery..**Arrang
-00004080: 656d 656e 7420 6f66 206d 756c 7469 706c  ement of multipl
-00004090: 6520 6178 6973 2d6c 6576 656c 2073 6561  e axis-level sea
-000040a0: 626f 726e 2070 6c6f 7473 2a2a 0a3c 696d  born plots**.<im
-000040b0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-000040c0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000040d0: 7465 6e74 2e63 6f6d 2f70 6f6e 6e68 6964  tent.com/ponnhid
-000040e0: 652f 7061 7463 6877 6f72 6b6c 6962 2f6d  e/patchworklib/m
-000040f0: 6169 6e2f 696d 672f 6178 3335 3231 345f  ain/img/ax35214_
-00004100: 7633 2e70 6e67 2220 7769 6474 683d 2231  v3.png" width="1
-00004110: 3030 3078 3130 3030 223e 0a0a 2a2a 4172  000x1000">..**Ar
-00004120: 7261 6e67 656d 656e 7420 6f66 206d 756c  rangement of mul
-00004130: 7469 706c 6520 506c 6f74 6e69 6e65 2070  tiple Plotnine p
-00004140: 6c6f 7473 2a2a 0a3c 696d 6720 7372 633d  lots**.<img src=
-00004150: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00004160: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00004170: 6f6d 2f70 6f6e 6e68 6964 652f 7061 7463  om/ponnhide/patc
-00004180: 6877 6f72 6b6c 6962 2f6d 6169 6e2f 696d  hworklib/main/im
-00004190: 672f 706c 6f74 6e69 6e65 2e70 6e67 2220  g/plotnine.png" 
-000041a0: 7769 6474 683d 2231 3030 3078 3130 3030  width="1000x1000
-000041b0: 223e 0a0a 2a2a 4172 7261 6e67 656d 656e  ">..**Arrangemen
-000041c0: 7420 6f66 206d 756c 7469 706c 6520 6669  t of multiple fi
-000041d0: 6775 7265 2d6c 6576 656c 2073 6561 626f  gure-level seabo
-000041e0: 726e 2070 6c6f 7473 2a2a 0a3c 696d 6720  rn plots**.<img 
-000041f0: 7372 633d 2268 7474 7073 3a2f 2f64 6576  src="https://dev
-00004200: 2d74 6f2d 7570 6c6f 6164 732e 7333 2e61  -to-uploads.s3.a
-00004210: 6d61 7a6f 6e61 7773 2e63 6f6d 2f75 706c  mazonaws.com/upl
-00004220: 6f61 6473 2f61 7274 6963 6c65 732f 6939  oads/articles/i9
-00004230: 6433 796f 6763 7471 3634 7336 6a33 3369  d3yogctq64s6j33i
-00004240: 7962 2e70 6e67 2220 7769 6474 683d 2231  yb.png" width="1
-00004250: 3030 3078 3130 3030 223e 0a0a 2323 2320  000x1000">..### 
-00004260: 4765 7474 696e 6720 7374 6172 7465 640a  Getting started.
-00004270: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
-00004280: 6172 793e 4578 616d 706c 6520 636f 6465  ary>Example code
-00004290: 733c 2f73 756d 6d61 7279 3e0a 0a2a 2a54  s</summary>..**T
-000042a0: 7574 6f72 6961 6c20 5c7e 2a43 6f6d 706f  utorial \~*Compo
-000042b0: 7365 206d 756c 7469 706c 6520 7365 6162  se multiple seab
-000042c0: 6f72 6e20 706c 6f74 732a 5c7e 2a2a 0a54  orn plots*\~**.T
-000042d0: 6865 2066 6f6c 6c77 6f69 6e67 2074 7574  he follwoing tut
-000042e0: 6f72 6961 6c20 636f 6465 7320 6361 6e20  orial codes can 
-000042f0: 6265 2065 7865 6375 7461 626c 6520 696e  be executable in
-00004300: 205b 7475 746f 7269 616c 315d 2868 7474   [tutorial1](htt
-00004310: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-00004320: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
-00004330: 7269 7665 2f31 5456 6348 3349 4a79 3667  rive/1TVcH3IJy6g
-00004340: 6544 5856 4a44 664f 4b43 5046 5073 5032  eDXVJDfOKCPFPsP2
-00004350: 477a 6a78 4875 3f75 7370 3d73 6861 7269  GzjxHu?usp=shari
-00004360: 6e67 290a 0a23 2323 2320 312e 2049 6d70  ng)..#### 1. Imp
-00004370: 6f72 7469 6e67 2070 6174 6368 776f 726b  orting patchwork
-00004380: 6c69 6220 6c69 6272 6172 790a 0a60 6060  lib library..```
-00004390: 7079 7468 6f6e 0a69 6d70 6f72 7420 7061  python.import pa
-000043a0: 7463 6877 6f72 6b6c 6962 2061 7320 7077  tchworklib as pw
-000043b0: 200a 666d 7269 203d 2073 6e73 2e6c 6f61   .fmri = sns.loa
-000043c0: 645f 6461 7461 7365 7428 2266 6d72 6922  d_dataset("fmri"
-000043d0: 290a 6178 3120 3d20 7077 2e42 7269 636b  ).ax1 = pw.Brick
-000043e0: 2822 6178 3122 2c20 6669 6773 697a 653d  ("ax1", figsize=
-000043f0: 2834 2c32 2929 0a73 6e73 2e6c 696e 6570  (4,2)).sns.linep
-00004400: 6c6f 7428 783d 2274 696d 6570 6f69 6e74  lot(x="timepoint
-00004410: 222c 2079 3d22 7369 676e 616c 222c 2068  ", y="signal", h
-00004420: 7565 3d22 7265 6769 6f6e 222c 2073 7479  ue="region", sty
-00004430: 6c65 3d22 6576 656e 7422 2c20 6461 7461  le="event", data
-00004440: 3d66 6d72 692c 2061 783d 6178 3129 0a61  =fmri, ax=ax1).a
-00004450: 7831 2e6d 6f76 655f 6c65 6765 6e64 286e  x1.move_legend(n
-00004460: 6577 5f6c 6f63 3d27 7570 7065 7220 7269  ew_loc='upper ri
-00004470: 6768 7427 290a 6178 312e 7365 745f 7469  ght').ax1.set_ti
-00004480: 746c 6528 2261 7831 2229 0a60 6060 0a0a  tle("ax1").```..
-00004490: 2323 2323 2032 2e20 4372 6561 7469 6e67  #### 2. Creating
-000044a0: 2065 7861 6d70 6c65 2070 6c6f 7473 0a20   example plots. 
-000044b0: 0a43 7265 6174 696e 6720 736f 6d65 2065  .Creating some e
-000044c0: 7861 6d70 6c65 2070 6c6f 7473 2075 7369  xample plots usi
-000044d0: 6e67 2074 6865 2073 6561 7262 6f72 6e20  ng the searborn 
-000044e0: 6d6f 6475 6c65 2e20 4272 6963 6b20 636c  module. Brick cl
-000044f0: 6173 7320 7072 6f76 6964 6564 2062 7920  ass provided by 
-00004500: 7468 6520 7061 7463 6877 6f72 6b6c 6962  the patchworklib
-00004510: 206d 6f64 756c 6520 6973 2069 6d70 6c65   module is imple
-00004520: 6d65 6e74 6564 2061 7320 7375 6263 6c61  mented as subcla
-00004530: 7373 206f 6620 606d 6174 706c 6f74 6c69  ss of `matplotli
-00004540: 622e 6178 6573 2e41 7865 7360 2e20 2054  b.axes.Axes`.  T
-00004550: 6865 7265 666f 7265 2c20 4272 6963 6b20  herefore, Brick 
-00004560: 636c 6173 7320 6f62 6a65 6374 2063 616e  class object can
-00004570: 2062 6520 6769 7665 6e20 746f 2074 6865   be given to the
-00004580: 2073 6561 626f 726e 2070 6c6f 7420 6675   seaborn plot fu
-00004590: 6e63 7469 6f6e 7320 7468 6174 2068 6176  nctions that hav
-000045a0: 6520 7468 6520 6061 7860 2070 6172 616d  e the `ax` param
-000045b0: 6574 6572 732e 2020 0a0a 5768 656e 2063  eters.  ..When c
-000045c0: 7265 6174 696e 6720 6120 4272 6963 6b20  reating a Brick 
-000045d0: 636c 6173 7320 6f62 6a65 6374 2c20 7468  class object, th
-000045e0: 6520 606c 6162 656c 6020 7661 6c75 6520  e `label` value 
-000045f0: 7368 6f75 6c64 2062 6520 7370 6563 6966  should be specif
-00004600: 6965 642c 2061 6e64 2069 7420 7368 6f75  ied, and it shou
-00004610: 6c64 2062 6520 756e 6971 7565 2061 6d6f  ld be unique amo
-00004620: 6e67 2074 6865 2042 7269 636b 2063 6c61  ng the Brick cla
-00004630: 7373 206f 626a 6563 7473 2067 656e 6572  ss objects gener
-00004640: 6174 6564 2069 6e20 7468 6520 7079 7468  ated in the pyth
-00004650: 6f6e 2073 6372 6970 7420 2849 6620 7468  on script (If th
-00004660: 6520 6c61 6265 6c20 7661 6c75 6520 6973  e label value is
-00004670: 206e 6f74 2073 7065 6369 6669 6564 2c20   not specified, 
-00004680: 7468 6520 756e 6971 7565 206c 6162 656c  the unique label
-00004690: 206e 616d 6520 6973 2061 7574 6f6d 6174   name is automat
-000046a0: 6963 616c 6c79 2067 6976 656e 2e20 4279  ically given. By
-000046b0: 2075 7369 6e67 2060 6765 745f 6c61 6265   using `get_labe
-000046c0: 6c28 2960 206d 6574 686f 642c 2074 6865  l()` method, the
-000046d0: 2076 616c 7565 2063 616e 2062 6520 636f   value can be co
-000046e0: 6e66 6972 6d65 6429 2e20 5468 6520 6066  nfirmed). The `f
-000046f0: 6967 6973 697a 6560 2070 6172 616d 6574  igisize` paramet
-00004700: 6572 2063 616e 2061 6c73 6f20 6265 2073  er can also be s
-00004710: 7065 6369 6669 6564 2e20 486f 7765 7665  pecified. Howeve
-00004720: 722c 2074 6865 2076 616c 7565 2069 7320  r, the value is 
-00004730: 6e6f 7420 7665 7279 2069 6d70 6f72 7461  not very importa
-00004740: 6e74 2062 6563 6175 7365 2074 6865 2066  nt because the f
-00004750: 6967 7572 6520 7369 7a65 206f 6620 4272  igure size of Br
-00004760: 6963 6b20 636c 6173 7320 6f62 6a65 6374  ick class object
-00004770: 7320 6361 6e20 6265 2061 7574 6f6d 6174  s can be automat
-00004780: 6963 616c 6c79 2061 646a 7573 7465 6420  ically adjusted 
-00004790: 696e 2061 7272 616e 6769 6e67 2074 6865  in arranging the
-000047a0: 2070 6c6f 7473 2e20 5468 6520 6073 6176   plots. The `sav
-000047b0: 6566 6967 2860 2a60 6669 6c65 6e61 6d65  efig(`*`filename
-000047c0: 3d73 7472 602a 6029 6020 6d65 7468 6f64  =str`*`)` method
-000047d0: 2072 6574 7572 6e73 2060 6d61 7470 6c6f   returns `matplo
-000047e0: 746c 6962 2e66 6967 7572 652e 4669 6775  tlib.figure.Figu
-000047f0: 7265 6020 636c 6173 7320 6f62 6a65 6374  re` class object
-00004800: 2e20 4966 2060 6669 6c65 6e61 6d65 6020  . If `filename` 
-00004810: 6973 2067 6976 656e 2c20 7468 6520 6669  is given, the fi
-00004820: 6775 7265 206f 626a 6563 7420 6361 6e20  gure object can 
-00004830: 6265 206f 7574 7075 7420 746f 2074 6865  be output to the
-00004840: 2066 696c 652e 0a0a 6060 6070 7974 686f   file...```pytho
-00004850: 6e0a 696d 706f 7274 2073 6561 626f 726e  n.import seaborn
-00004860: 2061 7320 736e 730a 2345 7861 6d70 6c65   as sns.#Example
-00004870: 2070 6c6f 7420 3120 2872 6566 3a20 6874   plot 1 (ref: ht
-00004880: 7470 733a 2f2f 7365 6162 6f72 6e2e 7079  tps://seaborn.py
-00004890: 6461 7461 2e6f 7267 2f65 7861 6d70 6c65  data.org/example
-000048a0: 732f 6572 726f 7262 616e 645f 6c69 6e65  s/errorband_line
-000048b0: 706c 6f74 732e 6874 6d6c 290a 666d 7269  plots.html).fmri
-000048c0: 203d 2073 6e73 2e6c 6f61 645f 6461 7461   = sns.load_data
-000048d0: 7365 7428 2266 6d72 6922 290a 6178 3120  set("fmri").ax1 
-000048e0: 3d20 7077 2e42 7269 636b 2822 6178 3122  = pw.Brick("ax1"
-000048f0: 2c20 6669 6773 697a 653d 2834 2c32 2929  , figsize=(4,2))
-00004900: 0a73 6e73 2e6c 696e 6570 6c6f 7428 783d  .sns.lineplot(x=
-00004910: 2274 696d 6570 6f69 6e74 222c 2079 3d22  "timepoint", y="
-00004920: 7369 676e 616c 222c 2068 7565 3d22 7265  signal", hue="re
-00004930: 6769 6f6e 222c 2073 7479 6c65 3d22 6576  gion", style="ev
-00004940: 656e 7422 2c20 6461 7461 3d66 6d72 692c  ent", data=fmri,
-00004950: 2061 783d 6178 3129 0a61 7831 2e6d 6f76   ax=ax1).ax1.mov
-00004960: 655f 6c65 6765 6e64 286e 6577 5f6c 6f63  e_legend(new_loc
-00004970: 3d27 7570 7065 7220 7269 6768 7427 290a  ='upper right').
-00004980: 6178 312e 7365 745f 7469 746c 6528 2261  ax1.set_title("a
-00004990: 7831 2229 0a61 7831 2e73 6176 6566 6967  x1").ax1.savefig
-000049a0: 2829 0a60 6060 0a0a 3c69 6d67 2073 7263  ().```..<img src
-000049b0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-000049c0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000049d0: 636f 6d2f 706f 6e6e 6869 6465 2f70 6174  com/ponnhide/pat
-000049e0: 6368 776f 726b 6c69 622f 6d61 696e 2f69  chworklib/main/i
-000049f0: 6d67 2f61 7831 2e70 6e67 2220 7769 6474  mg/ax1.png" widt
-00004a00: 683d 2233 3530 7833 3530 223e 0a0a 4272  h="350x350">..Br
-00004a10: 6963 6b20 636c 6173 7320 7072 6f76 6964  ick class provid
-00004a20: 6573 2074 6865 2060 6d6f 7665 6c65 6765  es the `movelege
-00004a30: 6e64 2860 2a60 6c6f 633d 7374 722c 2062  nd(`*`loc=str, b
-00004a40: 626f 785f 746f 5f61 6e63 686f 723d 2866  box_to_anchor=(f
-00004a50: 6c6f 6174 2c66 6c6f 6174 2960 2a60 2960  loat,float)`*`)`
-00004a60: 206d 6574 686f 642e 2042 7920 7573 696e   method. By usin
-00004a70: 6720 7468 6973 206d 6574 686f 642c 206c  g this method, l
-00004a80: 6567 656e 6420 6c6f 6361 7469 6f6e 2063  egend location c
-00004a90: 616e 2062 6520 7175 6963 6b6c 7920 6d6f  an be quickly mo
-00004aa0: 6469 6669 6564 2e0a 0a60 6060 7079 7468  dified...```pyth
-00004ab0: 6f6e 0a23 4578 616d 706c 6520 706c 6f74  on.#Example plot
-00004ac0: 2032 2028 7265 663a 2068 7474 7073 3a2f   2 (ref: https:/
-00004ad0: 2f73 6561 626f 726e 2e70 7964 6174 612e  /seaborn.pydata.
-00004ae0: 6f72 672f 7475 746f 7269 616c 2f63 6174  org/tutorial/cat
-00004af0: 6567 6f72 6963 616c 2e68 746d 6c29 0a74  egorical.html).t
-00004b00: 6974 616e 6963 203d 2073 6e73 2e6c 6f61  itanic = sns.loa
-00004b10: 645f 6461 7461 7365 7428 2274 6974 616e  d_dataset("titan
-00004b20: 6963 2229 0a61 7832 203d 2070 772e 4272  ic").ax2 = pw.Br
-00004b30: 6963 6b28 2261 7832 222c 2066 6967 7369  ick("ax2", figsi
-00004b40: 7a65 3d28 312c 3229 290a 736e 732e 6261  ze=(1,2)).sns.ba
-00004b50: 7270 6c6f 7428 783d 2273 6578 222c 2079  rplot(x="sex", y
-00004b60: 3d22 7375 7276 6976 6564 222c 2068 7565  ="survived", hue
-00004b70: 3d22 636c 6173 7322 2c20 6461 7461 3d74  ="class", data=t
-00004b80: 6974 616e 6963 2c20 6178 3d61 7832 290a  itanic, ax=ax2).
-00004b90: 6178 322e 6d6f 7665 5f6c 6567 656e 6428  ax2.move_legend(
-00004ba0: 6e65 775f 6c6f 633d 2775 7070 6572 206c  new_loc='upper l
-00004bb0: 6566 7427 2c20 6262 6f78 5f74 6f5f 616e  eft', bbox_to_an
-00004bc0: 6368 6f72 3d28 312e 3035 2c20 312e 3029  chor=(1.05, 1.0)
-00004bd0: 2920 234f 7269 6769 6e61 6c20 6d65 7468  ) #Original meth
-00004be0: 6f64 206f 6620 426c 6963 6b20 636c 6173  od of Blick clas
-00004bf0: 730a 6178 322e 7365 745f 7469 746c 6528  s.ax2.set_title(
-00004c00: 2261 7832 2229 0a61 7832 2e73 6176 6566  "ax2").ax2.savef
-00004c10: 6967 2829 0a60 6060 0a0a 3c69 6d67 2073  ig().```..<img s
-00004c20: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00004c30: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00004c40: 742e 636f 6d2f 706f 6e6e 6869 6465 2f70  t.com/ponnhide/p
-00004c50: 6174 6368 776f 726b 6c69 622f 6d61 696e  atchworklib/main
-00004c60: 2f69 6d67 2f61 7832 2e70 6e67 2220 7769  /img/ax2.png" wi
-00004c70: 6474 683d 2232 3530 7832 3530 223e 0a0a  dth="250x250">..
-00004c80: 6060 6070 7974 686f 6e0a 2345 7861 6d70  ```python.#Examp
-00004c90: 6c65 2070 6c6f 7420 3320 2872 6566 3a20  le plot 3 (ref: 
-00004ca0: 6874 7470 733a 2f2f 7365 6162 6f72 6e2e  https://seaborn.
-00004cb0: 7079 6461 7461 2e6f 7267 2f65 7861 6d70  pydata.org/examp
-00004cc0: 6c65 732f 6869 7374 6f67 7261 6d5f 7374  les/histogram_st
-00004cd0: 6163 6b65 642e 6874 6d6c 290a 6469 616d  acked.html).diam
-00004ce0: 6f6e 6473 203d 2073 6e73 2e6c 6f61 645f  onds = sns.load_
-00004cf0: 6461 7461 7365 7428 2264 6961 6d6f 6e64  dataset("diamond
-00004d00: 7322 290a 6178 3320 3d20 7077 2e42 7269  s").ax3 = pw.Bri
-00004d10: 636b 2822 6178 3322 2c20 2835 2c32 2929  ck("ax3", (5,2))
-00004d20: 0a73 6e73 2e68 6973 7470 6c6f 7428 6469  .sns.histplot(di
-00004d30: 616d 6f6e 6473 2c20 783d 2270 7269 6365  amonds, x="price
-00004d40: 222c 2068 7565 3d22 6375 7422 2c20 6d75  ", hue="cut", mu
-00004d50: 6c74 6970 6c65 3d22 7374 6163 6b22 2c0a  ltiple="stack",.
-00004d60: 2020 2020 7061 6c65 7474 653d 226c 6967      palette="lig
-00004d70: 6874 3a6d 5f72 222c 2065 6467 6563 6f6c  ht:m_r", edgecol
-00004d80: 6f72 3d22 2e33 222c 206c 696e 6577 6964  or=".3", linewid
-00004d90: 7468 3d2e 352c 206c 6f67 5f73 6361 6c65  th=.5, log_scale
-00004da0: 3d54 7275 652c 0a20 2020 2061 7820 3d20  =True,.    ax = 
-00004db0: 6178 3329 0a61 7833 2e73 6574 5f74 6974  ax3).ax3.set_tit
-00004dc0: 6c65 2822 6178 3322 290a 6178 332e 7361  le("ax3").ax3.sa
-00004dd0: 7665 6669 6728 290a 6060 600a 0a3c 696d  vefig().```..<im
-00004de0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00004df0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00004e00: 7465 6e74 2e63 6f6d 2f70 6f6e 6e68 6964  tent.com/ponnhid
-00004e10: 652f 7061 7463 6877 6f72 6b6c 6962 2f6d  e/patchworklib/m
-00004e20: 6169 6e2f 696d 672f 6178 332e 706e 6722  ain/img/ax3.png"
-00004e30: 2077 6964 7468 3d22 3430 3078 3430 3022   width="400x400"
-00004e40: 3e0a 0a60 6060 7079 7468 6f6e 0a23 4578  >..```python.#Ex
-00004e50: 616d 706c 6520 706c 6f74 2034 2028 7265  ample plot 4 (re
-00004e60: 663a 6874 7470 733a 2f2f 7365 6162 6f72  f:https://seabor
-00004e70: 6e2e 7079 6461 7461 2e6f 7267 2f65 7861  n.pydata.org/exa
-00004e80: 6d70 6c65 732f 6772 6f75 7065 645f 7669  mples/grouped_vi
-00004e90: 6f6c 696e 706c 6f74 732e 6874 6d6c 290a  olinplots.html).
-00004ea0: 7469 7073 203d 2073 6e73 2e6c 6f61 645f  tips = sns.load_
-00004eb0: 6461 7461 7365 7428 2274 6970 7322 290a  dataset("tips").
-00004ec0: 6178 3420 3d20 7077 2e42 7269 636b 2822  ax4 = pw.Brick("
-00004ed0: 6178 3422 2c20 2836 2c32 2929 0a73 6e73  ax4", (6,2)).sns
-00004ee0: 2e76 696f 6c69 6e70 6c6f 7428 6461 7461  .violinplot(data
-00004ef0: 3d74 6970 732c 2078 3d22 6461 7922 2c20  =tips, x="day", 
-00004f00: 793d 2274 6f74 616c 5f62 696c 6c22 2c20  y="total_bill", 
-00004f10: 6875 653d 2273 6d6f 6b65 7222 2c0a 2020  hue="smoker",.  
-00004f20: 2020 7370 6c69 743d 5472 7565 2c20 696e    split=True, in
-00004f30: 6e65 723d 2271 7561 7274 222c 206c 696e  ner="quart", lin
-00004f40: 6577 6964 7468 3d31 2c0a 2020 2020 7061  ewidth=1,.    pa
-00004f50: 6c65 7474 653d 7b22 5965 7322 3a20 2262  lette={"Yes": "b
-00004f60: 222c 2022 4e6f 223a 2022 2e38 3522 7d2c  ", "No": ".85"},
-00004f70: 0a20 2020 2061 783d 6178 3429 0a61 7834  .    ax=ax4).ax4
-00004f80: 2e73 6574 5f74 6974 6c65 2822 6178 3422  .set_title("ax4"
-00004f90: 290a 6178 342e 7361 7665 6669 6728 222e  ).ax4.savefig(".
-00004fa0: 2e2f 696d 672f 6178 342e 706e 6722 290a  ./img/ax4.png").
-00004fb0: 6060 600a 0a3c 696d 6720 7372 633d 2268  ```..<img src="h
-00004fc0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00004fd0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00004fe0: 2f70 6f6e 6e68 6964 652f 7061 7463 6877  /ponnhide/patchw
-00004ff0: 6f72 6b6c 6962 2f6d 6169 6e2f 696d 672f  orklib/main/img/
-00005000: 6178 342e 706e 6722 2077 6964 7468 3d22  ax4.png" width="
-00005010: 3430 3078 3430 3022 3e0a 0a60 6060 7079  400x400">..```py
-00005020: 7468 6f6e 0a23 4578 616d 706c 6520 706c  thon.#Example pl
-00005030: 6f74 2035 2028 7265 663a 6874 7470 733a  ot 5 (ref:https:
-00005040: 2f2f 7365 6162 6f72 6e2e 7079 6461 7461  //seaborn.pydata
-00005050: 2e6f 7267 2f65 7861 6d70 6c65 732f 7769  .org/examples/wi
-00005060: 6465 5f64 6174 615f 6c69 6e65 706c 6f74  de_data_lineplot
-00005070: 2e68 746d 6c29 0a72 7320 3d20 6e70 2e72  .html).rs = np.r
-00005080: 616e 646f 6d2e 5261 6e64 6f6d 5374 6174  andom.RandomStat
-00005090: 6528 3336 3529 0a76 616c 7565 7320 3d20  e(365).values = 
-000050a0: 7273 2e72 616e 646e 2833 3635 2c20 3429  rs.randn(365, 4)
-000050b0: 2e63 756d 7375 6d28 6178 6973 3d30 290a  .cumsum(axis=0).
-000050c0: 6461 7465 7320 3d20 7064 2e64 6174 655f  dates = pd.date_
-000050d0: 7261 6e67 6528 2231 2031 2032 3031 3622  range("1 1 2016"
-000050e0: 2c20 7065 7269 6f64 733d 3336 352c 2066  , periods=365, f
-000050f0: 7265 713d 2244 2229 0a64 6174 6120 3d20  req="D").data = 
-00005100: 7064 2e44 6174 6146 7261 6d65 2876 616c  pd.DataFrame(val
-00005110: 7565 732c 2064 6174 6573 2c20 636f 6c75  ues, dates, colu
-00005120: 6d6e 733d 5b22 4122 2c20 2242 222c 2022  mns=["A", "B", "
-00005130: 4322 2c20 2244 225d 290a 6461 7461 203d  C", "D"]).data =
-00005140: 2064 6174 612e 726f 6c6c 696e 6728 3729   data.rolling(7)
-00005150: 2e6d 6561 6e28 290a 6178 3520 3d20 7077  .mean().ax5 = pw
-00005160: 2e42 7269 636b 2822 6178 3522 2c20 2835  .Brick("ax5", (5
-00005170: 2c32 2929 0a73 6e73 2e6c 696e 6570 6c6f  ,2)).sns.lineplo
-00005180: 7428 6461 7461 3d64 6174 612c 2070 616c  t(data=data, pal
-00005190: 6574 7465 3d22 7461 6231 3022 2c20 6c69  ette="tab10", li
-000051a0: 6e65 7769 6474 683d 322e 352c 2061 783d  newidth=2.5, ax=
-000051b0: 6178 3529 0a61 7835 2e73 6574 5f78 6c61  ax5).ax5.set_xla
-000051c0: 6265 6c28 2264 6174 6522 290a 6178 352e  bel("date").ax5.
-000051d0: 7365 745f 796c 6162 656c 2822 7661 6c75  set_ylabel("valu
-000051e0: 6522 290a 6178 352e 7365 745f 7469 746c  e").ax5.set_titl
-000051f0: 6528 2261 7835 2229 0a61 7835 2e73 6176  e("ax5").ax5.sav
-00005200: 6566 6967 2829 0a60 6060 0a0a 3c69 6d67  efig().```..<img
-00005210: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00005220: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00005230: 656e 742e 636f 6d2f 706f 6e6e 6869 6465  ent.com/ponnhide
-00005240: 2f70 6174 6368 776f 726b 6c69 622f 6d61  /patchworklib/ma
-00005250: 696e 2f69 6d67 2f61 7835 2e70 6e67 2220  in/img/ax5.png" 
-00005260: 7769 6474 683d 2234 3030 7834 3030 223e  width="400x400">
-00005270: 0a0a 2323 2323 2033 2e20 4172 7261 6e67  ..#### 3. Arrang
-00005280: 696e 6720 616e 6420 7374 6163 6b69 6e67  ing and stacking
-00005290: 2070 6c6f 7473 0a0a 5468 6520 7061 7463   plots..The patc
-000052a0: 6877 6f72 6b6c 6962 206d 6f64 756c 6520  hworklib module 
-000052b0: 7072 6f76 6964 6573 2074 776f 206f 7065  provides two ope
-000052c0: 7261 746f 7273 2022 2060 7c60 222c 2022  rators " `|`", "
-000052d0: 602f 6022 2074 6861 7420 656e 6162 6c65  `/`" that enable
-000052e0: 2064 6573 6967 6e69 6e67 2074 6964 7920   designing tidy 
-000052f0: 6c61 796f 7574 2066 6f72 206d 756c 7469  layout for multi
-00005300: 706c 6520 706c 6f74 7320 7769 7468 2073  ple plots with s
-00005310: 696d 706c 6520 6f70 6572 6174 696f 6e73  imple operations
-00005320: 2e20 5468 6520 2260 7c60 2220 6f70 6572  . The "`|`" oper
-00005330: 6174 6f72 2077 696c 6c20 706c 6163 6520  ator will place 
-00005340: 7468 6520 706c 6f74 7320 6265 7369 6465  the plots beside
-00005350: 2065 6163 6820 6f74 6865 722c 2077 6869   each other, whi
-00005360: 6c65 2074 6865 2022 602f 6022 206f 7065  le the "`/`" ope
-00005370: 7261 746f 7220 7769 6c6c 2073 7461 636b  rator will stack
-00005380: 2074 6865 6d2e 0a0a 6060 6070 7974 686f   them...```pytho
-00005390: 6e0a 2341 7272 616e 6765 2022 6178 312c  n.#Arrange "ax1,
-000053a0: 2220 2261 7832 2c22 2061 6e64 2022 6178  " "ax2," and "ax
-000053b0: 3422 2068 6f72 697a 6f6e 7461 6c6c 792e  4" horizontally.
-000053c0: 0a61 7831 3234 203d 2061 7831 7c61 7832  .ax124 = ax1|ax2
-000053d0: 7c61 7834 0a61 7831 3234 2e73 6176 6566  |ax4.ax124.savef
-000053e0: 6967 2822 2e2e 2f69 6d67 2f61 7831 3234  ig("../img/ax124
-000053f0: 2e70 6e67 2229 0a60 6060 0a0a 3c69 6d67  .png").```..<img
-00005400: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00005410: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00005420: 656e 742e 636f 6d2f 706f 6e6e 6869 6465  ent.com/ponnhide
-00005430: 2f70 6174 6368 776f 726b 6c69 622f 6d61  /patchworklib/ma
-00005440: 696e 2f69 6d67 2f61 7831 3234 2e70 6e67  in/img/ax124.png
-00005450: 2220 7769 6474 683d 2231 3030 3078 3130  " width="1000x10
-00005460: 3030 223e 0a0a 5468 6520 6f62 6a65 6374  00">..The object
-00005470: 2067 656e 6572 6174 6564 2062 7920 6172   generated by ar
-00005480: 7261 6e67 696e 6720 6d75 6c74 6970 6c65  ranging multiple
-00005490: 2042 7269 636b 206f 626a 6563 7420 2842   Brick object (B
-000054a0: 7269 636b 7320 636c 6173 7320 6f62 6a65  ricks class obje
-000054b0: 6374 2920 6361 6e20 616c 736f 2062 6520  ct) can also be 
-000054c0: 6172 7261 6e67 6564 2061 6e64 2073 7461  arranged and sta
-000054d0: 636b 6564 2077 6974 6820 6f74 6865 7220  cked with other 
-000054e0: 4272 6963 6b20 6f62 6a65 6374 732e 2020  Brick objects.  
-000054f0: 4164 6469 7469 6f6e 616c 6c79 2c20 4974  Additionally, It
-00005500: 2069 7320 2070 6f73 7369 626c 6520 746f   is  possible to
-00005510: 2063 7265 6174 6520 6d6f 7265 2063 6f6d   create more com
-00005520: 706c 6578 206c 6179 6f75 7473 2062 7920  plex layouts by 
-00005530: 6e65 7374 696e 6720 7468 6520 6f70 6572  nesting the oper
-00005540: 6174 696f 6e73 2e0a 0a60 6060 7079 7468  ations...```pyth
-00005550: 6f6e 0a61 7831 3234 3335 203d 2061 7831  on.ax12435 = ax1
-00005560: 3234 2f28 6178 337c 6178 3529 0a61 7831  24/(ax3|ax5).ax1
-00005570: 3234 3335 2e73 6176 6566 6967 2822 2e2e  2435.savefig("..
-00005580: 2f69 6d67 2f61 7831 3234 3335 2e70 6e67  /img/ax12435.png
-00005590: 2229 0a60 6060 0a0a 3c69 6d67 2073 7263  ").```..<img src
-000055a0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-000055b0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000055c0: 636f 6d2f 706f 6e6e 6869 6465 2f70 6174  com/ponnhide/pat
-000055d0: 6368 776f 726b 6c69 622f 6d61 696e 2f69  chworklib/main/i
-000055e0: 6d67 2f61 7831 3234 3335 2e70 6e67 2220  mg/ax12435.png" 
-000055f0: 7769 6474 683d 2231 3030 3078 3130 3030  width="1000x1000
-00005600: 223e 0a0a 596f 7520 6361 6e20 7175 6963  ">..You can quic
-00005610: 6b6c 7920 7465 7374 2061 6e6f 7468 6572  kly test another
-00005620: 206c 6179 6f75 7420 6279 2072 6561 7272   layout by rearr
-00005630: 616e 6769 6e67 2074 6865 6d2e 0a0a 6060  anging them...``
-00005640: 6070 7974 686f 6e0a 6178 3335 3231 3420  `python.ax35214 
-00005650: 3d20 2861 7833 2f28 6178 327c 6178 3129  = (ax3/(ax2|ax1)
-00005660: 297c 2861 7835 2f61 7834 290a 6178 3335  )|(ax5/ax4).ax35
-00005670: 3231 342e 7361 7665 6669 6728 290a 6060  214.savefig().``
-00005680: 600a 0a3c 696d 6720 7372 633d 2268 7474  `..<img src="htt
-00005690: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-000056a0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f70  sercontent.com/p
-000056b0: 6f6e 6e68 6964 652f 7061 7463 6877 6f72  onnhide/patchwor
-000056c0: 6b6c 6962 2f6d 6169 6e2f 696d 672f 6178  klib/main/img/ax
-000056d0: 3335 3231 342e 706e 6722 2077 6964 7468  35214.png" width
-000056e0: 3d22 3130 3030 7831 3030 3022 3e0a 0a49  ="1000x1000">..I
-000056f0: 6620 796f 7520 7761 6e74 2074 6f20 6164  f you want to ad
-00005700: 6a75 7374 2074 6865 206d 6172 6769 6e73  just the margins
-00005710: 2062 6574 7765 656e 206f 626a 6563 7473   between objects
-00005720: 2c20 706c 6561 7365 2063 6861 6e67 6520  , please change 
-00005730: 7468 6520 7661 6c75 6520 6f66 2060 2e70  the value of `.p
-00005740: 6172 616d 5b22 6d61 7267 696e 225d 602e  aram["margin"]`.
-00005750: 0a0a 6060 6070 7974 686f 6e0a 7077 2e70  ..```python.pw.p
-00005760: 6172 616d 5b22 6d61 7267 696e 225d 3d30  aram["margin"]=0
-00005770: 2e32 2023 4465 6661 756c 7420 7661 6c75  .2 #Default valu
-00005780: 6520 6973 2030 2e35 2e0a 6178 3335 3231  e is 0.5..ax3521
-00005790: 3420 3d20 2861 7833 2f28 6178 327c 6178  4 = (ax3/(ax2|ax
-000057a0: 3129 297c 2861 7835 2f61 7834 290a 6178  1))|(ax5/ax4).ax
-000057b0: 3335 3231 342e 7361 7665 6669 6728 222e  35214.savefig(".
-000057c0: 2e2f 696d 672f 6178 3335 3231 345f 7631  ./img/ax35214_v1
-000057d0: 2e31 2e70 6e67 2229 0a60 6060 0a0a 3c69  .1.png").```..<i
-000057e0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000057f0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00005800: 6e74 656e 742e 636f 6d2f 706f 6e6e 6869  ntent.com/ponnhi
-00005810: 6465 2f70 6174 6368 776f 726b 6c69 622f  de/patchworklib/
-00005820: 6d61 696e 2f69 6d67 2f61 7833 3532 3134  main/img/ax35214
-00005830: 5f76 312e 312e 706e 6722 2077 6964 7468  _v1.1.png" width
-00005840: 3d22 3130 3030 7831 3030 3022 3e0a 0a41  ="1000x1000">..A
-00005850: 6c73 6f2c 2074 6865 2061 7370 6563 7420  lso, the aspect 
-00005860: 7261 7469 6f73 206f 6620 6561 6368 2070  ratios of each p
-00005870: 6c6f 7420 6361 6e20 6265 2066 7265 656c  lot can be freel
-00005880: 7920 6d6f 6469 6669 6162 6c65 2e0a 0a60  y modifiable...`
-00005890: 6060 7079 7468 6f6e 0a70 772e 7061 7261  ``python.pw.para
-000058a0: 6d5b 226d 6172 6769 6e22 5d3d 302e 350a  m["margin"]=0.5.
-000058b0: 6178 312e 6368 616e 6765 5f61 7370 6563  ax1.change_aspec
-000058c0: 7472 6174 696f 2828 342c 3229 290a 6178  tratio((4,2)).ax
-000058d0: 332e 6368 616e 6765 5f61 7370 6563 7472  3.change_aspectr
-000058e0: 6174 696f 2828 342c 3129 290a 6178 342e  atio((4,1)).ax4.
-000058f0: 6368 616e 6765 5f61 7370 6563 7472 6174  change_aspectrat
-00005900: 696f 2828 352c 3229 290a 6178 3335 3231  io((5,2)).ax3521
-00005910: 345f 7632 203d 2028 6178 332f 2861 7832  4_v2 = (ax3/(ax2
-00005920: 7c61 7831 2929 7c28 6178 352f 6178 3429  |ax1))|(ax5/ax4)
-00005930: 0a61 7833 3532 3134 5f76 322e 7361 7665  .ax35214_v2.save
-00005940: 6669 6728 290a 6060 600a 0a3c 696d 6720  fig().```..<img 
-00005950: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00005960: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00005970: 6e74 2e63 6f6d 2f70 6f6e 6e68 6964 652f  nt.com/ponnhide/
-00005980: 7061 7463 6877 6f72 6b6c 6962 2f6d 6169  patchworklib/mai
-00005990: 6e2f 696d 672f 6178 3335 3231 345f 7632  n/img/ax35214_v2
-000059a0: 2e70 6e67 2220 7769 6474 683d 2231 3430  .png" width="140
-000059b0: 3078 3134 3030 223e 0a0a 2323 2323 2034  0x1400">..#### 4
-000059c0: 2e20 5061 636b 696e 6720 706c 6f74 7320  . Packing plots 
-000059d0: 7769 7468 206c 6162 656c 2069 6e64 6578  with label index
-000059e0: 696e 6720 2841 6476 616e 6365 6420 6d65  ing (Advanced me
-000059f0: 7468 6f64 290a 0a42 7920 7370 6563 6966  thod)..By specif
-00005a00: 7969 6e67 2074 6865 2042 7269 636b 206f  ying the Brick o
-00005a10: 626a 6563 7473 2069 6e20 6120 4272 6963  bjects in a Bric
-00005a20: 6b73 206f 626a 6563 7420 7769 7468 2074  ks object with t
-00005a30: 6865 6972 206c 6162 656c 206e 616d 652c  heir label name,
-00005a40: 2079 6f75 2063 616e 2061 646a 7573 7420   you can adjust 
-00005a50: 7468 6520 706f 7369 7469 6f6e 206f 6620  the position of 
-00005a60: 616e 6f74 6865 7220 4272 6963 6b20 6f62  another Brick ob
-00005a70: 6a65 6374 2074 6f20 6265 2070 6163 6b65  ject to be packe
-00005a80: 642e 200a 0a60 6060 7079 7468 6f6e 0a61  d. ..```python.a
-00005a90: 7833 3231 203d 2061 7833 2f28 6178 327c  x321 = ax3/(ax2|
-00005aa0: 6178 3129 0a61 7833 3231 2e73 6176 6566  ax1).ax321.savef
-00005ab0: 6967 2822 2e2e 2f69 6d67 2f61 7833 3231  ig("../img/ax321
-00005ac0: 2e70 6e67 2229 0a60 6060 0a0a 3c69 6d67  .png").```..<img
-00005ad0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00005ae0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00005af0: 656e 742e 636f 6d2f 706f 6e6e 6869 6465  ent.com/ponnhide
-00005b00: 2f70 6174 6368 776f 726b 6c69 622f 6d61  /patchworklib/ma
-00005b10: 696e 2f69 6d67 2f61 7833 3231 2e70 6e67  in/img/ax321.png
-00005b20: 2220 7769 6474 683d 2236 3030 7836 3030  " width="600x600
-00005b30: 223e 0a0a 6060 6070 7974 686f 6e0a 6178  ">..```python.ax
-00005b40: 3332 3134 203d 2061 7833 3231 5b22 6178  3214 = ax321["ax
-00005b50: 3122 5d7c 6178 340a 6178 3332 3134 2e73  1"]|ax4.ax3214.s
-00005b60: 6176 6566 6967 2822 2e2e 2f69 6d67 2f61  avefig("../img/a
-00005b70: 7833 3231 342e 706e 6722 290a 6060 600a  x3214.png").```.
-00005b80: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
-00005b90: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00005ba0: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6f6e  rcontent.com/pon
-00005bb0: 6e68 6964 652f 7061 7463 6877 6f72 6b6c  nhide/patchworkl
-00005bc0: 6962 2f6d 6169 6e2f 696d 672f 6178 3332  ib/main/img/ax32
-00005bd0: 3134 2e70 6e67 2220 7769 6474 683d 2231  14.png" width="1
-00005be0: 3030 3078 3130 3030 223e 0a0a 6060 6070  000x1000">..```p
-00005bf0: 7974 686f 6e0a 6178 3335 3231 345f 7633  ython.ax35214_v3
-00005c00: 203d 2061 7833 3231 345b 2261 7833 225d   = ax3214["ax3"]
-00005c10: 7c61 7835 0a61 7833 3532 3134 5f76 332e  |ax5.ax35214_v3.
-00005c20: 7361 7665 6669 6728 222e 2e2f 696d 672f  savefig("../img/
-00005c30: 6178 3335 3231 345f 7633 2e70 6e67 2229  ax35214_v3.png")
-00005c40: 0a60 6060 0a0a 3c69 6d67 2073 7263 3d22  .```..<img src="
-00005c50: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00005c60: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00005c70: 6d2f 706f 6e6e 6869 6465 2f70 6174 6368  m/ponnhide/patch
-00005c80: 776f 726b 6c69 622f 6d61 696e 2f69 6d67  worklib/main/img
-00005c90: 2f61 7833 3532 3134 5f76 332e 706e 6722  /ax35214_v3.png"
-00005ca0: 2077 6964 7468 3d22 3130 3030 7831 3030   width="1000x100
-00005cb0: 3022 3e13 130a 0a54 6865 2061 626f 7665  0">....The above
-00005cc0: 2070 6163 6b69 6e67 2070 726f 6365 7373   packing process
-00005cd0: 2061 6c6c 6f77 7320 7468 6520 6178 6573   allows the axes
-00005ce0: 206f 6620 7468 6520 6f62 6a65 6374 7320   of the objects 
-00005cf0: 746f 2062 6520 6163 6375 7261 7465 6c79  to be accurately
-00005d00: 2061 6c69 676e 6564 2077 6974 6820 6561   aligned with ea
-00005d10: 6368 206f 7468 6572 2e20 4163 7475 616c  ch other. Actual
-00005d20: 6c79 2c20 696e 2022 6178 3335 3231 3422  ly, in "ax35214"
-00005d30: 2061 6e64 2022 6178 3335 3231 345f 7632   and "ax35214_v2
-00005d40: 222c 2074 6865 2062 6f74 746f 6d20 6178  ", the bottom ax
-00005d50: 6973 206c 696e 6573 206f 6620 6178 3320  is lines of ax3 
-00005d60: 616e 6420 6178 3520 6172 6520 6e6f 7420  and ax5 are not 
-00005d70: 7072 6563 6973 656c 7920 616c 6967 6e65  precisely aligne
-00005d80: 642c 2077 6869 6c65 2069 6e20 2261 7833  d, while in "ax3
-00005d90: 3532 3134 5f76 3322 2c20 7468 6569 7220  5214_v3", their 
-00005da0: 626f 7474 6f6d 2061 7869 7320 6c69 6e65  bottom axis line
-00005db0: 7320 6172 6520 6578 6163 746c 7920 616c  s are exactly al
-00005dc0: 6967 6e65 642e 2048 6f77 6576 6572 2c20  igned. However, 
-00005dd0: 706c 6561 7365 206e 6f74 6520 7468 6174  please note that
-00005de0: 2074 6869 7320 7061 636b 696e 6720 6d65   this packing me
-00005df0: 7468 6f64 2075 7369 6e67 206c 6162 656c  thod using label
-00005e00: 2069 6e64 6578 696e 6720 6368 616e 6765   indexing change
-00005e10: 7320 6173 7065 6374 2072 6174 696f 7320  s aspect ratios 
-00005e20: 6f66 2074 6865 2042 7269 636b 206f 626a  of the Brick obj
-00005e30: 6563 7473 2074 6f20 6265 2070 6163 6b65  ects to be packe
-00005e40: 6420 6672 6f6d 2074 6865 206f 7269 6769  d from the origi
-00005e50: 6e61 6c20 6f6e 6520 746f 2061 6c69 676e  nal one to align
-00005e60: 2074 6865 6972 2061 7869 7320 6c69 6e65   their axis line
-00005e70: 7320 7769 7468 206f 7468 6572 732e 0a0a  s with others...
-00005e80: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00005e90: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00005ea0: 636f 6e74 656e 742e 636f 6d2f 706f 6e6e  content.com/ponn
-00005eb0: 6869 6465 2f70 6174 6368 776f 726b 6c69  hide/patchworkli
-00005ec0: 622f 6d61 696e 2f69 6d67 2f61 7833 3532  b/main/img/ax352
-00005ed0: 3134 5f77 6c2e 706e 6722 2077 6964 7468  14_wl.png" width
-00005ee0: 3d22 3630 3078 3630 3022 3e0a 0a3c 696d  ="600x600">..<im
-00005ef0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00005f00: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00005f10: 7465 6e74 2e63 6f6d 2f70 6f6e 6e68 6964  tent.com/ponnhid
-00005f20: 652f 7061 7463 6877 6f72 6b6c 6962 2f6d  e/patchworklib/m
-00005f30: 6169 6e2f 696d 672f 6178 3335 3231 345f  ain/img/ax35214_
-00005f40: 7632 5f77 6c2e 706e 6722 2077 6964 7468  v2_wl.png" width
-00005f50: 3d22 3630 3078 3630 3022 3e0a 0a3c 696d  ="600x600">..<im
-00005f60: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00005f70: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00005f80: 7465 6e74 2e63 6f6d 2f70 6f6e 6e68 6964  tent.com/ponnhid
-00005f90: 652f 7061 7463 6877 6f72 6b6c 6962 2f6d  e/patchworklib/m
-00005fa0: 6169 6e2f 696d 672f 6178 3335 3231 345f  ain/img/ax35214_
-00005fb0: 7633 5f77 6c2e 706e 6722 2077 6964 7468  v3_wl.png" width
-00005fc0: 3d22 3630 3078 3630 3022 3e0a 0a3c 2f64  ="600x600">..</d
-00005fd0: 6574 6169 6c73 3e0a                      etails>.
+00000310: 7470 6c6f 746c 6962 2028 3e3d 332e 3429  tplotlib (>=3.4)
+00000320: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000330: 7061 6e64 6173 2028 3e3d 302e 3234 290a  pandas (>=0.24).
+00000340: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
+00000350: 756d 7079 2028 3e3d 312e 3136 290a 5265  umpy (>=1.16).Re
+00000360: 7175 6972 6573 2d44 6973 743a 2064 696c  quires-Dist: dil
+00000370: 6c0a 5265 7175 6972 6573 2d44 6973 743a  l.Requires-Dist:
+00000380: 2073 6561 626f 726e 0a52 6571 7569 7265   seaborn.Require
+00000390: 732d 4469 7374 3a20 706c 6f74 6e69 6e65  s-Dist: plotnine
+000003a0: 2028 3c3d 302e 3132 2e34 290a 0a23 2070   (<=0.12.4)..# p
+000003b0: 6174 6368 776f 726b 6c69 620a 5b50 6174  atchworklib.[Pat
+000003c0: 6368 776f 726b 6c69 625d 2868 7474 7073  chworklib](https
+000003d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
+000003e0: 6e6e 6869 6465 2f70 6174 6368 776f 726b  nnhide/patchwork
+000003f0: 6c69 6229 2069 7320 6120 756e 6976 6572  lib) is a univer
+00000400: 7361 6c20 636f 6d70 6f73 6572 206f 6620  sal composer of 
+00000410: 6d61 7470 6c6f 746c 6962 2d72 656c 6174  matplotlib-relat
+00000420: 6564 2070 6c6f 7473 2028 7369 6d70 6c65  ed plots (simple
+00000430: 206d 6174 706c 6f74 6c69 6220 706c 6f74   matplotlib plot
+00000440: 732c 2053 6561 626f 726e 2070 6c6f 7473  s, Seaborn plots
+00000450: 2028 626f 7468 2061 7869 732d 6c65 7665   (both axis-leve
+00000460: 6c20 616e 6420 6669 6775 7265 2d6c 6576  l and figure-lev
+00000470: 656c 292c 2061 6e64 2070 6c6f 746e 696e  el), and plotnin
+00000480: 6520 706c 6f74 7329 2e20 5468 6973 206c  e plots). This l
+00000490: 6962 7261 7279 2069 7320 696e 7370 6972  ibrary is inspir
+000004a0: 6564 2062 7920 5b70 6174 6368 776f 726b  ed by [patchwork
+000004b0: 5d28 6874 7470 733a 2f2f 7061 7463 6877  ](https://patchw
+000004c0: 6f72 6b2e 6461 7461 2d69 6d61 6769 6e69  ork.data-imagini
+000004d0: 7374 2e63 6f6d 2f29 2066 6f72 2067 6770  st.com/) for ggp
+000004e0: 6c6f 7432 2e20 4163 636f 7264 696e 676c  lot2. Accordingl
+000004f0: 792c 2061 7320 6f72 6967 696e 616c 2070  y, as original p
+00000500: 6174 6368 776f 726b 2c20 7573 6572 7320  atchwork, users 
+00000510: 6361 6e20 6561 7369 6c79 2061 6c69 676e  can easily align
+00000520: 206d 6174 706c 6f74 6c69 6220 706c 6f74   matplotlib plot
+00000530: 7320 7769 7468 206f 6e6c 7920 222f 2220  s with only "/" 
+00000540: 616e 6420 227c 2220 6f70 6572 6174 6f72  and "|" operator
+00000550: 732e 2041 6c74 686f 7567 6820 6120 676f  s. Although a go
+00000560: 6f64 2073 7562 706c 6f74 2063 6f6d 706f  od subplot compo
+00000570: 7365 722c 2022 7375 6270 6c6f 745f 6d6f  ser, "subplot_mo
+00000580: 7361 6963 2220 6973 2070 726f 7669 6465  saic" is provide
+00000590: 6420 6672 6f6d 206d 6174 706c 6f74 6c69  d from matplotli
+000005a0: 6220 666f 726d 616c 6c79 2c20 4920 6265  b formally, I be
+000005b0: 6c69 6576 6520 7468 6520 7761 7920 6f66  lieve the way of
+000005c0: 2070 6174 6368 776f 726b 6c69 6220 6973   patchworklib is
+000005d0: 206d 6f72 6520 7374 7261 6967 6874 666f   more straightfo
+000005e0: 7277 6172 6420 616e 6420 6d6f 7265 2066  rward and more f
+000005f0: 6c65 7869 626c 652e 0a0a 4164 6469 7469  lexible...Additi
+00000600: 6f6e 616c 6c79 2c20 7365 7665 7261 6c20  onally, several 
+00000610: 7468 6972 642d 7061 7274 7920 6c69 6272  third-party libr
+00000620: 6172 6965 7320 6261 7365 6420 6f6e 206d  aries based on m
+00000630: 6174 706c 6f74 6c69 622c 2073 7563 6820  atplotlib, such 
+00000640: 6173 2070 6c6f 746e 696e 6520 616e 6420  as plotnine and 
+00000650: 7365 6162 6f72 6e2c 2070 726f 7669 6465  seaborn, provide
+00000660: 2066 756e 6374 696f 6e73 2074 6f20 6765   functions to ge
+00000670: 6e65 7261 7465 2062 6561 7574 6966 756c  nerate beautiful
+00000680: 2070 6c6f 7473 2077 6974 6820 7369 6d70   plots with simp
+00000690: 6c65 2070 7974 686f 6e20 636f 6465 732c  le python codes,
+000006a0: 2062 7574 206d 616e 7920 6f66 2074 686f   but many of tho
+000006b0: 7365 2070 6c6f 7473 2063 616e 6e6f 7420  se plots cannot 
+000006c0: 6265 2068 616e 646c 6564 2061 7320 6d61  be handled as ma
+000006d0: 7470 6c6f 746c 6962 2073 7562 706c 6f74  tplotlib subplot
+000006e0: 732e 2054 6865 7265 666f 7265 2c20 7468  s. Therefore, th
+000006f0: 6569 7220 706c 6163 656d 656e 7420 6d75  eir placement mu
+00000700: 7374 2062 6520 6164 6a75 7374 6564 206d  st be adjusted m
+00000710: 616e 7561 6c6c 792e 204e 6f77 2c20 7363  anually. Now, sc
+00000720: 6965 6e74 6973 7473 2073 7065 6e64 2074  ientists spend t
+00000730: 6865 6972 2076 616c 7561 626c 6520 7469  heir valuable ti
+00000740: 6d65 2061 7272 616e 6769 6e67 2066 6967  me arranging fig
+00000750: 7572 6573 2e0a 0a50 6174 6368 776f 726b  ures...Patchwork
+00000760: 6c69 6220 7072 6f76 6964 6573 2061 2073  lib provides a s
+00000770: 6f6c 7574 696f 6e20 666f 7220 7468 6520  olution for the 
+00000780: 7072 6f62 6c65 6d2e 2042 7920 7573 696e  problem. By usin
+00000790: 6720 7061 7463 6877 6f72 6b6c 6962 2c20  g patchworklib, 
+000007a0: 616e 7920 6b69 6e64 206f 6620 7365 6162  any kind of seab
+000007b0: 6f72 6e20 616e 6420 706c 6f74 6e69 6e65  orn and plotnine
+000007c0: 2070 6c6f 7473 2063 616e 2062 6520 6861   plots can be ha
+000007d0: 6e64 6c65 6420 6173 206d 6174 706c 6f74  ndled as matplot
+000007e0: 6c69 6220 7375 6270 6c6f 7473 2e0a 0a23  lib subplots...#
+000007f0: 2323 204a 6f69 6e20 4f75 7220 5465 616d  ## Join Our Team
+00000800: 3a20 4269 6f69 6e66 6f72 6d61 7469 6373  : Bioinformatics
+00000810: 2052 6573 6561 7263 6865 7220 5761 6e74   Researcher Want
+00000820: 6564 2e0a 5765 2061 7265 2063 7572 7265  ed..We are curre
+00000830: 6e74 6c79 2073 6565 6b69 6e67 2061 2073  ntly seeking a s
+00000840: 6b69 6c6c 6564 2072 6573 6561 7263 6865  killed researche
+00000850: 7220 7769 7468 2065 7870 6572 7469 7365  r with expertise
+00000860: 2069 6e20 6269 6f69 6e66 6f72 6d61 7469   in bioinformati
+00000870: 6373 2074 6f20 6a6f 696e 206f 7572 206c  cs to join our l
+00000880: 6162 2e20 200a 466f 7220 6d6f 7265 2064  ab.  .For more d
+00000890: 6574 6169 6c73 2061 6e64 2074 6f20 6170  etails and to ap
+000008a0: 706c 792c 2070 6c65 6173 6520 7669 7369  ply, please visi
+000008b0: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
+000008c0: 5b55 524c 5d28 6874 7470 733a 2f2f 7072  [URL](https://pr
+000008d0: 696d 652e 6f73 616b 612d 752e 6163 2e6a  ime.osaka-u.ac.j
+000008e0: 702f 6361 7265 6572 732f 696d 6167 6573  p/careers/images
+000008f0: 2f43 5245 5354 5f72 6563 7275 6974 5f65  /CREST_recruit_e
+00000900: 6e5f 3230 3233 3131 3230 2e70 6466 292e  n_20231120.pdf).
+00000910: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000920: 6e0a 466f 7220 6e6f 726d 616c 2075 7365  n.For normal use
+00000930: 7273 2c20 7765 2072 6563 6f6d 6d65 6e64  rs, we recommend
+00000940: 6564 2079 6f75 2074 6f20 696e 7374 616c  ed you to instal
+00000950: 6c20 7468 6520 6f66 6669 6369 616c 2072  l the official r
+00000960: 656c 6561 7365 2061 7320 666f 6c6c 6f77  elease as follow
+00000970: 732e 2020 0a60 7069 7020 696e 7374 616c  s.  .`pip instal
+00000980: 6c20 7061 7463 6877 6f72 6b6c 6962 600a  l patchworklib`.
+00000990: 0a49 6620 796f 7520 7761 6e74 2074 6f20  .If you want to 
+000009a0: 7573 6520 6465 7665 6c6f 706d 656e 7461  use developmenta
+000009b0: 6c20 7665 7273 696f 6e2c 2069 7420 6361  l version, it ca
+000009c0: 6e20 6265 2069 6e73 7461 6c6c 6564 2075  n be installed u
+000009d0: 7369 6e67 2074 6865 2066 6f6c 6c6f 7769  sing the followi
+000009e0: 6e67 2073 696e 676c 6520 636f 6d6d 616e  ng single comman
+000009f0: 643a 2020 0a60 7069 7020 696e 7374 616c  d:  .`pip instal
+00000a00: 6c20 6769 742b 6874 7470 733a 2f2f 6769  l git+https://gi
+00000a10: 7468 7562 2e63 6f6d 2f70 6f6e 6e68 6964  thub.com/ponnhid
+00000a20: 652f 7061 7463 6877 6f72 6b6c 6962 2e67  e/patchworklib.g
+00000a30: 6974 600a 0a23 2320 4e65 7773 0a23 2323  it`..## News.###
+00000a40: 2320 3130 3233 3230 3233 3a20 7665 7273  # 10232023: vers
+00000a50: 696f 6e20 302e 362e 3320 6973 2072 656c  ion 0.6.3 is rel
+00000a60: 6561 7365 642e 200a 2d20 5365 6162 6f72  eased. .- Seabor
+00000a70: 6e20 7630 2e31 332e 3020 6973 206e 6f77  n v0.13.0 is now
+00000a80: 2073 7570 706f 7274 6564 2e0a 2d20 4920   supported..- I 
+00000a90: 6861 7665 2063 6f6e 6669 726d 6564 2070  have confirmed p
+00000aa0: 6174 6368 776f 726b 6c69 6220 7374 696c  atchworklib stil
+00000ab0: 6c20 776f 726b 7320 666f 7270 6c6f 746e  l works forplotn
+00000ac0: 696e 6520 7630 2e31 322e 332e 200a 0a23  ine v0.12.3. ..#
+00000ad0: 2323 2320 3035 3136 3230 3233 3a20 7665  ### 05162023: ve
+00000ae0: 7273 696f 6e20 302e 362e 3120 7761 7320  rsion 0.6.1 was 
+00000af0: 7265 6c65 6173 6564 2e0a 2d20 4920 636f  released..- I co
+00000b00: 756c 6420 6e6f 7420 6675 6c6c 7920 7375  uld not fully su
+00000b10: 7070 6f72 7420 706c 6f74 6e69 6e65 2076  pport plotnine v
+00000b20: 6572 7369 6f6e 2030 2e31 322e 3120 2849  ersion 0.12.1 (I
+00000b30: 7420 776f 726b 732c 2062 7574 2070 6174  t works, but pat
+00000b40: 6368 776f 726b 6c69 6220 6172 7261 6e67  chworklib arrang
+00000b50: 656d 656e 7420 7265 7375 6c74 7320 6172  ement results ar
+00000b60: 6520 6e6f 7420 6173 2065 7870 6563 7465  e not as expecte
+00000b70: 6429 2e20 4d61 7962 652c 2049 2077 696c  d). Maybe, I wil
+00000b80: 6c20 646f 206e 6f74 2073 7570 706f 7274  l do not support
+00000b90: 2070 6c6f 746e 696e 6520 696e 2074 6865   plotnine in the
+00000ba0: 2066 7574 7572 652e 200a 2d20 4272 6963   future. .- Bric
+00000bb0: 6b73 206f 626a 6563 7420 6761 696e 6564  ks object gained
+00000bc0: 2074 6865 206e 6577 206d 6574 686f 6473   the new methods
+00000bd0: 2060 616c 6967 6e5f 786c 6162 656c 7360   `align_xlabels`
+00000be0: 2061 6e64 2020 6061 6c69 676e 5f79 6c61   and  `align_yla
+00000bf0: 6265 6c73 602c 2077 6869 6368 2068 656c  bels`, which hel
+00000c00: 7020 7573 6572 7320 616c 6967 6e20 782f  p users align x/
+00000c10: 7920 6c61 6265 6c73 206f 6620 7468 6520  y labels of the 
+00000c20: 6769 7665 6e20 4272 6963 6b20 6f62 6a65  given Brick obje
+00000c30: 6374 2e0a 2d20 5468 6520 6e65 7720 6172  ct..- The new ar
+00000c40: 6775 6d65 6e74 2060 6571 7561 6c5f 7370  gument `equal_sp
+00000c50: 6163 696e 6760 2077 6173 2061 6464 6564  acing` was added
+00000c60: 2074 6f20 7468 6520 7374 6163 6b20 6675   to the stack fu
+00000c70: 6e63 7469 6f6e 2e20 4966 2074 6869 7320  nction. If this 
+00000c80: 7661 6c75 6520 6973 2060 5472 7565 602c  value is `True`,
+00000c90: 2061 7865 7320 626f 756e 6469 6e67 2d62   axes bounding-b
+00000ca0: 6f78 6573 2073 686f 756c 6420 6265 2070  oxes should be p
+00000cb0: 6c61 6365 6420 7769 7468 2065 7175 616c  laced with equal
+00000cc0: 2073 7061 6369 6e67 2062 6574 7765 656e   spacing between
+00000cd0: 2074 6865 6d2e 204f 7468 6572 7769 7365   them. Otherwise
+00000ce0: 2c20 6465 7065 6e64 696e 6720 6f6e 2074  , depending on t
+00000cf0: 6865 2074 6578 7420 7661 6c75 6573 206f  he text values o
+00000d00: 6620 782f 7920 7469 636b 206c 6162 656c  f x/y tick label
+00000d10: 7320 616e 6420 782f 7920 6c61 6265 6c73  s and x/y labels
+00000d20: 2c20 7468 6579 206d 6179 206e 6f74 2061  , they may not a
+00000d30: 6c77 6179 7320 6265 2065 7175 616c 6c79  lways be equally
+00000d40: 2073 7061 6365 642e 0a2d 2043 6c6f 7365   spaced..- Close
+00000d50: 6420 616e 6420 6d61 7962 6520 736f 6c76  d and maybe solv
+00000d60: 6564 2074 6865 2069 7373 7565 205b 2241  ed the issue ["A
+00000d70: 6c69 676e 206c 6162 656c 7320 6f66 2042  lign labels of B
+00000d80: 7269 636b 7320 7768 656e 2073 7562 706c  ricks when subpl
+00000d90: 6f74 2061 7865 7320 6172 6520 616c 6967  ot axes are alig
+00000da0: 6e65 642e 2023 3430 225d 2868 7474 7073  ned. #40"](https
+00000db0: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
+00000dc0: 6e6e 6869 6465 2f70 6174 6368 776f 726b  nnhide/patchwork
+00000dd0: 6c69 622f 6973 7375 6573 2f34 3029 200a  lib/issues/40) .
+00000de0: 2d20 436c 6f73 6564 2061 6e64 206d 6179  - Closed and may
+00000df0: 6265 2073 6f6c 7665 6420 7468 6520 6973  be solved the is
+00000e00: 7375 6520 5b22 446f 6573 6e27 7420 776f  sue ["Doesn't wo
+00000e10: 726b 2077 6974 6820 506c 6f74 6e69 6e65  rk with Plotnine
+00000e20: 2053 6561 626f 726e 2054 6865 6d65 2e20   Seaborn Theme. 
+00000e30: 2333 3722 5d28 6874 7470 733a 2f2f 6769  #37"](https://gi
+00000e40: 7468 7562 2e63 6f6d 2f70 6f6e 6e68 6964  thub.com/ponnhid
+00000e50: 652f 7061 7463 6877 6f72 6b6c 6962 2f69  e/patchworklib/i
+00000e60: 7373 7565 732f 3337 290a 2d20 436c 6f73  ssues/37).- Clos
+00000e70: 6564 2061 6e64 206d 6179 6265 2073 6f6c  ed and maybe sol
+00000e80: 7665 6420 7468 6520 6973 7375 6520 5b22  ved the issue ["
+00000e90: 5468 6520 706f 7369 7469 6f6e 206f 6620  The position of 
+00000ea0: 7468 6520 7469 746c 6520 6361 6e6e 6f74  the title cannot
+00000eb0: 2062 6520 7365 7420 696e 2070 6c6f 746e   be set in plotn
+00000ec0: 696e 652e 2023 3336 225d 2868 7474 7073  ine. #36"](https
+00000ed0: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
+00000ee0: 6e6e 6869 6465 2f70 6174 6368 776f 726b  nnhide/patchwork
+00000ef0: 6c69 622f 6973 7375 6573 2f33 3629 0a0a  lib/issues/36)..
+00000f00: 3c64 6574 6169 6c73 3e20 0a0a 3c73 756d  <details> ..<sum
+00000f10: 6d61 7279 3e20 3c68 323e 2043 6861 6e67  mary> <h2> Chang
+00000f20: 6520 6c6f 6720 3c2f 6832 3e20 3c2f 7375  e log </h2> </su
+00000f30: 6d6d 6172 793e 0a23 2323 2320 3132 3038  mmary>.#### 1208
+00000f40: 3230 3232 3a20 7665 7273 696f 6e20 302e  2022: version 0.
+00000f50: 352e 3020 7761 7320 7265 6c65 6173 6564  5.0 was released
+00000f60: 2e0a 2d20 4e65 7720 6f70 6572 6174 6f72  ..- New operator
+00000f70: 732c 2022 2b22 2061 6e64 2022 2d22 2c20  s, "+" and "-", 
+00000f80: 7765 7265 2061 6464 6564 2e20 0a2d 2070  were added. .- p
+00000f90: 6c6f 746e 696e 6520 3e20 7630 2e31 302e  lotnine > v0.10.
+00000fa0: 7820 6973 206e 6f77 2073 7570 706f 7274  x is now support
+00000fb0: 6564 2e0a 2d20 506c 6f74 7320 6765 6e65  ed..- Plots gene
+00000fc0: 7261 7465 6420 6279 206f 626a 6563 742d  rated by object-
+00000fd0: 6f72 6965 6e74 6564 2073 6561 626f 726e  oriented seaborn
+00000fe0: 2069 6e74 6572 6661 6365 2063 616e 206e   interface can n
+00000ff0: 6f77 2062 6520 6861 6e64 6c65 6420 6279  ow be handled by
+00001000: 2070 6174 6368 776f 726b 6c69 622e 0a2d   patchworklib..-
+00001010: 2044 6573 6372 6970 7469 6f6e 7320 6f66   Descriptions of
+00001020: 2065 6163 6820 6675 6e63 7469 6f6e 2061   each function a
+00001030: 6e64 2063 6c61 7373 2070 726f 7669 6465  nd class provide
+00001040: 6420 696e 2070 6174 6368 776f 726b 6c69  d in patchworkli
+00001050: 6220 7761 7320 6164 6465 6420 746f 2074  b was added to t
+00001060: 6869 7320 7265 706f 7369 746f 7279 2e20  his repository. 
+00001070: 4966 2079 6f75 2077 616e 7420 746f 206b  If you want to k
+00001080: 6e6f 7720 686f 7720 746f 2075 7365 2070  now how to use p
+00001090: 6174 6368 776f 726b 6c69 6220 696e 2064  atchworklib in d
+000010a0: 6574 6169 6c2c 2070 6c65 6173 6520 7365  etail, please se
+000010b0: 6520 5b41 5049 2e6d 645d 2868 7474 7073  e [API.md](https
+000010c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
+000010d0: 6e6e 6869 6465 2f70 6174 6368 776f 726b  nnhide/patchwork
+000010e0: 6c69 622f 626c 6f62 2f6d 6169 6e2f 4150  lib/blob/main/AP
+000010f0: 492e 6d64 292e 0a2d 2055 7064 6174 6564  I.md)..- Updated
+00001100: 205b 7061 7463 6877 6f72 6b6c 6962 2d65   [patchworklib-e
+00001110: 7861 6d70 6c65 735d 2868 7474 7073 3a2f  xamples](https:/
+00001120: 2f67 6974 6875 622e 636f 6d2f 706f 6e6e  /github.com/ponn
+00001130: 6869 6465 2f70 6174 6368 776f 726b 6c69  hide/patchworkli
+00001140: 622d 6578 616d 706c 6573 290a 0a23 2323  b-examples)..###
+00001150: 2320 3038 3135 3230 3232 3a20 5665 7273  # 08152022: Vers
+00001160: 696f 6e20 302e 342e 3720 7761 7320 7265  ion 0.4.7 was re
+00001170: 6c65 6173 6564 2e20 0a2d 2041 2066 6577  leased. .- A few
+00001180: 2062 7567 7320 7765 7265 2066 6978 6564   bugs were fixed
+00001190: 2e0a 2d20 4164 6420 696e 7365 7420 6675  ..- Add inset fu
+000011a0: 6e63 7469 6f6e 2e20 706c 6561 7365 2073  nction. please s
+000011b0: 6565 2074 6865 2066 6f6c 6c6f 7769 6e67  ee the following
+000011c0: 2065 7861 6d70 6c65 2e20 0a2d 2041 6464   example. .- Add
+000011d0: 2060 6b65 6570 5f61 7370 6563 7460 2070   `keep_aspect` p
+000011e0: 6172 616d 6574 6572 2074 6f20 6068 7374  arameter to `hst
+000011f0: 6163 6b60 2061 6e64 2060 7673 7461 636b  ack` and `vstack
+00001200: 6020 6675 6e63 6974 6f6e 2e0a 2d20 4578  ` funciton..- Ex
+00001210: 616d 706c 6520 636f 6465 7320 7765 7265  ample codes were
+00001220: 206d 6f76 6564 2074 6f20 5b70 6174 6368   moved to [patch
+00001230: 776f 726b 6c69 622d 6578 616d 706c 6573  worklib-examples
+00001240: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001250: 2e63 6f6d 2f70 6f6e 6e68 6964 652f 7061  .com/ponnhide/pa
+00001260: 7463 6877 6f72 6b6c 6962 2d65 7861 6d70  tchworklib-examp
+00001270: 6c65 7329 0a0a 3c64 6574 6169 6c73 3e20  les)..<details> 
+00001280: 0a3c 7375 6d6d 6172 793e 2043 7265 6174  .<summary> Creat
+00001290: 6520 616e 2069 6e73 6574 2065 6c65 6d65  e an inset eleme
+000012a0: 6e74 203c 2f73 756d 6d61 7279 3e0a 0a60  nt </summary>..`
+000012b0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+000012c0: 7061 7463 6877 6f72 6b6c 6962 2061 7320  patchworklib as 
+000012d0: 7077 0a66 726f 6d20 706c 6f74 6e69 6e65  pw.from plotnine
+000012e0: 2069 6d70 6f72 7420 2a0a 6672 6f6d 2070   import *.from p
+000012f0: 6c6f 746e 696e 652e 6461 7461 2069 6d70  lotnine.data imp
+00001300: 6f72 7420 2a0a 0a67 3120 203d 2070 772e  ort *..g1  = pw.
+00001310: 6c6f 6164 5f67 6770 6c6f 7428 6767 706c  load_ggplot(ggpl
+00001320: 6f74 286d 7463 6172 7329 202b 2067 656f  ot(mtcars) + geo
+00001330: 6d5f 706f 696e 7428 6165 7328 226d 7067  m_point(aes("mpg
+00001340: 222c 2022 6469 7370 2229 292c 6669 6773  ", "disp")),figs
+00001350: 697a 653d 2834 2c20 3229 290a 6732 2020  ize=(4, 2)).g2  
+00001360: 3d20 7077 2e6c 6f61 645f 6767 706c 6f74  = pw.load_ggplot
+00001370: 2867 6770 6c6f 7428 6d74 6361 7273 2920  (ggplot(mtcars) 
+00001380: 2b20 6765 6f6d 5f62 6f78 706c 6f74 2861  + geom_boxplot(a
+00001390: 6573 2822 6765 6172 222c 2022 6469 7370  es("gear", "disp
+000013a0: 222c 2067 726f 7570 203d 2022 6765 6172  ", group = "gear
+000013b0: 2229 2920 2b20 7468 656d 655f 636c 6173  ")) + theme_clas
+000013c0: 7369 6328 2929 0a67 3132 203d 2070 772e  sic()).g12 = pw.
+000013d0: 696e 7365 7428 6731 2c67 3229 0a67 3132  inset(g1,g2).g12
+000013e0: 2e73 6176 6566 6967 2829 0a60 6060 0a3c  .savefig().```.<
+000013f0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001400: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001410: 6f6e 7465 6e74 2e63 6f6d 2f70 6f6e 6e68  ontent.com/ponnh
+00001420: 6964 652f 7061 7463 6877 6f72 6b6c 6962  ide/patchworklib
+00001430: 2f6d 6169 6e2f 696d 672f 696e 7365 745f  /main/img/inset_
+00001440: 706c 6f74 6e69 6e65 2e70 6e67 2220 7769  plotnine.png" wi
+00001450: 6474 683d 2236 3030 7836 3030 223e 0a0a  dth="600x600">..
+00001460: 6060 6070 7974 686f 6e0a 6731 3220 3d20  ```python.g12 = 
+00001470: 7077 2e69 6e73 6574 2867 312c 6732 2c20  pw.inset(g1,g2, 
+00001480: 6c6f 633d 226c 6f77 6572 206c 6566 7422  loc="lower left"
+00001490: 2c20 6872 6174 696f 3d30 2e34 2c20 7772  , hratio=0.4, wr
+000014a0: 6174 696f 3d30 2e32 290a 6731 322e 7361  atio=0.2).g12.sa
+000014b0: 7665 6669 6728 2269 6e73 6574 5f70 6c6f  vefig("inset_plo
+000014c0: 746e 696e 6532 2e70 6e67 2229 0a60 6060  tnine2.png").```
+000014d0: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+000014e0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000014f0: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6f6e  rcontent.com/pon
+00001500: 6e68 6964 652f 7061 7463 6877 6f72 6b6c  nhide/patchworkl
+00001510: 6962 2f6d 6169 6e2f 696d 672f 696e 7365  ib/main/img/inse
+00001520: 745f 706c 6f74 6e69 6e65 322e 706e 6722  t_plotnine2.png"
+00001530: 2077 6964 7468 3d22 3630 3078 3630 3022   width="600x600"
+00001540: 3e0a 0a3c 2f64 6574 6169 6c73 3e0a 0a23  >..</details>..#
+00001550: 2323 2320 3038 3039 3230 3232 3a20 5665  ### 08092022: Ve
+00001560: 7273 696f 6e20 302e 342e 3620 7761 7320  rsion 0.4.6 was 
+00001570: 7265 6c65 6173 6564 2e20 0a2d 2041 2066  released. .- A f
+00001580: 6577 2062 7567 7320 7765 7265 2066 6978  ew bugs were fix
+00001590: 6564 2028 5365 6520 6973 7375 6520 5b23  ed (See issue [#
+000015a0: 3138 5d28 6874 7470 733a 2f2f 6769 7468  18](https://gith
+000015b0: 7562 2e63 6f6d 2f70 6f6e 6e68 6964 652f  ub.com/ponnhide/
+000015c0: 7061 7463 6877 6f72 6b6c 6962 2f69 7373  patchworklib/iss
+000015d0: 7565 732f 3138 2929 2e20 2020 0a2d 2050  ues/18)).   .- P
+000015e0: 6c6f 7474 696e 6720 7370 6565 6420 7761  lotting speed wa
+000015f0: 7320 696d 7072 6f76 6564 2e0a 0a23 2323  s improved...###
+00001600: 2320 3037 3230 3230 3232 3a20 5665 7273  # 07202022: Vers
+00001610: 696f 6e20 302e 342e 3520 7761 7320 7265  ion 0.4.5 was re
+00001620: 6c65 6173 6564 2e20 0a2d 2041 2066 6577  leased. .- A few
+00001630: 2062 7567 7320 7765 7265 2066 6978 6564   bugs were fixed
+00001640: 2e0a 2d20 4d6f 6469 6669 6564 2066 756e  ..- Modified fun
+00001650: 6374 696f 6e73 2072 656c 6174 696e 6720  ctions relating 
+00001660: 746f 2074 6865 2069 6e68 6572 6974 616e  to the inheritan
+00001670: 6365 206f 6620 7468 6520 6767 706c 6f74  ce of the ggplot
+00001680: 2074 6865 6d65 2e20 4966 2079 6f75 2075   theme. If you u
+00001690: 7365 2070 6174 6368 776f 726b 6c69 6220  se patchworklib 
+000016a0: 666f 7220 6861 6e64 6c69 6e67 2070 6c6f  for handling plo
+000016b0: 746e 696e 6520 706c 6f74 732c 2070 6c65  tnine plots, ple
+000016c0: 6173 6520 646f 2075 7064 6174 652e 0a2d  ase do update..-
+000016d0: 2057 6865 6e20 7370 6563 6966 7969 6e67   When specifying
+000016e0: 2061 2070 6c6f 7420 2842 7269 636b 206f   a plot (Brick o
+000016f0: 626a 6563 7429 2069 6e20 4272 6963 6b73  bject) in Bricks
+00001700: 206f 626a 6563 742c 2079 6f75 2063 616e   object, you can
+00001710: 2073 7065 6369 6679 2074 6865 2042 7269   specify the Bri
+00001720: 636b 206f 626a 6563 7420 6469 7265 6374  ck object direct
+00001730: 6c79 2069 6e73 7465 6164 206f 6620 7468  ly instead of th
+00001740: 6520 6c61 6265 6c20 6e61 6d65 206f 6620  e label name of 
+00001750: 7468 6520 4272 6963 6b20 6f62 6a65 6374  the Brick object
+00001760: 2e20 506c 6561 7365 2073 6565 2074 6865  . Please see the
+00001770: 2066 6f6c 6c6f 7769 6e67 2065 7861 6d70   following examp
+00001780: 6c65 2e20 0a3c 6465 7461 696c 733e 200a  le. .<details> .
+00001790: 3c73 756d 6d61 7279 3e20 416c 6967 6e6d  <summary> Alignm
+000017a0: 656e 7420 6f66 2061 2070 6c6f 7469 6e65  ent of a plotine
+000017b0: 2070 6c6f 7420 6279 2073 7065 6369 6679   plot by specify
+000017c0: 696e 6720 6120 4272 6963 6b20 6f62 6a65  ing a Brick obje
+000017d0: 6374 2069 6e20 7468 6520 4272 6963 6b73  ct in the Bricks
+000017e0: 206f 626a 6563 742e 203c 2f73 756d 6d61   object. </summa
+000017f0: 7279 3e0a 0a60 6060 7079 7468 6f6e 0a69  ry>..```python.i
+00001800: 6d70 6f72 7420 7061 7463 6877 6f72 6b6c  mport patchworkl
+00001810: 6962 2061 7320 7077 0a66 726f 6d20 706c  ib as pw.from pl
+00001820: 6f74 6e69 6e65 2069 6d70 6f72 7420 2a0a  otnine import *.
+00001830: 6672 6f6d 2070 6c6f 746e 696e 652e 6461  from plotnine.da
+00001840: 7461 2069 6d70 6f72 7420 2a0a 0a67 3120  ta import *..g1 
+00001850: 3d20 7077 2e6c 6f61 645f 6767 706c 6f74  = pw.load_ggplot
+00001860: 2867 6770 6c6f 7428 6d70 672c 2061 6573  (ggplot(mpg, aes
+00001870: 2878 3d27 6374 7927 2c20 636f 6c6f 723d  (x='cty', color=
+00001880: 2764 7276 272c 2066 696c 6c3d 2764 7276  'drv', fill='drv
+00001890: 2729 2920 2b0a 2020 2020 2020 2020 2020  ')) +.          
+000018a0: 2020 2020 2020 2020 2020 6765 6f6d 5f64            geom_d
+000018b0: 656e 7369 7479 2861 6573 2879 3d61 6674  ensity(aes(y=aft
+000018c0: 6572 5f73 7461 7428 2763 6f75 6e74 2729  er_stat('count')
+000018d0: 292c 2061 6c70 6861 3d30 2e31 2920 2b0a  ), alpha=0.1) +.
+000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018f0: 2020 2020 7363 616c 655f 636f 6c6f 725f      scale_color_
+00001900: 6469 7363 7265 7465 2867 7569 6465 3d46  discrete(guide=F
+00001910: 616c 7365 2920 2b0a 2020 2020 2020 2020  alse) +.        
+00001920: 2020 2020 2020 2020 2020 2020 7468 656d              them
+00001930: 6528 6178 6973 5f74 6963 6b73 5f6d 616a  e(axis_ticks_maj
+00001940: 6f72 5f78 3d65 6c65 6d65 6e74 5f62 6c61  or_x=element_bla
+00001950: 6e6b 2829 2c0a 2020 2020 2020 2020 2020  nk(),.          
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 6178 6973 5f74 6578 745f 7820 3d65 6c65  axis_text_x =ele
+00001980: 6d65 6e74 5f62 6c61 6e6b 2829 2c0a 2020  ment_blank(),.  
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2020 2020 2020 2020 6178 6973 5f74 6974          axis_tit
+000019b0: 6c65 5f78 3d65 6c65 6d65 6e74 5f62 6c61  le_x=element_bla
+000019c0: 6e6b 2829 2c0a 2020 2020 2020 2020 2020  nk(),.          
+000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019e0: 6178 6973 5f74 6578 745f 7920 3d65 6c65  axis_text_y =ele
+000019f0: 6d65 6e74 5f74 6578 7428 7369 7a65 3d31  ment_text(size=1
+00001a00: 3229 2c0a 2020 2020 2020 2020 2020 2020  2),.            
+00001a10: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+00001a20: 6973 5f74 6974 6c65 5f79 3d65 6c65 6d65  is_title_y=eleme
+00001a30: 6e74 5f74 6578 7428 7369 7a65 3d31 3429  nt_text(size=14)
+00001a40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001a50: 2020 2020 2020 2020 2020 2020 6c65 6765              lege
+00001a60: 6e64 5f70 6f73 6974 696f 6e3d 226e 6f6e  nd_position="non
+00001a70: 6522 292c 0a20 2020 2020 2020 2020 2020  e"),.           
+00001a80: 2020 2020 2020 2020 2066 6967 7369 7a65           figsize
+00001a90: 3d28 342c 3129 290a 0a67 3220 3d20 7077  =(4,1))..g2 = pw
+00001aa0: 2e6c 6f61 645f 6767 706c 6f74 2867 6770  .load_ggplot(ggp
+00001ab0: 6c6f 7428 6d70 672c 2061 6573 2878 3d27  lot(mpg, aes(x='
+00001ac0: 6877 7927 2c20 636f 6c6f 723d 2764 7276  hwy', color='drv
+00001ad0: 272c 2066 696c 6c3d 2764 7276 2729 2920  ', fill='drv')) 
+00001ae0: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
+00001af0: 2020 2020 2020 6765 6f6d 5f64 656e 7369        geom_densi
+00001b00: 7479 2861 6573 2879 3d61 6674 6572 5f73  ty(aes(y=after_s
+00001b10: 7461 7428 2763 6f75 6e74 2729 292c 2061  tat('count')), a
+00001b20: 6c70 6861 3d30 2e31 2920 2b0a 2020 2020  lpha=0.1) +.    
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b40: 636f 6f72 645f 666c 6970 2829 202b 0a20  coord_flip() +. 
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 2020 2074 6865 6d65 2861 7869 735f 7469     theme(axis_ti
+00001b70: 636b 735f 6d61 6a6f 725f 793d 656c 656d  cks_major_y=elem
+00001b80: 656e 745f 626c 616e 6b28 292c 0a20 2020  ent_blank(),.   
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ba0: 2020 2020 2020 2061 7869 735f 7465 7874         axis_text
+00001bb0: 5f79 203d 656c 656d 656e 745f 626c 616e  _y =element_blan
+00001bc0: 6b28 292c 0a20 2020 2020 2020 2020 2020  k(),.           
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00001be0: 7869 735f 7469 746c 655f 793d 656c 656d  xis_title_y=elem
+00001bf0: 656e 745f 626c 616e 6b28 292c 0a20 2020  ent_blank(),.   
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 2020 2061 7869 735f 7465 7874         axis_text
+00001c20: 5f78 203d 656c 656d 656e 745f 7465 7874  _x =element_text
+00001c30: 2873 697a 653d 3132 292c 0a20 2020 2020  (size=12),.     
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 2020 2020 2061 7869 735f 7469 746c 655f       axis_title_
+00001c60: 783d 656c 656d 656e 745f 7465 7874 2873  x=element_text(s
+00001c70: 697a 653d 3134 290a 2020 2020 2020 2020  ize=14).        
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00001ca0: 2020 2020 2020 2020 6669 6773 697a 653d          figsize=
+00001cb0: 2831 2c34 2929 0a0a 6733 203d 2070 772e  (1,4))..g3 = pw.
+00001cc0: 6c6f 6164 5f67 6770 6c6f 7428 6767 706c  load_ggplot(ggpl
+00001cd0: 6f74 286d 7067 2920 2b0a 2020 2020 2020  ot(mpg) +.      
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 6765                ge
+00001cf0: 6f6d 5f70 6f69 6e74 2861 6573 2878 3d22  om_point(aes(x="
+00001d00: 6374 7922 2c20 793d 2268 7779 222c 2063  cty", y="hwy", c
+00001d10: 6f6c 6f72 3d22 6472 7622 2929 202b 0a20  olor="drv")) +. 
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2073 6361 6c65 5f63 6f6c 6f72 5f64     scale_color_d
+00001d40: 6973 6372 6574 6528 6775 6964 653d 4661  iscrete(guide=Fa
+00001d50: 6c73 6529 202b 0a20 2020 2020 2020 2020  lse) +.         
+00001d60: 2020 2020 2020 2020 2020 2074 6865 6d65             theme
+00001d70: 2861 7869 735f 7465 7874 203d 656c 656d  (axis_text =elem
+00001d80: 656e 745f 7465 7874 2873 697a 653d 3132  ent_text(size=12
+00001d90: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00001da0: 2020 2020 2020 2020 2020 2020 2061 7869               axi
+00001db0: 735f 7469 746c 653d 656c 656d 656e 745f  s_title=element_
+00001dc0: 7465 7874 2873 697a 653d 3134 290a 2020  text(size=14).  
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001de0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00001df0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00001e00: 6773 697a 653d 2834 2c34 2929 0a0a 7077  gsize=(4,4))..pw
+00001e10: 2e70 6172 616d 5b22 6d61 7267 696e 225d  .param["margin"]
+00001e20: 203d 2030 2e32 0a28 6731 2f28 6733 7c67   = 0.2.(g1/(g3|g
+00001e30: 3229 5b67 335d 292e 7361 7665 6669 6728  2)[g3]).savefig(
+00001e40: 2920 2342 7920 7370 6563 6966 7969 6e67  ) #By specifying
+00001e50: 2067 3320 696e 2028 6733 7c67 3229 2c20   g3 in (g3|g2), 
+00001e60: 6731 2069 7320 706f 7369 7469 6f6e 6564  g1 is positioned
+00001e70: 2065 7861 6374 6c79 206f 6e20 6733 2e20   exactly on g3. 
+00001e80: 0a0a 6060 600a 0a3c 696d 6720 7372 633d  ..```..<img src=
+00001e90: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00001ea0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001eb0: 6f6d 2f70 6f6e 6e68 6964 652f 7061 7463  om/ponnhide/patc
+00001ec0: 6877 6f72 6b6c 6962 2f6d 6169 6e2f 696d  hworklib/main/im
+00001ed0: 672f 6a6f 696e 745f 706c 6f74 5f70 6c6f  g/joint_plot_plo
+00001ee0: 746e 696e 652e 706e 6722 2077 6964 7468  tnine.png" width
+00001ef0: 3d22 3830 3078 3830 3022 3e0a 0a3c 2f64  ="800x800">..</d
+00001f00: 6574 6169 6c73 3e0a 0a23 2323 2320 3037  etails>..#### 07
+00001f10: 3139 3230 3232 3a20 5665 7273 696f 6e20  192022: Version 
+00001f20: 302e 342e 3320 7761 7320 7265 6c65 6173  0.4.3 was releas
+00001f30: 6564 2e20 0a2d 2041 2066 6577 2062 7567  ed. .- A few bug
+00001f40: 7320 7765 7265 2066 6978 6564 2e20 200a  s were fixed.  .
+00001f50: 2d20 6062 6173 6566 6967 7572 6560 2070  - `basefigure` p
+00001f60: 6172 616d 6574 6572 2077 6173 2061 6464  arameter was add
+00001f70: 6564 2e20 596f 7520 6361 6e20 6163 6365  ed. You can acce
+00001f80: 7373 2074 6865 2062 6173 6520 6669 6775  ss the base figu
+00001f90: 7265 206f 6620 7061 7463 6877 6f72 6b6c  re of patchworkl
+00001fa0: 6962 2062 7920 6070 6174 6368 776f 726b  ib by `patchwork
+00001fb0: 6c69 622e 6261 7365 6669 6775 7265 600a  lib.basefigure`.
+00001fc0: 2d20 706c 6f74 6e69 6e65 2076 302e 392e  - plotnine v0.9.
+00001fd0: 3020 7761 7320 6e6f 7720 7375 7070 6f72  0 was now suppor
+00001fe0: 7465 642e 2050 726f 6261 626c 792c 2069  ted. Probably, i
+00001ff0: 7420 7374 696c 6c20 6861 7665 2073 6f6d  t still have som
+00002000: 6520 6275 6773 2e20 4966 2079 6f75 2066  e bugs. If you f
+00002010: 696e 6420 6275 6773 2c20 706c 6561 7365  ind bugs, please
+00002020: 206c 6574 206d 6520 6b6e 6f77 206f 6e20   let me know on 
+00002030: 7468 6520 6973 7375 652e 0a0a 2323 2323  the issue...####
+00002040: 2030 3432 3232 3032 323a 2056 6572 7369   04222022: Versi
+00002050: 6f6e 2030 2e34 2e32 2077 6173 2072 656c  on 0.4.2 was rel
+00002060: 6561 7365 642e 200a 2d20 4120 6665 7720  eased. .- A few 
+00002070: 6275 6773 2077 6572 6520 6669 7865 642e  bugs were fixed.
+00002080: 2020 0a0a 2323 2323 2030 3431 3832 3032    ..#### 0418202
+00002090: 323a 2056 6572 7369 6f6e 2030 2e34 2e31  2: Version 0.4.1
+000020a0: 2077 6173 2072 656c 6561 7365 642e 200a   was released. .
+000020b0: 2d20 606c 6f61 645f 7365 6162 6f72 6e67  - `load_seaborng
+000020c0: 7269 6460 2063 616e 2061 6363 6570 7473  rid` can accepts
+000020d0: 2061 2060 7365 6162 6f72 6e2e 636c 7573   a `seaborn.clus
+000020e0: 7465 726d 6170 6020 706c 6f74 2e20 466f  termap` plot. Fo
+000020f0: 7220 6465 7461 696c 732c 2073 6565 2065  r details, see e
+00002100: 7861 6d70 6c65 2063 6f64 6520 6f6e 205b  xample code on [
+00002110: 476f 6f67 6c65 2063 6f6c 6162 5d28 6874  Google colab](ht
+00002120: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
+00002130: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
+00002140: 6472 6976 652f 3177 5151 7942 484c 4e58  drive/1wQQyBHLNX
+00002150: 4a35 4b73 3665 7638 3849 6a58 6847 6654  J5Ks6ev88IjXhGfT
+00002160: 3938 5347 4a75 4d3f 7573 703d 7368 6172  98SGJuM?usp=shar
+00002170: 696e 6729 0a2d 2041 2066 6577 2062 7567  ing).- A few bug
+00002180: 7320 7765 7265 2066 6978 6564 2e20 200a  s were fixed.  .
+00002190: 0a23 2323 2320 3033 3237 3230 3232 3a20  .#### 03272022: 
+000021a0: 5665 7273 696f 6e20 302e 342e 3020 7761  Version 0.4.0 wa
+000021b0: 7320 7265 6c65 6173 6564 2e20 0a2d 2041  s released. .- A
+000021c0: 6464 2064 6f63 7374 7269 6e67 2066 6f72  dd docstring for
+000021d0: 2065 6163 6820 6d65 7468 6f64 2061 6e64   each method and
+000021e0: 2063 6c61 7373 2e20 200a 2d20 4164 6420   class.  .- Add 
+000021f0: 7365 7665 7261 6c20 6e65 7720 6d65 7468  several new meth
+00002200: 6f64 7320 6f66 2060 7061 7463 6877 6f72  ods of `patchwor
+00002210: 6b6c 6962 2e42 7269 636b 7360 2063 6c61  klib.Bricks` cla
+00002220: 7373 2074 6f20 7365 7420 636f 6d6d 6f6e  ss to set common
+00002230: 206c 6162 656c 2c20 7469 746c 652c 2073   label, title, s
+00002240: 7069 6e65 2061 6e64 2063 6f6c 6f72 6261  pine and colorba
+00002250: 7220 666f 7220 6042 7269 636b 6020 6f62  r for `Brick` ob
+00002260: 6a65 7473 2069 6e20 7468 6520 6042 7269  jets in the `Bri
+00002270: 636b 7360 206f 626a 6563 742e 2020 0ae3  cks` object.  ..
+00002280: 8080 466f 7220 7573 6167 652c 2070 6c65  ..For usage, ple
+00002290: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
+000022a0: 2064 6f63 7374 7269 6e67 206f 7220 7468   docstring or th
+000022b0: 6520 6578 616d 706c 6520 636f 6465 7320  e example codes 
+000022c0: 6f6e 205b 476f 6f67 6c65 2063 6f6c 6162  on [Google colab
+000022d0: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+000022e0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+000022f0: 636f 6d2f 6472 6976 652f 3166 3036 4151  com/drive/1f06AQ
+00002300: 4f71 4e6e 5359 506a 6339 456b 7765 4333  OqNnSYPjc9EkweC3
+00002310: 5f48 6d79 3461 6272 2d67 6f3f 7573 703d  _Hmy4abr-go?usp=
+00002320: 7368 6172 696e 6729 2e0a 0a23 2323 2320  sharing)...#### 
+00002330: 3032 3034 3230 3232 3a20 5665 7273 696f  02042022: Versio
+00002340: 6e20 302e 332e 3620 7761 7320 7265 6c65  n 0.3.6 was rele
+00002350: 6173 6564 2e20 0a2d 2041 2066 6577 2062  ased. .- A few b
+00002360: 7567 7320 7265 6c61 7469 6e67 2077 6974  ugs relating wit
+00002370: 6820 7468 6520 6675 6e63 7469 6f6e 2074  h the function t
+00002380: 6f20 6172 7261 6e67 6520 6d75 6c74 6970  o arrange multip
+00002390: 6c65 2070 6f6c 6172 2070 6c6f 7420 6f62  le polar plot ob
+000023a0: 6a65 6374 732e 0a0a 2323 2323 2030 3230  jects...#### 020
+000023b0: 3432 3032 323a 2056 6572 7369 6f6e 2030  42022: Version 0
+000023c0: 2e33 2e35 2077 6173 2072 656c 6561 7365  .3.5 was release
+000023d0: 642e 0a2d 2041 2066 6577 2062 7567 7320  d..- A few bugs 
+000023e0: 696e 2060 6d6f 7665 5f6c 6567 656e 6460  in `move_legend`
+000023f0: 2077 6572 6520 6669 7865 642e 2028 5468   were fixed. (Th
+00002400: 6520 606d 6f76 655f 6c65 6765 6e64 6020  e `move_legend` 
+00002410: 666f 7220 7365 6162 6f72 6e20 6772 6964  for seaborn grid
+00002420: 6564 2070 6c6f 7420 7761 7320 6e6f 7420  ed plot was not 
+00002430: 776f 726b 696e 6720 7072 6f70 6572 6c79  working properly
+00002440: 2e29 0a2d 2049 6d70 726f 7665 6420 7468  .).- Improved th
+00002450: 6520 7370 6565 6420 6f66 2060 7361 7665  e speed of `save
+00002460: 6669 6760 206f 7065 7261 7469 6f6e 2e0a  fig` operation..
+00002470: 0a23 2323 2320 3031 3234 3230 3232 3a20  .#### 01242022: 
+00002480: 5665 7273 696f 6e20 302e 332e 3320 7761  Version 0.3.3 wa
+00002490: 7320 7265 6c65 6173 6564 2e20 0a2d 2041  s released. .- A
+000024a0: 2066 6577 2062 7567 7320 7765 7265 2066   few bugs were f
+000024b0: 6978 6564 2e0a 090a 2323 2323 2030 3132  ixed....#### 012
+000024c0: 3232 3032 323a 2056 6572 7369 6f6e 2030  22022: Version 0
+000024d0: 2e33 2e30 2077 6173 2072 656c 6561 7365  .3.0 was release
+000024e0: 642e 0a3c 6465 7461 696c 733e 0a3c 7375  d..<details>.<su
+000024f0: 6d6d 6172 793e 2050 6174 6368 776f 726b  mmary> Patchwork
+00002500: 6c69 6220 6e6f 7720 7375 7070 6f72 7473  lib now supports
+00002510: 2074 6865 2066 756e 6374 696f 6e20 746f   the function to
+00002520: 2061 7272 616e 6765 206d 6174 706c 6f74   arrange matplot
+00002530: 6c69 622e 7072 6f6a 6563 7469 6f6e 732e  lib.projections.
+00002540: 706f 6c61 722e 506f 6c61 7241 7865 7320  polar.PolarAxes 
+00002550: 6f6a 6265 6374 732e 2020 3c2f 7375 6d6d  ojbects.  </summ
+00002560: 6172 793e 0a0a 5768 656e 2079 6f75 206c  ary>..When you l
+00002570: 6f61 6420 6120 6d61 7470 6c6f 746c 6962  oad a matplotlib
+00002580: 2e70 726f 6a65 6374 696f 6e73 2e70 6f6c  .projections.pol
+00002590: 6172 2e50 6f6c 6172 4178 6573 206f 626a  ar.PolarAxes obj
+000025a0: 6563 7420 6173 2061 2042 7269 636b 2063  ect as a Brick c
+000025b0: 6c61 7373 206f 626a 6563 742c 2070 6c65  lass object, ple
+000025c0: 6173 6520 7573 6520 2763 4272 6963 6b27  ase use 'cBrick'
+000025d0: 2069 6e73 7465 6164 206f 6620 2742 7269   instead of 'Bri
+000025e0: 636b 272e 0a4e 6f77 2c20 796f 7520 6361  ck'..Now, you ca
+000025f0: 6e20 6172 7261 6e67 6520 6d75 6c74 6970  n arrange multip
+00002600: 6c65 2063 6972 636f 7320 706c 6f74 7320  le circos plots 
+00002610: 7573 696e 6720 5b70 7963 6972 636f 735d  using [pycircos]
+00002620: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002630: 636f 6d2f 706f 6e6e 6869 6465 2f70 7943  com/ponnhide/pyC
+00002640: 6972 636f 7329 2061 6e64 2070 6174 6368  ircos) and patch
+00002650: 776f 726b 6c69 622e 2050 6c65 6173 6520  worklib. Please 
+00002660: 7365 6520 7468 6520 666f 6c6c 6f77 696e  see the followin
+00002670: 6720 6578 616d 706c 6520 636f 6465 2e20  g example code. 
+00002680: 200a 6874 7470 733a 2f2f 636f 6c61 622e   .https://colab.
+00002690: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+000026a0: 636f 6d2f 6472 6976 652f 3174 6b6e 3770  com/drive/1tkn7p
+000026b0: 7852 7168 3942 7935 7254 4671 5262 564e  xRqh9By5rTFqRbVN
+000026c0: 4456 7773 2d6f 2d79 537a 393f 7573 703d  DVws-o-ySz9?usp=
+000026d0: 7368 6172 696e 670a 0a3c 2f64 6574 6169  sharing..</detai
+000026e0: 6c73 3e0a 0a23 2323 2320 3031 3231 3230  ls>..#### 012120
+000026f0: 3232 3a20 5665 7273 696f 6e20 302e 322e  22: Version 0.2.
+00002700: 3120 7761 7320 7265 6c65 6173 6564 2e20  1 was released. 
+00002710: 200a 2d20 4120 6665 7720 6275 6773 2066   .- A few bugs f
+00002720: 6f72 2027 6c6f 6164 5f73 6561 626f 726e  or 'load_seaborn
+00002730: 6772 6964 2720 7765 7265 2066 6978 6564  grid' were fixed
+00002740: 2e0a 0a23 2323 2320 3031 3230 3230 3232  ...#### 01202022
+00002750: 3a20 5665 7273 696f 6e20 302e 322e 3020  : Version 0.2.0 
+00002760: 7761 7320 7265 6c65 6173 6564 2e0a 3c64  was released..<d
+00002770: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00002780: 3e20 5061 7463 6877 6f72 6b6c 6962 2069  > Patchworklib i
+00002790: 7320 6e6f 7720 706f 7373 6962 6c65 2074  s now possible t
+000027a0: 6f20 6172 7261 6e67 6520 5365 6162 726f  o arrange Seabro
+000027b0: 6e20 6772 6964 6465 6420 706c 6f74 732e  n gridded plots.
+000027c0: 2054 6865 2022 7374 6163 6b22 2066 756e   The "stack" fun
+000027d0: 6374 696f 6e20 6973 2061 6464 6564 2e20  ction is added. 
+000027e0: 4120 6665 7720 6275 6773 2077 6572 6520  A few bugs were 
+000027f0: 6669 7865 642e 203c 2f73 756d 6d61 7279  fixed. </summary
+00002800: 3e0a 090a 2323 2323 2041 7272 616e 6769  >...#### Arrangi
+00002810: 6e67 2073 6561 626f 726e 2067 7269 6464  ng seaborn gridd
+00002820: 6564 2070 6c6f 7473 200a 5061 7463 6877  ed plots .Patchw
+00002830: 6f72 6b6c 6962 2073 7570 706f 7274 6564  orklib supported
+00002840: 2074 6865 2066 756e 6374 696f 6e20 746f   the function to
+00002850: 2061 7261 6e67 6520 6d75 6c74 6970 6c65   arange multiple
+00002860: 2073 6562 6f72 6e20 706c 6f74 7320 6765   seborn plots ge
+00002870: 6e65 7261 7465 6420 6261 7365 6420 6f6e  nerated based on
+00002880: 2061 7869 7367 7269 6420 2846 6163 6574   axisgrid (Facet
+00002890: 4772 6964 2c20 5061 6972 4772 6964 2c20  Grid, PairGrid, 
+000028a0: 616e 6420 4a6f 696e 7447 7269 6429 2e0a  and JointGrid)..
+000028b0: 4c65 7427 7320 7365 6520 7468 6520 666f  Let's see the fo
+000028c0: 6c6c 776f 696e 6720 6578 616d 706c 652e  llwoing example.
+000028d0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+000028e0: 7274 206f 730a 696d 706f 7274 2073 6561  rt os.import sea
+000028f0: 626f 726e 2061 7320 736e 730a 696d 706f  born as sns.impo
+00002900: 7274 2070 6174 6368 776f 726b 6c69 6220  rt patchworklib 
+00002910: 6173 2070 770a 6672 6f6d 2066 756e 6374  as pw.from funct
+00002920: 6f6f 6c73 2069 6d70 6f72 7420 7265 6475  ools import redu
+00002930: 6365 0a70 772e 6f76 6572 7772 6974 655f  ce.pw.overwrite_
+00002940: 6178 6973 6772 6964 2829 2023 5768 656e  axisgrid() #When
+00002950: 2079 6f75 2075 7365 2070 772e 6c6f 6164   you use pw.load
+00002960: 5f73 6561 676f 726e 6772 6964 2c20 276f  _seagorngrid, 'o
+00002970: 7665 7277 7269 7465 5f61 7869 7367 7269  verwrite_axisgri
+00002980: 6427 2073 686f 756c 6420 6265 2065 7865  d' should be exe
+00002990: 6375 7465 642e 0a0a 6466 203d 2073 6e73  cuted...df = sns
+000029a0: 2e6c 6f61 645f 6461 7461 7365 7428 2270  .load_dataset("p
+000029b0: 656e 6775 696e 7322 290a 6731 2020 3d20  enguins").g1  = 
+000029c0: 736e 732e 7061 6972 706c 6f74 2864 662c  sns.pairplot(df,
+000029d0: 2068 7565 3d22 7370 6563 6965 7322 290a   hue="species").
+000029e0: 6731 2020 3d20 7077 2e6c 6f61 645f 7365  g1  = pw.load_se
+000029f0: 6162 6f72 6e67 7269 6428 6731 290a 6731  aborngrid(g1).g1
+00002a00: 2e6d 6f76 655f 6c65 6765 6e64 2822 7570  .move_legend("up
+00002a10: 7065 7220 6c65 6674 222c 2062 626f 785f  per left", bbox_
+00002a20: 746f 5f61 6e63 686f 723d 2830 2e30 382c  to_anchor=(0.08,
+00002a30: 312e 3031 2929 0a0a 706c 616e 6574 7320  1.01))..planets 
+00002a40: 3d20 736e 732e 6c6f 6164 5f64 6174 6173  = sns.load_datas
+00002a50: 6574 2822 706c 616e 6574 7322 290a 636d  et("planets").cm
+00002a60: 6170 203d 2073 6e73 2e63 7562 6568 656c  ap = sns.cubehel
+00002a70: 6978 5f70 616c 6574 7465 2872 6f74 3d2d  ix_palette(rot=-
+00002a80: 2e32 2c20 6173 5f63 6d61 703d 5472 7565  .2, as_cmap=True
+00002a90: 290a 6732 203d 2073 6e73 2e72 656c 706c  ).g2 = sns.relpl
+00002aa0: 6f74 280a 2020 2020 6461 7461 3d70 6c61  ot(.    data=pla
+00002ab0: 6e65 7473 2c0a 2020 2020 783d 2264 6973  nets,.    x="dis
+00002ac0: 7461 6e63 6522 2c20 793d 226f 7262 6974  tance", y="orbit
+00002ad0: 616c 5f70 6572 696f 6422 2c0a 2020 2020  al_period",.    
+00002ae0: 6875 653d 2279 6561 7222 2c20 7369 7a65  hue="year", size
+00002af0: 3d22 6d61 7373 222c 0a20 2020 2070 616c  ="mass",.    pal
+00002b00: 6574 7465 3d63 6d61 702c 2073 697a 6573  ette=cmap, sizes
+00002b10: 3d28 3130 2c20 3230 3029 2c0a 290a 6732  =(10, 200),.).g2
+00002b20: 2e73 6574 2878 7363 616c 653d 226c 6f67  .set(xscale="log
+00002b30: 222c 2079 7363 616c 653d 226c 6f67 2229  ", yscale="log")
+00002b40: 0a67 322e 6178 2e78 6178 6973 2e67 7269  .g2.ax.xaxis.gri
+00002b50: 6428 5472 7565 2c20 226d 696e 6f72 222c  d(True, "minor",
+00002b60: 206c 696e 6577 6964 7468 3d2e 3235 290a   linewidth=.25).
+00002b70: 6732 2e61 782e 7961 7869 732e 6772 6964  g2.ax.yaxis.grid
+00002b80: 2854 7275 652c 2022 6d69 6e6f 7222 2c20  (True, "minor", 
+00002b90: 6c69 6e65 7769 6474 683d 2e32 3529 0a67  linewidth=.25).g
+00002ba0: 322e 6465 7370 696e 6528 6c65 6674 3d54  2.despine(left=T
+00002bb0: 7275 652c 2062 6f74 746f 6d3d 5472 7565  rue, bottom=True
+00002bc0: 290a 6732 203d 2070 772e 6c6f 6164 5f73  ).g2 = pw.load_s
+00002bd0: 6561 626f 726e 6772 6964 2867 3229 0a0a  eaborngrid(g2)..
+00002be0: 7065 6e67 7569 6e73 203d 2073 6e73 2e6c  penguins = sns.l
+00002bf0: 6f61 645f 6461 7461 7365 7428 2270 656e  oad_dataset("pen
+00002c00: 6775 696e 7322 290a 6733 203d 2073 6e73  guins").g3 = sns
+00002c10: 2e6a 6f69 6e74 706c 6f74 280a 2020 2020  .jointplot(.    
+00002c20: 6461 7461 3d70 656e 6775 696e 732c 0a20  data=penguins,. 
+00002c30: 2020 2078 3d22 6269 6c6c 5f6c 656e 6774     x="bill_lengt
+00002c40: 685f 6d6d 222c 2079 3d22 6269 6c6c 5f64  h_mm", y="bill_d
+00002c50: 6570 7468 5f6d 6d22 2c20 6875 653d 2273  epth_mm", hue="s
+00002c60: 7065 6369 6573 222c 0a20 2020 206b 696e  pecies",.    kin
+00002c70: 643d 226b 6465 222c 0a29 0a67 3320 3d20  d="kde",.).g3 = 
+00002c80: 7077 2e6c 6f61 645f 7365 6162 6f72 6e67  pw.load_seaborng
+00002c90: 7269 6428 6733 2c20 6c61 6265 6c73 3d5b  rid(g3, labels=[
+00002ca0: 226a 6f69 6e74 222c 226d 6172 675f 7822  "joint","marg_x"
+00002cb0: 2c22 6d61 7267 5f79 225d 290a 2828 6732  ,"marg_y"]).((g2
+00002cc0: 2f67 335b 226d 6172 675f 7822 5d29 7c67  /g3["marg_x"])|g
+00002cd0: 3129 2e73 6176 6566 6967 2829 0a60 6060  1).savefig().```
+00002ce0: 0a3c 696d 6720 7372 633d 2269 6d67 2f73  .<img src="img/s
+00002cf0: 6561 626f 726e 5f67 7269 6473 2e70 6e67  eaborn_grids.png
+00002d00: 2220 7769 6474 683d 2238 3030 7838 3030  " width="800x800
+00002d10: 223e 0a0a 416c 736f 2c20 736f 6d65 2065  ">..Also, some e
+00002d20: 7861 6d70 6c65 2063 6f64 6573 2061 7265  xample codes are
+00002d30: 206d 6164 6520 6578 6563 7574 6162 6c65   made executable
+00002d40: 2069 6e20 476f 6f67 6c65 2043 6f6c 6162   in Google Colab
+00002d50: 6f72 6174 6f72 792e 0a2d 205b 7365 6162  oratory..- [seab
+00002d60: 6f72 6e20 6772 6964 5d28 6874 7470 733a  orn grid](https:
+00002d70: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00002d80: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
+00002d90: 652f 317a 3030 334c 6162 5077 6f66 6273  e/1z003LabPwofbs
+00002da0: 4e38 3778 7333 3646 4271 4b63 4d67 5473  N87xs36FBqKcMgTs
+00002db0: 774f 343f 7573 703d 7368 6172 696e 6729  wO4?usp=sharing)
+00002dc0: 0a2d 205b 7365 6162 6f72 6e5f 6767 706c  .- [seaborn_ggpl
+00002dd0: 6f74 5d28 6874 7470 733a 2f2f 636f 6c61  ot](https://cola
+00002de0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00002df0: 652e 636f 6d2f 6472 6976 652f 3153 5049  e.com/drive/1SPI
+00002e00: 316a 536f 4837 4c30 6866 5837 346e 7551  1jSoH7L0hfX74nuQ
+00002e10: 7434 4277 5935 524b 7772 5857 573f 7573  t4BwY5RKwrXWW?us
+00002e20: 703d 7368 6172 696e 6729 0a0a 2323 2323  p=sharing)..####
+00002e30: 2022 7374 6163 6b22 2066 7563 6e74 696f   "stack" fucntio
+00002e40: 6e0a 4920 696d 706c 656d 656e 7465 6420  n.I implemented 
+00002e50: 7468 6520 6073 7461 636b 6020 6675 6e63  the `stack` func
+00002e60: 7469 6f6e 2e20 5468 6973 2066 756e 6374  tion. This funct
+00002e70: 696f 6e20 616c 6c6f 7773 2075 7365 7273  ion allows users
+00002e80: 2074 6f20 6172 7261 6e67 6520 6d75 6c74   to arrange mult
+00002e90: 6970 6c65 2028 6d6f 7265 2074 6861 6e20  iple (more than 
+00002ea0: 7477 6f29 2042 7269 636b 206f 7220 4272  two) Brick or Br
+00002eb0: 6963 6b73 206f 626a 6563 7473 2061 6c6f  icks objects alo
+00002ec0: 6e67 2074 6865 2073 7065 6369 6669 6564  ng the specified
+00002ed0: 2064 6972 6563 7469 6f6e 2061 7320 666f   direction as fo
+00002ee0: 6c6c 6f77 732e 0a0a 6060 6070 7974 686f  llows...```pytho
+00002ef0: 6e0a 696d 706f 7274 2070 6174 6368 776f  n.import patchwo
+00002f00: 726b 6c69 6220 6173 2070 770a 6178 5f6c  rklib as pw.ax_l
+00002f10: 6973 7420 3d20 5b5d 0a66 6f72 2069 2069  ist = [].for i i
+00002f20: 6e20 7261 6e67 6528 3130 293a 0a20 2020  n range(10):.   
+00002f30: 2061 785f 6c69 7374 2e61 7070 656e 6428   ax_list.append(
+00002f40: 7077 2e42 7269 636b 2866 6967 7369 7a65  pw.Brick(figsize
+00002f50: 3d28 322c 3229 2c20 6c61 6265 6c3d 2261  =(2,2), label="a
+00002f60: 787b 7d22 2e66 6f72 6d61 7428 6929 2929  x{}".format(i)))
+00002f70: 0a73 7461 636b 6564 5f61 7865 7320 3d20  .stacked_axes = 
+00002f80: 7077 2e73 7461 636b 2861 785f 6c69 7374  pw.stack(ax_list
+00002f90: 2c20 6f70 6572 6174 6f72 3d22 7c22 2c20  , operator="|", 
+00002fa0: 6d61 7267 696e 3d30 2e32 290a 7374 6163  margin=0.2).stac
+00002fb0: 6b65 645f 6178 6573 2e73 6176 6566 6967  ked_axes.savefig
+00002fc0: 2829 0a60 6060 0a3c 696d 6720 7372 633d  ().```.<img src=
+00002fd0: 2269 6d67 2f73 7461 636b 5f65 7861 6d70  "img/stack_examp
+00002fe0: 6c65 2e70 6e67 2220 7769 6474 683d 2238  le.png" width="8
+00002ff0: 3030 7838 3030 223e 0a0a 0a3c 2f64 6574  00x800">...</det
+00003000: 6169 6c73 3e0a 090a 2323 2323 2030 3131  ails>...#### 011
+00003010: 3432 3032 323a 2056 6572 7369 6f6e 2030  42022: Version 0
+00003020: 2e31 2e30 2077 6173 2072 656c 6561 7365  .1.0 was release
+00003030: 642e 2020 0a2d 2050 6174 6368 776f 726b  d.  .- Patchwork
+00003040: 6c69 6220 7761 7320 6e6f 7720 6176 6961  lib was now avia
+00003050: 6c61 626c 6520 7468 726f 7567 6820 7069  lable through pi
+00003060: 702e 0a0a 3c64 6574 6169 6c73 3e0a 3c73  p...<details>.<s
+00003070: 756d 6d61 7279 3e20 3c62 3e30 3131 3332  ummary> <b>01132
+00003080: 3032 323a 2022 7370 6163 6572 2220 636c  022: "spacer" cl
+00003090: 6173 7320 7761 7320 696d 706c 656d 656e  ass was implemen
+000030a0: 7465 6420 616e 6420 2263 6173 6522 2070  ted and "case" p
+000030b0: 6172 616d 6574 6572 2077 6173 2061 6464  arameter was add
+000030c0: 6564 2074 6f20 4272 6963 6b73 2063 6c61  ed to Bricks cla
+000030d0: 7373 2e3c 2f62 3e20 3c2f 7375 6d6d 6172  ss.</b> </summar
+000030e0: 793e 0a0a 2a2a 4164 6420 656d 7074 7920  y>..**Add empty 
+000030f0: 7370 6163 6573 2061 726f 756e 6420 6120  spaces around a 
+00003100: 706c 6f74 2a2a 200a 6060 6070 7974 686f  plot** .```pytho
+00003110: 6e0a 2370 7265 7061 7261 7469 6f6e 206f  n.#preparation o
+00003120: 6620 706c 6f74 2064 6174 610a 696d 706f  f plot data.impo
+00003130: 7274 206e 756d 7079 2061 7320 6e70 200a  rt numpy as np .
+00003140: 696d 706f 7274 206d 6174 706c 6f74 6c69  import matplotli
+00003150: 6220 6173 206d 706c 0a69 6d70 6f72 7420  b as mpl.import 
+00003160: 7061 7463 6877 6f72 6b6c 6962 2061 7320  patchworklib as 
+00003170: 7077 0a0a 6461 7461 3120 3d20 3230 202a  pw..data1 = 20 *
+00003180: 206e 702e 7261 6e64 6f6d 2e72 616e 6428   np.random.rand(
+00003190: 3130 302c 3130 3029 202d 2031 300a 6461  100,100) - 10.da
+000031a0: 7461 3220 3d20 3230 202a 206e 702e 7261  ta2 = 20 * np.ra
+000031b0: 6e64 6f6d 2e72 616e 6428 3130 302c 3130  ndom.rand(100,10
+000031c0: 3029 202d 2031 300a 636d 6170 203d 206d  0) - 10.cmap = m
+000031d0: 706c 2e63 6d2e 5265 6473 0a6e 6f72 6d20  pl.cm.Reds.norm 
+000031e0: 3d20 6d70 6c2e 636f 6c6f 7273 2e4e 6f72  = mpl.colors.Nor
+000031f0: 6d61 6c69 7a65 2876 6d69 6e3d 2d31 302c  malize(vmin=-10,
+00003200: 2076 6d61 783d 3130 290a 6178 3120 3d20   vmax=10).ax1 = 
+00003210: 7077 2e42 7269 636b 2822 6178 7822 2c20  pw.Brick("axx", 
+00003220: 6669 6773 697a 653d 2833 2c33 2929 0a61  figsize=(3,3)).a
+00003230: 7832 203d 2070 772e 4272 6963 6b28 2261  x2 = pw.Brick("a
+00003240: 7879 222c 2066 6967 7369 7a65 3d28 332c  xy", figsize=(3,
+00003250: 3329 290a 6178 312e 696d 7368 6f77 2864  3)).ax1.imshow(d
+00003260: 6174 6131 2c20 696e 7465 7270 6f6c 6174  ata1, interpolat
+00003270: 696f 6e3d 276e 6561 7265 7374 272c 2063  ion='nearest', c
+00003280: 6d61 703d 636d 6170 2c20 6173 7065 6374  map=cmap, aspect
+00003290: 3d22 6175 746f 2229 0a61 7832 2e69 6d73  ="auto").ax2.ims
+000032a0: 686f 7728 6461 7461 322c 2069 6e74 6572  how(data2, inter
+000032b0: 706f 6c61 7469 6f6e 3d27 6e65 6172 6573  polation='neares
+000032c0: 7427 2c20 636d 6170 3d63 6d61 702c 2061  t', cmap=cmap, a
+000032d0: 7370 6563 743d 2261 7574 6f22 290a 6060  spect="auto").``
+000032e0: 600a 0a77 2f6f 2073 7061 6365 720a 6060  `..w/o spacer.``
+000032f0: 6070 7974 686f 6e0a 6178 5f63 6220 2020  `python.ax_cb   
+00003300: 203d 2070 772e 4272 6963 6b28 2261 785f   = pw.Brick("ax_
+00003310: 6362 222c 2066 6967 7369 7a65 3d28 302e  cb", figsize=(0.
+00003320: 312c 3329 290a 6362 2020 2020 2020 203d  1,3)).cb       =
+00003330: 206d 706c 2e63 6f6c 6f72 6261 722e 436f   mpl.colorbar.Co
+00003340: 6c6f 7262 6172 4261 7365 2861 785f 6362  lorbarBase(ax_cb
+00003350: 2c20 636d 6170 3d63 6d61 702c 206e 6f72  , cmap=cmap, nor
+00003360: 6d3d 6e6f 726d 290a 6178 3132 2020 2020  m=norm).ax12    
+00003370: 203d 2061 7831 7c61 7832 0a68 6561 746d   = ax1|ax2.heatm
+00003380: 6170 3220 3d20 6178 3132 207c 2061 785f  ap2 = ax12 | ax_
+00003390: 6362 0a68 6561 746d 6170 322e 7361 7665  cb.heatmap2.save
+000033a0: 6669 6728 290a 6060 600a 3c69 6d67 2073  fig().```.<img s
+000033b0: 7263 3d22 696d 672f 6865 6174 6d61 702d  rc="img/heatmap-
+000033c0: 312e 706e 6722 2077 6964 7468 3d22 3430  1.png" width="40
+000033d0: 3078 3430 3022 3e0a 0a77 2f20 7370 6163  0x400">..w/ spac
+000033e0: 6572 0a60 6060 7079 7468 6f6e 0a61 785f  er.```python.ax_
+000033f0: 6362 3220 2020 3d20 7077 2e42 7269 636b  cb2   = pw.Brick
+00003400: 2822 6178 5f63 6232 222c 2066 6967 7369  ("ax_cb2", figsi
+00003410: 7a65 3d28 302e 312c 312e 3529 290a 6362  ze=(0.1,1.5)).cb
+00003420: 3220 2020 2020 203d 206d 706c 2e63 6f6c  2      = mpl.col
+00003430: 6f72 6261 722e 436f 6c6f 7262 6172 4261  orbar.ColorbarBa
+00003440: 7365 2861 785f 6362 322c 2063 6d61 703d  se(ax_cb2, cmap=
+00003450: 636d 6170 2c20 6e6f 726d 3d6e 6f72 6d29  cmap, norm=norm)
+00003460: 0a68 6561 746d 6170 3220 3d20 6178 3132  .heatmap2 = ax12
+00003470: 207c 2028 7077 2e73 7061 6365 7228 6178   | (pw.spacer(ax
+00003480: 5f63 6232 2c30 2e35 292f 6178 5f63 6232  _cb2,0.5)/ax_cb2
+00003490: 2f70 772e 7370 6163 6572 2861 785f 6362  /pw.spacer(ax_cb
+000034a0: 322c 302e 3529 290a 6865 6174 6d61 7032  2,0.5)).heatmap2
+000034b0: 2e73 6176 6566 6967 2829 0a60 6060 0a3c  .savefig().```.<
+000034c0: 696d 6720 7372 633d 2269 6d67 2f68 6561  img src="img/hea
+000034d0: 746d 6170 2d32 2e70 6e67 2220 7769 6474  tmap-2.png" widt
+000034e0: 683d 2234 3030 7834 3030 223e 0a0a 2a2a  h="400x400">..**
+000034f0: 5375 7065 7220 7469 7469 6c65 2066 6f72  Super titile for
+00003500: 206d 756c 7469 706c 6520 706c 6f74 732a   multiple plots*
+00003510: 2a20 200a 536f 6d65 7469 6d65 732c 2061  *  .Sometimes, a
+00003520: 6c6c 2074 6861 7420 6973 206e 6565 6465  ll that is neede
+00003530: 6420 746f 2068 6176 6520 636f 6d6d 6f6e  d to have common
+00003540: 206c 6162 656c 7320 616e 6420 7469 746c   labels and titl
+00003550: 6520 666f 7220 6d75 6c74 6970 6c65 2070  e for multiple p
+00003560: 6c6f 7473 2e20 2020 0a42 7920 7370 6563  lots.   .By spec
+00003570: 6966 7969 6e67 2060 6361 7365 6020 7061  ifying `case` pa
+00003580: 7261 6d65 7465 7220 6f66 2061 2042 7269  rameter of a Bri
+00003590: 636b 7320 636c 6173 7320 6f62 6a65 6374  cks class object
+000035a0: 2c20 636f 6d6d 6f6e 206d 6174 706c 6f74  , common matplot
+000035b0: 6c69 6220 6172 7469 7374 206f 6a62 6563  lib artist ojbec
+000035c0: 7473 2066 6f72 206d 756c 7469 706c 6520  ts for multiple 
+000035d0: 706c 6f74 7320 6361 6e20 6265 2068 616e  plots can be han
+000035e0: 646c 6564 2e0a 6060 6070 7974 686f 6e0a  dled..```python.
+000035f0: 6178 3132 2e63 6173 652e 7365 745f 7469  ax12.case.set_ti
+00003600: 746c 6528 2241 2067 6c6f 6261 6c20 7469  tle("A global ti
+00003610: 746c 6520 666f 7220 6d75 6c74 6970 6c65  tle for multiple
+00003620: 2070 6c6f 7473 222c 2070 6164 3d31 3029   plots", pad=10)
+00003630: 0a68 6561 746d 6170 3220 3d20 6178 3132  .heatmap2 = ax12
+00003640: 7c28 7077 2e73 7061 6365 7228 6178 5f63  |(pw.spacer(ax_c
+00003650: 622c 302e 3529 2f61 785f 6362 2f70 772e  b,0.5)/ax_cb/pw.
+00003660: 7370 6163 6572 2861 785f 6362 2c30 2e35  spacer(ax_cb,0.5
+00003670: 2929 0a68 6561 746d 6170 322e 7361 7665  )).heatmap2.save
+00003680: 6669 6728 2222 290a 6060 600a 3c69 6d67  fig("").```.<img
+00003690: 2073 7263 3d22 696d 672f 6865 6174 6d61   src="img/heatma
+000036a0: 702d 332e 706e 6722 2077 6964 7468 3d22  p-3.png" width="
+000036b0: 3430 3078 3430 3022 3e0a 0a3c 2f64 6574  400x400">..</det
+000036c0: 6169 6c73 3e0a 0a0a 3c64 6574 6169 6c73  ails>...<details
+000036d0: 3e0a 3c73 756d 6d61 7279 3e20 3c62 3e30  >.<summary> <b>0
+000036e0: 3130 3732 3032 323a 2050 6174 6368 776f  1072022: Patchwo
+000036f0: 726b 6c69 6220 7761 7320 7570 6461 7465  rklib was update
+00003700: 6420 746f 2061 6c6c 6f77 2061 7272 616e  d to allow arran
+00003710: 6769 6e67 206d 756c 7469 706c 6520 706c  ging multiple pl
+00003720: 6f74 7320 6765 6e65 7261 7465 6420 6279  ots generated by
+00003730: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00003740: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6173  //github.com/has
+00003750: 326b 312f 706c 6f74 6e69 6e65 223e 706c  2k1/plotnine">pl
+00003760: 6f74 6e69 6e65 3c2f 613e 2e3c 2f62 3e20  otnine</a>.</b> 
+00003770: 3c2f 7375 6d6d 6172 793e 0a0a 6060 6070  </summary>..```p
+00003780: 7974 686f 6e0a 696d 706f 7274 2070 6174  ython.import pat
+00003790: 6368 776f 726b 6c69 6220 6173 2070 770a  chworklib as pw.
+000037a0: 6672 6f6d 2070 6c6f 746e 696e 6520 696d  from plotnine im
+000037b0: 706f 7274 202a 0a66 726f 6d20 706c 6f74  port *.from plot
+000037c0: 6e69 6e65 2e64 6174 6120 696d 706f 7274  nine.data import
+000037d0: 202a 0a67 3120 3d20 7077 2e6c 6f61 645f   *.g1 = pw.load_
+000037e0: 6767 706c 6f74 2867 6770 6c6f 7428 6d74  ggplot(ggplot(mt
+000037f0: 6361 7273 2920 2b20 6765 6f6d 5f70 6f69  cars) + geom_poi
+00003800: 6e74 2861 6573 2822 6d70 6722 2c20 2264  nt(aes("mpg", "d
+00003810: 6973 7022 2929 202b 2074 6865 6d65 2866  isp")) + theme(f
+00003820: 6967 7572 655f 7369 7a65 3d28 322c 2033  igure_size=(2, 3
+00003830: 2929 290a 6732 203d 2070 772e 6c6f 6164  ))).g2 = pw.load
+00003840: 5f67 6770 6c6f 7428 6767 706c 6f74 286d  _ggplot(ggplot(m
+00003850: 7463 6172 7329 202b 2067 656f 6d5f 626f  tcars) + geom_bo
+00003860: 7870 6c6f 7428 6165 7328 2267 6561 7222  xplot(aes("gear"
+00003870: 2c20 2264 6973 7022 2c20 6772 6f75 7020  , "disp", group 
+00003880: 3d20 2267 6561 7222 2929 202b 2074 6865  = "gear")) + the
+00003890: 6d65 2866 6967 7572 655f 7369 7a65 3d28  me(figure_size=(
+000038a0: 322c 2033 2929 290a 6731 3220 3d20 6731  2, 3))).g12 = g1
+000038b0: 207c 2067 320a 6731 322e 7361 7665 6669   | g2.g12.savefi
+000038c0: 6728 290a 6060 600a 0a3c 696d 6720 7372  g().```..<img sr
+000038d0: 633d 2269 6d67 2f67 3132 2e70 6e67 2220  c="img/g12.png" 
+000038e0: 7769 6474 683d 2234 3030 7834 3030 223e  width="400x400">
+000038f0: 0a0a 6060 6070 7974 686f 6e0a 6733 203d  ..```python.g3 =
+00003900: 2070 772e 6c6f 6164 5f67 6770 6c6f 7428   pw.load_ggplot(
+00003910: 6767 706c 6f74 286d 7067 2c20 6165 7328  ggplot(mpg, aes(
+00003920: 783d 2764 6973 706c 272c 2079 3d27 6877  x='displ', y='hw
+00003930: 7927 2929 202b 2067 656f 6d5f 706f 696e  y')) + geom_poin
+00003940: 7428 2920 2b20 6765 6f6d 5f73 6d6f 6f74  t() + geom_smoot
+00003950: 6828 7370 616e 3d2e 3329 202b 2074 6865  h(span=.3) + the
+00003960: 6d65 2866 6967 7572 655f 7369 7a65 3d28  me(figure_size=(
+00003970: 322c 2033 2929 290a 6734 203d 2070 772e  2, 3))).g4 = pw.
+00003980: 6c6f 6164 5f67 6770 6c6f 7428 6767 706c  load_ggplot(ggpl
+00003990: 6f74 286d 7463 6172 7329 202b 2067 656f  ot(mtcars) + geo
+000039a0: 6d5f 6261 7228 6165 7328 2263 6172 6222  m_bar(aes("carb"
+000039b0: 2929 202b 2074 6865 6d65 2866 6967 7572  )) + theme(figur
+000039c0: 655f 7369 7a65 3d28 372c 2032 2929 290a  e_size=(7, 2))).
+000039d0: 6731 3233 3420 3d20 2867 317c 6732 7c67  g1234 = (g1|g2|g
+000039e0: 3329 2f67 340a 6731 3233 342e 7361 7665  3)/g4.g1234.save
+000039f0: 6669 6728 290a 6060 600a 3c69 6d67 2073  fig().```.<img s
+00003a00: 7263 3d22 696d 672f 6731 3233 342e 706e  rc="img/g1234.pn
+00003a10: 6722 2077 6964 7468 3d22 3630 3078 3630  g" width="600x60
+00003a20: 3022 3e0a 0a3c 2f64 6574 6169 6c73 3e0a  0">..</details>.
+00003a30: 3c2f 6465 7461 696c 733e 200a 0a23 2320  </details> ..## 
+00003a40: 5573 6167 650a 3e20 5f49 6620 796f 7520  Usage.> _If you 
+00003a50: 7761 6e74 2074 6f20 6b6e 6f77 2068 6f77  want to know how
+00003a60: 2074 6f20 7573 6520 7061 7463 6877 6f72   to use patchwor
+00003a70: 6b6c 6962 2069 6e20 6465 7461 696c 2c20  klib in detail, 
+00003a80: 706c 6561 7365 2073 6565 205b 4150 492e  please see [API.
+00003a90: 6d64 5d28 6874 7470 733a 2f2f 6769 7468  md](https://gith
+00003aa0: 7562 2e63 6f6d 2f70 6f6e 6e68 6964 652f  ub.com/ponnhide/
+00003ab0: 7061 7463 6877 6f72 6b6c 6962 2f62 6c6f  patchworklib/blo
+00003ac0: 622f 6d61 696e 2f41 5049 2e6d 6429 2e5f  b/main/API.md)._
+00003ad0: 2020 0a3e 0a55 7369 6e67 2060 7061 7463    .>.Using `patc
+00003ae0: 6877 6f72 6b6c 6962 602c 2079 6f75 2063  hworklib`, you c
+00003af0: 616e 2071 7569 636b 6c79 2061 6e64 2066  an quickly and f
+00003b00: 7265 656c 7920 6172 7261 6e67 6520 6d61  reely arrange ma
+00003b10: 7470 6c6f 746c 6962 2070 6c6f 7473 2077  tplotlib plots w
+00003b20: 6974 6820 6f6e 6c79 2060 7c60 2061 6e64  ith only `|` and
+00003b30: 2060 2f60 206f 7061 7261 746f 7273 2061   `/` oparators a
+00003b40: 7320 666f 6c6c 6f77 732e 0a0a 6060 6070  s follows...```p
+00003b50: 7974 686f 6e0a 696d 706f 7274 2070 6174  ython.import pat
+00003b60: 6368 776f 726b 6c69 6220 6173 2070 770a  chworklib as pw.
+00003b70: 696d 706f 7274 2073 6561 626f 726e 2061  import seaborn a
+00003b80: 7320 736e 7320 0a0a 666d 7269 203d 2073  s sns ..fmri = s
+00003b90: 6e73 2e6c 6f61 645f 6461 7461 7365 7428  ns.load_dataset(
+00003ba0: 2266 6d72 6922 290a 6178 3120 3d20 7077  "fmri").ax1 = pw
+00003bb0: 2e42 7269 636b 2866 6967 7369 7a65 3d28  .Brick(figsize=(
+00003bc0: 332c 3229 290a 736e 732e 6c69 6e65 706c  3,2)).sns.linepl
+00003bd0: 6f74 2878 3d22 7469 6d65 706f 696e 7422  ot(x="timepoint"
+00003be0: 2c20 793d 2273 6967 6e61 6c22 2c20 6875  , y="signal", hu
+00003bf0: 653d 2272 6567 696f 6e22 2c20 7374 796c  e="region", styl
+00003c00: 653d 2265 7665 6e74 222c 2064 6174 613d  e="event", data=
+00003c10: 666d 7269 2c20 6178 3d61 7831 290a 6178  fmri, ax=ax1).ax
+00003c20: 312e 6c65 6765 6e64 2862 626f 785f 746f  1.legend(bbox_to
+00003c30: 5f61 6e63 686f 723d 2831 2e30 352c 2031  _anchor=(1.05, 1
+00003c40: 2e30 292c 206c 6f63 3d27 7570 7065 7220  .0), loc='upper 
+00003c50: 6c65 6674 2729 0a61 7831 2e73 6574 5f74  left').ax1.set_t
+00003c60: 6974 6c65 2822 6178 3122 290a 200a 7469  itle("ax1"). .ti
+00003c70: 7461 6e69 6320 3d20 736e 732e 6c6f 6164  tanic = sns.load
+00003c80: 5f64 6174 6173 6574 2822 7469 7461 6e69  _dataset("titani
+00003c90: 6322 290a 6178 3220 3d20 7077 2e42 7269  c").ax2 = pw.Bri
+00003ca0: 636b 2866 6967 7369 7a65 3d28 312c 3229  ck(figsize=(1,2)
+00003cb0: 290a 736e 732e 6261 7270 6c6f 7428 783d  ).sns.barplot(x=
+00003cc0: 2273 6578 222c 2079 3d22 7375 7276 6976  "sex", y="surviv
+00003cd0: 6564 222c 2068 7565 3d22 636c 6173 7322  ed", hue="class"
+00003ce0: 2c20 6461 7461 3d74 6974 616e 6963 2c20  , data=titanic, 
+00003cf0: 6178 3d61 7832 290a 6178 322e 6d6f 7665  ax=ax2).ax2.move
+00003d00: 5f6c 6567 656e 6428 6e65 775f 6c6f 633d  _legend(new_loc=
+00003d10: 2775 7070 6572 206c 6566 7427 2c20 6262  'upper left', bb
+00003d20: 6f78 5f74 6f5f 616e 6368 6f72 3d28 312e  ox_to_anchor=(1.
+00003d30: 3035 2c20 312e 3029 290a 6178 322e 7365  05, 1.0)).ax2.se
+00003d40: 745f 7469 746c 6528 2261 7832 2229 0a0a  t_title("ax2")..
+00003d50: 6178 3132 203d 2061 7831 7c61 7832 0a61  ax12 = ax1|ax2.a
+00003d60: 7831 322e 7361 7665 6669 6728 2261 7831  x12.savefig("ax1
+00003d70: 322e 706e 6722 290a 6060 600a 0a3c 696d  2.png").```..<im
+00003d80: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00003d90: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00003da0: 7465 6e74 2e63 6f6d 2f70 6f6e 6e68 6964  tent.com/ponnhid
+00003db0: 652f 7061 7463 6877 6f72 6b6c 6962 2f6d  e/patchworklib/m
+00003dc0: 6169 6e2f 696d 672f 6178 3132 2e70 6e67  ain/img/ax12.png
+00003dd0: 2220 7769 6474 683d 2236 3030 7836 3030  " width="600x600
+00003de0: 223e 0a0a 4a75 7079 7465 7220 4e6f 7465  ">..Jupyter Note
+00003df0: 626f 6f6b 2066 696c 6573 2066 6f72 2061  book files for a
+00003e00: 6c6c 206f 6620 7468 6520 6578 616d 706c  ll of the exampl
+00003e10: 6520 636f 6465 7320 6172 6520 7072 6f76  e codes are prov
+00003e20: 6964 6564 2069 6e20 5b70 6174 6368 776f  ided in [patchwo
+00003e30: 726b 6c69 622d 6578 616d 706c 6573 5d28  rklib-examples](
+00003e40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003e50: 6f6d 2f70 6f6e 6e68 6964 652f 7061 7463  om/ponnhide/patc
+00003e60: 6877 6f72 6b6c 6962 2d65 7861 6d70 6c65  hworklib-example
+00003e70: 7329 2061 6e64 2061 6c73 6f20 6d61 6465  s) and also made
+00003e80: 2065 7865 6375 7461 626c 6520 696e 2047   executable in G
+00003e90: 6f6f 676c 6520 436f 6c61 626f 7261 746f  oogle Colaborato
+00003ea0: 7279 2e0a 2d20 5b74 7574 6f72 6961 6c5d  ry..- [tutorial]
+00003eb0: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
+00003ec0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00003ed0: 6f6d 2f64 7269 7665 2f31 4e66 6a79 754b  om/drive/1NfjyuK
+00003ee0: 5039 6e71 414d 3068 616e 7652 4851 502d  P9nqAM0hanvRHQP-
+00003ef0: 6b44 3167 626d 5039 517a 3f75 7370 3d73  kD1gbmP9Qz?usp=s
+00003f00: 6861 7269 6e67 293a 2042 6173 6963 2065  haring): Basic e
+00003f10: 7861 6d70 6c65 2063 6f64 6573 206f 6620  xample codes of 
+00003f20: 7061 7463 6877 6f72 6b6c 6962 200a 2d20  patchworklib .- 
+00003f30: 5b73 7562 706c 6f74 7320 666f 7220 706c  [subplots for pl
+00003f40: 6f74 6e69 6e65 5d28 6874 7470 733a 2f2f  otnine](https://
+00003f50: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00003f60: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
+00003f70: 3137 6f74 5870 7668 2d6a 4c6e 306a 6f49  17otXpvh-jLn0joI
+00003f80: 324d 7764 7954 3652 4b4a 7a78 3641 6e77  2MwdyT6RKJzx6Anw
+00003f90: 703f 7573 703d 7368 6172 696e 6729 3a20  p?usp=sharing): 
+00003fa0: 4172 7261 6e67 696e 6720 706c 6f74 6e69  Arranging plotni
+00003fb0: 6e65 2070 6c6f 7473 2075 7369 6e67 2070  ne plots using p
+00003fc0: 6174 6368 776f 726b 6c69 620a 2d20 5b73  atchworklib.- [s
+00003fd0: 7562 706c 6f74 7320 666f 7220 7365 6162  ubplots for seab
+00003fe0: 6f72 6e67 7269 645d 2868 7474 7073 3a2f  orngrid](https:/
+00003ff0: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+00004000: 676f 6f67 6c65 2e63 6f6d 2f64 7269 7665  google.com/drive
+00004010: 2f31 4331 454e 312d 354c 3251 6a6e 4141  /1C1EN1-5L2QjnAA
+00004020: 566f 3476 7078 5f69 396b 6e44 527a 5834  Vo4vpx_i9knDRzX4
+00004030: 6a79 3f75 7370 3d73 6861 7269 6e67 293a  jy?usp=sharing):
+00004040: 2041 7272 616e 6769 6e67 2066 6967 7572   Arranging figur
+00004050: 652d 6c65 7665 6c20 7365 6162 6f72 6e20  e-level seaborn 
+00004060: 706c 6f74 7320 7573 696e 6720 7061 7463  plots using patc
+00004070: 6877 6f72 6b6c 6962 0a2d 205b 706c 6163  hworklib.- [plac
+00004080: 696e 675f 7375 7065 725f 656c 656d 656e  ing_super_elemen
+00004090: 7473 5d28 6874 7470 733a 2f2f 636f 6c61  ts](https://cola
+000040a0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+000040b0: 652e 636f 6d2f 6472 6976 652f 3166 3036  e.com/drive/1f06
+000040c0: 4151 4f71 4e6e 5359 506a 6339 456b 7765  AQOqNnSYPjc9Ekwe
+000040d0: 4333 5f48 6d79 3461 6272 2d67 6f3f 7573  C3_Hmy4abr-go?us
+000040e0: 703d 7368 6172 696e 6729 3a20 506c 6163  p=sharing): Plac
+000040f0: 696e 6720 7375 7065 7220 6c61 6265 6c73  ing super labels
+00004100: 2061 6e64 2073 7069 6e65 7320 666f 7220   and spines for 
+00004110: 6120 7365 7420 6f66 206d 756c 7469 706c  a set of multipl
+00004120: 6520 7375 6270 6c6f 7473 2e20 200a 416c  e subplots.  .Al
+00004130: 736f 2c20 706c 6561 7365 2073 6565 2068  so, please see h
+00004140: 7474 7073 3a2f 2f70 7974 686f 6e2e 706c  ttps://python.pl
+00004150: 6169 6e65 6e67 6c69 7368 2e69 6f2f 612d  ainenglish.io/a-
+00004160: 7375 6270 6c6f 742d 6d61 6e61 6765 722d  subplot-manager-
+00004170: 666f 722d 696e 7475 6974 6976 652d 6c61  for-intuitive-la
+00004180: 796f 7574 2d69 6e2d 6d61 7470 6c6f 746c  yout-in-matplotl
+00004190: 6962 2d62 6430 3337 6665 3936 3766 340a  ib-bd037fe967f4.
+000041a0: 2323 2047 616c 6c65 7279 0a0a 2a2a 4172  ## Gallery..**Ar
+000041b0: 7261 6e67 656d 656e 7420 6f66 206d 756c  rangement of mul
+000041c0: 7469 706c 6520 6178 6973 2d6c 6576 656c  tiple axis-level
+000041d0: 2073 6561 626f 726e 2070 6c6f 7473 2a2a   seaborn plots**
+000041e0: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+000041f0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00004200: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6f6e  rcontent.com/pon
+00004210: 6e68 6964 652f 7061 7463 6877 6f72 6b6c  nhide/patchworkl
+00004220: 6962 2f6d 6169 6e2f 696d 672f 6178 3335  ib/main/img/ax35
+00004230: 3231 345f 7633 2e70 6e67 2220 7769 6474  214_v3.png" widt
+00004240: 683d 2231 3030 3078 3130 3030 223e 0a0a  h="1000x1000">..
+00004250: 2a2a 4172 7261 6e67 656d 656e 7420 6f66  **Arrangement of
+00004260: 206d 756c 7469 706c 6520 506c 6f74 6e69   multiple Plotni
+00004270: 6e65 2070 6c6f 7473 2a2a 0a3c 696d 6720  ne plots**.<img 
+00004280: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00004290: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000042a0: 6e74 2e63 6f6d 2f70 6f6e 6e68 6964 652f  nt.com/ponnhide/
+000042b0: 7061 7463 6877 6f72 6b6c 6962 2f6d 6169  patchworklib/mai
+000042c0: 6e2f 696d 672f 706c 6f74 6e69 6e65 2e70  n/img/plotnine.p
+000042d0: 6e67 2220 7769 6474 683d 2231 3030 3078  ng" width="1000x
+000042e0: 3130 3030 223e 0a0a 2a2a 4172 7261 6e67  1000">..**Arrang
+000042f0: 656d 656e 7420 6f66 206d 756c 7469 706c  ement of multipl
+00004300: 6520 6669 6775 7265 2d6c 6576 656c 2073  e figure-level s
+00004310: 6561 626f 726e 2070 6c6f 7473 2a2a 0a3c  eaborn plots**.<
+00004320: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00004330: 2f64 6576 2d74 6f2d 7570 6c6f 6164 732e  /dev-to-uploads.
+00004340: 7333 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  s3.amazonaws.com
+00004350: 2f75 706c 6f61 6473 2f61 7274 6963 6c65  /uploads/article
+00004360: 732f 6939 6433 796f 6763 7471 3634 7336  s/i9d3yogctq64s6
+00004370: 6a33 3369 7962 2e70 6e67 2220 7769 6474  j33iyb.png" widt
+00004380: 683d 2231 3030 3078 3130 3030 223e 0a0a  h="1000x1000">..
+00004390: 2323 2320 4765 7474 696e 6720 7374 6172  ### Getting star
+000043a0: 7465 640a 0a3c 6465 7461 696c 733e 0a3c  ted..<details>.<
+000043b0: 7375 6d6d 6172 793e 4578 616d 706c 6520  summary>Example 
+000043c0: 636f 6465 733c 2f73 756d 6d61 7279 3e0a  codes</summary>.
+000043d0: 0a2a 2a54 7574 6f72 6961 6c20 5c7e 2a43  .**Tutorial \~*C
+000043e0: 6f6d 706f 7365 206d 756c 7469 706c 6520  ompose multiple 
+000043f0: 7365 6162 6f72 6e20 706c 6f74 732a 5c7e  seaborn plots*\~
+00004400: 2a2a 0a54 6865 2066 6f6c 6c77 6f69 6e67  **.The follwoing
+00004410: 2074 7574 6f72 6961 6c20 636f 6465 7320   tutorial codes 
+00004420: 6361 6e20 6265 2065 7865 6375 7461 626c  can be executabl
+00004430: 6520 696e 205b 7475 746f 7269 616c 315d  e in [tutorial1]
+00004440: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
+00004450: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00004460: 6f6d 2f64 7269 7665 2f31 5456 6348 3349  om/drive/1TVcH3I
+00004470: 4a79 3667 6544 5856 4a44 664f 4b43 5046  Jy6geDXVJDfOKCPF
+00004480: 5073 5032 477a 6a78 4875 3f75 7370 3d73  PsP2GzjxHu?usp=s
+00004490: 6861 7269 6e67 290a 0a23 2323 2320 312e  haring)..#### 1.
+000044a0: 2049 6d70 6f72 7469 6e67 2070 6174 6368   Importing patch
+000044b0: 776f 726b 6c69 6220 6c69 6272 6172 790a  worklib library.
+000044c0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+000044d0: 7420 7061 7463 6877 6f72 6b6c 6962 2061  t patchworklib a
+000044e0: 7320 7077 200a 666d 7269 203d 2073 6e73  s pw .fmri = sns
+000044f0: 2e6c 6f61 645f 6461 7461 7365 7428 2266  .load_dataset("f
+00004500: 6d72 6922 290a 6178 3120 3d20 7077 2e42  mri").ax1 = pw.B
+00004510: 7269 636b 2822 6178 3122 2c20 6669 6773  rick("ax1", figs
+00004520: 697a 653d 2834 2c32 2929 0a73 6e73 2e6c  ize=(4,2)).sns.l
+00004530: 696e 6570 6c6f 7428 783d 2274 696d 6570  ineplot(x="timep
+00004540: 6f69 6e74 222c 2079 3d22 7369 676e 616c  oint", y="signal
+00004550: 222c 2068 7565 3d22 7265 6769 6f6e 222c  ", hue="region",
+00004560: 2073 7479 6c65 3d22 6576 656e 7422 2c20   style="event", 
+00004570: 6461 7461 3d66 6d72 692c 2061 783d 6178  data=fmri, ax=ax
+00004580: 3129 0a61 7831 2e6d 6f76 655f 6c65 6765  1).ax1.move_lege
+00004590: 6e64 286e 6577 5f6c 6f63 3d27 7570 7065  nd(new_loc='uppe
+000045a0: 7220 7269 6768 7427 290a 6178 312e 7365  r right').ax1.se
+000045b0: 745f 7469 746c 6528 2261 7831 2229 0a60  t_title("ax1").`
+000045c0: 6060 0a0a 2323 2323 2032 2e20 4372 6561  ``..#### 2. Crea
+000045d0: 7469 6e67 2065 7861 6d70 6c65 2070 6c6f  ting example plo
+000045e0: 7473 0a20 0a43 7265 6174 696e 6720 736f  ts. .Creating so
+000045f0: 6d65 2065 7861 6d70 6c65 2070 6c6f 7473  me example plots
+00004600: 2075 7369 6e67 2074 6865 2073 6561 7262   using the searb
+00004610: 6f72 6e20 6d6f 6475 6c65 2e20 4272 6963  orn module. Bric
+00004620: 6b20 636c 6173 7320 7072 6f76 6964 6564  k class provided
+00004630: 2062 7920 7468 6520 7061 7463 6877 6f72   by the patchwor
+00004640: 6b6c 6962 206d 6f64 756c 6520 6973 2069  klib module is i
+00004650: 6d70 6c65 6d65 6e74 6564 2061 7320 7375  mplemented as su
+00004660: 6263 6c61 7373 206f 6620 606d 6174 706c  bclass of `matpl
+00004670: 6f74 6c69 622e 6178 6573 2e41 7865 7360  otlib.axes.Axes`
+00004680: 2e20 2054 6865 7265 666f 7265 2c20 4272  .  Therefore, Br
+00004690: 6963 6b20 636c 6173 7320 6f62 6a65 6374  ick class object
+000046a0: 2063 616e 2062 6520 6769 7665 6e20 746f   can be given to
+000046b0: 2074 6865 2073 6561 626f 726e 2070 6c6f   the seaborn plo
+000046c0: 7420 6675 6e63 7469 6f6e 7320 7468 6174  t functions that
+000046d0: 2068 6176 6520 7468 6520 6061 7860 2070   have the `ax` p
+000046e0: 6172 616d 6574 6572 732e 2020 0a0a 5768  arameters.  ..Wh
+000046f0: 656e 2063 7265 6174 696e 6720 6120 4272  en creating a Br
+00004700: 6963 6b20 636c 6173 7320 6f62 6a65 6374  ick class object
+00004710: 2c20 7468 6520 606c 6162 656c 6020 7661  , the `label` va
+00004720: 6c75 6520 7368 6f75 6c64 2062 6520 7370  lue should be sp
+00004730: 6563 6966 6965 642c 2061 6e64 2069 7420  ecified, and it 
+00004740: 7368 6f75 6c64 2062 6520 756e 6971 7565  should be unique
+00004750: 2061 6d6f 6e67 2074 6865 2042 7269 636b   among the Brick
+00004760: 2063 6c61 7373 206f 626a 6563 7473 2067   class objects g
+00004770: 656e 6572 6174 6564 2069 6e20 7468 6520  enerated in the 
+00004780: 7079 7468 6f6e 2073 6372 6970 7420 2849  python script (I
+00004790: 6620 7468 6520 6c61 6265 6c20 7661 6c75  f the label valu
+000047a0: 6520 6973 206e 6f74 2073 7065 6369 6669  e is not specifi
+000047b0: 6564 2c20 7468 6520 756e 6971 7565 206c  ed, the unique l
+000047c0: 6162 656c 206e 616d 6520 6973 2061 7574  abel name is aut
+000047d0: 6f6d 6174 6963 616c 6c79 2067 6976 656e  omatically given
+000047e0: 2e20 4279 2075 7369 6e67 2060 6765 745f  . By using `get_
+000047f0: 6c61 6265 6c28 2960 206d 6574 686f 642c  label()` method,
+00004800: 2074 6865 2076 616c 7565 2063 616e 2062   the value can b
+00004810: 6520 636f 6e66 6972 6d65 6429 2e20 5468  e confirmed). Th
+00004820: 6520 6066 6967 6973 697a 6560 2070 6172  e `figisize` par
+00004830: 616d 6574 6572 2063 616e 2061 6c73 6f20  ameter can also 
+00004840: 6265 2073 7065 6369 6669 6564 2e20 486f  be specified. Ho
+00004850: 7765 7665 722c 2074 6865 2076 616c 7565  wever, the value
+00004860: 2069 7320 6e6f 7420 7665 7279 2069 6d70   is not very imp
+00004870: 6f72 7461 6e74 2062 6563 6175 7365 2074  ortant because t
+00004880: 6865 2066 6967 7572 6520 7369 7a65 206f  he figure size o
+00004890: 6620 4272 6963 6b20 636c 6173 7320 6f62  f Brick class ob
+000048a0: 6a65 6374 7320 6361 6e20 6265 2061 7574  jects can be aut
+000048b0: 6f6d 6174 6963 616c 6c79 2061 646a 7573  omatically adjus
+000048c0: 7465 6420 696e 2061 7272 616e 6769 6e67  ted in arranging
+000048d0: 2074 6865 2070 6c6f 7473 2e20 5468 6520   the plots. The 
+000048e0: 6073 6176 6566 6967 2860 2a60 6669 6c65  `savefig(`*`file
+000048f0: 6e61 6d65 3d73 7472 602a 6029 6020 6d65  name=str`*`)` me
+00004900: 7468 6f64 2072 6574 7572 6e73 2060 6d61  thod returns `ma
+00004910: 7470 6c6f 746c 6962 2e66 6967 7572 652e  tplotlib.figure.
+00004920: 4669 6775 7265 6020 636c 6173 7320 6f62  Figure` class ob
+00004930: 6a65 6374 2e20 4966 2060 6669 6c65 6e61  ject. If `filena
+00004940: 6d65 6020 6973 2067 6976 656e 2c20 7468  me` is given, th
+00004950: 6520 6669 6775 7265 206f 626a 6563 7420  e figure object 
+00004960: 6361 6e20 6265 206f 7574 7075 7420 746f  can be output to
+00004970: 2074 6865 2066 696c 652e 0a0a 6060 6070   the file...```p
+00004980: 7974 686f 6e0a 696d 706f 7274 2073 6561  ython.import sea
+00004990: 626f 726e 2061 7320 736e 730a 2345 7861  born as sns.#Exa
+000049a0: 6d70 6c65 2070 6c6f 7420 3120 2872 6566  mple plot 1 (ref
+000049b0: 3a20 6874 7470 733a 2f2f 7365 6162 6f72  : https://seabor
+000049c0: 6e2e 7079 6461 7461 2e6f 7267 2f65 7861  n.pydata.org/exa
+000049d0: 6d70 6c65 732f 6572 726f 7262 616e 645f  mples/errorband_
+000049e0: 6c69 6e65 706c 6f74 732e 6874 6d6c 290a  lineplots.html).
+000049f0: 666d 7269 203d 2073 6e73 2e6c 6f61 645f  fmri = sns.load_
+00004a00: 6461 7461 7365 7428 2266 6d72 6922 290a  dataset("fmri").
+00004a10: 6178 3120 3d20 7077 2e42 7269 636b 2822  ax1 = pw.Brick("
+00004a20: 6178 3122 2c20 6669 6773 697a 653d 2834  ax1", figsize=(4
+00004a30: 2c32 2929 0a73 6e73 2e6c 696e 6570 6c6f  ,2)).sns.lineplo
+00004a40: 7428 783d 2274 696d 6570 6f69 6e74 222c  t(x="timepoint",
+00004a50: 2079 3d22 7369 676e 616c 222c 2068 7565   y="signal", hue
+00004a60: 3d22 7265 6769 6f6e 222c 2073 7479 6c65  ="region", style
+00004a70: 3d22 6576 656e 7422 2c20 6461 7461 3d66  ="event", data=f
+00004a80: 6d72 692c 2061 783d 6178 3129 0a61 7831  mri, ax=ax1).ax1
+00004a90: 2e6d 6f76 655f 6c65 6765 6e64 286e 6577  .move_legend(new
+00004aa0: 5f6c 6f63 3d27 7570 7065 7220 7269 6768  _loc='upper righ
+00004ab0: 7427 290a 6178 312e 7365 745f 7469 746c  t').ax1.set_titl
+00004ac0: 6528 2261 7831 2229 0a61 7831 2e73 6176  e("ax1").ax1.sav
+00004ad0: 6566 6967 2829 0a60 6060 0a0a 3c69 6d67  efig().```..<img
+00004ae0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00004af0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00004b00: 656e 742e 636f 6d2f 706f 6e6e 6869 6465  ent.com/ponnhide
+00004b10: 2f70 6174 6368 776f 726b 6c69 622f 6d61  /patchworklib/ma
+00004b20: 696e 2f69 6d67 2f61 7831 2e70 6e67 2220  in/img/ax1.png" 
+00004b30: 7769 6474 683d 2233 3530 7833 3530 223e  width="350x350">
+00004b40: 0a0a 4272 6963 6b20 636c 6173 7320 7072  ..Brick class pr
+00004b50: 6f76 6964 6573 2074 6865 2060 6d6f 7665  ovides the `move
+00004b60: 6c65 6765 6e64 2860 2a60 6c6f 633d 7374  legend(`*`loc=st
+00004b70: 722c 2062 626f 785f 746f 5f61 6e63 686f  r, bbox_to_ancho
+00004b80: 723d 2866 6c6f 6174 2c66 6c6f 6174 2960  r=(float,float)`
+00004b90: 2a60 2960 206d 6574 686f 642e 2042 7920  *`)` method. By 
+00004ba0: 7573 696e 6720 7468 6973 206d 6574 686f  using this metho
+00004bb0: 642c 206c 6567 656e 6420 6c6f 6361 7469  d, legend locati
+00004bc0: 6f6e 2063 616e 2062 6520 7175 6963 6b6c  on can be quickl
+00004bd0: 7920 6d6f 6469 6669 6564 2e0a 0a60 6060  y modified...```
+00004be0: 7079 7468 6f6e 0a23 4578 616d 706c 6520  python.#Example 
+00004bf0: 706c 6f74 2032 2028 7265 663a 2068 7474  plot 2 (ref: htt
+00004c00: 7073 3a2f 2f73 6561 626f 726e 2e70 7964  ps://seaborn.pyd
+00004c10: 6174 612e 6f72 672f 7475 746f 7269 616c  ata.org/tutorial
+00004c20: 2f63 6174 6567 6f72 6963 616c 2e68 746d  /categorical.htm
+00004c30: 6c29 0a74 6974 616e 6963 203d 2073 6e73  l).titanic = sns
+00004c40: 2e6c 6f61 645f 6461 7461 7365 7428 2274  .load_dataset("t
+00004c50: 6974 616e 6963 2229 0a61 7832 203d 2070  itanic").ax2 = p
+00004c60: 772e 4272 6963 6b28 2261 7832 222c 2066  w.Brick("ax2", f
+00004c70: 6967 7369 7a65 3d28 312c 3229 290a 736e  igsize=(1,2)).sn
+00004c80: 732e 6261 7270 6c6f 7428 783d 2273 6578  s.barplot(x="sex
+00004c90: 222c 2079 3d22 7375 7276 6976 6564 222c  ", y="survived",
+00004ca0: 2068 7565 3d22 636c 6173 7322 2c20 6461   hue="class", da
+00004cb0: 7461 3d74 6974 616e 6963 2c20 6178 3d61  ta=titanic, ax=a
+00004cc0: 7832 290a 6178 322e 6d6f 7665 5f6c 6567  x2).ax2.move_leg
+00004cd0: 656e 6428 6e65 775f 6c6f 633d 2775 7070  end(new_loc='upp
+00004ce0: 6572 206c 6566 7427 2c20 6262 6f78 5f74  er left', bbox_t
+00004cf0: 6f5f 616e 6368 6f72 3d28 312e 3035 2c20  o_anchor=(1.05, 
+00004d00: 312e 3029 2920 234f 7269 6769 6e61 6c20  1.0)) #Original 
+00004d10: 6d65 7468 6f64 206f 6620 426c 6963 6b20  method of Blick 
+00004d20: 636c 6173 730a 6178 322e 7365 745f 7469  class.ax2.set_ti
+00004d30: 746c 6528 2261 7832 2229 0a61 7832 2e73  tle("ax2").ax2.s
+00004d40: 6176 6566 6967 2829 0a60 6060 0a0a 3c69  avefig().```..<i
+00004d50: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00004d60: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00004d70: 6e74 656e 742e 636f 6d2f 706f 6e6e 6869  ntent.com/ponnhi
+00004d80: 6465 2f70 6174 6368 776f 726b 6c69 622f  de/patchworklib/
+00004d90: 6d61 696e 2f69 6d67 2f61 7832 2e70 6e67  main/img/ax2.png
+00004da0: 2220 7769 6474 683d 2232 3530 7832 3530  " width="250x250
+00004db0: 223e 0a0a 6060 6070 7974 686f 6e0a 2345  ">..```python.#E
+00004dc0: 7861 6d70 6c65 2070 6c6f 7420 3320 2872  xample plot 3 (r
+00004dd0: 6566 3a20 6874 7470 733a 2f2f 7365 6162  ef: https://seab
+00004de0: 6f72 6e2e 7079 6461 7461 2e6f 7267 2f65  orn.pydata.org/e
+00004df0: 7861 6d70 6c65 732f 6869 7374 6f67 7261  xamples/histogra
+00004e00: 6d5f 7374 6163 6b65 642e 6874 6d6c 290a  m_stacked.html).
+00004e10: 6469 616d 6f6e 6473 203d 2073 6e73 2e6c  diamonds = sns.l
+00004e20: 6f61 645f 6461 7461 7365 7428 2264 6961  oad_dataset("dia
+00004e30: 6d6f 6e64 7322 290a 6178 3320 3d20 7077  monds").ax3 = pw
+00004e40: 2e42 7269 636b 2822 6178 3322 2c20 2835  .Brick("ax3", (5
+00004e50: 2c32 2929 0a73 6e73 2e68 6973 7470 6c6f  ,2)).sns.histplo
+00004e60: 7428 6469 616d 6f6e 6473 2c20 783d 2270  t(diamonds, x="p
+00004e70: 7269 6365 222c 2068 7565 3d22 6375 7422  rice", hue="cut"
+00004e80: 2c20 6d75 6c74 6970 6c65 3d22 7374 6163  , multiple="stac
+00004e90: 6b22 2c0a 2020 2020 7061 6c65 7474 653d  k",.    palette=
+00004ea0: 226c 6967 6874 3a6d 5f72 222c 2065 6467  "light:m_r", edg
+00004eb0: 6563 6f6c 6f72 3d22 2e33 222c 206c 696e  ecolor=".3", lin
+00004ec0: 6577 6964 7468 3d2e 352c 206c 6f67 5f73  ewidth=.5, log_s
+00004ed0: 6361 6c65 3d54 7275 652c 0a20 2020 2061  cale=True,.    a
+00004ee0: 7820 3d20 6178 3329 0a61 7833 2e73 6574  x = ax3).ax3.set
+00004ef0: 5f74 6974 6c65 2822 6178 3322 290a 6178  _title("ax3").ax
+00004f00: 332e 7361 7665 6669 6728 290a 6060 600a  3.savefig().```.
+00004f10: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+00004f20: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00004f30: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6f6e  rcontent.com/pon
+00004f40: 6e68 6964 652f 7061 7463 6877 6f72 6b6c  nhide/patchworkl
+00004f50: 6962 2f6d 6169 6e2f 696d 672f 6178 332e  ib/main/img/ax3.
+00004f60: 706e 6722 2077 6964 7468 3d22 3430 3078  png" width="400x
+00004f70: 3430 3022 3e0a 0a60 6060 7079 7468 6f6e  400">..```python
+00004f80: 0a23 4578 616d 706c 6520 706c 6f74 2034  .#Example plot 4
+00004f90: 2028 7265 663a 6874 7470 733a 2f2f 7365   (ref:https://se
+00004fa0: 6162 6f72 6e2e 7079 6461 7461 2e6f 7267  aborn.pydata.org
+00004fb0: 2f65 7861 6d70 6c65 732f 6772 6f75 7065  /examples/groupe
+00004fc0: 645f 7669 6f6c 696e 706c 6f74 732e 6874  d_violinplots.ht
+00004fd0: 6d6c 290a 7469 7073 203d 2073 6e73 2e6c  ml).tips = sns.l
+00004fe0: 6f61 645f 6461 7461 7365 7428 2274 6970  oad_dataset("tip
+00004ff0: 7322 290a 6178 3420 3d20 7077 2e42 7269  s").ax4 = pw.Bri
+00005000: 636b 2822 6178 3422 2c20 2836 2c32 2929  ck("ax4", (6,2))
+00005010: 0a73 6e73 2e76 696f 6c69 6e70 6c6f 7428  .sns.violinplot(
+00005020: 6461 7461 3d74 6970 732c 2078 3d22 6461  data=tips, x="da
+00005030: 7922 2c20 793d 2274 6f74 616c 5f62 696c  y", y="total_bil
+00005040: 6c22 2c20 6875 653d 2273 6d6f 6b65 7222  l", hue="smoker"
+00005050: 2c0a 2020 2020 7370 6c69 743d 5472 7565  ,.    split=True
+00005060: 2c20 696e 6e65 723d 2271 7561 7274 222c  , inner="quart",
+00005070: 206c 696e 6577 6964 7468 3d31 2c0a 2020   linewidth=1,.  
+00005080: 2020 7061 6c65 7474 653d 7b22 5965 7322    palette={"Yes"
+00005090: 3a20 2262 222c 2022 4e6f 223a 2022 2e38  : "b", "No": ".8
+000050a0: 3522 7d2c 0a20 2020 2061 783d 6178 3429  5"},.    ax=ax4)
+000050b0: 0a61 7834 2e73 6574 5f74 6974 6c65 2822  .ax4.set_title("
+000050c0: 6178 3422 290a 6178 342e 7361 7665 6669  ax4").ax4.savefi
+000050d0: 6728 222e 2e2f 696d 672f 6178 342e 706e  g("../img/ax4.pn
+000050e0: 6722 290a 6060 600a 0a3c 696d 6720 7372  g").```..<img sr
+000050f0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00005100: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00005110: 2e63 6f6d 2f70 6f6e 6e68 6964 652f 7061  .com/ponnhide/pa
+00005120: 7463 6877 6f72 6b6c 6962 2f6d 6169 6e2f  tchworklib/main/
+00005130: 696d 672f 6178 342e 706e 6722 2077 6964  img/ax4.png" wid
+00005140: 7468 3d22 3430 3078 3430 3022 3e0a 0a60  th="400x400">..`
+00005150: 6060 7079 7468 6f6e 0a23 4578 616d 706c  ``python.#Exampl
+00005160: 6520 706c 6f74 2035 2028 7265 663a 6874  e plot 5 (ref:ht
+00005170: 7470 733a 2f2f 7365 6162 6f72 6e2e 7079  tps://seaborn.py
+00005180: 6461 7461 2e6f 7267 2f65 7861 6d70 6c65  data.org/example
+00005190: 732f 7769 6465 5f64 6174 615f 6c69 6e65  s/wide_data_line
+000051a0: 706c 6f74 2e68 746d 6c29 0a72 7320 3d20  plot.html).rs = 
+000051b0: 6e70 2e72 616e 646f 6d2e 5261 6e64 6f6d  np.random.Random
+000051c0: 5374 6174 6528 3336 3529 0a76 616c 7565  State(365).value
+000051d0: 7320 3d20 7273 2e72 616e 646e 2833 3635  s = rs.randn(365
+000051e0: 2c20 3429 2e63 756d 7375 6d28 6178 6973  , 4).cumsum(axis
+000051f0: 3d30 290a 6461 7465 7320 3d20 7064 2e64  =0).dates = pd.d
+00005200: 6174 655f 7261 6e67 6528 2231 2031 2032  ate_range("1 1 2
+00005210: 3031 3622 2c20 7065 7269 6f64 733d 3336  016", periods=36
+00005220: 352c 2066 7265 713d 2244 2229 0a64 6174  5, freq="D").dat
+00005230: 6120 3d20 7064 2e44 6174 6146 7261 6d65  a = pd.DataFrame
+00005240: 2876 616c 7565 732c 2064 6174 6573 2c20  (values, dates, 
+00005250: 636f 6c75 6d6e 733d 5b22 4122 2c20 2242  columns=["A", "B
+00005260: 222c 2022 4322 2c20 2244 225d 290a 6461  ", "C", "D"]).da
+00005270: 7461 203d 2064 6174 612e 726f 6c6c 696e  ta = data.rollin
+00005280: 6728 3729 2e6d 6561 6e28 290a 6178 3520  g(7).mean().ax5 
+00005290: 3d20 7077 2e42 7269 636b 2822 6178 3522  = pw.Brick("ax5"
+000052a0: 2c20 2835 2c32 2929 0a73 6e73 2e6c 696e  , (5,2)).sns.lin
+000052b0: 6570 6c6f 7428 6461 7461 3d64 6174 612c  eplot(data=data,
+000052c0: 2070 616c 6574 7465 3d22 7461 6231 3022   palette="tab10"
+000052d0: 2c20 6c69 6e65 7769 6474 683d 322e 352c  , linewidth=2.5,
+000052e0: 2061 783d 6178 3529 0a61 7835 2e73 6574   ax=ax5).ax5.set
+000052f0: 5f78 6c61 6265 6c28 2264 6174 6522 290a  _xlabel("date").
+00005300: 6178 352e 7365 745f 796c 6162 656c 2822  ax5.set_ylabel("
+00005310: 7661 6c75 6522 290a 6178 352e 7365 745f  value").ax5.set_
+00005320: 7469 746c 6528 2261 7835 2229 0a61 7835  title("ax5").ax5
+00005330: 2e73 6176 6566 6967 2829 0a60 6060 0a0a  .savefig().```..
+00005340: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00005350: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00005360: 636f 6e74 656e 742e 636f 6d2f 706f 6e6e  content.com/ponn
+00005370: 6869 6465 2f70 6174 6368 776f 726b 6c69  hide/patchworkli
+00005380: 622f 6d61 696e 2f69 6d67 2f61 7835 2e70  b/main/img/ax5.p
+00005390: 6e67 2220 7769 6474 683d 2234 3030 7834  ng" width="400x4
+000053a0: 3030 223e 0a0a 2323 2323 2033 2e20 4172  00">..#### 3. Ar
+000053b0: 7261 6e67 696e 6720 616e 6420 7374 6163  ranging and stac
+000053c0: 6b69 6e67 2070 6c6f 7473 0a0a 5468 6520  king plots..The 
+000053d0: 7061 7463 6877 6f72 6b6c 6962 206d 6f64  patchworklib mod
+000053e0: 756c 6520 7072 6f76 6964 6573 2074 776f  ule provides two
+000053f0: 206f 7065 7261 746f 7273 2022 2060 7c60   operators " `|`
+00005400: 222c 2022 602f 6022 2074 6861 7420 656e  ", "`/`" that en
+00005410: 6162 6c65 2064 6573 6967 6e69 6e67 2074  able designing t
+00005420: 6964 7920 6c61 796f 7574 2066 6f72 206d  idy layout for m
+00005430: 756c 7469 706c 6520 706c 6f74 7320 7769  ultiple plots wi
+00005440: 7468 2073 696d 706c 6520 6f70 6572 6174  th simple operat
+00005450: 696f 6e73 2e20 5468 6520 2260 7c60 2220  ions. The "`|`" 
+00005460: 6f70 6572 6174 6f72 2077 696c 6c20 706c  operator will pl
+00005470: 6163 6520 7468 6520 706c 6f74 7320 6265  ace the plots be
+00005480: 7369 6465 2065 6163 6820 6f74 6865 722c  side each other,
+00005490: 2077 6869 6c65 2074 6865 2022 602f 6022   while the "`/`"
+000054a0: 206f 7065 7261 746f 7220 7769 6c6c 2073   operator will s
+000054b0: 7461 636b 2074 6865 6d2e 0a0a 6060 6070  tack them...```p
+000054c0: 7974 686f 6e0a 2341 7272 616e 6765 2022  ython.#Arrange "
+000054d0: 6178 312c 2220 2261 7832 2c22 2061 6e64  ax1," "ax2," and
+000054e0: 2022 6178 3422 2068 6f72 697a 6f6e 7461   "ax4" horizonta
+000054f0: 6c6c 792e 0a61 7831 3234 203d 2061 7831  lly..ax124 = ax1
+00005500: 7c61 7832 7c61 7834 0a61 7831 3234 2e73  |ax2|ax4.ax124.s
+00005510: 6176 6566 6967 2822 2e2e 2f69 6d67 2f61  avefig("../img/a
+00005520: 7831 3234 2e70 6e67 2229 0a60 6060 0a0a  x124.png").```..
+00005530: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00005540: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00005550: 636f 6e74 656e 742e 636f 6d2f 706f 6e6e  content.com/ponn
+00005560: 6869 6465 2f70 6174 6368 776f 726b 6c69  hide/patchworkli
+00005570: 622f 6d61 696e 2f69 6d67 2f61 7831 3234  b/main/img/ax124
+00005580: 2e70 6e67 2220 7769 6474 683d 2231 3030  .png" width="100
+00005590: 3078 3130 3030 223e 0a0a 5468 6520 6f62  0x1000">..The ob
+000055a0: 6a65 6374 2067 656e 6572 6174 6564 2062  ject generated b
+000055b0: 7920 6172 7261 6e67 696e 6720 6d75 6c74  y arranging mult
+000055c0: 6970 6c65 2042 7269 636b 206f 626a 6563  iple Brick objec
+000055d0: 7420 2842 7269 636b 7320 636c 6173 7320  t (Bricks class 
+000055e0: 6f62 6a65 6374 2920 6361 6e20 616c 736f  object) can also
+000055f0: 2062 6520 6172 7261 6e67 6564 2061 6e64   be arranged and
+00005600: 2073 7461 636b 6564 2077 6974 6820 6f74   stacked with ot
+00005610: 6865 7220 4272 6963 6b20 6f62 6a65 6374  her Brick object
+00005620: 732e 2020 4164 6469 7469 6f6e 616c 6c79  s.  Additionally
+00005630: 2c20 4974 2069 7320 2070 6f73 7369 626c  , It is  possibl
+00005640: 6520 746f 2063 7265 6174 6520 6d6f 7265  e to create more
+00005650: 2063 6f6d 706c 6578 206c 6179 6f75 7473   complex layouts
+00005660: 2062 7920 6e65 7374 696e 6720 7468 6520   by nesting the 
+00005670: 6f70 6572 6174 696f 6e73 2e0a 0a60 6060  operations...```
+00005680: 7079 7468 6f6e 0a61 7831 3234 3335 203d  python.ax12435 =
+00005690: 2061 7831 3234 2f28 6178 337c 6178 3529   ax124/(ax3|ax5)
+000056a0: 0a61 7831 3234 3335 2e73 6176 6566 6967  .ax12435.savefig
+000056b0: 2822 2e2e 2f69 6d67 2f61 7831 3234 3335  ("../img/ax12435
+000056c0: 2e70 6e67 2229 0a60 6060 0a0a 3c69 6d67  .png").```..<img
+000056d0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+000056e0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+000056f0: 656e 742e 636f 6d2f 706f 6e6e 6869 6465  ent.com/ponnhide
+00005700: 2f70 6174 6368 776f 726b 6c69 622f 6d61  /patchworklib/ma
+00005710: 696e 2f69 6d67 2f61 7831 3234 3335 2e70  in/img/ax12435.p
+00005720: 6e67 2220 7769 6474 683d 2231 3030 3078  ng" width="1000x
+00005730: 3130 3030 223e 0a0a 596f 7520 6361 6e20  1000">..You can 
+00005740: 7175 6963 6b6c 7920 7465 7374 2061 6e6f  quickly test ano
+00005750: 7468 6572 206c 6179 6f75 7420 6279 2072  ther layout by r
+00005760: 6561 7272 616e 6769 6e67 2074 6865 6d2e  earranging them.
+00005770: 0a0a 6060 6070 7974 686f 6e0a 6178 3335  ..```python.ax35
+00005780: 3231 3420 3d20 2861 7833 2f28 6178 327c  214 = (ax3/(ax2|
+00005790: 6178 3129 297c 2861 7835 2f61 7834 290a  ax1))|(ax5/ax4).
+000057a0: 6178 3335 3231 342e 7361 7665 6669 6728  ax35214.savefig(
+000057b0: 290a 6060 600a 0a3c 696d 6720 7372 633d  ).```..<img src=
+000057c0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+000057d0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000057e0: 6f6d 2f70 6f6e 6e68 6964 652f 7061 7463  om/ponnhide/patc
+000057f0: 6877 6f72 6b6c 6962 2f6d 6169 6e2f 696d  hworklib/main/im
+00005800: 672f 6178 3335 3231 342e 706e 6722 2077  g/ax35214.png" w
+00005810: 6964 7468 3d22 3130 3030 7831 3030 3022  idth="1000x1000"
+00005820: 3e0a 0a49 6620 796f 7520 7761 6e74 2074  >..If you want t
+00005830: 6f20 6164 6a75 7374 2074 6865 206d 6172  o adjust the mar
+00005840: 6769 6e73 2062 6574 7765 656e 206f 626a  gins between obj
+00005850: 6563 7473 2c20 706c 6561 7365 2063 6861  ects, please cha
+00005860: 6e67 6520 7468 6520 7661 6c75 6520 6f66  nge the value of
+00005870: 2060 2e70 6172 616d 5b22 6d61 7267 696e   `.param["margin
+00005880: 225d 602e 0a0a 6060 6070 7974 686f 6e0a  "]`...```python.
+00005890: 7077 2e70 6172 616d 5b22 6d61 7267 696e  pw.param["margin
+000058a0: 225d 3d30 2e32 2023 4465 6661 756c 7420  "]=0.2 #Default 
+000058b0: 7661 6c75 6520 6973 2030 2e35 2e0a 6178  value is 0.5..ax
+000058c0: 3335 3231 3420 3d20 2861 7833 2f28 6178  35214 = (ax3/(ax
+000058d0: 327c 6178 3129 297c 2861 7835 2f61 7834  2|ax1))|(ax5/ax4
+000058e0: 290a 6178 3335 3231 342e 7361 7665 6669  ).ax35214.savefi
+000058f0: 6728 222e 2e2f 696d 672f 6178 3335 3231  g("../img/ax3521
+00005900: 345f 7631 2e31 2e70 6e67 2229 0a60 6060  4_v1.1.png").```
+00005910: 0a0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
+00005920: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00005930: 6572 636f 6e74 656e 742e 636f 6d2f 706f  ercontent.com/po
+00005940: 6e6e 6869 6465 2f70 6174 6368 776f 726b  nnhide/patchwork
+00005950: 6c69 622f 6d61 696e 2f69 6d67 2f61 7833  lib/main/img/ax3
+00005960: 3532 3134 5f76 312e 312e 706e 6722 2077  5214_v1.1.png" w
+00005970: 6964 7468 3d22 3130 3030 7831 3030 3022  idth="1000x1000"
+00005980: 3e0a 0a41 6c73 6f2c 2074 6865 2061 7370  >..Also, the asp
+00005990: 6563 7420 7261 7469 6f73 206f 6620 6561  ect ratios of ea
+000059a0: 6368 2070 6c6f 7420 6361 6e20 6265 2066  ch plot can be f
+000059b0: 7265 656c 7920 6d6f 6469 6669 6162 6c65  reely modifiable
+000059c0: 2e0a 0a60 6060 7079 7468 6f6e 0a70 772e  ...```python.pw.
+000059d0: 7061 7261 6d5b 226d 6172 6769 6e22 5d3d  param["margin"]=
+000059e0: 302e 350a 6178 312e 6368 616e 6765 5f61  0.5.ax1.change_a
+000059f0: 7370 6563 7472 6174 696f 2828 342c 3229  spectratio((4,2)
+00005a00: 290a 6178 332e 6368 616e 6765 5f61 7370  ).ax3.change_asp
+00005a10: 6563 7472 6174 696f 2828 342c 3129 290a  ectratio((4,1)).
+00005a20: 6178 342e 6368 616e 6765 5f61 7370 6563  ax4.change_aspec
+00005a30: 7472 6174 696f 2828 352c 3229 290a 6178  tratio((5,2)).ax
+00005a40: 3335 3231 345f 7632 203d 2028 6178 332f  35214_v2 = (ax3/
+00005a50: 2861 7832 7c61 7831 2929 7c28 6178 352f  (ax2|ax1))|(ax5/
+00005a60: 6178 3429 0a61 7833 3532 3134 5f76 322e  ax4).ax35214_v2.
+00005a70: 7361 7665 6669 6728 290a 6060 600a 0a3c  savefig().```..<
+00005a80: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00005a90: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00005aa0: 6f6e 7465 6e74 2e63 6f6d 2f70 6f6e 6e68  ontent.com/ponnh
+00005ab0: 6964 652f 7061 7463 6877 6f72 6b6c 6962  ide/patchworklib
+00005ac0: 2f6d 6169 6e2f 696d 672f 6178 3335 3231  /main/img/ax3521
+00005ad0: 345f 7632 2e70 6e67 2220 7769 6474 683d  4_v2.png" width=
+00005ae0: 2231 3430 3078 3134 3030 223e 0a0a 2323  "1400x1400">..##
+00005af0: 2323 2034 2e20 5061 636b 696e 6720 706c  ## 4. Packing pl
+00005b00: 6f74 7320 7769 7468 206c 6162 656c 2069  ots with label i
+00005b10: 6e64 6578 696e 6720 2841 6476 616e 6365  ndexing (Advance
+00005b20: 6420 6d65 7468 6f64 290a 0a42 7920 7370  d method)..By sp
+00005b30: 6563 6966 7969 6e67 2074 6865 2042 7269  ecifying the Bri
+00005b40: 636b 206f 626a 6563 7473 2069 6e20 6120  ck objects in a 
+00005b50: 4272 6963 6b73 206f 626a 6563 7420 7769  Bricks object wi
+00005b60: 7468 2074 6865 6972 206c 6162 656c 206e  th their label n
+00005b70: 616d 652c 2079 6f75 2063 616e 2061 646a  ame, you can adj
+00005b80: 7573 7420 7468 6520 706f 7369 7469 6f6e  ust the position
+00005b90: 206f 6620 616e 6f74 6865 7220 4272 6963   of another Bric
+00005ba0: 6b20 6f62 6a65 6374 2074 6f20 6265 2070  k object to be p
+00005bb0: 6163 6b65 642e 200a 0a60 6060 7079 7468  acked. ..```pyth
+00005bc0: 6f6e 0a61 7833 3231 203d 2061 7833 2f28  on.ax321 = ax3/(
+00005bd0: 6178 327c 6178 3129 0a61 7833 3231 2e73  ax2|ax1).ax321.s
+00005be0: 6176 6566 6967 2822 2e2e 2f69 6d67 2f61  avefig("../img/a
+00005bf0: 7833 3231 2e70 6e67 2229 0a60 6060 0a0a  x321.png").```..
+00005c00: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00005c10: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00005c20: 636f 6e74 656e 742e 636f 6d2f 706f 6e6e  content.com/ponn
+00005c30: 6869 6465 2f70 6174 6368 776f 726b 6c69  hide/patchworkli
+00005c40: 622f 6d61 696e 2f69 6d67 2f61 7833 3231  b/main/img/ax321
+00005c50: 2e70 6e67 2220 7769 6474 683d 2236 3030  .png" width="600
+00005c60: 7836 3030 223e 0a0a 6060 6070 7974 686f  x600">..```pytho
+00005c70: 6e0a 6178 3332 3134 203d 2061 7833 3231  n.ax3214 = ax321
+00005c80: 5b22 6178 3122 5d7c 6178 340a 6178 3332  ["ax1"]|ax4.ax32
+00005c90: 3134 2e73 6176 6566 6967 2822 2e2e 2f69  14.savefig("../i
+00005ca0: 6d67 2f61 7833 3231 342e 706e 6722 290a  mg/ax3214.png").
+00005cb0: 6060 600a 0a3c 696d 6720 7372 633d 2268  ```..<img src="h
+00005cc0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00005cd0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00005ce0: 2f70 6f6e 6e68 6964 652f 7061 7463 6877  /ponnhide/patchw
+00005cf0: 6f72 6b6c 6962 2f6d 6169 6e2f 696d 672f  orklib/main/img/
+00005d00: 6178 3332 3134 2e70 6e67 2220 7769 6474  ax3214.png" widt
+00005d10: 683d 2231 3030 3078 3130 3030 223e 0a0a  h="1000x1000">..
+00005d20: 6060 6070 7974 686f 6e0a 6178 3335 3231  ```python.ax3521
+00005d30: 345f 7633 203d 2061 7833 3231 345b 2261  4_v3 = ax3214["a
+00005d40: 7833 225d 7c61 7835 0a61 7833 3532 3134  x3"]|ax5.ax35214
+00005d50: 5f76 332e 7361 7665 6669 6728 222e 2e2f  _v3.savefig("../
+00005d60: 696d 672f 6178 3335 3231 345f 7633 2e70  img/ax35214_v3.p
+00005d70: 6e67 2229 0a60 6060 0a0a 3c69 6d67 2073  ng").```..<img s
+00005d80: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00005d90: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00005da0: 742e 636f 6d2f 706f 6e6e 6869 6465 2f70  t.com/ponnhide/p
+00005db0: 6174 6368 776f 726b 6c69 622f 6d61 696e  atchworklib/main
+00005dc0: 2f69 6d67 2f61 7833 3532 3134 5f76 332e  /img/ax35214_v3.
+00005dd0: 706e 6722 2077 6964 7468 3d22 3130 3030  png" width="1000
+00005de0: 7831 3030 3022 3e13 130a 0a54 6865 2061  x1000">....The a
+00005df0: 626f 7665 2070 6163 6b69 6e67 2070 726f  bove packing pro
+00005e00: 6365 7373 2061 6c6c 6f77 7320 7468 6520  cess allows the 
+00005e10: 6178 6573 206f 6620 7468 6520 6f62 6a65  axes of the obje
+00005e20: 6374 7320 746f 2062 6520 6163 6375 7261  cts to be accura
+00005e30: 7465 6c79 2061 6c69 676e 6564 2077 6974  tely aligned wit
+00005e40: 6820 6561 6368 206f 7468 6572 2e20 4163  h each other. Ac
+00005e50: 7475 616c 6c79 2c20 696e 2022 6178 3335  tually, in "ax35
+00005e60: 3231 3422 2061 6e64 2022 6178 3335 3231  214" and "ax3521
+00005e70: 345f 7632 222c 2074 6865 2062 6f74 746f  4_v2", the botto
+00005e80: 6d20 6178 6973 206c 696e 6573 206f 6620  m axis lines of 
+00005e90: 6178 3320 616e 6420 6178 3520 6172 6520  ax3 and ax5 are 
+00005ea0: 6e6f 7420 7072 6563 6973 656c 7920 616c  not precisely al
+00005eb0: 6967 6e65 642c 2077 6869 6c65 2069 6e20  igned, while in 
+00005ec0: 2261 7833 3532 3134 5f76 3322 2c20 7468  "ax35214_v3", th
+00005ed0: 6569 7220 626f 7474 6f6d 2061 7869 7320  eir bottom axis 
+00005ee0: 6c69 6e65 7320 6172 6520 6578 6163 746c  lines are exactl
+00005ef0: 7920 616c 6967 6e65 642e 2048 6f77 6576  y aligned. Howev
+00005f00: 6572 2c20 706c 6561 7365 206e 6f74 6520  er, please note 
+00005f10: 7468 6174 2074 6869 7320 7061 636b 696e  that this packin
+00005f20: 6720 6d65 7468 6f64 2075 7369 6e67 206c  g method using l
+00005f30: 6162 656c 2069 6e64 6578 696e 6720 6368  abel indexing ch
+00005f40: 616e 6765 7320 6173 7065 6374 2072 6174  anges aspect rat
+00005f50: 696f 7320 6f66 2074 6865 2042 7269 636b  ios of the Brick
+00005f60: 206f 626a 6563 7473 2074 6f20 6265 2070   objects to be p
+00005f70: 6163 6b65 6420 6672 6f6d 2074 6865 206f  acked from the o
+00005f80: 7269 6769 6e61 6c20 6f6e 6520 746f 2061  riginal one to a
+00005f90: 6c69 676e 2074 6865 6972 2061 7869 7320  lign their axis 
+00005fa0: 6c69 6e65 7320 7769 7468 206f 7468 6572  lines with other
+00005fb0: 732e 0a0a 3c69 6d67 2073 7263 3d22 6874  s...<img src="ht
+00005fc0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00005fd0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00005fe0: 706f 6e6e 6869 6465 2f70 6174 6368 776f  ponnhide/patchwo
+00005ff0: 726b 6c69 622f 6d61 696e 2f69 6d67 2f61  rklib/main/img/a
+00006000: 7833 3532 3134 5f77 6c2e 706e 6722 2077  x35214_wl.png" w
+00006010: 6964 7468 3d22 3630 3078 3630 3022 3e0a  idth="600x600">.
+00006020: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+00006030: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00006040: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6f6e  rcontent.com/pon
+00006050: 6e68 6964 652f 7061 7463 6877 6f72 6b6c  nhide/patchworkl
+00006060: 6962 2f6d 6169 6e2f 696d 672f 6178 3335  ib/main/img/ax35
+00006070: 3231 345f 7632 5f77 6c2e 706e 6722 2077  214_v2_wl.png" w
+00006080: 6964 7468 3d22 3630 3078 3630 3022 3e0a  idth="600x600">.
+00006090: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+000060a0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000060b0: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6f6e  rcontent.com/pon
+000060c0: 6e68 6964 652f 7061 7463 6877 6f72 6b6c  nhide/patchworkl
+000060d0: 6962 2f6d 6169 6e2f 696d 672f 6178 3335  ib/main/img/ax35
+000060e0: 3231 345f 7633 5f77 6c2e 706e 6722 2077  214_v3_wl.png" w
+000060f0: 6964 7468 3d22 3630 3078 3630 3022 3e0a  idth="600x600">.
+00006100: 0a3c 2f64 6574 6169 6c73 3e0a            .</details>.
```

