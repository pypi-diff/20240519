# Comparing `tmp/yolo_world_onnx-0.1.0.tar.gz` & `tmp/yolo_world_onnx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolo_world_onnx-0.1.0.tar", last modified: Sun May 19 05:24:23 2024, max compression
+gzip compressed data, was "yolo_world_onnx-0.1.1.tar", last modified: Sun May 19 05:31:11 2024, max compression
```

## Comparing `yolo_world_onnx-0.1.0.tar` & `yolo_world_onnx-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-19 05:24:23.593271 yolo_world_onnx-0.1.0/
--rw-r--r--   0 ziad      (1000) ziad      (1000)     9403 2024-05-19 05:24:23.593271 yolo_world_onnx-0.1.0/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8445 2024-05-19 05:20:47.000000 yolo_world_onnx-0.1.0/README.md
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       38 2024-05-19 05:24:23.593271 yolo_world_onnx-0.1.0/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1225 2024-05-19 05:22:08.000000 yolo_world_onnx-0.1.0/setup.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-19 05:24:23.593271 yolo_world_onnx-0.1.0/yolo_world_onnx/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       43 2024-05-19 04:06:58.000000 yolo_world_onnx-0.1.0/yolo_world_onnx/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7198 2024-05-18 19:38:56.000000 yolo_world_onnx-0.1.0/yolo_world_onnx/model.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-19 05:24:23.593271 yolo_world_onnx-0.1.0/yolo_world_onnx.egg-info/
--rw-r--r--   0 ziad      (1000) ziad      (1000)     9403 2024-05-19 05:24:23.000000 yolo_world_onnx-0.1.0/yolo_world_onnx.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      265 2024-05-19 05:24:23.000000 yolo_world_onnx-0.1.0/yolo_world_onnx.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-19 05:24:23.000000 yolo_world_onnx-0.1.0/yolo_world_onnx.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       85 2024-05-19 05:24:23.000000 yolo_world_onnx-0.1.0/yolo_world_onnx.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       16 2024-05-19 05:24:23.000000 yolo_world_onnx-0.1.0/yolo_world_onnx.egg-info/top_level.txt
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-19 05:31:11.895380 yolo_world_onnx-0.1.1/
+-rw-r--r--   0 ziad      (1000) ziad      (1000)     9404 2024-05-19 05:31:11.895380 yolo_world_onnx-0.1.1/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8446 2024-05-19 05:30:53.000000 yolo_world_onnx-0.1.1/README.md
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       38 2024-05-19 05:31:11.895380 yolo_world_onnx-0.1.1/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1225 2024-05-19 05:31:00.000000 yolo_world_onnx-0.1.1/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-19 05:31:11.891380 yolo_world_onnx-0.1.1/yolo_world_onnx/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       43 2024-05-19 04:06:58.000000 yolo_world_onnx-0.1.1/yolo_world_onnx/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7198 2024-05-18 19:38:56.000000 yolo_world_onnx-0.1.1/yolo_world_onnx/model.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-19 05:31:11.891380 yolo_world_onnx-0.1.1/yolo_world_onnx.egg-info/
+-rw-r--r--   0 ziad      (1000) ziad      (1000)     9404 2024-05-19 05:31:11.000000 yolo_world_onnx-0.1.1/yolo_world_onnx.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      265 2024-05-19 05:31:11.000000 yolo_world_onnx-0.1.1/yolo_world_onnx.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-19 05:31:11.000000 yolo_world_onnx-0.1.1/yolo_world_onnx.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       85 2024-05-19 05:31:11.000000 yolo_world_onnx-0.1.1/yolo_world_onnx.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       16 2024-05-19 05:31:11.000000 yolo_world_onnx-0.1.1/yolo_world_onnx.egg-info/top_level.txt
```

### Comparing `yolo_world_onnx-0.1.0/PKG-INFO` & `yolo_world_onnx-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolo-world-onnx
-Version: 0.1.0
+Version: 0.1.1
 Summary: ONNX-YOLO is a Python package for running inference on YOLO-WORLD open-vocabulary object detection models using ONNX runtime.
 Home-page: https://github.com/Ziad-Algrafi/onnx-yolo
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 [![PyPI version](https://badge.fury.io/py/yolo-world-onnx.svg)](https://badge.fury.io/py/yolo-world-onnx)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ziad-Algrafi/yolo-world-onnx/blob/main/assets/YOLO_World_ONNX.ipynb)
 [![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 </div>
 
-![Parking Lot Prompt Red Car](https://github.com/Ziad-Algrafi/yolo-world-onnx/blob/main/assets/Object%20Detection.png)
+![Prompt is red car](https://raw.githubusercontent.com/Ziad-Algrafi/yolo-world-onnx/main/assets/Object%20Detection.png)
 
 YOLO-World-ONNX is a Python package that enables running inference on YOLO-WORLD open-vocabulary object detection models using ONNX runtime. It provides a user-friendly interface for performing object detection on images or videos. The package leverages ONNX models to deliver fast inference time, making it suitable for a wide range of object detection applications.
 
 ## Installation
 
 You can install YOLO-World-ONNX using pip:
```

### Comparing `yolo_world_onnx-0.1.0/README.md` & `yolo_world_onnx-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPI version](https://badge.fury.io/py/yolo-world-onnx.svg)](https://badge.fury.io/py/yolo-world-onnx)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ziad-Algrafi/yolo-world-onnx/blob/main/assets/YOLO_World_ONNX.ipynb)
 [![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 </div>
 
-![Parking Lot Prompt Red Car](https://github.com/Ziad-Algrafi/yolo-world-onnx/blob/main/assets/Object%20Detection.png)
+![Prompt is red car](https://raw.githubusercontent.com/Ziad-Algrafi/yolo-world-onnx/main/assets/Object%20Detection.png)
 
 YOLO-World-ONNX is a Python package that enables running inference on YOLO-WORLD open-vocabulary object detection models using ONNX runtime. It provides a user-friendly interface for performing object detection on images or videos. The package leverages ONNX models to deliver fast inference time, making it suitable for a wide range of object detection applications.
 
 ## Installation
 
 You can install YOLO-World-ONNX using pip:
```

### Comparing `yolo_world_onnx-0.1.0/setup.py` & `yolo_world_onnx-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="yolo-world-onnx",
-    version="0.1.0",
+    version="0.1.1",
     packages=["yolo_world_onnx"],
     include_package_data=True,
     install_requires=[
         "numpy",
         "opencv-python",
         "onnxruntime-gpu",
         "torch>=1.7.0",
```

### Comparing `yolo_world_onnx-0.1.0/yolo_world_onnx/model.py` & `yolo_world_onnx-0.1.1/yolo_world_onnx/model.py`

 * *Files identical despite different names*

### Comparing `yolo_world_onnx-0.1.0/yolo_world_onnx.egg-info/PKG-INFO` & `yolo_world_onnx-0.1.1/yolo_world_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolo-world-onnx
-Version: 0.1.0
+Version: 0.1.1
 Summary: ONNX-YOLO is a Python package for running inference on YOLO-WORLD open-vocabulary object detection models using ONNX runtime.
 Home-page: https://github.com/Ziad-Algrafi/onnx-yolo
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 [![PyPI version](https://badge.fury.io/py/yolo-world-onnx.svg)](https://badge.fury.io/py/yolo-world-onnx)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ziad-Algrafi/yolo-world-onnx/blob/main/assets/YOLO_World_ONNX.ipynb)
 [![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 </div>
 
-![Parking Lot Prompt Red Car](https://github.com/Ziad-Algrafi/yolo-world-onnx/blob/main/assets/Object%20Detection.png)
+![Prompt is red car](https://raw.githubusercontent.com/Ziad-Algrafi/yolo-world-onnx/main/assets/Object%20Detection.png)
 
 YOLO-World-ONNX is a Python package that enables running inference on YOLO-WORLD open-vocabulary object detection models using ONNX runtime. It provides a user-friendly interface for performing object detection on images or videos. The package leverages ONNX models to deliver fast inference time, making it suitable for a wide range of object detection applications.
 
 ## Installation
 
 You can install YOLO-World-ONNX using pip:
```

