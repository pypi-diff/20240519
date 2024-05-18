# Comparing `tmp/hamming-sdk-0.0.4.tar.gz` & `tmp/hamming_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamming-sdk-0.0.4.tar", last modified: Wed Mar 27 03:17:19 2024, max compression
+gzip compressed data, was "hamming_sdk-0.0.5.tar", last modified: Sat May 18 23:45:46 2024, max compression
```

## Comparing `hamming-sdk-0.0.4.tar` & `hamming_sdk-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-03-27 03:17:19.685631 hamming-sdk-0.0.4/
--rw-r--r--   0 marius     (501) staff       (20)     1074 2024-02-11 14:45:52.000000 hamming-sdk-0.0.4/LICENSE
--rw-r--r--   0 marius     (501) staff       (20)      988 2024-03-27 03:17:19.685433 hamming-sdk-0.0.4/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)      414 2024-02-19 20:22:09.000000 hamming-sdk-0.0.4/README.md
--rw-r--r--   0 marius     (501) staff       (20)      647 2024-03-27 03:15:20.000000 hamming-sdk-0.0.4/pyproject.toml
--rw-r--r--   0 marius     (501) staff       (20)       38 2024-03-27 03:17:19.685666 hamming-sdk-0.0.4/setup.cfg
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-03-27 03:17:19.681436 hamming-sdk-0.0.4/src/
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-03-27 03:17:19.683259 hamming-sdk-0.0.4/src/hamming/
--rw-r--r--   0 marius     (501) staff       (20)       46 2024-02-13 02:06:22.000000 hamming-sdk-0.0.4/src/hamming/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      879 2024-03-01 03:07:45.000000 hamming-sdk-0.0.4/src/hamming/framework.py
--rw-r--r--   0 marius     (501) staff       (20)     1601 2024-02-15 01:54:38.000000 hamming-sdk-0.0.4/src/hamming/http_client.py
--rw-r--r--   0 marius     (501) staff       (20)     6944 2024-03-01 03:07:45.000000 hamming-sdk-0.0.4/src/hamming/oai.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-03-27 03:17:19.684379 hamming-sdk-0.0.4/src/hamming/resources/
--rw-r--r--   0 marius     (501) staff       (20)      122 2024-03-01 03:07:45.000000 hamming-sdk-0.0.4/src/hamming/resources/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      251 2024-03-01 03:07:45.000000 hamming-sdk-0.0.4/src/hamming/resources/api_resource.py
--rw-r--r--   0 marius     (501) staff       (20)      701 2024-03-01 03:07:45.000000 hamming-sdk-0.0.4/src/hamming/resources/datasets.py
--rw-r--r--   0 marius     (501) staff       (20)     4003 2024-03-01 03:07:45.000000 hamming-sdk-0.0.4/src/hamming/resources/experiments.py
--rw-r--r--   0 marius     (501) staff       (20)     2561 2024-03-27 03:15:06.000000 hamming-sdk-0.0.4/src/hamming/resources/logger.py
--rw-r--r--   0 marius     (501) staff       (20)     4355 2024-03-01 03:07:45.000000 hamming-sdk-0.0.4/src/hamming/resources/monitoring.py
--rw-r--r--   0 marius     (501) staff       (20)     3505 2024-03-27 03:15:06.000000 hamming-sdk-0.0.4/src/hamming/resources/tracing.py
--rw-r--r--   0 marius     (501) staff       (20)     4276 2024-03-01 03:07:45.000000 hamming-sdk-0.0.4/src/hamming/types.py
--rw-r--r--   0 marius     (501) staff       (20)      148 2024-02-14 04:37:24.000000 hamming-sdk-0.0.4/src/hamming/utils.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-03-27 03:17:19.685231 hamming-sdk-0.0.4/src/hamming_sdk.egg-info/
--rw-r--r--   0 marius     (501) staff       (20)      988 2024-03-27 03:17:19.000000 hamming-sdk-0.0.4/src/hamming_sdk.egg-info/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)      607 2024-03-27 03:17:19.000000 hamming-sdk-0.0.4/src/hamming_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 marius     (501) staff       (20)        1 2024-03-27 03:17:19.000000 hamming-sdk-0.0.4/src/hamming_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 marius     (501) staff       (20)       33 2024-03-27 03:17:19.000000 hamming-sdk-0.0.4/src/hamming_sdk.egg-info/requires.txt
--rw-r--r--   0 marius     (501) staff       (20)        8 2024-03-27 03:17:19.000000 hamming-sdk-0.0.4/src/hamming_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.753833 hamming_sdk-0.0.5/
+-rw-r--r--   0 marius     (501) staff       (20)     1074 2024-02-11 14:45:52.000000 hamming_sdk-0.0.5/LICENSE
+-rw-r--r--   0 marius     (501) staff       (20)      988 2024-05-18 23:45:46.753611 hamming_sdk-0.0.5/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)      414 2024-02-19 20:22:09.000000 hamming_sdk-0.0.5/README.md
+-rw-r--r--   0 marius     (501) staff       (20)      647 2024-05-18 23:45:32.000000 hamming_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0 marius     (501) staff       (20)       38 2024-05-18 23:45:46.753871 hamming_sdk-0.0.5/setup.cfg
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.748804 hamming_sdk-0.0.5/src/
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.750967 hamming_sdk-0.0.5/src/hamming/
+-rw-r--r--   0 marius     (501) staff       (20)       46 2024-02-13 02:06:22.000000 hamming_sdk-0.0.5/src/hamming/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      879 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/framework.py
+-rw-r--r--   0 marius     (501) staff       (20)     1601 2024-02-15 01:54:38.000000 hamming_sdk-0.0.5/src/hamming/http_client.py
+-rw-r--r--   0 marius     (501) staff       (20)     6944 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/oai.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.752563 hamming_sdk-0.0.5/src/hamming/resources/
+-rw-r--r--   0 marius     (501) staff       (20)      122 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/resources/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      251 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/resources/api_resource.py
+-rw-r--r--   0 marius     (501) staff       (20)      701 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/resources/datasets.py
+-rw-r--r--   0 marius     (501) staff       (20)     4102 2024-05-18 23:45:32.000000 hamming_sdk-0.0.5/src/hamming/resources/experiments.py
+-rw-r--r--   0 marius     (501) staff       (20)     2561 2024-03-27 03:15:06.000000 hamming_sdk-0.0.5/src/hamming/resources/logger.py
+-rw-r--r--   0 marius     (501) staff       (20)     4355 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/resources/monitoring.py
+-rw-r--r--   0 marius     (501) staff       (20)     3505 2024-03-27 03:15:06.000000 hamming_sdk-0.0.5/src/hamming/resources/tracing.py
+-rw-r--r--   0 marius     (501) staff       (20)     4276 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/types.py
+-rw-r--r--   0 marius     (501) staff       (20)      148 2024-02-14 04:37:24.000000 hamming_sdk-0.0.5/src/hamming/utils.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.753415 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/
+-rw-r--r--   0 marius     (501) staff       (20)      988 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)      607 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 marius     (501) staff       (20)        1 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 marius     (501) staff       (20)       33 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/requires.txt
+-rw-r--r--   0 marius     (501) staff       (20)        8 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/top_level.txt
```

### Comparing `hamming-sdk-0.0.4/LICENSE` & `hamming_sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/PKG-INFO` & `hamming_sdk-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamming-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: SDK for interacting with Hamming AI platform
 Author-email: Hamming <contact@hamming.ai>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hamming-sdk-0.0.4/pyproject.toml` & `hamming_sdk-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hamming-sdk"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Hamming", email="contact@hamming.ai" },
 ]
 description = "SDK for interacting with Hamming AI platform"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `hamming-sdk-0.0.4/src/hamming/framework.py` & `hamming_sdk-0.0.5/src/hamming/framework.py`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/src/hamming/http_client.py` & `hamming_sdk-0.0.5/src/hamming/http_client.py`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/src/hamming/oai.py` & `hamming_sdk-0.0.5/src/hamming/oai.py`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/src/hamming/resources/datasets.py` & `hamming_sdk-0.0.5/src/hamming/resources/datasets.py`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/src/hamming/resources/experiments.py` & `hamming_sdk-0.0.5/src/hamming/resources/experiments.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,19 @@
         duration_sec = (datetime.now() - start_ts).total_seconds()
         duration_ms = int(duration_sec * 1000)
 
         self._client.tracing._flush(item.id)
         self._client.request(
             "PATCH",
             f"/experiments/{item.experimentId}/items/{item.id}",
-            json={"output": output, "metrics": {"durationMs": duration_ms}},
+            json={
+                "output": output,
+                "scores": {}, # TODO: Custom Scores
+                "metrics": {"durationMs": duration_ms},
+            },
         )
 
 
 class Experiments(APIResource):
     _items: ExperimentItems
 
     @staticmethod
```

### Comparing `hamming-sdk-0.0.4/src/hamming/resources/logger.py` & `hamming_sdk-0.0.5/src/hamming/resources/logger.py`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/src/hamming/resources/monitoring.py` & `hamming_sdk-0.0.5/src/hamming/resources/monitoring.py`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/src/hamming/resources/tracing.py` & `hamming_sdk-0.0.5/src/hamming/resources/tracing.py`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/src/hamming/types.py` & `hamming_sdk-0.0.5/src/hamming/types.py`

 * *Files identical despite different names*

### Comparing `hamming-sdk-0.0.4/src/hamming_sdk.egg-info/PKG-INFO` & `hamming_sdk-0.0.5/src/hamming_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamming-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: SDK for interacting with Hamming AI platform
 Author-email: Hamming <contact@hamming.ai>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hamming-sdk-0.0.4/src/hamming_sdk.egg-info/SOURCES.txt` & `hamming_sdk-0.0.5/src/hamming_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

