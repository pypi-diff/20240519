# Comparing `tmp/origametry-0.0.2.tar.gz` & `tmp/origametry-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "origametry-0.0.2.tar", last modified: Sat May 18 06:04:52 2024, max compression
+gzip compressed data, was "origametry-0.0.3.tar", last modified: Sat May 18 06:31:09 2024, max compression
```

## Comparing `origametry-0.0.2.tar` & `origametry-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 06:04:52.585845 origametry-0.0.2/
--rw-rw-rw-   0        0        0    11558 2024-05-18 05:07:56.000000 origametry-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     7399 2024-05-18 06:04:52.584767 origametry-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6436 2024-05-18 05:07:56.000000 origametry-0.0.2/README.md
--rw-rw-rw-   0        0        0      823 2024-05-18 05:07:56.000000 origametry-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 06:04:52.585845 origametry-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1308 2024-05-18 06:04:37.000000 origametry-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 06:04:52.540152 origametry-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-18 06:04:52.556525 origametry-0.0.2/src/origametry/
--rw-rw-rw-   0        0        0      104 2024-05-18 05:41:39.000000 origametry-0.0.2/src/origametry/__init__.py
--rw-rw-rw-   0        0        0       19 2024-05-18 05:23:32.000000 origametry-0.0.2/src/origametry/constants.py
--rw-rw-rw-   0        0        0    15523 2024-05-18 05:23:32.000000 origametry-0.0.2/src/origametry/fold.py
--rw-rw-rw-   0        0        0     3376 2024-05-18 05:56:07.000000 origametry-0.0.2/src/origametry/helpers.py
--rw-rw-rw-   0        0        0     5613 2024-05-18 05:23:32.000000 origametry-0.0.2/src/origametry/line.py
--rw-rw-rw-   0        0        0      726 2024-05-18 05:23:32.000000 origametry-0.0.2/src/origametry/point.py
--rw-rw-rw-   0        0        0      915 2024-05-18 05:23:32.000000 origametry-0.0.2/src/origametry/reflect.py
-drwxrwxrwx   0        0        0        0 2024-05-18 06:04:52.583594 origametry-0.0.2/src/origametry.egg-info/
--rw-rw-rw-   0        0        0     7399 2024-05-18 06:04:52.000000 origametry-0.0.2/src/origametry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-05-18 06:04:52.000000 origametry-0.0.2/src/origametry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 06:04:52.000000 origametry-0.0.2/src/origametry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 06:04:52.000000 origametry-0.0.2/src/origametry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 06:31:09.514481 origametry-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-18 05:07:56.000000 origametry-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7466 2024-05-18 06:31:09.512390 origametry-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6436 2024-05-18 05:07:56.000000 origametry-0.0.3/README.md
+-rw-rw-rw-   0        0        0      823 2024-05-18 06:29:53.000000 origametry-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 06:31:09.515483 origametry-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2024-05-18 06:30:54.000000 origametry-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 06:31:09.474541 origametry-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 06:31:09.497944 origametry-0.0.3/src/origametry/
+-rw-rw-rw-   0        0        0      104 2024-05-18 05:41:39.000000 origametry-0.0.3/src/origametry/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-05-18 05:23:32.000000 origametry-0.0.3/src/origametry/constants.py
+-rw-rw-rw-   0        0        0    15523 2024-05-18 05:23:32.000000 origametry-0.0.3/src/origametry/fold.py
+-rw-rw-rw-   0        0        0     3376 2024-05-18 05:56:07.000000 origametry-0.0.3/src/origametry/helpers.py
+-rw-rw-rw-   0        0        0     5613 2024-05-18 05:23:32.000000 origametry-0.0.3/src/origametry/line.py
+-rw-rw-rw-   0        0        0      726 2024-05-18 05:23:32.000000 origametry-0.0.3/src/origametry/point.py
+-rw-rw-rw-   0        0        0      915 2024-05-18 05:23:32.000000 origametry-0.0.3/src/origametry/reflect.py
+drwxrwxrwx   0        0        0        0 2024-05-18 06:31:09.511295 origametry-0.0.3/src/origametry.egg-info/
+-rw-rw-rw-   0        0        0     7466 2024-05-18 06:31:09.000000 origametry-0.0.3/src/origametry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-18 06:31:09.000000 origametry-0.0.3/src/origametry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 06:31:09.000000 origametry-0.0.3/src/origametry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 06:31:09.000000 origametry-0.0.3/src/origametry.egg-info/top_level.txt
```

### Comparing `origametry-0.0.2/LICENSE` & `origametry-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `origametry-0.0.2/PKG-INFO` & `origametry-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: origametry
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to perform calculations using the Huzita-Justin axioms for 2-dimensional origami
 Author: Alastair Stanley
+Project-URL: Source, https://github.com/optim-ally/origametry.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `origametry-0.0.2/README.md` & `origametry-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `origametry-0.0.2/pyproject.toml` & `origametry-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `origametry-0.0.2/setup.py` & `origametry-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 
 
 HERE = pathlib.Path(__file__).parent.resolve()
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="origametry",
-    version="0.0.2",
+    version="0.0.3",
     description="Package to perform calculations using the Huzita-Justin axioms for 2-dimensional origami",
     author="Alastair Stanley",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     python_requires=">=3.9.0",
+    project_urls={
+        "Source": "https://github.com/optim-ally/origametry.git",
+    },
     classifiers=[
         # see https://pypi.org/classifiers/
         "Development Status :: 3 - Alpha",
 
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
```

### Comparing `origametry-0.0.2/src/origametry/fold.py` & `origametry-0.0.3/src/origametry/fold.py`

 * *Files identical despite different names*

### Comparing `origametry-0.0.2/src/origametry/helpers.py` & `origametry-0.0.3/src/origametry/helpers.py`

 * *Files identical despite different names*

### Comparing `origametry-0.0.2/src/origametry/line.py` & `origametry-0.0.3/src/origametry/line.py`

 * *Files identical despite different names*

### Comparing `origametry-0.0.2/src/origametry/point.py` & `origametry-0.0.3/src/origametry/point.py`

 * *Files identical despite different names*

### Comparing `origametry-0.0.2/src/origametry/reflect.py` & `origametry-0.0.3/src/origametry/reflect.py`

 * *Files identical despite different names*

### Comparing `origametry-0.0.2/src/origametry.egg-info/PKG-INFO` & `origametry-0.0.3/src/origametry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: origametry
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to perform calculations using the Huzita-Justin axioms for 2-dimensional origami
 Author: Alastair Stanley
+Project-URL: Source, https://github.com/optim-ally/origametry.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
```

