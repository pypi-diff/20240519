# Comparing `tmp/pycutee-0.0.3.tar.gz` & `tmp/pycutee-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycutee-0.0.3.tar", last modified: Sun May 19 11:05:21 2024, max compression
+gzip compressed data, was "pycutee-0.0.4.tar", last modified: Sun May 19 11:06:34 2024, max compression
```

## Comparing `pycutee-0.0.3.tar` & `pycutee-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 11:05:21.396052 pycutee-0.0.3/
--rw-rw-rw-   0        0        0     1086 2024-05-19 11:05:11.000000 pycutee-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2464 2024-05-19 11:05:21.395052 pycutee-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 11:05:21.379450 pycutee-0.0.3/PyCutee/
--rw-rw-rw-   0        0        0      135 2024-04-16 16:28:03.000000 pycutee-0.0.3/PyCutee/__init__.py
--rw-rw-rw-   0        0        0     1003 2024-04-16 16:41:36.000000 pycutee-0.0.3/PyCutee/button_rounded.py
--rw-rw-rw-   0        0        0      792 2024-04-16 16:38:54.000000 pycutee-0.0.3/PyCutee/button_simple.py
-drwxrwxrwx   0        0        0        0 2024-05-19 11:05:21.394053 pycutee-0.0.3/PyCutee.egg-info/
--rw-rw-rw-   0        0        0     2464 2024-05-19 11:05:21.000000 pycutee-0.0.3/PyCutee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-19 11:05:21.000000 pycutee-0.0.3/PyCutee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 11:05:21.000000 pycutee-0.0.3/PyCutee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-19 11:05:21.000000 pycutee-0.0.3/PyCutee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 11:05:21.000000 pycutee-0.0.3/PyCutee.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1793 2024-05-19 11:02:19.000000 pycutee-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 11:05:21.396052 pycutee-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1139 2024-05-19 11:05:20.000000 pycutee-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:06:34.183307 pycutee-0.0.4/
+-rw-rw-rw-   0        0        0     2489 2024-05-19 11:06:34.183307 pycutee-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 11:06:34.165048 pycutee-0.0.4/PyCutee/
+-rw-rw-rw-   0        0        0      135 2024-04-16 16:28:03.000000 pycutee-0.0.4/PyCutee/__init__.py
+-rw-rw-rw-   0        0        0     1003 2024-04-16 16:41:36.000000 pycutee-0.0.4/PyCutee/button_rounded.py
+-rw-rw-rw-   0        0        0      792 2024-04-16 16:38:54.000000 pycutee-0.0.4/PyCutee/button_simple.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:06:34.181803 pycutee-0.0.4/PyCutee.egg-info/
+-rw-rw-rw-   0        0        0     2489 2024-05-19 11:06:34.000000 pycutee-0.0.4/PyCutee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-05-19 11:06:34.000000 pycutee-0.0.4/PyCutee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:06:34.000000 pycutee-0.0.4/PyCutee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-19 11:06:34.000000 pycutee-0.0.4/PyCutee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 11:06:34.000000 pycutee-0.0.4/PyCutee.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1841 2024-05-19 11:06:21.000000 pycutee-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:06:34.183307 pycutee-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2024-05-19 11:06:29.000000 pycutee-0.0.4/setup.py
```

### Comparing `pycutee-0.0.3/PKG-INFO` & `pycutee-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: PyCutee
-Version: 0.0.3
+Version: 0.0.4
 Summary: This app is a lil framework for PyQt5 like bootstrap for HTML5
 Author: Codingrule
 Author-email: <ioumih32@gmail.com>
 Keywords: python,framework,pyqt5,frontend,customize,UI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: PyQt5
 
 
 # PyCutee (The PyQt5 Framework) V0.0.1
 
 PyCutee is a lightweight and stylish framework for PyQt5, designed to simplify the creation of modern and visually appealing graphical user interfaces (GUIs) in Python.
 
@@ -69,8 +68,8 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 ## License
 
-PyCutee is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
+PyCutee is licensed under the MIT License. See [LICENSE](https://github.com/CodingRule/PyCutee/blob/main/LICENSE) for more information.
```

### Comparing `pycutee-0.0.3/PyCutee/button_rounded.py` & `pycutee-0.0.4/PyCutee/button_rounded.py`

 * *Files identical despite different names*

### Comparing `pycutee-0.0.3/PyCutee/button_simple.py` & `pycutee-0.0.4/PyCutee/button_simple.py`

 * *Files identical despite different names*

### Comparing `pycutee-0.0.3/PyCutee.egg-info/PKG-INFO` & `pycutee-0.0.4/PyCutee.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: PyCutee
-Version: 0.0.3
+Version: 0.0.4
 Summary: This app is a lil framework for PyQt5 like bootstrap for HTML5
 Author: Codingrule
 Author-email: <ioumih32@gmail.com>
 Keywords: python,framework,pyqt5,frontend,customize,UI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: PyQt5
 
 
 # PyCutee (The PyQt5 Framework) V0.0.1
 
 PyCutee is a lightweight and stylish framework for PyQt5, designed to simplify the creation of modern and visually appealing graphical user interfaces (GUIs) in Python.
 
@@ -69,8 +68,8 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 ## License
 
-PyCutee is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
+PyCutee is licensed under the MIT License. See [LICENSE](https://github.com/CodingRule/PyCutee/blob/main/LICENSE) for more information.
```

### Comparing `pycutee-0.0.3/README.md` & `pycutee-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 ## License
 
-PyCutee is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
+PyCutee is licensed under the MIT License. See [LICENSE](https://github.com/CodingRule/PyCutee/blob/main/LICENSE) for more information.
```

### Comparing `pycutee-0.0.3/setup.py` & `pycutee-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'This app is a lil framework for PyQt5 like bootstrap for HTML5'
 LONG_DESCRIPTION = 'A package that allows to build simple PyQt5 apps faster and cooler.'
 
 # Setting up
 setup(
     name="PyCutee",
     version=VERSION,
```

