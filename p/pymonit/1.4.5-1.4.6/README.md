# Comparing `tmp/pymonit-1.4.5.tar.gz` & `tmp/pymonit-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.4.5.tar", last modified: Sat May 18 19:09:00 2024, max compression
+gzip compressed data, was "pymonit-1.4.6.tar", last modified: Sat May 18 19:09:55 2024, max compression
```

## Comparing `pymonit-1.4.5.tar` & `pymonit-1.4.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:00.594062 pymonit-1.4.5/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.5/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1811 2024-05-18 19:09:00.594062 pymonit-1.4.5/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1176 2024-05-18 19:08:35.000000 pymonit-1.4.5/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:00.590729 pymonit-1.4.5/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.5/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.5/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.5/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2054 2024-05-18 18:45:14.000000 pymonit-1.4.5/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.5/monit/http.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.5/monit/init.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.5/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.5/monit/logger.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:00.594062 pymonit-1.4.5/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1811 2024-05-18 19:09:00.000000 pymonit-1.4.5/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 19:09:00.000000 pymonit-1.4.5/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 19:09:00.000000 pymonit-1.4.5/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 19:09:00.000000 pymonit-1.4.5/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 19:09:00.000000 pymonit-1.4.5/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 19:09:00.594062 pymonit-1.4.5/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 19:08:56.000000 pymonit-1.4.5/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:55.566207 pymonit-1.4.6/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.6/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1803 2024-05-18 19:09:55.566207 pymonit-1.4.6/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1168 2024-05-18 19:09:33.000000 pymonit-1.4.6/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:55.562874 pymonit-1.4.6/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.6/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.6/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.6/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2054 2024-05-18 18:45:14.000000 pymonit-1.4.6/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.6/monit/http.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.6/monit/init.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.6/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.6/monit/logger.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:55.566207 pymonit-1.4.6/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1803 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 19:09:55.566207 pymonit-1.4.6/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 19:09:51.000000 pymonit-1.4.6/setup.py
```

### Comparing `pymonit-1.4.5/LICENSE` & `pymonit-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.5/PKG-INFO` & `pymonit-1.4.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.5
+Version: 1.4.6
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -63,18 +63,18 @@
 ```Python
 from time import sleep
 
 from monit.core import Monitor as monit
 from monit.logger import Logger
 from monit.log2file import Log2File
 
-def main():
+Log2File() # Salva todo o log em um arquivo
+log = Logger()
 
-    Log2File() # Salva todo o log em um arquivo
-    log = Logger()
+def main():
 
     try:
         log.info("Hello, World!")
 
         sleep(2)
         raise ValueError("This is a sample error.")
```

### Comparing `pymonit-1.4.5/README.md` & `pymonit-1.4.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 ```Python
 from time import sleep
 
 from monit.core import Monitor as monit
 from monit.logger import Logger
 from monit.log2file import Log2File
 
-def main():
+Log2File() # Salva todo o log em um arquivo
+log = Logger()
 
-    Log2File() # Salva todo o log em um arquivo
-    log = Logger()
+def main():
 
     try:
         log.info("Hello, World!")
 
         sleep(2)
         raise ValueError("This is a sample error.")
```

### Comparing `pymonit-1.4.5/monit/config.py` & `pymonit-1.4.6/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.5/monit/core.py` & `pymonit-1.4.6/monit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.5/monit/func.py` & `pymonit-1.4.6/monit/func.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.5/monit/http.py` & `pymonit-1.4.6/monit/http.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.5/monit/log2file.py` & `pymonit-1.4.6/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.5/monit/logger.py` & `pymonit-1.4.6/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.5/pymonit.egg-info/PKG-INFO` & `pymonit-1.4.6/pymonit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.5
+Version: 1.4.6
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -63,18 +63,18 @@
 ```Python
 from time import sleep
 
 from monit.core import Monitor as monit
 from monit.logger import Logger
 from monit.log2file import Log2File
 
-def main():
+Log2File() # Salva todo o log em um arquivo
+log = Logger()
 
-    Log2File() # Salva todo o log em um arquivo
-    log = Logger()
+def main():
 
     try:
         log.info("Hello, World!")
 
         sleep(2)
         raise ValueError("This is a sample error.")
```

### Comparing `pymonit-1.4.5/setup.py` & `pymonit-1.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.4.5',
+    version='1.4.6',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

