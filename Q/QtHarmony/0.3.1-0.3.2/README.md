# Comparing `tmp/qtharmony-0.3.1.tar.gz` & `tmp/qtharmony-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.3.1.tar", max compression
+gzip compressed data, was "qtharmony-0.3.2.tar", max compression
```

## Comparing `qtharmony-0.3.1.tar` & `qtharmony-0.3.2.tar`

### file list

```diff
@@ -1,55 +1,59 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.3.1/LICENSE
--rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.3.1/README.md
--rw-r--r--   0        0        0      312 2024-05-19 15:12:11.570344 qtharmony-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.3.1/qtharmony/__init__.py
--rw-r--r--   0        0        0       22 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/config/config.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.3.1/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      628 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0      120 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/font.py
--rw-r--r--   0        0        0      876 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/load.py
--rw-r--r--   0        0        0     2020 2024-05-19 14:58:03.557732 qtharmony-0.3.1/qtharmony/core/sizes.py
--rw-r--r--   0        0        0     1235 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/theme/__init__.py
--rw-r--r--   0        0        0     1295 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/theme/theme_builder.py
--rw-r--r--   0        0        0     2345 2024-05-14 15:55:11.674548 qtharmony-0.3.1/qtharmony/core/theme/theme_manager.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.3.1/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     4715 2024-05-14 17:26:45.157068 qtharmony-0.3.1/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.3.1/qtharmony/resources/themes/dark-green.json
--rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.3.1/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.3.1/qtharmony/resources/themes/light-green.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.3.1/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.3.1/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.3.1/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.3.1/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2504 2024-05-19 14:22:26.904287 qtharmony-0.3.1/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2674 2024-05-19 15:01:36.144234 qtharmony-0.3.1/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2672 2024-05-19 15:09:27.901563 qtharmony-0.3.1/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3646 2024-05-19 15:09:43.817463 qtharmony-0.3.1/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2676 2024-05-19 15:10:11.259475 qtharmony-0.3.1/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0     1028 2024-05-19 15:10:26.328749 qtharmony-0.3.1/qtharmony/widgets/basic/frame.py
--rw-r--r--   0        0        0     2899 2024-05-19 15:10:40.941378 qtharmony-0.3.1/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3473 2024-05-19 15:10:54.327400 qtharmony-0.3.1/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     4033 2024-05-19 15:11:09.779989 qtharmony-0.3.1/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     2072 2024-05-19 15:11:26.499183 qtharmony-0.3.1/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     2395 2024-05-19 15:01:03.742453 qtharmony-0.3.1/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.3.1/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.3.1/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.3.1/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.3.1/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.3.1/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.3.1/qtharmony/widgets/basic/styles/frame.css
--rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.3.1/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.3.1/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.3.1/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.3.1/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.3.1/qtharmony/widgets/basic/styles/splitter.css
--rw-r--r--   0        0        0        0 2024-05-14 17:18:13.597694 qtharmony-0.3.1/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1460 2024-05-19 15:11:53.071236 qtharmony-0.3.1/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.3.1/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2679 2024-05-14 15:55:11.677882 qtharmony-0.3.1/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.3.1/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 qtharmony-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.3.2/README.md
+-rw-r--r--   0        0        0      332 2024-05-19 17:07:52.647658 qtharmony-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.3.2/qtharmony/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/config/config.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.3.2/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0      120 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/load.py
+-rw-r--r--   0        0        0     2097 2024-05-19 15:26:04.110161 qtharmony-0.3.2/qtharmony/core/sizes.py
+-rw-r--r--   0        0        0     1235 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/theme/__init__.py
+-rw-r--r--   0        0        0     1295 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     2345 2024-05-14 15:55:11.674548 qtharmony-0.3.2/qtharmony/core/theme/theme_manager.py
+-rw-r--r--   0        0        0       34 2024-05-19 15:35:15.130208 qtharmony-0.3.2/qtharmony/gui/icon.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.3.2/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     4753 2024-05-19 17:01:05.587092 qtharmony-0.3.2/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.3.2/qtharmony/resources/themes/dark-green.json
+-rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.3.2/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.3.2/qtharmony/resources/themes/light-green.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.3.2/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.3.2/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.3.2/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0      545 2024-05-19 16:53:04.636656 qtharmony-0.3.2/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2931 2024-05-19 15:37:08.484731 qtharmony-0.3.2/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2674 2024-05-19 15:13:06.504362 qtharmony-0.3.2/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2672 2024-05-19 15:13:06.504362 qtharmony-0.3.2/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3646 2024-05-19 15:13:06.504362 qtharmony-0.3.2/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2676 2024-05-19 15:13:06.504362 qtharmony-0.3.2/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0     1028 2024-05-19 15:13:06.504362 qtharmony-0.3.2/qtharmony/widgets/basic/frame.py
+-rw-r--r--   0        0        0     2899 2024-05-19 15:13:06.504362 qtharmony-0.3.2/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3463 2024-05-19 16:52:12.462465 qtharmony-0.3.2/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0      389 2024-05-19 15:50:59.741231 qtharmony-0.3.2/qtharmony/widgets/basic/picture.py
+-rw-r--r--   0        0        0     2072 2024-05-19 15:13:06.507695 qtharmony-0.3.2/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     2395 2024-05-19 15:13:06.507695 qtharmony-0.3.2/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.3.2/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.3.2/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.3.2/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.3.2/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.3.2/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.3.2/qtharmony/widgets/basic/styles/frame.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.3.2/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.3.2/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.3.2/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.3.2/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.3.2/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0        0 2024-05-19 16:52:39.931162 qtharmony-0.3.2/qtharmony/widgets/basic/styles/text_box.css
+-rw-r--r--   0        0        0        0 2024-05-19 15:13:06.507695 qtharmony-0.3.2/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1550 2024-05-19 16:54:20.933031 qtharmony-0.3.2/qtharmony/widgets/basic/text_box.py
+-rw-r--r--   0        0        0     1460 2024-05-19 15:13:06.514361 qtharmony-0.3.2/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0     4047 2024-05-19 15:42:22.159574 qtharmony-0.3.2/qtharmony/widgets/custom/path_entry.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.3.2/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2679 2024-05-14 15:55:11.677882 qtharmony-0.3.2/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.3.2/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 qtharmony-0.3.2/PKG-INFO
```

### Comparing `qtharmony-0.3.1/LICENSE` & `qtharmony-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/README.md` & `qtharmony-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/constructor/initialize.py` & `qtharmony-0.3.2/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/core/dialog.py` & `qtharmony-0.3.2/qtharmony/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/core/font.py` & `qtharmony-0.3.2/qtharmony/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/core/load.py` & `qtharmony-0.3.2/qtharmony/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/core/sizes.py` & `qtharmony-0.3.2/qtharmony/core/sizes.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     height: Optional[int]
 
     def ratio(self) -> str:
         if len(self.valid_size()) == 2: 
             return "Size"
         else:
             return [i for i in ("width", "height") 
-                    if not i.startswith("_") and getattr(self, i) is not None][0].capitalize()
+                    if getattr(self, i) is not None][0].capitalize()
 
     def valid_size(self) -> tuple[int]:
         return tuple(filter(
             lambda x: isinstance(x, int), (self.width, self.height)
         ))  # type: ignore
 
 
@@ -30,14 +30,17 @@
     @abstractmethod
     def use(self, widget: "QWidget") -> None:
         ...
 
 
 class SizeBuilder(AbstractSize):
     def __init__(self, width: Optional[int], height: Optional[int], method) -> None:
+        if width is None and height is None:
+            raise ValueError("Both arguments are None.")
+
         self.size: Size = Size(width, height)
         self.method = method
 
     def use(self, widget: "QWidget") -> None:
         method = f"{self.method}{self.size.ratio()}"
 
         if hasattr(widget, method):
```

### Comparing `qtharmony-0.3.1/qtharmony/core/stylesheet.py` & `qtharmony-0.3.2/qtharmony/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/core/theme/theme_builder.py` & `qtharmony-0.3.2/qtharmony/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/core/theme/theme_manager.py` & `qtharmony-0.3.2/qtharmony/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.3.2/qtharmony/resources/themes/dark-default.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933035714285714%*

 * *Differences: {"'TextBox'": "{'': {'background-color': '#404040', 'border-radius': '6px'}}"}*

```diff
@@ -162,15 +162,16 @@
         "object-name": "QRadioButton#radio-button"
     },
     "Splitter": {
         "object-name": "QSplitter#splitter"
     },
     "TextBox": {
         "": {
-            "background-color": "green"
+            "background-color": "#404040",
+            "border-radius": "6px"
         },
         "object-name": "QPlainTextEdit#text-box"
     },
     "WidgetsList": {
         "": {
             "background-color": "#404040",
             "border": "none",
```

### Comparing `qtharmony-0.3.1/qtharmony/resources/themes/dark-green.json` & `qtharmony-0.3.2/qtharmony/resources/themes/dark-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/resources/themes/light-default.json` & `qtharmony-0.3.2/qtharmony/resources/themes/light-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/resources/themes/light-green.json` & `qtharmony-0.3.2/qtharmony/resources/themes/light-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/resources/ui/Icon.png` & `qtharmony-0.3.2/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/resources/ui/Logo.png` & `qtharmony-0.3.2/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.3.2/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/button.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/button.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from PySide6.QtWidgets import QPushButton
+from PySide6.QtGui import QIcon
 from PySide6.QtCore import QSize
 
 from qtharmony.core import StyleSheetLoader
 from qtharmony.core.theme import ThemeManager
 from qtharmony.core.sizes import AbstractSize
 
-from typing import Optional, TYPE_CHECKING
+from typing import Optional, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
-    from PySide6.QtGui import QFont
+    from PySide6.QtGui import QFont, QPixmap
 
 
 class PushButton(QPushButton):
     """
     Custom QPushButton widget for push button functionality.
 
     Methods:
@@ -26,14 +27,16 @@
 
     def __init__(
             self, 
             text: Optional[str] = None,
             size: Optional[AbstractSize] = None,
             font: Optional["QFont"] = None, 
             is_active: bool = True,
+            icon: Optional[Union[str, "QIcon", "QPixmap"]] = None,
+            icon_size: Optional[tuple[int, int]] = None,
             *,
             object_name: str = "button",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None, 
     ) -> None:
         """
         Initializes the PushButton widget with optional text, size, font, and stylesheet.
@@ -45,14 +48,23 @@
             stylesheet (Optional[str], optional): Custom stylesheet for the push button widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the push button. Defaults to None.
         """ 
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
+        if icon is not None: 
+            if isinstance(icon, str):
+                self.setIcon(QIcon(icon))
+            else:
+                self.setIcon(icon)
+        
+        if icon_size is not None:
+            self.setIconSize(QSize(*icon_size))
+
         if font is not None: self.setFont(font)
         self.setDisabled(not is_active)
 
         self.setObjectName(object_name)
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/button.css", 
             name=self.__class__.__name__, obj_name=f"QPushButton#{self.objectName()}",
```

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/check_box.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/digital_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/entry.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/frame.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/frame.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/groups.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/label.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/label.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             text: str,
             font_family: str, 
             font_size: int,
             bold: bool = False,
             italic: bool = False,
             color: Optional[str] = None,
             size: Optional[AbstractSize] = None,
-            word_wrap: bool = False,
+            wrap: bool = False,
             is_active: bool = True,
             *,
             object_name: str = "label",
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
@@ -67,15 +67,15 @@
 
         self.setText(text)
         if color is not None: self.set_color(color)
         if size is not None: size.use(self)
 
         self.setDisabled(not is_active)
         
-        self.setWordWrap(word_wrap)
+        self.setWordWrap(wrap)
         self.setFont(Font.get_system_font(font_family, font_size, bold, italic))
     
     def set_color(self, color: str) -> None:
         """
         Sets the color of the label text.
 
         Args:
```

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.3.2/qtharmony/widgets/custom/path_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     QWidget, QHBoxLayout, 
     QSpacerItem, QSizePolicy
 )
 
 from qtharmony.core import FileDialog, StyleSheetLoader
 from qtharmony.core.sizes import AbstractSize, FixedSize
 
-from .button import PushButton
-from .entry import Entry
+from ..basic.button import PushButton
+from ..basic.entry import Entry
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
 
 
 class PathEntry(QWidget):
```

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/radio_button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/splitter.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.3.2/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/qtharmony/windows/main_window.py` & `qtharmony-0.3.2/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.1/PKG-INFO` & `qtharmony-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: pyside6 (>=6.7.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img src="logo.png">
 </p>
 <h1></h1>
```

