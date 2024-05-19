# Comparing `tmp/ipyslides-3.9.0.tar.gz` & `tmp/ipyslides-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.9.0.tar", last modified: Sat May 18 23:19:04 2024, max compression
+gzip compressed data, was "ipyslides-3.9.1.tar", last modified: Sun May 19 01:55:50 2024, max compression
```

## Comparing `ipyslides-3.9.0.tar` & `ipyslides-3.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.392292 ipyslides-3.9.0/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.0/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-18 23:19:04.390292 ipyslides-3.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.348810 ipyslides-3.9.0/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.0/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-18 23:18:27.000000 ipyslides-3.9.0/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.387218 ipyslides-3.9.0/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.0/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    40837 2024-05-18 22:21:10.000000 ipyslides-3.9.0/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.0/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.9.0/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.0/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.0/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.0/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    11666 2024-05-18 21:58:12.000000 ipyslides-3.9.0/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.389280 ipyslides-3.9.0/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.0/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.9.0/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.0/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.9.0/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    11991 2024-05-18 22:39:08.000000 ipyslides-3.9.0/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.0/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.0/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.9.0/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    16113 2024-05-18 22:07:00.000000 ipyslides-3.9.0/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.9.0/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    47862 2024-05-18 22:39:14.000000 ipyslides-3.9.0/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.0/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.0/ipyslides/source.py
--rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.9.0/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.0/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.0/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.373140 ipyslides-3.9.0/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 23:19:04.392292 ipyslides-3.9.0/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.591514 ipyslides-3.9.1/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.1/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-19 01:55:50.590304 ipyslides-3.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.515630 ipyslides-3.9.1/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.1/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-19 01:55:02.000000 ipyslides-3.9.1/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.583974 ipyslides-3.9.1/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.1/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    40933 2024-05-19 01:14:46.000000 ipyslides-3.9.1/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.1/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.9.1/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.1/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.1/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.1/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    11666 2024-05-18 21:58:12.000000 ipyslides-3.9.1/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.585307 ipyslides-3.9.1/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.1/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.9.1/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.1/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.9.1/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11757 2024-05-19 01:44:52.000000 ipyslides-3.9.1/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.1/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.1/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.9.1/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16152 2024-05-19 01:36:13.000000 ipyslides-3.9.1/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.9.1/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47862 2024-05-18 22:39:14.000000 ipyslides-3.9.1/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.1/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.1/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.9.1/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.1/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.1/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.559037 ipyslides-3.9.1/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-19 01:55:49.000000 ipyslides-3.9.1/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-19 01:55:50.000000 ipyslides-3.9.1/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 01:55:49.000000 ipyslides-3.9.1/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-19 01:55:49.000000 ipyslides-3.9.1/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 01:55:49.000000 ipyslides-3.9.1/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 01:55:50.591876 ipyslides-3.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.1/setup.py
```

### Comparing `ipyslides-3.9.0/LICENSE` & `ipyslides-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/PKG-INFO` & `ipyslides-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.0
+Version: 3.9.1
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.0/README.md` & `ipyslides-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/_layout_css.py` & `ipyslides-3.9.1/ipyslides/_base/_layout_css.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,18 @@
                     "left": 0,
                     "top":0,
                     "z-index": "9 !important",
                     "width": "36px !important",
                     "^:active, ^.mod-active": {"box-shadow": "none !important","opacity": "1 !important",},
                 },
             },
-            ".CropBox": {"z-index": "15 !important",}, # above others
+            ".CropBox": {
+                "z-index": "15 !important", # above others
+                ".CropHtml img": {"border": "1px dashed red;"}
+            },
             ".Draw-Widget": {
                 "backdrop-filter": "blur(50px)",
                 "margin": 0,
                 "z-index": 6,
                 "overflow": "hidden !important",
                 "transition": "height 200ms",
                 "^, > div": {
```

### Comparing `ipyslides-3.9.0/ipyslides/_base/_widgets.py` & `ipyslides-3.9.1/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/base.py` & `ipyslides-3.9.1/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/export_html.py` & `ipyslides-3.9.1/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/export_template.py` & `ipyslides-3.9.1/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/icons.py` & `ipyslides-3.9.1/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/intro.py` & `ipyslides-3.9.1/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/js/interaction.js` & `ipyslides-3.9.1/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/js/notes.js` & `ipyslides-3.9.1/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/navigation.py` & `ipyslides-3.9.1/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/notes.py` & `ipyslides-3.9.1/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/screenshot.py` & `ipyslides-3.9.1/ipyslides/_base/screenshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,36 +42,30 @@
             self.widgets.sliders.crop_w.max = im.width
             self.widgets.sliders.crop_w.value = (0, im.width)
             self.widgets.sliders.crop_h.max = im.height
             self.widgets.sliders.crop_h.value = (0, im.height)
 
     def _toggle_crop_window(self, btn):
         if self.widgets.cropbox.layout.height == '0':
+            with suppress(BaseException): # not all of systems support screenshot
+                self._cimage = ImageGrab.grab() # full screen image
+                self._crop_image(None) # do before opening panel for smooth experience
+            
             self.widgets.cropbox.layout.height = '100%'
             self.btn_crop.description = 'Close'
-            if self.__images:
-                self._load_image(self.images[0]) # load from ordered images
-            else:
-                self.widgets.htmls.crop.value = 'Screenshot appears here for cropping!'
         else:
             self.widgets.cropbox.layout.height = '0'
             self.btn_crop.description = 'Set Crop Bounding Box'
-    
-    def _load_image(self, im):
-        self._cimage = im
-        self.widgets.htmls.crop.value = image(im,width='100%').value
 
     def _crop_image(self, change):
         if self._cimage is not None:
             x1,x2 = self.widgets.sliders.crop_w.value
             y2,y1 = [self.widgets.sliders.crop_h.max - v for v in self.widgets.sliders.crop_h.value]
             self._crop_bbox = [x1,y1,x2,y2]
             self.widgets.htmls.crop.value = image(self._cimage.crop([x1,y1,x2,y2]), width='100%').value
-        elif self.__images:
-            self._load_image(self.images[0]) 
 
     @contextmanager
     def capture_mode(self, *additional_widgets_to_hide):
         """Hide some widgets and while capturing a screenshot, show them back again.
         You can provide additional widgets to hide while capturing as well."""
         hide_widgets = [self.widgets.controls, # now other buttons are inside Menu-Box which gets hidden 
                         self.widgets.htmls.toast,
@@ -119,16 +113,15 @@
     def capture(self,btn):
         "Saves screenshot of current slide into self.__images dictionary when corresponding button clicked. Use in fullscreen mode or set bbox using `.capture_setup`."
         with self.capture_mode():
             sleep(0.05) # Just for above clearance of widgets views
             if self.widgets.sliders.progress.label not in self.__images:
                 self.__images[self.widgets.sliders.progress.label] = [] # container to store images
             
-            self._cimage = ImageGrab.grab(bbox = None) # keep for cropping
-            self.__images[self.widgets.sliders.progress.label].append(self._cimage) # Append to existing list
+            self.__images[self.widgets.sliders.progress.label].append(ImageGrab.grab(bbox = None)) # Append to existing list
     
     def __sort_images(self):
         ims = [] #sorting
         for label, _ in self.widgets.sliders.progress.options:
             if label in self.__images:
                 ims = [*ims,*self.__images[label]]
```

### Comparing `ipyslides-3.9.0/ipyslides/_base/settings.py` & `ipyslides-3.9.1/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/slide.py` & `ipyslides-3.9.1/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/styles.py` & `ipyslides-3.9.1/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/_base/widgets.py` & `ipyslides-3.9.1/ipyslides/_base/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     loading = HTML(layout=Layout(display='none')).add_class('Loading') #SVG Animation in it
     logo    = HtmlWidget('').add_class('LogoHtml')
     toast   = HtmlWidget('').add_class('Toast') # For notifications
     cursor  = HtmlWidget('').add_class('LaserPointer') # For beautiful cursor
     hilite  = HTML() # Updated in settings on creation. For code blocks.
     zoom    = HTML() # zoom CSS, do not add here!
     glass   = HTML().add_class('BackLayer') # For glass effect
-    crop    = HTML('Screenshot appears here for cropping!', layout=Layout(margin='auto',padding='0')).add_class('CropHtml')
+    crop    = HTML('Screenshot appears here for cropping!', layout=Layout(margin='0',padding='0',height='100',overflow='auto')).add_class('CropHtml')
 
 @dataclass(frozen=True)
 class _Checks:
     """
     Instantiate under `Widgets` class only.
     """
     reflow  = ipw.Checkbox(value=False,description='Reflow Content',layout=auto_layout)
@@ -115,15 +115,15 @@
     """
     Instantiate under `Widgets` class only.
     """
     progress = ipw.SelectionSlider(options=[('0',0)], value=0, continuous_update=False,readout=True)
     width    = ipw.IntSlider(**describe('Width (vw)'),min=20,max=100, value = 60,continuous_update=False).add_class('Width-Slider') 
     fontsize = ipw.IntSlider(**describe('Font Size'),min=8,max=64,step=1, value = 20,continuous_update=False, tooltip="If you need more larger/smaller font size, use `Slides.settings.set_font_size`")
     crop_w   = ipw.IntRangeSlider(**describe('w', margin='8px'), min=0,max=100,value=[20,80],step=1, continuous_update=False, readout=False) # step for upto 4k screen by default
-    crop_h   = ipw.IntRangeSlider(**describe('h',height='auto',margin='8px'), min=0,max=100,value=[25,75],step=1, continuous_update=False, readout=False,orientation='vertical')
+    crop_h   = ipw.IntRangeSlider(**describe('h',height='calc(100% - 16px)',margin='8px'), min=0,max=100,value=[25,75],step=1, continuous_update=False, readout=False,orientation='vertical')
 
 @dataclass(frozen=True)
 class _Dropdowns:
     """
     Instantiate under `Widgets` class only.
     """
     theme  = ipw.Dropdown(**describe('Theme'),options=[*styles.theme_colors.keys(),'Custom'],value='Inherit')
```

### Comparing `ipyslides-3.9.0/ipyslides/_demo.py` & `ipyslides-3.9.1/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/core.py` & `ipyslides-3.9.1/ipyslides/core.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/formatters.py` & `ipyslides-3.9.1/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/source.py` & `ipyslides-3.9.1/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/utils.py` & `ipyslides-3.9.1/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/writer.py` & `ipyslides-3.9.1/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides/xmd.py` & `ipyslides-3.9.1/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.9.1/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.0
+Version: 3.9.1
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.0/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.9.1/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.0/setup.py` & `ipyslides-3.9.1/setup.py`

 * *Files identical despite different names*

