# Comparing `tmp/pygamextras-1.1.6.tar.gz` & `tmp/pygamextras-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygamextras-1.1.6.tar", max compression
+gzip compressed data, was "pygamextras-1.1.7.tar", max compression
```

## Comparing `pygamextras-1.1.6.tar` & `pygamextras-1.1.7.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0     1091 2023-09-24 01:46:21.865382 pygamextras-1.1.6/LICENSE.txt
--rw-r--r--   0        0        0       28 2023-09-23 15:29:20.709795 pygamextras-1.1.6/main/PygameXtras/__init__.py
--rw-r--r--   0        0        0        0 2023-09-23 16:11:25.887474 pygamextras-1.1.6/main/PygameXtras/src/__init__.py
--rw-r--r--   0        0        0      772 2024-05-09 23:08:33.613728 pygamextras-1.1.6/main/PygameXtras/src/classes/__init__.py
--rw-r--r--   0        0        0     9617 2023-11-25 20:44:04.832441 pygamextras-1.1.6/main/PygameXtras/src/classes/Bar.py
--rw-r--r--   0        0        0     3900 2023-09-23 15:53:12.120929 pygamextras-1.1.6/main/PygameXtras/src/classes/Button.py
--rw-r--r--   0        0        0     5619 2024-02-16 00:25:11.507109 pygamextras-1.1.6/main/PygameXtras/src/classes/C.py
--rw-r--r--   0        0        0     1625 2024-03-11 20:52:23.893174 pygamextras-1.1.6/main/PygameXtras/src/classes/Collisions.py
--rw-r--r--   0        0        0    12895 2023-04-21 00:07:14.084627 pygamextras-1.1.6/main/PygameXtras/src/classes/Colors.py
--rw-r--r--   0        0        0     2555 2023-11-25 20:46:23.639451 pygamextras-1.1.6/main/PygameXtras/src/classes/CustomTemplate.py
--rw-r--r--   0        0        0    39244 2023-11-25 20:59:50.919919 pygamextras-1.1.6/main/PygameXtras/src/classes/Entity.py
--rw-r--r--   0        0        0    13596 2023-12-02 00:50:40.682100 pygamextras-1.1.6/main/PygameXtras/src/classes/Entry.py
--rw-r--r--   0        0        0    11526 2023-09-23 15:52:44.078009 pygamextras-1.1.6/main/PygameXtras/src/classes/Function.py
--rw-r--r--   0        0        0     6867 2023-11-25 20:48:13.714174 pygamextras-1.1.6/main/PygameXtras/src/classes/Functions.py
--rw-r--r--   0        0        0     5114 2023-11-25 20:49:10.824661 pygamextras-1.1.6/main/PygameXtras/src/classes/Keyboard.py
--rw-r--r--   0        0        0    34983 2023-11-25 20:59:58.646965 pygamextras-1.1.6/main/PygameXtras/src/classes/Label.py
--rw-r--r--   0        0        0     6052 2023-09-23 15:51:24.540925 pygamextras-1.1.6/main/PygameXtras/src/classes/Messagebox.py
--rw-r--r--   0        0        0      480 2023-01-08 13:28:54.080041 pygamextras-1.1.6/main/PygameXtras/src/classes/OneClickManager.py
--rw-r--r--   0        0        0    20637 2023-09-23 15:51:15.063234 pygamextras-1.1.6/main/PygameXtras/src/classes/Paragraph.py
--rw-r--r--   0        0        0     1492 2023-11-25 20:43:20.479244 pygamextras-1.1.6/main/PygameXtras/src/classes/PerformanceGraph.py
--rw-r--r--   0        0        0     5561 2023-09-23 15:51:09.818079 pygamextras-1.1.6/main/PygameXtras/src/classes/PlayStationController.py
--rw-r--r--   0        0        0     6856 2024-05-09 23:25:24.426620 pygamextras-1.1.6/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg.py
--rw-r--r--   0        0        0     4685 2024-05-09 23:06:43.658058 pygamextras-1.1.6/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg_util.py
--rw-r--r--   0        0        0     2792 2023-09-23 15:51:05.104310 pygamextras-1.1.6/main/PygameXtras/src/classes/PopupMessage.py
--rw-r--r--   0        0        0    25214 2023-09-23 15:50:41.846248 pygamextras-1.1.6/main/PygameXtras/src/classes/RandomClasses.py
--rw-r--r--   0        0        0     6651 2023-09-23 15:50:58.115828 pygamextras-1.1.6/main/PygameXtras/src/classes/ScrollableButtonList.py
--rw-r--r--   0        0        0     4480 2023-01-08 13:33:47.321223 pygamextras-1.1.6/main/PygameXtras/src/classes/Spritesheet.py
--rw-r--r--   0        0        0     2235 2023-01-08 13:34:43.904812 pygamextras-1.1.6/main/PygameXtras/src/classes/Table.py
--rw-r--r--   0        0        0        0 2023-09-23 15:31:37.487011 pygamextras-1.1.6/main/PygameXtras/src/images/__init__.py
--rw-r--r--   0        0        0      410 2022-12-18 00:36:16.366358 pygamextras-1.1.6/main/PygameXtras/src/images/decrease_size.png
--rw-r--r--   0        0        0      418 2022-12-18 00:36:15.311921 pygamextras-1.1.6/main/PygameXtras/src/images/increase_size.png
--rw-r--r--   0        0        0     1724 2023-09-23 15:53:58.435943 pygamextras-1.1.6/main/PygameXtras/test/Bar.py
--rw-r--r--   0        0        0     1445 2023-09-23 15:54:10.083261 pygamextras-1.1.6/main/PygameXtras/test/CustomTemplate.py
--rw-r--r--   0        0        0      988 2023-09-23 15:54:18.546103 pygamextras-1.1.6/main/PygameXtras/test/Entry.py
--rw-r--r--   0        0        0     1927 2023-09-23 15:54:24.219499 pygamextras-1.1.6/main/PygameXtras/test/Label.py
--rw-r--r--   0        0        0     1687 2023-09-23 15:54:56.993224 pygamextras-1.1.6/main/PygameXtras/test/PopupMessage.py
--rw-r--r--   0        0        0     1475 2024-05-09 23:31:08.283405 pygamextras-1.1.6/main/PygameXtras/test/PSVG.py
--rw-r--r--   0        0        0      483 2024-05-09 23:32:36.549109 pygamextras-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      244 2023-12-04 14:48:57.853907 pygamextras-1.1.6/README.md
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 pygamextras-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-09-24 01:46:21.865382 pygamextras-1.1.7/LICENSE.txt
+-rw-r--r--   0        0        0       28 2023-09-23 15:29:20.709795 pygamextras-1.1.7/main/PygameXtras/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-23 16:11:25.887474 pygamextras-1.1.7/main/PygameXtras/src/__init__.py
+-rw-r--r--   0        0        0      808 2024-05-18 22:30:51.598339 pygamextras-1.1.7/main/PygameXtras/src/classes/__init__.py
+-rw-r--r--   0        0        0     9617 2023-11-25 20:44:04.832441 pygamextras-1.1.7/main/PygameXtras/src/classes/Bar.py
+-rw-r--r--   0        0        0     3900 2023-09-23 15:53:12.120929 pygamextras-1.1.7/main/PygameXtras/src/classes/Button.py
+-rw-r--r--   0        0        0     5619 2024-02-16 00:25:11.507109 pygamextras-1.1.7/main/PygameXtras/src/classes/C.py
+-rw-r--r--   0        0        0     6283 2024-05-18 22:26:16.712874 pygamextras-1.1.7/main/PygameXtras/src/classes/Collisions.py
+-rw-r--r--   0        0        0    12895 2023-04-21 00:07:14.084627 pygamextras-1.1.7/main/PygameXtras/src/classes/Colors.py
+-rw-r--r--   0        0        0     2555 2023-11-25 20:46:23.639451 pygamextras-1.1.7/main/PygameXtras/src/classes/CustomTemplate.py
+-rw-r--r--   0        0        0    39244 2023-11-25 20:59:50.919919 pygamextras-1.1.7/main/PygameXtras/src/classes/Entity.py
+-rw-r--r--   0        0        0    13596 2023-12-02 00:50:40.682100 pygamextras-1.1.7/main/PygameXtras/src/classes/Entry.py
+-rw-r--r--   0        0        0    11526 2023-09-23 15:52:44.078009 pygamextras-1.1.7/main/PygameXtras/src/classes/Function.py
+-rw-r--r--   0        0        0     6867 2023-11-25 20:48:13.714174 pygamextras-1.1.7/main/PygameXtras/src/classes/Functions.py
+-rw-r--r--   0        0        0     5114 2023-11-25 20:49:10.824661 pygamextras-1.1.7/main/PygameXtras/src/classes/Keyboard.py
+-rw-r--r--   0        0        0    34983 2023-11-25 20:59:58.646965 pygamextras-1.1.7/main/PygameXtras/src/classes/Label.py
+-rw-r--r--   0        0        0     6052 2023-09-23 15:51:24.540925 pygamextras-1.1.7/main/PygameXtras/src/classes/Messagebox.py
+-rw-r--r--   0        0        0      480 2023-01-08 13:28:54.080041 pygamextras-1.1.7/main/PygameXtras/src/classes/OneClickManager.py
+-rw-r--r--   0        0        0    20637 2023-09-23 15:51:15.063234 pygamextras-1.1.7/main/PygameXtras/src/classes/Paragraph.py
+-rw-r--r--   0        0        0     1492 2023-11-25 20:43:20.479244 pygamextras-1.1.7/main/PygameXtras/src/classes/PerformanceGraph.py
+-rw-r--r--   0        0        0     5561 2023-09-23 15:51:09.818079 pygamextras-1.1.7/main/PygameXtras/src/classes/PlayStationController.py
+-rw-r--r--   0        0        0     6856 2024-05-09 23:25:24.426620 pygamextras-1.1.7/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg.py
+-rw-r--r--   0        0        0     4685 2024-05-09 23:06:43.658058 pygamextras-1.1.7/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg_util.py
+-rw-r--r--   0        0        0     2792 2023-09-23 15:51:05.104310 pygamextras-1.1.7/main/PygameXtras/src/classes/PopupMessage.py
+-rw-r--r--   0        0        0    25214 2023-09-23 15:50:41.846248 pygamextras-1.1.7/main/PygameXtras/src/classes/RandomClasses.py
+-rw-r--r--   0        0        0     6651 2023-09-23 15:50:58.115828 pygamextras-1.1.7/main/PygameXtras/src/classes/ScrollableButtonList.py
+-rw-r--r--   0        0        0     4480 2023-01-08 13:33:47.321223 pygamextras-1.1.7/main/PygameXtras/src/classes/Spritesheet.py
+-rw-r--r--   0        0        0     2235 2023-01-08 13:34:43.904812 pygamextras-1.1.7/main/PygameXtras/src/classes/Table.py
+-rw-r--r--   0        0        0        0 2023-09-23 15:31:37.487011 pygamextras-1.1.7/main/PygameXtras/src/images/__init__.py
+-rw-r--r--   0        0        0      410 2022-12-18 00:36:16.366358 pygamextras-1.1.7/main/PygameXtras/src/images/decrease_size.png
+-rw-r--r--   0        0        0      418 2022-12-18 00:36:15.311921 pygamextras-1.1.7/main/PygameXtras/src/images/increase_size.png
+-rw-r--r--   0        0        0       15 2024-05-18 22:29:53.527009 pygamextras-1.1.7/main/PygameXtras/test/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-23 15:53:58.435943 pygamextras-1.1.7/main/PygameXtras/test/Bar.py
+-rw-r--r--   0        0        0     1445 2023-09-23 15:54:10.083261 pygamextras-1.1.7/main/PygameXtras/test/CustomTemplate.py
+-rw-r--r--   0        0        0      988 2023-09-23 15:54:18.546103 pygamextras-1.1.7/main/PygameXtras/test/Entry.py
+-rw-r--r--   0        0        0     1927 2023-09-23 15:54:24.219499 pygamextras-1.1.7/main/PygameXtras/test/Label.py
+-rw-r--r--   0        0        0     1687 2023-09-23 15:54:56.993224 pygamextras-1.1.7/main/PygameXtras/test/PopupMessage.py
+-rw-r--r--   0        0        0     1475 2024-05-09 23:31:08.283405 pygamextras-1.1.7/main/PygameXtras/test/PSVG.py
+-rw-r--r--   0        0        0     3533 2024-05-18 22:27:08.940615 pygamextras-1.1.7/main/PygameXtras/test/test_collisions.py
+-rw-r--r--   0        0        0      483 2024-05-18 22:31:44.612395 pygamextras-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-12-04 14:48:57.853907 pygamextras-1.1.7/README.md
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 pygamextras-1.1.7/PKG-INFO
```

### Comparing `pygamextras-1.1.6/LICENSE.txt` & `pygamextras-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/__init__.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .Bar import Bar
 from .Button import Button
 from .C import C
+from .Collisions import Collisions
 from .Colors import Colors
 from .CustomTemplate import CustomTemplate
 from .Entity import Entity
 from .Entry import Entry
 from .Function import Function
 from .Functions import *
 from .Keyboard import Keyboard
```

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Bar.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Bar.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Button.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Button.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/C.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/C.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Colors.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Colors.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/CustomTemplate.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/CustomTemplate.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Entity.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Entity.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Entry.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Entry.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Function.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Function.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Functions.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Functions.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Keyboard.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Keyboard.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Label.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Label.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Messagebox.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Messagebox.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Paragraph.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Paragraph.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/PerformanceGraph.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/PerformanceGraph.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/PlayStationController.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/PlayStationController.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg_util.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg_util.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/PopupMessage.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/PopupMessage.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/RandomClasses.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/RandomClasses.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/ScrollableButtonList.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/ScrollableButtonList.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Spritesheet.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Spritesheet.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/src/classes/Table.py` & `pygamextras-1.1.7/main/PygameXtras/src/classes/Table.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/test/Bar.py` & `pygamextras-1.1.7/main/PygameXtras/test/Bar.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/test/CustomTemplate.py` & `pygamextras-1.1.7/main/PygameXtras/test/CustomTemplate.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/test/Entry.py` & `pygamextras-1.1.7/main/PygameXtras/test/Entry.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/test/Label.py` & `pygamextras-1.1.7/main/PygameXtras/test/Label.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/test/PopupMessage.py` & `pygamextras-1.1.7/main/PygameXtras/test/PopupMessage.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/main/PygameXtras/test/PSVG.py` & `pygamextras-1.1.7/main/PygameXtras/test/PSVG.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.6/PKG-INFO` & `pygamextras-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameXtras
-Version: 1.1.6
+Version: 1.1.7
 Summary: Labels, Buttons and much more for pygame
 Home-page: https://github.com/marcelm9/PygameXtras.git
 License: MIT
 Author: marcelm9
 Author-email: marcel.menzel09@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

