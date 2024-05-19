# Comparing `tmp/ipyslides-3.8.9.tar.gz` & `tmp/ipyslides-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.8.9.tar", last modified: Sat May 18 22:11:48 2024, max compression
+gzip compressed data, was "ipyslides-3.9.0.tar", last modified: Sat May 18 23:19:04 2024, max compression
```

## Comparing `ipyslides-3.8.9.tar` & `ipyslides-3.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.285028 ipyslides-3.8.9/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.9/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-18 22:11:48.285028 ipyslides-3.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.160575 ipyslides-3.8.9/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.9/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-18 22:10:59.000000 ipyslides-3.8.9/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.285028 ipyslides-3.8.9/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.9/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    40807 2024-05-18 22:04:23.000000 ipyslides-3.8.9/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.8.9/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.9/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.8.9/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.8.9/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.8.9/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    11666 2024-05-18 21:58:12.000000 ipyslides-3.8.9/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.285028 ipyslides-3.8.9/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12476 2024-05-17 22:26:29.000000 ipyslides-3.8.9/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.9/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.9/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.9/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    11993 2024-05-18 21:24:06.000000 ipyslides-3.8.9/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-14 00:03:47.000000 ipyslides-3.8.9/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.8.9/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.8.9/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    16113 2024-05-18 22:07:00.000000 ipyslides-3.8.9/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.9/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    47862 2024-05-18 17:47:27.000000 ipyslides-3.8.9/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.9/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.9/ipyslides/source.py
--rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.8.9/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.9/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.9/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.236154 ipyslides-3.8.9/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 22:11:48.300662 ipyslides-3.8.9/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.392292 ipyslides-3.9.0/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.0/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-18 23:19:04.390292 ipyslides-3.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.348810 ipyslides-3.9.0/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.0/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-18 23:18:27.000000 ipyslides-3.9.0/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.387218 ipyslides-3.9.0/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.0/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    40837 2024-05-18 22:21:10.000000 ipyslides-3.9.0/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.0/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.9.0/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.0/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.0/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.0/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    11666 2024-05-18 21:58:12.000000 ipyslides-3.9.0/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.389280 ipyslides-3.9.0/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.0/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.9.0/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.0/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.9.0/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11991 2024-05-18 22:39:08.000000 ipyslides-3.9.0/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.0/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.0/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.9.0/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16113 2024-05-18 22:07:00.000000 ipyslides-3.9.0/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.9.0/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47862 2024-05-18 22:39:14.000000 ipyslides-3.9.0/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.0/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.0/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.9.0/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.0/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.0/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:19:04.373140 ipyslides-3.9.0/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 23:19:04.000000 ipyslides-3.9.0/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 23:19:04.392292 ipyslides-3.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.0/setup.py
```

### Comparing `ipyslides-3.8.9/LICENSE` & `ipyslides-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/PKG-INFO` & `ipyslides-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.9
+Version: 3.9.0
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.9/README.md` & `ipyslides-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/_layout_css.py` & `ipyslides-3.9.0/ipyslides/_base/_layout_css.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                         "opacity": "0.5",
                     },
                     "to": {
                         "transform": "translateX(0)",
                         "opacity": "1",
                     },
                 },
-                "^.InView-Title .Arrows.Prev-Btn, ^.InView-Last .Arrows.Next-Btn": {
+                "^.InView-Title .Arrows.Prev-Btn, ^.InView-Last .Arrows.Next-Btn, ^.InView-Title .Slide-Number": {
                     "display": "none !important",
                 },  # still should be clickable
                 "^.InView-Title .Arrows.Next-Btn, ^.InView-Other .Arrows.Next-Btn": {
                     "animation-name": "heart-beat",
                     "animation-duration": "2s",
                     "animation-iteration-count": "10", # 10 times to catch attention of speaker
                     "animation-timing-function": "steps(8, end)",
```

### Comparing `ipyslides-3.8.9/ipyslides/_base/_widgets.py` & `ipyslides-3.9.0/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/base.py` & `ipyslides-3.9.0/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/export_html.py` & `ipyslides-3.9.0/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/export_template.py` & `ipyslides-3.9.0/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/icons.py` & `ipyslides-3.9.0/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/intro.py` & `ipyslides-3.9.0/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/js/interaction.js` & `ipyslides-3.9.0/ipyslides/_base/js/interaction.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -61,18 +61,22 @@
     'g': 'TPAN', // Setting panel
     'k': 'KSC', // keyboard shortcuts
     'l': 'TLSR', // L toggle laser
     'v': 'TVP', // V for toggle viewport, only in voila and LinkedOutputView
     'e': 'EDIT', // Edit source cell
 }
 
-
 function keyboardEvents(box, model) {
     function keyOnSlides(e) {
-        e.preventDefault();
+        e.preventDefault(); // stop default actions
+        e.stopPropagation(); // stop propagation to jupyterlab events and other views 
+        if (e.target !== box) {
+            return true; // inside componets should work properly, avoid going outside
+        };
+
         let key = e.key; // True unicode key
         let message = '';
         if ('123456789'.includes(key)) { // send to shift slides by numbers
             message = (e.ctrlKey ? "SHIFT:-" + key : "SHIFT:" + key);
         } else if (key === 'x' || key === 'd') {
             alert("Pressing X or D,D may cut selected cell! Click outside slides to capture these keys!");
             e.stopPropagation(); // stop propagation to jupyterlab events
@@ -90,16 +94,14 @@
             message = 'NEXT';
         } else if (key === '0') {
             message = (e.ctrlKey ? "HOME" : "END"); // Numbers don't change with control
         } else if (key in keyMessage) {
             message = keyMessage[key];
         }
 
-        e.stopPropagation(); // stop propagation to jupyterlab events and other views 
-        e.preventDefault(); // stop default actions
         model.set("msg_topy", message);
         model.save_changes();
     }
 
     box.onkeydown = keyOnSlides;
 };
```

### Comparing `ipyslides-3.8.9/ipyslides/_base/js/notes.js` & `ipyslides-3.9.0/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/navigation.py` & `ipyslides-3.9.0/ipyslides/_base/navigation.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,22 +47,18 @@
             self.btn_next.icon = 'chevron-right'
     
     def _toggle_panel(self,change):
         if self.btn_settings.icon == 'plus':
             self.btn_settings.icon  = 'minus'
             self.btn_settings.tooltip = "Close Settings [G]"
             self.widgets.panelbox.layout.height = "100%"
-            self.btn_next.disabled = True
-            self.btn_prev.disabled = True
         else:
             self.btn_settings.icon = 'plus' #'ellipsis-v'
             self.btn_settings.tooltip = "Open Settings [G]"
             self.widgets.panelbox.layout.height = "0"
-            self.btn_next.disabled = False
-            self.btn_prev.disabled = False
             
     def _goto_home(self,btn):
         try:
             self.progress_slider.index = 0
             if self.widgets.buttons.toc.icon == 'minus':
                 self.widgets.buttons.toc.click() # Close TOC but only if it was open, let other things work
         except:
```

### Comparing `ipyslides-3.8.9/ipyslides/_base/notes.py` & `ipyslides-3.9.0/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/screenshot.py` & `ipyslides-3.9.0/ipyslides/_base/screenshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,27 +28,27 @@
         self._crop_bbox = None
         self.__capture_settings = {'load_time':0.8,'quality':95}
         self._capturing = False
         
         self.btn_capture.on_click(self.capture)
         self.btn_pdf.on_click(self.__save_pdf)
         self.btn_cap_all.on_click(self.__capture_all)
-        self.btn_crop.on_click(self.__toggle_crop_window)
+        self.btn_crop.on_click(self._toggle_crop_window)
         self.widgets.ddowns.clear.observe(self.__clear_images)
         self.widgets.sliders.crop_w.observe(self._crop_image, names="value")
         self.widgets.sliders.crop_h.observe(self._crop_image, names="value")
 
         with suppress(BaseException): # only on supportive systems silently
             im = ImageGrab.grab()
             self.widgets.sliders.crop_w.max = im.width
             self.widgets.sliders.crop_w.value = (0, im.width)
             self.widgets.sliders.crop_h.max = im.height
             self.widgets.sliders.crop_h.value = (0, im.height)
 
-    def __toggle_crop_window(self, btn):
+    def _toggle_crop_window(self, btn):
         if self.widgets.cropbox.layout.height == '0':
             self.widgets.cropbox.layout.height = '100%'
             self.btn_crop.description = 'Close'
             if self.__images:
                 self._load_image(self.images[0]) # load from ordered images
             else:
                 self.widgets.htmls.crop.value = 'Screenshot appears here for cropping!'
```

### Comparing `ipyslides-3.8.9/ipyslides/_base/settings.py` & `ipyslides-3.9.0/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/slide.py` & `ipyslides-3.9.0/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/styles.py` & `ipyslides-3.9.0/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_base/widgets.py` & `ipyslides-3.9.0/ipyslides/_base/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/_demo.py` & `ipyslides-3.9.0/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/core.py` & `ipyslides-3.9.0/ipyslides/core.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/formatters.py` & `ipyslides-3.9.0/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/source.py` & `ipyslides-3.9.0/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/utils.py` & `ipyslides-3.9.0/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/writer.py` & `ipyslides-3.9.0/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides/xmd.py` & `ipyslides-3.9.0/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.9.0/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.9
+Version: 3.9.0
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.9/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.9.0/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.9/setup.py` & `ipyslides-3.9.0/setup.py`

 * *Files identical despite different names*

