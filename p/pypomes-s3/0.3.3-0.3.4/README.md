# Comparing `tmp/pypomes_s3-0.3.3.tar.gz` & `tmp/pypomes_s3-0.3.4.tar.gz`

## Comparing `pypomes_s3-0.3.3.tar` & `pypomes_s3-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/__init__.py
--rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/aws_pomes.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/minio_client.py
--rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/minio_pomes.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/s3_common.py
--rw-r--r--   0        0        0    27222 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/s3_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/__init__.py
+-rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/aws_pomes.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/minio_client.py
+-rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/minio_pomes.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/s3_common.py
+-rw-r--r--   0        0        0    27222 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/s3_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/PKG-INFO
```

### Comparing `pypomes_s3-0.3.3/src/pypomes_s3/__init__.py` & `pypomes_s3-0.3.4/src/pypomes_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.3/src/pypomes_s3/aws_pomes.py` & `pypomes_s3-0.3.4/src/pypomes_s3/aws_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.3/src/pypomes_s3/minio_client.py` & `pypomes_s3-0.3.4/src/pypomes_s3/minio_client.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.3/src/pypomes_s3/minio_pomes.py` & `pypomes_s3-0.3.4/src/pypomes_s3/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.3/src/pypomes_s3/s3_common.py` & `pypomes_s3-0.3.4/src/pypomes_s3/s3_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.3/src/pypomes_s3/s3_pomes.py` & `pypomes_s3-0.3.4/src/pypomes_s3/s3_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.3/LICENSE` & `pypomes_s3-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.3/pyproject.toml` & `pypomes_s3-0.3.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_s3"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (S3 storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "boto3>=1.34.108",
-    "minio>=7.2.7",
+    # "boto3>=1.34.108",
+    # "minio>=7.2.7",
     "pip>=24.0",
     "pypomes_core>=1.0.4",
     "setuptools>=68.0.0",
     "Unidecode>=1.3.6",
     "wheel>=0.42.0"
 ]
```

### Comparing `pypomes_s3-0.3.3/PKG-INFO` & `pypomes_s3-0.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.3
 Name: pypomes_s3
-Version: 0.3.3
+Version: 0.3.4
 Summary: A collection of Python pomes, pennyeach (S3 storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-S3
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-S3/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: boto3>=1.34.108
-Requires-Dist: minio>=7.2.7
 Requires-Dist: pip>=24.0
 Requires-Dist: pypomes-core>=1.0.4
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: wheel>=0.42.0
```

