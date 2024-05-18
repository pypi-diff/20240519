# Comparing `tmp/ipyslides-3.8.7.tar.gz` & `tmp/ipyslides-3.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.8.7.tar", last modified: Sun May 12 19:33:56 2024, max compression
+gzip compressed data, was "ipyslides-3.8.8.tar", last modified: Sat May 18 00:40:56 2024, max compression
```

## Comparing `ipyslides-3.8.7.tar` & `ipyslides-3.8.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 19:33:56.754566 ipyslides-3.8.7/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.7/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-12 19:33:56.749287 ipyslides-3.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 19:33:56.673298 ipyslides-3.8.7/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.7/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-12 19:33:18.000000 ipyslides-3.8.7/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 19:33:56.748433 ipyslides-3.8.7/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.7/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    40058 2024-05-12 19:29:33.000000 ipyslides-3.8.7/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6084 2024-05-10 20:38:34.000000 ipyslides-3.8.7/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.7/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.8.7/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.8.7/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.8.7/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    12158 2024-05-10 07:35:58.000000 ipyslides-3.8.7/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-12 19:33:56.749287 ipyslides-3.8.7/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12864 2024-05-10 21:19:34.000000 ipyslides-3.8.7/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.7/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.7/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.7/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.8.7/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-12 19:00:33.000000 ipyslides-3.8.7/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.8.7/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.8.7/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    15382 2024-05-12 18:40:31.000000 ipyslides-3.8.7/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.7/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    48033 2024-05-12 18:00:49.000000 ipyslides-3.8.7/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.7/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.7/ipyslides/source.py
--rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.8.7/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.7/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.7/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-12 19:33:56.717317 ipyslides-3.8.7/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-12 19:33:56.000000 ipyslides-3.8.7/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-12 19:33:56.000000 ipyslides-3.8.7/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 19:33:56.000000 ipyslides-3.8.7/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-12 19:33:56.000000 ipyslides-3.8.7/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 19:33:56.000000 ipyslides-3.8.7/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 19:33:56.755313 ipyslides-3.8.7/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.950660 ipyslides-3.8.8/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.8/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-18 00:40:56.950660 ipyslides-3.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.873007 ipyslides-3.8.8/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.8/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-18 00:39:35.000000 ipyslides-3.8.8/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.947119 ipyslides-3.8.8/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.8/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    40305 2024-05-18 00:25:03.000000 ipyslides-3.8.8/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.8.8/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.8/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.8.8/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.8.8/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.8.8/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    12158 2024-05-10 07:35:58.000000 ipyslides-3.8.8/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.949176 ipyslides-3.8.8/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12476 2024-05-17 22:26:29.000000 ipyslides-3.8.8/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.8/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.8/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.8/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    13446 2024-05-18 00:06:17.000000 ipyslides-3.8.8/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23555 2024-05-14 00:03:47.000000 ipyslides-3.8.8/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.8.8/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.8.8/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    15530 2024-05-18 00:36:33.000000 ipyslides-3.8.8/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.8/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    48149 2024-05-18 00:08:30.000000 ipyslides-3.8.8/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.8/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.8/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.8.8/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.8/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.8/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.919278 ipyslides-3.8.8/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 00:40:56.950660 ipyslides-3.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.8/setup.py
```

### Comparing `ipyslides-3.8.7/LICENSE` & `ipyslides-3.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/PKG-INFO` & `ipyslides-3.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.7
+Version: 3.8.8
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.7/README.md` & `ipyslides-3.8.8/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/_layout_css.py` & `ipyslides-3.8.8/ipyslides/_base/_layout_css.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 
 def layout_css(accent_color, aspect):
     uclass = get_unique_css_class()
     return _build_css(
         (uclass,),
         {
             "a.jp-InternalAnchorLink": {"display": "none !important"},
+            "<.SlidesContainer": {"padding": "2px !important",}, # for box-shadow to appear all sides
             "^.SlidesWrapper": {
-                "container": "slides / inline-size",
+                "container": "slides / inline-size !important",
                 "z-index": "1 !important",
+                "box-shadow": "var(--jp-border-color1,#8988) 0px 0px 1px 0.5px !important", # for screenshot clear boundaries
                 "^.SingleSlide .Controls": {
                     "display": "none !important",
                 },
                 "^:focus": {
                     "outline" : "none !important",
                 },
                 "^.CaptureMode": {
@@ -32,15 +34,15 @@
                 "^.PresentMode .SlideBox .SlideArea .ProxyPasteBtns": {
                     "display": "none !important"
                 },  # Hide in presentation mode
                 "^.FullWindow, ^.FullScreen": {
                     ".Width-Slider, .Source-Btn": {"display": "none !important"},
                 },
                 "^.FullScreen": {
-                    ".FullWindow-Btn": {"display": "none !important"},
+                    ".FullWindow-Btn, .Bbox-Controls": {"display": "none !important"},
                 },
                 "@keyframes heart-beat": {
                     "from": {
                         "transform": "translateX(-16px)",
                         "opacity": "0.5",
                     },
                     "to": {
@@ -211,14 +213,17 @@
                         "background": "var(--accent-color)",
                         "border-color": "var(--accent-color)",
                         "^:hover, ^:focus": {
                             "background": "var(--hover-bg) !important",
                             "border-color": "var(--hover-bg) !important",
                         },
                     },
+                    ".noUi-connect.noUi-draggable": { # for ranger sliders
+                        "background": "var(--accent-color)",
+                    },
                 },
                 ".widget-html": {
                     "^:not(div.LaserPointer), .widget-html-content > div": {
                         "display": "grid !important",
                         "font-size": "var(--text-size) !important",
                     },
                     ".widget-html-content": {
@@ -233,15 +238,14 @@
                     "border": "none",
                     "padding": "0 !important",
                     "width": "60% !important",
                     "z-index": "10",
                     "top": "0px !important",
                     "left": "0px !important",
                     "transition": "height 400ms ease-in-out",
-                    "border-right" : "2px inset var(--alternate-bg)",
                     "@container slides (max-width: 650px)": {"width": "100% !important"},
                     ".CaptureHtml": {
                         "border": "1px solid var(--secondary-fg)",
                         "figure": {
                             "width": "100% !important",
                             "margin": "0",
                             "padding": "0",
@@ -744,15 +748,14 @@
                     "width": "100% !important",
                     "height": "100% !important",
                     "> .SlidesWrapper": {
                         "width": "100% !important",
                         "height": "auto !important",
                         "aspect-ratio": f"{aspect} !important",
                         "margin": "auto !important",
-                        "box-shadow": "var(--jp-border-color1,#D1D9E1) 0px 0px 1px 1px !important",
                         f"@container resize-box (aspect-ratio > {aspect})": {
                             "width": "auto !important",
                             "height": "100% !important",
                         },
                         ".Width-Slider": {"display": "none !important",},
                     },
                 },
```

### Comparing `ipyslides-3.8.7/ipyslides/_base/_widgets.py` & `ipyslides-3.8.8/ipyslides/_base/_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import traitlets
 import sysconfig
 import anywidget
 
 from pathlib import Path
 from IPython.display import display
 
-
 def _hot_reload_dev_only(file):
     path = Path(__file__).with_name('js') / file
     egg_path = Path(sysconfig.get_paths()["purelib"]) / 'ipyslides.egg-link'
     if egg_path.exists(): # Package installed as editable
         return path # Developers
     return path.read_text() # Normal users
```

### Comparing `ipyslides-3.8.7/ipyslides/_base/base.py` & `ipyslides-3.8.8/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/export_html.py` & `ipyslides-3.8.8/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/export_template.py` & `ipyslides-3.8.8/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/icons.py` & `ipyslides-3.8.8/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/intro.py` & `ipyslides-3.8.8/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/js/interaction.js` & `ipyslides-3.8.8/ipyslides/_base/js/interaction.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -244,15 +244,14 @@
         setScale(box);
     });
 
     resizeObs.observe(box);
     setScale(box); // First time set
 }
 
-
 export function render({
     model,
     el
 }) {
     model.syncIntervalID = null; // Need for Markdown Sync
     let style = document.createElement('style');
     //  Trick to get main slide element is to wait for a loadable element
@@ -305,15 +304,14 @@
             if (!msg) {
                 return false
             }; // empty message, don't waste time
             handleMessage(model, msg, box, cursor);
         })
 
         // Handle notifications
-
         let toast = box.getElementsByClassName('Toast')[0]; // Define once
         toast.style = "top:-120%;transition: top 200ms"; // other props in CSS
         toast.timerId = null; // Need to auto remove after some time
 
         model.on("msg:custom", (msg) => {
             handleToastMessage(toast, msg);
         })
```

### Comparing `ipyslides-3.8.7/ipyslides/_base/js/notes.js` & `ipyslides-3.8.8/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/navigation.py` & `ipyslides-3.8.8/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/notes.py` & `ipyslides-3.8.8/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/screenshot.py` & `ipyslides-3.8.8/ipyslides/_base/screenshot.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,34 +20,37 @@
         "Instnace should be inside `Slides` class."
         self.widgets = _instanceWidgets
         self.btn_cap_all = self.widgets.buttons.cap_all
         self.btn_pdf = self.widgets.buttons.pdf
         self.btn_png = self.widgets.buttons.png
         self.btn_capture = self.widgets.buttons.capture
         self.btn_settings = self.widgets.buttons.setting
-        self.bbox = self.widgets.inputs.bbox
         
         self.__images = {} #Store screenshots
         self.__capture_settings = {'load_time':0.8,'quality':95,'bbox':None}
-        self.capturing = False
+        self._screen_bbox = None # will be store on display
+        self._capturing = False
         
         self.btn_capture.on_click(self.capture)
         self.btn_pdf.on_click(self.__save_pdf)
         self.btn_png.on_click(self.__save_images)
         self.btn_cap_all.on_click(self.__capture_all)
         self.widgets.ddowns.clear.observe(self.__clear_images)
-        self.bbox.on_submit(self._set_bbox)
+        self.widgets.sliders.crop_w.observe(self._set_bbox, names="value")
+        self.widgets.sliders.crop_h.observe(self._set_bbox, names="value")
 
     def _set_bbox(self, change):
-        x1,y1,x2,y2 = tuple(map(int,self.bbox.value.split(',')[:4]))
+        im = ImageGrab.grab() # full image initially
+        x1,x2 = [int(im.width*w/100) for w in self.widgets.sliders.crop_w.value]
+        y1,y2 = [int(im.height*h/100) for h in self.widgets.sliders.crop_h.value]
 
-        if (x2 < x1) or (y2 < y1):
-            self.widgets._push_toast(alert('left < right and top < bottom should hold!').value, timeout=10)
+        if (x2 <= x1) or (y2 <= y1):
+            return # No need at zero width
         
-        arr = np.asarray(ImageGrab.grab(bbox=(x1,y1,x2,y2)))
+        arr = np.asarray(im.crop([x1,y1,x2,y2]))
         new_arr = np.concatenate([arr[:100],np.zeros_like(arr[:5]), arr[-100:]])
         new_arr = np.concatenate([new_arr[:,:160], np.zeros_like(new_arr[:, :5]), new_arr[:,-160:]],axis=1)
 
         img = image(Image.fromarray(new_arr),width='100%') 
         self.widgets._push_toast(img.value, timeout=20) # needs enough time to see result
 
         self.capture_setup(**{**self.capture_settings, 'bbox':(x1,y1,x2,y2)})
@@ -62,28 +65,30 @@
                         *additional_widgets_to_hide
                         ]
         old_pref = self.widgets.htmls.toast.layout.visibility # To keep user prefernce back after screenshot
         for w in hide_widgets:
             w.layout.visibility = 'hidden'
         try:  
             self.widgets.mainbox.add_class('CaptureMode') # Used to hide other things on slide  
-            self.capturing = True # Must be for main class to know
+            self._capturing = True # Must be for main class to know
             yield
         finally:
             self.widgets.mainbox.remove_class('CaptureMode')
-            self.capturing = False # Back to normal
+            self._capturing = False # Back to normal
             for w in hide_widgets:
                 w.layout.visibility = 'visible' 
             self.widgets.htmls.toast.layout.visibility = old_pref 
             
     @property           
     def screen_bbox(self):
         "Return screen's bounding box in pixels."
-        img = ImageGrab.grab(bbox=None) # Just to get bounding box
-        return (0,0, *img.size)
+        if not self._screen_bbox:
+            img = ImageGrab.grab(bbox=None) # Just to get bounding box
+            self._screen_bbox = (0,0, *img.size)
+        return self._screen_bbox
 
     def capture_setup(self,load_time=0.5,quality=95,bbox = None):
         """Setting for screen capture. 
         - load_time: 0.5; time in seconds for each slide to load before print, only applied to Capture All, not on manual screenshot. 
         - quality: 95; In term of current screen. Will not chnage too much above 95. 
         - bbox: None; None for full screen on any platform. Given screen position of slides in pixels as [left,top,right,bottom].
         > Note: Auto detection of bbox in frontends where javascript runs is under progress. """
```

### Comparing `ipyslides-3.8.7/ipyslides/_base/settings.py` & `ipyslides-3.8.8/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/slide.py` & `ipyslides-3.8.8/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/styles.py` & `ipyslides-3.8.8/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/_base/widgets.py` & `ipyslides-3.8.8/ipyslides/_base/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,22 +92,15 @@
     loading = HTML(layout=Layout(display='none')).add_class('Loading') #SVG Animation in it
     logo    = HtmlWidget('').add_class('LogoHtml')
     toast   = HtmlWidget('').add_class('Toast') # For notifications
     cursor  = HtmlWidget('').add_class('LaserPointer') # For beautiful cursor
     hilite  = HTML() # Updated in settings on creation. For code blocks.
     zoom    = HTML() # zoom CSS, do not add here!
     glass   = HTML().add_class('BackLayer') # For glass effect
-    
-@dataclass(frozen=True)
-class _Inputs:
-    """
-    Instantiate under `Widgets` class only.
-    """
-    bbox = ipw.Text(description='L,T,R,B (px)',layout=auto_layout,value='Type left,top, right,bottom pixel values and press ↲').add_class('Bbox-Input')
-    
+
 @dataclass(frozen=True)
 class _Checks:
     """
     Instantiate under `Widgets` class only.
     """
     reflow  = ipw.Checkbox(indent = False, value=False,description='Reflow Content',layout=auto_layout)
     notes   = ipw.Checkbox(indent = False, value=False,description='Notes',layout=auto_layout) # do not observe, just keep track when slides work
@@ -120,14 +113,16 @@
 class _Sliders:
     """
     Instantiate under `Widgets` class only.
     """
     progress = ipw.SelectionSlider(options=[('0',0)], value=0, continuous_update=False,readout=True)
     width    = ipw.IntSlider(**describe('Width (vw)'),min=20,max=100, value = 60,continuous_update=False).add_class('Width-Slider') 
     fontsize = ipw.IntSlider(**describe('Font Size'),min=8,max=64,step=1, value = 20,continuous_update=False, tooltip="If you need more larger/smaller font size, use `Slides.settings.set_font_size`")
+    crop_w   = ipw.FloatRangeSlider(**describe('Width (%)'), min=0,max=100,value=[20,80],step=0.025, continuous_update=False) # step for upto 4k screen by default
+    crop_h   = ipw.FloatRangeSlider(**describe('Height (%)'), min=0,max=100,value=[25,75],step=0.025, continuous_update=False)
 
 @dataclass(frozen=True)
 class _Dropdowns:
     """
     Instantiate under `Widgets` class only.
     """
     theme  = ipw.Dropdown(**describe('Theme'),options=[*styles.theme_colors.keys(),'Custom'],value='Inherit')
@@ -151,15 +146,14 @@
         # print(f'Inside: {self.__class__.__name__}')
         self._tmp_out = Output(layout=dict(margin='0',width='0',height='0')) # For adding slide's CSS and animations
         self._progbar = ipw.Box([ipw.Box().add_class("Progress")],layout=dict(width="100%",height="3px", visibility = "visible")).add_class("Progress-Box") # border not working everywhere
         self._snum   = Button(description='',layout= Layout(width='auto',height='auto')).add_class("Slide-Number").add_class('Menu-Item')
         self.buttons = _Buttons()
         self.toggles = _Toggles()
         self.sliders = _Sliders()
-        self.inputs  = _Inputs()
         self.checks  = _Checks()
         self.htmls   = _Htmls()
         self.ddowns  = _Dropdowns()
         self.iw      = InteractionWidget(self)
         self.notes   = NotesWidget(value = 'Notes Preview')
         self.drawer  = ipw.Box([TldrawWidget().add_class('Draw-Widget'), self.toggles.draw]).add_class('Draw-Wrapper')
         self.drawer.layout = dict(width='100%',height='0',overflow='hidden') # height will be chnaged by button
@@ -203,16 +197,19 @@
                     self.checks.proxy,self.checks.navgui,self.checks.focus,
                     self.buttons.cap_all,self.buttons.pdf,self.buttons.png,
                 ],layout=Layout(width='auto',overflow_x='scroll',
                                 grid_template_columns='1fr 1fr 1fr',grid_gap='4px',
                                 padding='4px',margin='8px auto')
                 )],layout=Layout(min_height='120px')),# This ensures no collapse and scrollable Grid
                 self.ddowns.clear,
-                HTML('<span style="font-size:14px;">Set screenshot bounding box (if slides not fullscreen)</span>'),
-                self.inputs.bbox,
+                VBox([
+                    HTML('<span style="font-size:14px;">Set screenshot bounding box (if slides not fullscreen)</span>'),
+                    self.sliders.crop_w,
+                    self.sliders.crop_h,
+                ], layout=Layout(min_height='90px')).add_class("Bbox-Controls"),
                 self._tmp_out,
                 self.notes, # Just to be there for acting on a popup window
             ],layout=Layout(width='auto',height='auto',overflow_y='scroll',padding='12px',margin='0')),
         ],layout = Layout(width='70%',min_width='50%',height='0',overflow='hidden')).add_class('SidePanel') 
         
         self.tocbox = VBox([],layout = Layout(width='30%',min_width='400px',height='0',overflow='auto')).add_class('TOC')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ipyslides-3.8.7/ipyslides/_demo.py` & `ipyslides-3.8.8/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/core.py` & `ipyslides-3.8.8/ipyslides/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,17 @@
     def _setup(self):
         # Only in Jupyter Notebook
         if self.shell and self.shell.__class__.__name__ != "TerminalInteractiveShell":
             if self._max_index == 0:  # prevent overwrite
                 self._add_clean_title()
 
             with suppress(BaseException):  # Does not work everywhere.
-                self.widgets.inputs.bbox.value = ", ".join(map(str,self.screenshot.screen_bbox))
+                *_, w, h = self.screenshot.screen_bbox
+                self.widgets.sliders.crop_w.step = 100/w # precise step as given by screen pixels
+                self.widgets.sliders.crop_h.step = 100/h
         else:
             if self._max_index == 0:  # prevent overwrite
                 self._slides_dict["0"] = Slide(self, "0")  # just for completeness
                 self.refresh()  # Refresh to update number of slides etc
 
     def __repr__(self):
         repr_all = ",\n    ".join(repr(s) for s in self._iterable)
@@ -574,15 +576,15 @@
         _objs = [
             self._iterable[new_index].css,
             self.html(
                 "style",
                 f"{uclass} .toc-item.s{self._sectionindex} {{font-weight:bold;}}",
             )]
 
-        if self.screenshot.capturing == False:
+        if self.screenshot._capturing == False:
             _objs.append(self._iterable[new_index].animation)
 
         self._update_tmp_output(*_objs)
         self.widgets.update_progressbar()
 
         if (old_index + 1) > len(self.widgets.slidebox.children):
             old_index = new_index  # Just safe
```

### Comparing `ipyslides-3.8.7/ipyslides/formatters.py` & `ipyslides-3.8.8/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/source.py` & `ipyslides-3.8.8/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/utils.py` & `ipyslides-3.8.8/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/writer.py` & `ipyslides-3.8.8/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides/xmd.py` & `ipyslides-3.8.8/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.8.8/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.7
+Version: 3.8.8
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.7/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.8.8/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.7/setup.py` & `ipyslides-3.8.8/setup.py`

 * *Files identical despite different names*

