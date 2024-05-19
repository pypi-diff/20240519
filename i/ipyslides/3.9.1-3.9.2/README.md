# Comparing `tmp/ipyslides-3.9.1.tar.gz` & `tmp/ipyslides-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.9.1.tar", last modified: Sun May 19 01:55:50 2024, max compression
+gzip compressed data, was "ipyslides-3.9.2.tar", last modified: Sun May 19 17:47:16 2024, max compression
```

## Comparing `ipyslides-3.9.1.tar` & `ipyslides-3.9.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.591514 ipyslides-3.9.1/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.1/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-19 01:55:50.590304 ipyslides-3.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.515630 ipyslides-3.9.1/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.1/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-19 01:55:02.000000 ipyslides-3.9.1/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.583974 ipyslides-3.9.1/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.1/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    40933 2024-05-19 01:14:46.000000 ipyslides-3.9.1/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.1/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.9.1/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.1/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.1/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.1/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    11666 2024-05-18 21:58:12.000000 ipyslides-3.9.1/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.585307 ipyslides-3.9.1/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.1/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.9.1/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.1/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.9.1/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    11757 2024-05-19 01:44:52.000000 ipyslides-3.9.1/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.1/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.1/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.9.1/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    16152 2024-05-19 01:36:13.000000 ipyslides-3.9.1/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.9.1/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    47862 2024-05-18 22:39:14.000000 ipyslides-3.9.1/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.1/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.1/ipyslides/source.py
--rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.9.1/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.1/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.1/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-19 01:55:50.559037 ipyslides-3.9.1/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-19 01:55:49.000000 ipyslides-3.9.1/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-19 01:55:50.000000 ipyslides-3.9.1/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 01:55:49.000000 ipyslides-3.9.1/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-19 01:55:49.000000 ipyslides-3.9.1/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-19 01:55:49.000000 ipyslides-3.9.1/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 01:55:50.591876 ipyslides-3.9.1/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:47:16.379970 ipyslides-3.9.2/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.2/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-19 17:47:16.377225 ipyslides-3.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 17:47:16.260561 ipyslides-3.9.2/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.2/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-19 17:46:35.000000 ipyslides-3.9.2/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:47:16.367663 ipyslides-3.9.2/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.2/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    41105 2024-05-19 04:28:44.000000 ipyslides-3.9.2/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.2/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.9.2/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.2/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.2/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.2/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    11793 2024-05-19 17:44:37.000000 ipyslides-3.9.2/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:47:16.374216 ipyslides-3.9.2/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.2/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.9.2/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.2/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.9.2/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11908 2024-05-19 16:37:54.000000 ipyslides-3.9.2/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.2/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.2/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.2/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16285 2024-05-19 17:25:46.000000 ipyslides-3.9.2/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.9.2/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47862 2024-05-18 22:39:14.000000 ipyslides-3.9.2/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.2/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.2/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29507 2024-05-19 04:17:26.000000 ipyslides-3.9.2/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.2/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.2/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:47:16.324445 ipyslides-3.9.2/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-19 17:47:15.000000 ipyslides-3.9.2/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-19 17:47:15.000000 ipyslides-3.9.2/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:47:15.000000 ipyslides-3.9.2/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-19 17:47:15.000000 ipyslides-3.9.2/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 17:47:15.000000 ipyslides-3.9.2/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:47:16.380565 ipyslides-3.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.2/setup.py
```

### Comparing `ipyslides-3.9.1/LICENSE` & `ipyslides-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/PKG-INFO` & `ipyslides-3.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.1
+Version: 3.9.2
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.1/README.md` & `ipyslides-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/_layout_css.py` & `ipyslides-3.9.2/ipyslides/_base/_layout_css.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,19 @@
                     "z-index": "9 !important",
                     "width": "36px !important",
                     "^:active, ^.mod-active": {"box-shadow": "none !important","opacity": "1 !important",},
                 },
             },
             ".CropBox": {
                 "z-index": "15 !important", # above others
-                ".CropHtml img": {"border": "1px dashed red;"}
+                ".CropHtml img": {
+                    "border": "1px dashed red",
+                    "padding": "0 !important",
+                    "margin-bottom": "0 !important",
+                    "box-sizing":"border-box"},
             },
             ".Draw-Widget": {
                 "backdrop-filter": "blur(50px)",
                 "margin": 0,
                 "z-index": 6,
                 "overflow": "hidden !important",
                 "transition": "height 200ms",
```

### Comparing `ipyslides-3.9.1/ipyslides/_base/_widgets.py` & `ipyslides-3.9.2/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/base.py` & `ipyslides-3.9.2/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/export_html.py` & `ipyslides-3.9.2/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/export_template.py` & `ipyslides-3.9.2/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/icons.py` & `ipyslides-3.9.2/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/intro.py` & `ipyslides-3.9.2/ipyslides/_base/intro.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,22 +141,24 @@
 | {_key('V')}                                 | {_icons["win-maximize"]}, {_icons["win-restore"]} | {key_maps["V"]}        |
 | {_key('G')}                                 | {_icons["settings"]}, {_icons["close"]}           | {key_maps["G"]}        |
 | {_key('E')}                                 | {_icons["code"]}                                  | {key_maps["E"]}        |
 | {_key('L')}                                 | {_icons["laser"]}, {_icons["circle"]}             | {key_maps["L"]}        |
 | {_key('K')}                                 |                                                   | {key_maps["K"]}        |
 """ 
 
-how_to_print = """
-- Capture screenshot of current state of slide by camera button in toolbar or by pressing `S` key. 
-    This will collect screenshots of current slide in order of capturing. 
-- Press `Capture Screenshots of all Slides` button in side panel to capture a single image of each slide. 
-    - Add images over it by manually capturing multiple states of a slide as shown in previous step.
-    - Delete screenshots with dropdown in settings panel.
-    - Set crop bounding box if not in fullscreen mode.
-- Press `Save as PDF File` button to save all screenshots as PDF.
+how_to_print = f"""
+Screenshot of current state of slide can be taken by camera button in toolbar or by pressing {_key('S')}. 
+Order of screenshots is preserved. To capture all slides screenshots, follow process as below.
+
+- Press alert`Capture Screenshots of all Slides` button in side panel to capture a single image of each slide. 
+    - Add images over it by manually capturing multiple states of a slide as shown above.
+    - Delete screenshots with dropdown (all or current slide only and can retake).
+- After all screenshots are ready:
+    - Press alert`Set Crop Bounding Box` to crop an image which applies to all.
+    - Press alert`Save as PDF File` button to save all cropped screenshots as PDF.
 
 ::: note-warning
     Avoid scrolling during taking screenshot. You will set same bounding box for all screenshots
     which can change position if scrolled.
 
 ::: note-tip
     You can also get PDF from exported HTML file, but can't have the freedom of capturing
```

### Comparing `ipyslides-3.9.1/ipyslides/_base/js/interaction.js` & `ipyslides-3.9.2/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/js/notes.js` & `ipyslides-3.9.2/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/navigation.py` & `ipyslides-3.9.2/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/notes.py` & `ipyslides-3.9.2/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/screenshot.py` & `ipyslides-3.9.2/ipyslides/_base/screenshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,29 +43,32 @@
             self.widgets.sliders.crop_w.value = (0, im.width)
             self.widgets.sliders.crop_h.max = im.height
             self.widgets.sliders.crop_h.value = (0, im.height)
 
     def _toggle_crop_window(self, btn):
         if self.widgets.cropbox.layout.height == '0':
             with suppress(BaseException): # not all of systems support screenshot
-                self._cimage = ImageGrab.grab() # full screen image
+                if self.__images:
+                    self._cimage = self.images[0] # sorted first image
+                else:
+                    self._cimage = ImageGrab.grab() # full screen image
                 self._crop_image(None) # do before opening panel for smooth experience
             
             self.widgets.cropbox.layout.height = '100%'
             self.btn_crop.description = 'Close'
         else:
             self.widgets.cropbox.layout.height = '0'
             self.btn_crop.description = 'Set Crop Bounding Box'
 
     def _crop_image(self, change):
         if self._cimage is not None:
             x1,x2 = self.widgets.sliders.crop_w.value
             y2,y1 = [self.widgets.sliders.crop_h.max - v for v in self.widgets.sliders.crop_h.value]
             self._crop_bbox = [x1,y1,x2,y2]
-            self.widgets.htmls.crop.value = image(self._cimage.crop([x1,y1,x2,y2]), width='100%').value
+            self.widgets.htmls.crop.value = image(self._cimage.crop([x1,y1,x2,y2]), as_figure=False, width='100%').value
 
     @contextmanager
     def capture_mode(self, *additional_widgets_to_hide):
         """Hide some widgets and while capturing a screenshot, show them back again.
         You can provide additional widgets to hide while capturing as well."""
         hide_widgets = [self.widgets.controls, # now other buttons are inside Menu-Box which gets hidden 
                         self.widgets.htmls.toast,
```

### Comparing `ipyslides-3.9.1/ipyslides/_base/settings.py` & `ipyslides-3.9.2/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/slide.py` & `ipyslides-3.9.2/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/styles.py` & `ipyslides-3.9.2/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/_base/widgets.py` & `ipyslides-3.9.2/ipyslides/_base/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # patching for correct order of outputs, loaded with ipywidgets import when ipyslides is present
 ipw.interaction.Output = Output
 ipw.Output = Output
 ipw.widget_output.Output = Output
 
 auto_layout =  Layout(width='auto')
 def describe(value,**kwargs): 
-    return {'description': value, 'description_width': 'initial','layout':Layout(width='auto',**kwargs)}
+    return {'description': value, 'description_width': 'initial','layout':Layout(**{'width':'auto',**kwargs})} # let change width too
 
 
 @dataclass(frozen=True)
 class _Buttons:
     """
     Instantiate under `Widgets` class only.
     """
@@ -92,15 +92,15 @@
     loading = HTML(layout=Layout(display='none')).add_class('Loading') #SVG Animation in it
     logo    = HtmlWidget('').add_class('LogoHtml')
     toast   = HtmlWidget('').add_class('Toast') # For notifications
     cursor  = HtmlWidget('').add_class('LaserPointer') # For beautiful cursor
     hilite  = HTML() # Updated in settings on creation. For code blocks.
     zoom    = HTML() # zoom CSS, do not add here!
     glass   = HTML().add_class('BackLayer') # For glass effect
-    crop    = HTML('Screenshot appears here for cropping!', layout=Layout(margin='0',padding='0',height='100',overflow='auto')).add_class('CropHtml')
+    crop    = HtmlWidget('Screenshot appears here for cropping!', layout=Layout(margin='0',padding='0',height='100',overflow='auto')).add_class('CropHtml')
 
 @dataclass(frozen=True)
 class _Checks:
     """
     Instantiate under `Widgets` class only.
     """
     reflow  = ipw.Checkbox(value=False,description='Reflow Content',layout=auto_layout)
@@ -114,16 +114,16 @@
 class _Sliders:
     """
     Instantiate under `Widgets` class only.
     """
     progress = ipw.SelectionSlider(options=[('0',0)], value=0, continuous_update=False,readout=True)
     width    = ipw.IntSlider(**describe('Width (vw)'),min=20,max=100, value = 60,continuous_update=False).add_class('Width-Slider') 
     fontsize = ipw.IntSlider(**describe('Font Size'),min=8,max=64,step=1, value = 20,continuous_update=False, tooltip="If you need more larger/smaller font size, use `Slides.settings.set_font_size`")
-    crop_w   = ipw.IntRangeSlider(**describe('w', margin='8px'), min=0,max=100,value=[20,80],step=1, continuous_update=False, readout=False) # step for upto 4k screen by default
-    crop_h   = ipw.IntRangeSlider(**describe('h',height='calc(100% - 16px)',margin='8px'), min=0,max=100,value=[25,75],step=1, continuous_update=False, readout=False,orientation='vertical')
+    crop_w   = ipw.IntRangeSlider(**describe('w', margin='8px 32px 8px -16px'), min=0,max=100,value=[20,80],step=1, continuous_update=False, readout=False) # step for upto 4k screen by default
+    crop_h   = ipw.IntRangeSlider(**describe('h',width='36px', height='calc(100% - 32px)',margin='16px'), min=0,max=100,value=[25,75],step=1, continuous_update=False, readout=False,orientation='vertical')
 
 @dataclass(frozen=True)
 class _Dropdowns:
     """
     Instantiate under `Widgets` class only.
     """
     theme  = ipw.Dropdown(**describe('Theme'),options=[*styles.theme_colors.keys(),'Custom'],value='Inherit')
@@ -195,20 +195,19 @@
                 self.sliders.width,
                 self.ddowns.theme,
                 HTML('<b>Additional Features</b>',layout = _html_layout),
                 self.checks.notes,self.checks.toast,self.checks.reflow,
                 self.checks.proxy,self.checks.navgui,self.checks.focus,
                 HTML('<b>HTML File Export</b>',layout = _html_layout),
                 self.buttons.export,
-                HTML('<b>Screenshot Export</b>',layout = _html_layout),
-                self.buttons.cap_all,
+                HTML(html('details',[html('summary','<b>Screenshot Export</b>'), how_to_print]).value,layout = _html_layout),
                 self.ddowns.clear,
+                self.buttons.cap_all,
                 self.buttons.crop,
                 self.buttons.pdf,
-                HTML(html('details',[html('summary','How to Screenshot'), how_to_print]).value),
                 self._tmp_out,
                 self.notes, # Just to be there for acting on a popup window
             ],layout=Layout(width='auto',height='max-content',overflow_y='scroll',padding='12px',margin='0')),
         ],layout = Layout(width='70%',min_width='50%',height='0',overflow='hidden')).add_class('SidePanel') 
         
         self.tocbox = VBox([],layout = Layout(width='30%',min_width='400px',height='0',overflow='auto')).add_class('TOC')
         
@@ -225,23 +224,23 @@
             if hasattr(btn, 'on_click'):
                 btn.on_click(close_quick_menu)
             else:
                 btn.observe(close_quick_menu, names=["value"])
         
         self.cropbox = GridBox([
             self.sliders.crop_w,
-            HBox([self.sliders.crop_h, self.htmls.crop]),
-            HBox([self.buttons.pdf, self.buttons.crop], layout = Layout(justify_content='flex-end')),
+            HBox([self.sliders.crop_h, self.htmls.crop], layout = Layout(overflow='hidden',padding='0 16px 0 0',margin='0')),
+            HBox([self.buttons.pdf, self.buttons.crop], layout = Layout(justify_content='flex-end',padding='8px', border_top='1px solid #8988')),
             ], layout = Layout(
                 margin='0',
                 padding='0', 
                 width='100%', 
                 height='0',
-                grid_gap = '8px',
-                grid_template_rows='40px auto 40px',
+                grid_gap = '4px',
+                grid_template_rows='36px auto 36px',
             )).add_class("CropBox")
         
         self.mainbox = VBox([
             self.htmls.glass, # This is the glass pane, should be before everything, otherwise it will cover the slide area
             self.htmls.loading, 
             self.htmls.toast,
             self.htmls.main,
```

### Comparing `ipyslides-3.9.1/ipyslides/_demo.py` & `ipyslides-3.9.2/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/core.py` & `ipyslides-3.9.2/ipyslides/core.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/formatters.py` & `ipyslides-3.9.2/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/source.py` & `ipyslides-3.9.2/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/utils.py` & `ipyslides-3.9.2/ipyslides/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from IPython import get_ipython
 from IPython.display import SVG, IFrame
 from IPython.core.display import Image, display
 import ipywidgets as ipw
 
 from .formatters import XTML, fix_ipy_image, htmlize
-from .xmd import get_unique_css_class, error, raw, capture_content # raw error for export from here
+from .xmd import get_unique_css_class, capture_content # raw error for export from here
 from .writer import Writer, AltForWidget
 
 def is_jupyter_session():
      "Return True if code is executed inside jupyter session even while being imported."
      shell = get_ipython()
      if shell.__class__.__name__ in ("ZMQInteractiveShell","Shell"):
          return True # Verify Jupyter and Colab
@@ -336,40 +336,54 @@
         im_bytes = BytesIO()
         data.save(im_bytes,data.format if data.format else 'PNG',quality=95) #Save image to BytesIO in format of given image
         return im_bytes.getvalue()
     return data # if not return back data
 
 _fig_style_inline = "margin-block:0.5em;margin-inline:0.5em" # its 40px by defualt, ruins space, not working in CSS outside
 
-def image(data=None,width='95%',caption=None, **kwargs):
+def image(data=None,width='95%',caption=None, as_figure = True, **kwargs):
     """Displays PNG/JPEG files or image data etc, `kwrags` are passed to IPython.display.Image. 
     You can provide following to `data` parameter:
         
     - An opened PIL image. Useful for image operations and then direct writing to slides. 
     - A file path to image file.
     - A url to image file.
     - A str/bytes object containing image data.  
     - A str like "clip:image.png" will load an image saved using `Slides.clipboard_image('image.png')`. 
+
+    If `as_figure = False` caption is not used.
     """
     if isinstance(width,int):
         width = f'{width}px'
     
     if isinstance(data, str) and data.startswith("clip:"):
         data = get_child_dir(".ipyslides-assets", "clips", create = True) / data[5:] # strip clip by index, don't strip other characters
         if not data.exists():
             raise FileNotFoundError(f"File: {data!r} does not exist!")
     
     _data = _check_pil_image(data) #Check if data is a PIL Image or return data
     img = fix_ipy_image(Image(data = _data,**kwargs),width=width) # gievs XTML object
+
+    if not as_figure:
+        return img
+    
     cap = f'<figcaption class="no-zoom">{caption}</figcaption>' if caption else ''
     return html('figure', img.value + cap, className='zoom-child', style = _fig_style_inline)  
 
-def svg(data=None,width = '95%',caption=None,**kwargs):
-    "Display svg file or svg string/bytes with additional customizations. `kwrags` are passed to IPython.display.SVG. You can provide url/string/bytes/filepath for svg."
+def svg(data=None,width = '95%',caption=None, as_figure=True, **kwargs):
+    """Display svg file or svg string/bytes with additional customizations. 
+    `kwrags` are passed to IPython.display.SVG. You can provide url/string/bytes/filepath for svg.
+    
+    If `as_figure = False` caption is not used.
+    """
     svg = SVG(data=data, **kwargs)._repr_svg_()
+    
+    if not as_figure:
+        return XTML(svg)
+    
     cap = f'<figcaption class="no-zoom">{caption}</figcaption>' if caption else ''
     style = f'width:{width}px;' if isinstance(width,int) else f'width:{width};' + _fig_style_inline
     return html('figure', svg + cap, className='zoom-child', style=style) 
 
 
 def iframe(src, width='100%',height='auto',**kwargs):
     "Display `src` in an iframe. `kwrags` are passed to IPython.display.IFrame"
```

### Comparing `ipyslides-3.9.1/ipyslides/writer.py` & `ipyslides-3.9.2/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides/xmd.py` & `ipyslides-3.9.2/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.9.2/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.1
+Version: 3.9.2
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.1/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.9.2/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.1/setup.py` & `ipyslides-3.9.2/setup.py`

 * *Files identical despite different names*

