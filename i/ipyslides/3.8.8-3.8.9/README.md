# Comparing `tmp/ipyslides-3.8.8.tar.gz` & `tmp/ipyslides-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.8.8.tar", last modified: Sat May 18 00:40:56 2024, max compression
+gzip compressed data, was "ipyslides-3.8.9.tar", last modified: Sat May 18 22:11:48 2024, max compression
```

## Comparing `ipyslides-3.8.8.tar` & `ipyslides-3.8.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.950660 ipyslides-3.8.8/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.8/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-18 00:40:56.950660 ipyslides-3.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.873007 ipyslides-3.8.8/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.8/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-18 00:39:35.000000 ipyslides-3.8.8/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.947119 ipyslides-3.8.8/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.8/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    40305 2024-05-18 00:25:03.000000 ipyslides-3.8.8/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.8.8/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.8/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.8.8/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.8.8/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.8.8/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    12158 2024-05-10 07:35:58.000000 ipyslides-3.8.8/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.949176 ipyslides-3.8.8/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12476 2024-05-17 22:26:29.000000 ipyslides-3.8.8/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.8/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.8/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.8/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    13446 2024-05-18 00:06:17.000000 ipyslides-3.8.8/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-14 00:03:47.000000 ipyslides-3.8.8/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.8.8/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.8.8/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    15530 2024-05-18 00:36:33.000000 ipyslides-3.8.8/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.8/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    48149 2024-05-18 00:08:30.000000 ipyslides-3.8.8/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.8/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.8/ipyslides/source.py
--rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.8.8/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.8/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.8/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:40:56.919278 ipyslides-3.8.8/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 00:40:56.000000 ipyslides-3.8.8/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 00:40:56.950660 ipyslides-3.8.8/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.285028 ipyslides-3.8.9/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.9/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-18 22:11:48.285028 ipyslides-3.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.160575 ipyslides-3.8.9/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.9/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-18 22:10:59.000000 ipyslides-3.8.9/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.285028 ipyslides-3.8.9/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.9/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    40807 2024-05-18 22:04:23.000000 ipyslides-3.8.9/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.8.9/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.9/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.8.9/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.8.9/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.8.9/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    11666 2024-05-18 21:58:12.000000 ipyslides-3.8.9/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.285028 ipyslides-3.8.9/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12476 2024-05-17 22:26:29.000000 ipyslides-3.8.9/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.9/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.9/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.9/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11993 2024-05-18 21:24:06.000000 ipyslides-3.8.9/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23555 2024-05-14 00:03:47.000000 ipyslides-3.8.9/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.8.9/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.8.9/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16113 2024-05-18 22:07:00.000000 ipyslides-3.8.9/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.9/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47862 2024-05-18 17:47:27.000000 ipyslides-3.8.9/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.9/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.9/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.8.9/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.9/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.9/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-18 22:11:48.236154 ipyslides-3.8.9/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 22:11:47.000000 ipyslides-3.8.9/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 22:11:48.300662 ipyslides-3.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.9/setup.py
```

### Comparing `ipyslides-3.8.8/LICENSE` & `ipyslides-3.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/PKG-INFO` & `ipyslides-3.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.8
+Version: 3.8.9
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.8/README.md` & `ipyslides-3.8.9/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/_layout_css.py` & `ipyslides-3.8.9/ipyslides/_base/_layout_css.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 "^.PresentMode .SlideBox .SlideArea .ProxyPasteBtns": {
                     "display": "none !important"
                 },  # Hide in presentation mode
                 "^.FullWindow, ^.FullScreen": {
                     ".Width-Slider, .Source-Btn": {"display": "none !important"},
                 },
                 "^.FullScreen": {
-                    ".FullWindow-Btn, .Bbox-Controls": {"display": "none !important"},
+                    ".FullWindow-Btn": {"display": "none !important"},
                 },
                 "@keyframes heart-beat": {
                     "from": {
                         "transform": "translateX(-16px)",
                         "opacity": "0.5",
                     },
                     "to": {
@@ -248,25 +248,31 @@
                         "figure": {
                             "width": "100% !important",
                             "margin": "0",
                             "padding": "0",
                             "background": "var(--secondary-bg)",
                         },
                     },
+                    ".widget-html-content": {"font-size": "var(--jp-widgets-font-size) !important",},
+                    ":not(.TopBar) :is(button, .jupyter-button)": {
+                        "margin-left":"var(--jp-widgets-inline-label-width) !important",
+                        "width": "max-content !important",
+                        "min-height": "28px !important",
+                    },
                     ".Settings-Btn": {
                         "border": "none !important",
                         "outline": "none !important",
                         "font-size": "20px",
                         "background": "transparent !important",
                         "> i": {
                             "color": "var(--accent-color) !important",
                         },
                     },
                 },
-                ":is(.SlideBox, .SidePanel) :is(button, .jupyter-button)": {
+                ".SlideBox :is(button, .jupyter-button)": {
                     "border": "1px solid var(--accent-color)",
                     "border-radius": "4px",
                     "min-height": "28px",
                     "min-width": "28px",
                 },
                 "^, *": {
                     "box-sizing": "border-box",
@@ -510,30 +516,32 @@
             },
             ".jp-RenderedText": {
                 "*": {"font-size": "0.9em !important",},
                 "^, pre": {
                     "color": "var(--primary-fg) !important",
                 },
             },
-            ".Draw-Wrapper": { # height is set dynamically
+            ".Draw-Wrapper, .CropBox": { # height is set dynamically
                 "position": "absolute !important",
                 "left": 0,
                 "top":0,
                 "z-index": "8 !important",
                 "overflow": "hidden !important",
                 "transition": "height 200ms",
+                "backdrop-filter": "blur(50px)",
                 "> .Draw-Btn" : {
                     "position": "absolute !important",
                     "left": 0,
                     "top":0,
                     "z-index": "9 !important",
                     "width": "36px !important",
                     "^:active, ^.mod-active": {"box-shadow": "none !important","opacity": "1 !important",},
                 },
             },
+            ".CropBox": {"z-index": "15 !important",}, # above others
             ".Draw-Widget": {
                 "backdrop-filter": "blur(50px)",
                 "margin": 0,
                 "z-index": 6,
                 "overflow": "hidden !important",
                 "transition": "height 200ms",
                 "^, > div": {
```

### Comparing `ipyslides-3.8.8/ipyslides/_base/_widgets.py` & `ipyslides-3.8.9/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/base.py` & `ipyslides-3.8.9/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/export_html.py` & `ipyslides-3.8.9/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/export_template.py` & `ipyslides-3.8.9/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/icons.py` & `ipyslides-3.8.9/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/intro.py` & `ipyslides-3.8.9/ipyslides/_base/intro.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,14 @@
         <path d="M22.5 7.5L10 20L20 30L30 20L40 30L27.5 42.5" stroke="teal"/>
         <path d="M7.5 27.5L22.5 42.5" stroke="crimson"/>
         <path d="M32.5 32.5L20 20L30 10L42.5 22.5" stroke="red"/>
         <text x="55" y="37.5" stroke-width="0" fill="currentColor" style="font-size:1.5em;font-weight:bold;">{V}</text>
     </svg>'''
 
 
-how_to_ppt = """### Powerpoint Presentation
-- Save all screenshots using `Save PNG` button and go to folder just created.
-- You know the aspect ratio while taking screenshots, if not, read details of any of picture to find it.
-- Open Powerpoint, got to `Design` tab and select `Slide Size`. If pictures here are of aspect ratio 4:3 or 16:9, select that,
-otherwise select `Custom Slide Size` and change size there according to found aspect ratio. 
-- You will see a slide of your prefered size now. Go to `Insert` tab and select `Photo Album > New Photo Album`.
-- Select `File/Disk` option to insert pictures and make sure `Picture Layout` option is `Fit to slide`.
-- Now click `Create` and you will see all pictures as slides.
-
-::: note-warning
-    Do not use PDF from Powerpoint as that will lower quality, generate PDF from slides instead. 
-"""
-
 how_to_slide = """# Creating Slides
 ::: align-center
     alert`Abdul Saboor`sup`1`, Unknown Authorsup`2`     
     center`today```
 
     ::: text-box
         sup`1`My University is somewhere in the middle of nowhere
@@ -154,14 +141,31 @@
 | {_key('V')}                                 | {_icons["win-maximize"]}, {_icons["win-restore"]} | {key_maps["V"]}        |
 | {_key('G')}                                 | {_icons["settings"]}, {_icons["close"]}           | {key_maps["G"]}        |
 | {_key('E')}                                 | {_icons["code"]}                                  | {key_maps["E"]}        |
 | {_key('L')}                                 | {_icons["laser"]}, {_icons["circle"]}             | {key_maps["L"]}        |
 | {_key('K')}                                 |                                                   | {key_maps["K"]}        |
 """ 
 
+how_to_print = """
+- Capture screenshot of current state of slide by camera button in toolbar or by pressing `S` key. 
+    This will collect screenshots of current slide in order of capturing. 
+- Press `Capture Screenshots of all Slides` button in side panel to capture a single image of each slide. 
+    - Add images over it by manually capturing multiple states of a slide as shown in previous step.
+    - Delete screenshots with dropdown in settings panel.
+    - Set crop bounding box if not in fullscreen mode.
+- Press `Save as PDF File` button to save all screenshots as PDF.
+
+::: note-warning
+    Avoid scrolling during taking screenshot. You will set same bounding box for all screenshots
+    which can change position if scrolled.
+
+::: note-tip
+    You can also get PDF from exported HTML file, but can't have the freedom of capturing 
+    many views of single slide.
+"""
 more_instructions = f"""{get_logo('2em', 'IPySlides')}
 ::: note-tip
     In JupyterLab, right click on the slides and select `Create New View for Output` for optimized display.
 
 **Key Bindings**{{.success}} {_Icon("pencil", color="var(--accent-color)", rotation=45)}
 
 Having slides in focus, you can use follwoing keys/combinations:
@@ -173,31 +177,26 @@
 
 ::: note-tip
     - Other keys are blocked so that you may not delete or do some random actions on notebook cells.
     - Jupyter[Retro, Notebook, Lab]/Voila is optimized for keyboard. Other frontends like VSCode, may not work properly.
     - Pressing `S` to save screenshot of current state of slide. Different slides' screenshots are kept in order.
 
 ### PDF Printing (by Screen Capture)
-- Capture screenshot of current state of slide by camera button in toolbar or by pressing `S` key. 
-    This will collect screenshots of current slide in order of capturing. 
-    This is a manual process but you can collect content as you want. You can hover top-right corner to use a slider to adjust height of visible content.
-- Press `Capture All` button in side panel to capture a single image of each slide. Then you can add images over it by manually capturing.
-- Press `Save PDF` button to save all screenshots as PDF.
+{how_to_print}
 
 {how_to_slide}
 
 ::: note-info
     Slides should be only in top cell as it collects slides in local namespace, auto refresh is enabled.
 
 ::: note-warning
     Restart Kernel if you make mistake in slide numbers to avoid hidden state problem.
 """
 
 instructions = f"""{more_instructions}
-{how_to_ppt}
 ### Custom Theme
 For custom themes, change below `Theme` dropdown to `Custom` and use `Slides.settings.set_theme_colors` to set colors.
           
 --------
 For matching plots style with theme, run following code in a cell above slides.
 
 **Matplotlib**{{.success}}
```

### Comparing `ipyslides-3.8.8/ipyslides/_base/js/interaction.js` & `ipyslides-3.8.9/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/js/notes.js` & `ipyslides-3.8.9/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/navigation.py` & `ipyslides-3.8.9/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/notes.py` & `ipyslides-3.8.9/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/screenshot.py` & `ipyslides-3.8.9/ipyslides/_base/screenshot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,77 @@
 """
 Author Notes: Classes in this module should only be instantiated in Slides class or it's parent class
 and then provided to other classes via composition, not inheritance.
 """
 
 import os 
 from time import sleep
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 
 from PIL import Image, ImageGrab
-import numpy as np
 
-from ..utils import image, alert, get_child_dir
+from ..utils import image, get_child_dir
 from ..writer import CustomDisplay
-from . import intro
 
 
 class ScreenShot:
     def __init__(self, _instanceWidgets):
         "Instnace should be inside `Slides` class."
         self.widgets = _instanceWidgets
         self.btn_cap_all = self.widgets.buttons.cap_all
         self.btn_pdf = self.widgets.buttons.pdf
-        self.btn_png = self.widgets.buttons.png
+        self.btn_crop = self.widgets.buttons.crop
         self.btn_capture = self.widgets.buttons.capture
         self.btn_settings = self.widgets.buttons.setting
         
         self.__images = {} #Store screenshots
-        self.__capture_settings = {'load_time':0.8,'quality':95,'bbox':None}
-        self._screen_bbox = None # will be store on display
+        self._cimage = None # cureent image
+        self._crop_bbox = None
+        self.__capture_settings = {'load_time':0.8,'quality':95}
         self._capturing = False
         
         self.btn_capture.on_click(self.capture)
         self.btn_pdf.on_click(self.__save_pdf)
-        self.btn_png.on_click(self.__save_images)
         self.btn_cap_all.on_click(self.__capture_all)
+        self.btn_crop.on_click(self.__toggle_crop_window)
         self.widgets.ddowns.clear.observe(self.__clear_images)
-        self.widgets.sliders.crop_w.observe(self._set_bbox, names="value")
-        self.widgets.sliders.crop_h.observe(self._set_bbox, names="value")
+        self.widgets.sliders.crop_w.observe(self._crop_image, names="value")
+        self.widgets.sliders.crop_h.observe(self._crop_image, names="value")
 
-    def _set_bbox(self, change):
-        im = ImageGrab.grab() # full image initially
-        x1,x2 = [int(im.width*w/100) for w in self.widgets.sliders.crop_w.value]
-        y1,y2 = [int(im.height*h/100) for h in self.widgets.sliders.crop_h.value]
-
-        if (x2 <= x1) or (y2 <= y1):
-            return # No need at zero width
-        
-        arr = np.asarray(im.crop([x1,y1,x2,y2]))
-        new_arr = np.concatenate([arr[:100],np.zeros_like(arr[:5]), arr[-100:]])
-        new_arr = np.concatenate([new_arr[:,:160], np.zeros_like(new_arr[:, :5]), new_arr[:,-160:]],axis=1)
-
-        img = image(Image.fromarray(new_arr),width='100%') 
-        self.widgets._push_toast(img.value, timeout=20) # needs enough time to see result
-
-        self.capture_setup(**{**self.capture_settings, 'bbox':(x1,y1,x2,y2)})
+        with suppress(BaseException): # only on supportive systems silently
+            im = ImageGrab.grab()
+            self.widgets.sliders.crop_w.max = im.width
+            self.widgets.sliders.crop_w.value = (0, im.width)
+            self.widgets.sliders.crop_h.max = im.height
+            self.widgets.sliders.crop_h.value = (0, im.height)
+
+    def __toggle_crop_window(self, btn):
+        if self.widgets.cropbox.layout.height == '0':
+            self.widgets.cropbox.layout.height = '100%'
+            self.btn_crop.description = 'Close'
+            if self.__images:
+                self._load_image(self.images[0]) # load from ordered images
+            else:
+                self.widgets.htmls.crop.value = 'Screenshot appears here for cropping!'
+        else:
+            self.widgets.cropbox.layout.height = '0'
+            self.btn_crop.description = 'Set Crop Bounding Box'
+    
+    def _load_image(self, im):
+        self._cimage = im
+        self.widgets.htmls.crop.value = image(im,width='100%').value
+
+    def _crop_image(self, change):
+        if self._cimage is not None:
+            x1,x2 = self.widgets.sliders.crop_w.value
+            y2,y1 = [self.widgets.sliders.crop_h.max - v for v in self.widgets.sliders.crop_h.value]
+            self._crop_bbox = [x1,y1,x2,y2]
+            self.widgets.htmls.crop.value = image(self._cimage.crop([x1,y1,x2,y2]), width='100%').value
+        elif self.__images:
+            self._load_image(self.images[0]) 
 
     @contextmanager
     def capture_mode(self, *additional_widgets_to_hide):
         """Hide some widgets and while capturing a screenshot, show them back again.
         You can provide additional widgets to hide while capturing as well."""
         hide_widgets = [self.widgets.controls, # now other buttons are inside Menu-Box which gets hidden 
                         self.widgets.htmls.toast,
@@ -73,37 +87,23 @@
             yield
         finally:
             self.widgets.mainbox.remove_class('CaptureMode')
             self._capturing = False # Back to normal
             for w in hide_widgets:
                 w.layout.visibility = 'visible' 
             self.widgets.htmls.toast.layout.visibility = old_pref 
-            
-    @property           
-    def screen_bbox(self):
-        "Return screen's bounding box in pixels."
-        if not self._screen_bbox:
-            img = ImageGrab.grab(bbox=None) # Just to get bounding box
-            self._screen_bbox = (0,0, *img.size)
-        return self._screen_bbox
 
-    def capture_setup(self,load_time=0.5,quality=95,bbox = None):
+    def capture_setup(self,load_time=0.5,quality=95):
         """Setting for screen capture. 
-        - load_time: 0.5; time in seconds for each slide to load before print, only applied to Capture All, not on manual screenshot. 
-        - quality: 95; In term of current screen. Will not chnage too much above 95. 
-        - bbox: None; None for full screen on any platform. Given screen position of slides in pixels as [left,top,right,bottom].
-        > Note: Auto detection of bbox in frontends where javascript runs is under progress. """
+        - load_time: 0.5; time in seconds for each slide to load before print. 
+        - quality: 95; In term of current screen. Will not chnage too much above 95."""
         if load_time < 0.1:
             return print("load_time must be greater than 0.1 to at least load the slide")
-        if bbox and len(bbox) != 4:
-            return print("bbox expects [left,top,right,bottom] in integers")
-        self.__capture_settings = {'load_time':load_time,'quality':quality,'bbox':bbox if bbox else self.screen_bbox} # get full if none given
-        # Display what user sets
-        if bbox:
-            return image(ImageGrab.grab(bbox=bbox),width='100%')
+        
+        self.__capture_settings = {'load_time':load_time,'quality':quality} 
 
     @property  
     def capture_settings(self):
         "See the settings applied for screenshot. Use `self.capture_setup` function to adjust settings."
         return self.__capture_settings    
     
     def __set_resolution(self,image):
@@ -119,26 +119,27 @@
     def capture(self,btn):
         "Saves screenshot of current slide into self.__images dictionary when corresponding button clicked. Use in fullscreen mode or set bbox using `.capture_setup`."
         with self.capture_mode():
             sleep(0.05) # Just for above clearance of widgets views
             if self.widgets.sliders.progress.label not in self.__images:
                 self.__images[self.widgets.sliders.progress.label] = [] # container to store images
             
-            # Keep full image if in fullscreen
-            bbox = None if "FullScreen" in self.widgets.mainbox._dom_classes else self.capture_settings['bbox']
-            self.__images[self.widgets.sliders.progress.label].append(ImageGrab.grab(bbox = bbox)) # Append to existing list
+            self._cimage = ImageGrab.grab(bbox = None) # keep for cropping
+            self.__images[self.widgets.sliders.progress.label].append(self._cimage) # Append to existing list
     
     def __sort_images(self):
         ims = [] #sorting
         for label, _ in self.widgets.sliders.progress.options:
             if label in self.__images:
                 ims = [*ims,*self.__images[label]]
+
+        ims = [im.crop(self._crop_bbox) if self._crop_bbox else im for im in ims] # crop here, not in property images
         return tuple(ims)
             
-    def save_pdf(self,filename='IPySlides.pdf'):
+    def save_pdf(self,filename='Slides.pdf'):
         "Converts saved screenshots to PDF!"
         ims = self.__sort_images()    
         if ims: # make sure not empty
             self.btn_pdf.description = 'Generatingting PDF...'
             ims[0].save(filename,'PDF',quality= self.capture_settings['quality'] ,save_all=True,append_images=ims[1:],
                         resolution=self.__set_resolution(ims[0]),subsampling=0)
             self.btn_pdf.description = 'Save PDF'
@@ -152,47 +153,24 @@
     def __capture_all(self,btn):
         "Quickly capture all slides and save them as images."
         self.btn_settings.click() # Close side panel
         for label, _ in self.widgets.sliders.progress.options:
             with self.capture_mode():
                 self.widgets.sliders.progress.label = label # swicth to that slide
                 sleep(self.capture_settings['load_time']) #keep waiting here until it almost loads 
-                self.__images[label] = [ImageGrab.grab(bbox = self.capture_settings['bbox']),] # Save image in a list on which we can add others
+                self.__images[label] = [ImageGrab.grab(bbox = None),] # Save image in a list on which we can add others
         
-        self.widgets._push_toast("All slides captured. Use Save PDF/Save PNG buttons to save them.") 
+        self.widgets._push_toast("All slides captured. Use Save PDF button to save them.") 
          
     
     @property
     def images(self):
         "Get all captured screenshots in order."
         return self.__sort_images()
     
-    def save_images(self):
-        "Save all screenshots as PNG in given `notebook_dir/.ipyslides-assets/images`. Names are auto ordered"
-        self.btn_png.description = 'Saving PNGs...'
-        directory = get_child_dir('.ipyslides-assets', 'images', create=True)
-        
-        ims = self.images
-        if ims:    
-            for i,im in enumerate(ims):
-                im.save(os.path.join(directory,f'Slide-{i:03}.png'),'PNG',quality= self.capture_settings['quality'],subsampling=0,optimize=True)  # Do not lose image quality at least here
-            md_file = os.path.join(directory,'Make-PPT.md')
-            with open(md_file,'w', encoding='utf-8') as f:
-                f.write(intro.how_to_ppt)
-            self.widgets._push_toast(f'''All captured images are saved in "{directory}"<br/> 
-                         <em>See file "{md_file}" as bonus option!</em>''',timeout=10)
-        else:
-            self.widgets._push_toast('No images found to save. Take screenshots of slides, then use this option.')
-        
-        self.btn_png.description = 'Save PNG'
-        
-    def __save_images(self,btn):
-        "With Button call"
-        self.save_images()
-    
     def __clear_images(self,change):
         if 'Current' in self.widgets.ddowns.clear.value:
             _how_many = [img.close() for img in self.__images.get(self.widgets.sliders.progress.label,[])] # Close image to save mememory          
             self.__images[self.widgets.sliders.progress.label] = [] # Clear images at that slide       
             
             if _how_many:
                 self.widgets._push_toast(f'Deleting screenshots of current slide. {len(_how_many)} images deleted.')
```

### Comparing `ipyslides-3.8.8/ipyslides/_base/settings.py` & `ipyslides-3.8.9/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/slide.py` & `ipyslides-3.8.9/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/styles.py` & `ipyslides-3.8.9/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/_base/widgets.py` & `ipyslides-3.8.9/ipyslides/_base/widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses import dataclass
 import ipywidgets as ipw
 from ipywidgets import HTML, VBox, HBox, Box, GridBox, Layout, Button
 from IPython import get_ipython
 from tldraw import TldrawWidget
 from . import styles, _layout_css
 from ._widgets import InteractionWidget, HtmlWidget, NotesWidget
-from .intro import get_logo
+from .intro import get_logo, how_to_print
 from ..utils import html
 
 
 class Output(ipw.Output):
     __doc__ = ipw.Output.__doc__ # same docs
 
     _ipyshell = get_ipython()
@@ -38,16 +38,16 @@
 
 # patching for correct order of outputs, loaded with ipywidgets import when ipyslides is present
 ipw.interaction.Output = Output
 ipw.Output = Output
 ipw.widget_output.Output = Output
 
 auto_layout =  Layout(width='auto')
-def describe(value): 
-    return {'description': value, 'description_width': 'initial','layout':Layout(width='auto')}
+def describe(value,**kwargs): 
+    return {'description': value, 'description_width': 'initial','layout':Layout(width='auto',**kwargs)}
 
 
 @dataclass(frozen=True)
 class _Buttons:
     """
     Instantiate under `Widgets` class only.
     """
@@ -55,22 +55,22 @@
     next    =  Button(icon='chevron-right',layout= Layout(width='auto',height='auto'),tooltip='Next Slide [>, Space]').add_class('Arrows').add_class('Next-Btn')
     setting =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Open Settings [G]').add_class('Menu-Item').add_class('Settings-Btn')
     toc     =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Toggle Table of Contents').add_class('Menu-Item').add_class('Toc-Btn')
     refresh =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'),tooltip='Refresh Dynamic Content').add_class('Menu-Item').add_class('Refresh-Btn')
     source  =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Edit Source Cell [E]').add_class('Menu-Item').add_class('Source-Btn')
     home    =  Button(icon='plus',layout= Layout(width='auto',height='auto'), tooltip='Go to Title Page').add_class('Menu-Item').add_class('Home-Btn')
     end     =  Button(icon='plus',layout= Layout(width='auto',height='auto'), tooltip='Go To End of Slides').add_class('Menu-Item').add_class('End-Btn')
-    info    =  Button(icon='plus',layout= Layout(width='auto',height='auto'), tooltip='Information').add_class('Menu-Item').add_class('Info-Btn')
+    info    =  Button(icon='plus',layout= Layout(width='auto',height='auto'), tooltip='Read Information').add_class('Menu-Item').add_class('Info-Btn')
     capture =  Button(icon='camera',layout= Layout(width='auto',height='auto'),
                 tooltip='Take Screen short in full screen. Order of multiple shots in a slide is preserved! [S]',
                 ).add_class('Screenshot-Btn').add_class('Menu-Item')
-    pdf     = Button(description='Save PDF',layout= Layout(width='auto',height='auto'))
-    png     = Button(description='Save PNG',layout= Layout(width='auto',height='auto'))
-    cap_all = Button(description='Capture All',layout= Layout(width='auto',height='auto'))
-    export  = Button(description="Export to HTML",layout= Layout(width='auto',height='auto'))
+    pdf     = Button(description='Save as PDF File',layout= Layout(width='auto',height='auto'))
+    cap_all = Button(description='Capture Screenshots of all Slides',layout= Layout(width='auto',height='auto'))
+    export  = Button(description="Export to HTML File",layout= Layout(width='auto',height='auto'))
+    crop    = Button(description='Set Crop Bounding Box',layout= Layout(width='auto',height='auto'), tooltip='Toggle Crop GUI').add_class('Menu-Item')
     
 @dataclass(frozen=True)
 class _Toggles:
     """
     Instantiate under `Widgets` class only.
     """
     window  = ipw.ToggleButton(icon='plus',value = False, tooltip ='Fill Viewport [V]').add_class('FullWindow-Btn').add_class('Menu-Item')
@@ -92,37 +92,38 @@
     loading = HTML(layout=Layout(display='none')).add_class('Loading') #SVG Animation in it
     logo    = HtmlWidget('').add_class('LogoHtml')
     toast   = HtmlWidget('').add_class('Toast') # For notifications
     cursor  = HtmlWidget('').add_class('LaserPointer') # For beautiful cursor
     hilite  = HTML() # Updated in settings on creation. For code blocks.
     zoom    = HTML() # zoom CSS, do not add here!
     glass   = HTML().add_class('BackLayer') # For glass effect
+    crop    = HTML('Screenshot appears here for cropping!', layout=Layout(margin='auto',padding='0')).add_class('CropHtml')
 
 @dataclass(frozen=True)
 class _Checks:
     """
     Instantiate under `Widgets` class only.
     """
-    reflow  = ipw.Checkbox(indent = False, value=False,description='Reflow Content',layout=auto_layout)
-    notes   = ipw.Checkbox(indent = False, value=False,description='Notes',layout=auto_layout) # do not observe, just keep track when slides work
-    toast   = ipw.Checkbox(indent = False, value = True, description='Notifications',layout=auto_layout)
-    focus   = ipw.Checkbox(indent = False, value = True, description='Auto Focus',layout=auto_layout)
-    proxy   = ipw.Checkbox(indent = False, value = True, description='Proxy Buttons',layout=auto_layout)
-    navgui  = ipw.Checkbox(indent = False, value = True, description='Show Nav. GUI',layout=auto_layout)
+    reflow  = ipw.Checkbox(value=False,description='Reflow Content',layout=auto_layout)
+    notes   = ipw.Checkbox(value=False,description='Notes',layout=auto_layout) # do not observe, just keep track when slides work
+    toast   = ipw.Checkbox(value = True, description='Notifications',layout=auto_layout)
+    focus   = ipw.Checkbox(value = True, description='Auto Focus',layout=auto_layout)
+    proxy   = ipw.Checkbox(value = True, description='Proxy Buttons',layout=auto_layout)
+    navgui  = ipw.Checkbox(value = True, description='Show Nav. GUI',layout=auto_layout)
 
 @dataclass(frozen=True)
 class _Sliders:
     """
     Instantiate under `Widgets` class only.
     """
     progress = ipw.SelectionSlider(options=[('0',0)], value=0, continuous_update=False,readout=True)
     width    = ipw.IntSlider(**describe('Width (vw)'),min=20,max=100, value = 60,continuous_update=False).add_class('Width-Slider') 
     fontsize = ipw.IntSlider(**describe('Font Size'),min=8,max=64,step=1, value = 20,continuous_update=False, tooltip="If you need more larger/smaller font size, use `Slides.settings.set_font_size`")
-    crop_w   = ipw.FloatRangeSlider(**describe('Width (%)'), min=0,max=100,value=[20,80],step=0.025, continuous_update=False) # step for upto 4k screen by default
-    crop_h   = ipw.FloatRangeSlider(**describe('Height (%)'), min=0,max=100,value=[25,75],step=0.025, continuous_update=False)
+    crop_w   = ipw.IntRangeSlider(**describe('w', margin='8px'), min=0,max=100,value=[20,80],step=1, continuous_update=False, readout=False) # step for upto 4k screen by default
+    crop_h   = ipw.IntRangeSlider(**describe('h',height='auto',margin='8px'), min=0,max=100,value=[25,75],step=1, continuous_update=False, readout=False,orientation='vertical')
 
 @dataclass(frozen=True)
 class _Dropdowns:
     """
     Instantiate under `Widgets` class only.
     """
     theme  = ipw.Dropdown(**describe('Theme'),options=[*styles.theme_colors.keys(),'Custom'],value='Inherit')
@@ -179,40 +180,38 @@
         ],layout=Layout(height='28px')).add_class('NavBox')
         
         self.navbox = VBox([
             self.footerbox,
         ]).add_class('NavWrapper')   #class is must
 
         _many_btns = [self.buttons.setting, self.toggles.window, self.toggles.fscreen, self.toggles.laser, self.toggles.zoom, self.buttons.refresh, self.toggles.draw]
+        _html_layout = Layout(border_bottom='1px solid #8988', margin='8px 0 0 8px')
         
         self.panelbox = VBox([
             self.htmls.glass,
             HBox(_many_btns).add_class('TopBar').add_class('Inside'),
             VBox([
+                HTML('<b>Layout and Theme</b>',layout = _html_layout),
                 self.sliders.fontsize,
                 self.sliders.width,
                 self.ddowns.theme,
-                Box([GridBox([
-                    self.buttons.export, self.buttons.info, HTML(), # empty space
-                    self.checks.notes,self.checks.toast,self.checks.reflow,
-                    self.checks.proxy,self.checks.navgui,self.checks.focus,
-                    self.buttons.cap_all,self.buttons.pdf,self.buttons.png,
-                ],layout=Layout(width='auto',overflow_x='scroll',
-                                grid_template_columns='1fr 1fr 1fr',grid_gap='4px',
-                                padding='4px',margin='8px auto')
-                )],layout=Layout(min_height='120px')),# This ensures no collapse and scrollable Grid
+                HTML('<b>Additional Features</b>',layout = _html_layout),
+                self.checks.notes,self.checks.toast,self.checks.reflow,
+                self.checks.proxy,self.checks.navgui,self.checks.focus,
+                HTML('<b>HTML File Export</b>',layout = _html_layout),
+                self.buttons.export,
+                HTML('<b>Screenshot Export</b>',layout = _html_layout),
+                self.buttons.cap_all,
                 self.ddowns.clear,
-                VBox([
-                    HTML('<span style="font-size:14px;">Set screenshot bounding box (if slides not fullscreen)</span>'),
-                    self.sliders.crop_w,
-                    self.sliders.crop_h,
-                ], layout=Layout(min_height='90px')).add_class("Bbox-Controls"),
+                self.buttons.crop,
+                self.buttons.pdf,
+                HTML(html('details',[html('summary','How to Screenshot'), how_to_print]).value),
                 self._tmp_out,
                 self.notes, # Just to be there for acting on a popup window
-            ],layout=Layout(width='auto',height='auto',overflow_y='scroll',padding='12px',margin='0')),
+            ],layout=Layout(width='auto',height='max-content',overflow_y='scroll',padding='12px',margin='0')),
         ],layout = Layout(width='70%',min_width='50%',height='0',overflow='hidden')).add_class('SidePanel') 
         
         self.tocbox = VBox([],layout = Layout(width='30%',min_width='400px',height='0',overflow='auto')).add_class('TOC')
         
         self.slidebox = Box([
             # Slides are added here dynamically
         ],layout= Layout(min_width='100%',min_height='100%', overflow='hidden')).add_class('SlideBox') 
@@ -223,15 +222,28 @@
             self.toggles.menu.value = False
 
         for btn in self.quick_menu.children: # All buttons should close menu
             if hasattr(btn, 'on_click'):
                 btn.on_click(close_quick_menu)
             else:
                 btn.observe(close_quick_menu, names=["value"])
-
+        
+        self.cropbox = GridBox([
+            self.sliders.crop_w,
+            HBox([self.sliders.crop_h, self.htmls.crop]),
+            HBox([self.buttons.pdf, self.buttons.crop], layout = Layout(justify_content='flex-end')),
+            ], layout = Layout(
+                margin='0',
+                padding='0', 
+                width='100%', 
+                height='0',
+                grid_gap = '8px',
+                grid_template_rows='40px auto 40px',
+            )).add_class("CropBox")
+        
         self.mainbox = VBox([
             self.htmls.glass, # This is the glass pane, should be before everything, otherwise it will cover the slide area
             self.htmls.loading, 
             self.htmls.toast,
             self.htmls.main,
             self.htmls.theme,
             self.htmls.logo,
@@ -244,14 +256,15 @@
             self.htmls.zoom,
             HBox([ #Slide_box must be in a box to have animations work
                 self.tocbox, # Should be on left of slides
                 self.slidebox , 
             ],layout= Layout(width='100%',max_width='100%',height='100%',overflow='hidden')), #should be hidden for animation purpose
             self.controls, # Importnat for unique display
             self.drawer, 
+            self.cropbox,
             self.navbox,
             self._snum,
             self._progbar # progressbar should come last
             ],layout= Layout(width=f'{self.sliders.width.value}vw', height=f'{int(self.sliders.width.value*9/16)}vw',margin='auto') # 9/16 is default, will change by setting
         ).add_class('SlidesWrapper')  #Very Important to add this class
 
         for child in self.mainbox.children:
```

### Comparing `ipyslides-3.8.8/ipyslides/_demo.py` & `ipyslides-3.8.9/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/core.py` & `ipyslides-3.8.9/ipyslides/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,19 +196,14 @@
             self.notify('No source cell found!')
 
     def _setup(self):
         # Only in Jupyter Notebook
         if self.shell and self.shell.__class__.__name__ != "TerminalInteractiveShell":
             if self._max_index == 0:  # prevent overwrite
                 self._add_clean_title()
-
-            with suppress(BaseException):  # Does not work everywhere.
-                *_, w, h = self.screenshot.screen_bbox
-                self.widgets.sliders.crop_w.step = 100/w # precise step as given by screen pixels
-                self.widgets.sliders.crop_h.step = 100/h
         else:
             if self._max_index == 0:  # prevent overwrite
                 self._slides_dict["0"] = Slide(self, "0")  # just for completeness
                 self.refresh()  # Refresh to update number of slides etc
 
     def __repr__(self):
         repr_all = ",\n    ".join(repr(s) for s in self._iterable)
```

### Comparing `ipyslides-3.8.8/ipyslides/formatters.py` & `ipyslides-3.8.9/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/source.py` & `ipyslides-3.8.9/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/utils.py` & `ipyslides-3.8.9/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/writer.py` & `ipyslides-3.8.9/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides/xmd.py` & `ipyslides-3.8.9/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.8.9/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.8
+Version: 3.8.9
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.8/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.8.9/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.8/setup.py` & `ipyslides-3.8.9/setup.py`

 * *Files identical despite different names*

