# Comparing `tmp/tap_airtable-0.1.0.dev4.tar.gz` & `tmp/tap_airtable-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_airtable-0.1.0.dev4.tar", max compression
+gzip compressed data, was "tap_airtable-0.1.0.dev5.tar", max compression
```

## Comparing `tap_airtable-0.1.0.dev4.tar` & `tap_airtable-0.1.0.dev5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1093 2024-05-19 20:33:42.816923 tap_airtable-0.1.0.dev4/LICENSE.md
--rw-r--r--   0        0        0     1669 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/README.md
--rw-r--r--   0        0        0     1771 2024-05-19 20:34:10.921060 tap_airtable-0.1.0.dev4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/tap_airtable/__init__.py
--rw-r--r--   0        0        0     3079 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/tap_airtable/client.py
--rw-r--r--   0        0        0     1069 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/tap_airtable/entities.py
--rw-r--r--   0        0        0     1377 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/tap_airtable/streams.py
--rw-r--r--   0        0        0     1684 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/tap_airtable/tap.py
--rw-r--r--   0        0        0       35 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/tap_airtable/tests/__init__.py
--rw-r--r--   0        0        0      112 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/tap_airtable/tests/test_tap.py
--rw-r--r--   0        0        0     2295 2024-05-19 20:33:42.820923 tap_airtable-0.1.0.dev4/tap_airtable/types.py
--rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 tap_airtable-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-05-19 20:39:03.513572 tap_airtable-0.1.0.dev5/LICENSE.md
+-rw-r--r--   0        0        0     1669 2024-05-19 20:39:03.513572 tap_airtable-0.1.0.dev5/README.md
+-rw-r--r--   0        0        0     1771 2024-05-19 20:39:31.777460 tap_airtable-0.1.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 20:39:03.517572 tap_airtable-0.1.0.dev5/tap_airtable/__init__.py
+-rw-r--r--   0        0        0     3079 2024-05-19 20:39:03.517572 tap_airtable-0.1.0.dev5/tap_airtable/client.py
+-rw-r--r--   0        0        0     1069 2024-05-19 20:39:03.517572 tap_airtable-0.1.0.dev5/tap_airtable/entities.py
+-rw-r--r--   0        0        0     1377 2024-05-19 20:39:03.517572 tap_airtable-0.1.0.dev5/tap_airtable/streams.py
+-rw-r--r--   0        0        0     1684 2024-05-19 20:39:03.517572 tap_airtable-0.1.0.dev5/tap_airtable/tap.py
+-rw-r--r--   0        0        0       35 2024-05-19 20:39:03.517572 tap_airtable-0.1.0.dev5/tap_airtable/tests/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-19 20:39:03.517572 tap_airtable-0.1.0.dev5/tap_airtable/tests/test_tap.py
+-rw-r--r--   0        0        0     2295 2024-05-19 20:39:03.517572 tap_airtable-0.1.0.dev5/tap_airtable/types.py
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 tap_airtable-0.1.0.dev5/PKG-INFO
```

### Comparing `tap_airtable-0.1.0.dev4/LICENSE.md` & `tap_airtable-0.1.0.dev5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tap_airtable-0.1.0.dev4/README.md` & `tap_airtable-0.1.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `tap_airtable-0.1.0.dev4/pyproject.toml` & `tap_airtable-0.1.0.dev5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-airtable"
-version = "0.1.0-dev4"
+version = "0.1.0-dev5"
 description = "`tap-airtable` is a Singer tap for Airtable, built with the Meltano SDK for Singer Taps."
 authors = ["Tomas Votava"]
 keywords = ["ELT", "Airtable"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `tap_airtable-0.1.0.dev4/tap_airtable/client.py` & `tap_airtable-0.1.0.dev5/tap_airtable/client.py`

 * *Files identical despite different names*

### Comparing `tap_airtable-0.1.0.dev4/tap_airtable/entities.py` & `tap_airtable-0.1.0.dev5/tap_airtable/entities.py`

 * *Files identical despite different names*

### Comparing `tap_airtable-0.1.0.dev4/tap_airtable/streams.py` & `tap_airtable-0.1.0.dev5/tap_airtable/streams.py`

 * *Files identical despite different names*

### Comparing `tap_airtable-0.1.0.dev4/tap_airtable/tap.py` & `tap_airtable-0.1.0.dev5/tap_airtable/tap.py`

 * *Files identical despite different names*

### Comparing `tap_airtable-0.1.0.dev4/tap_airtable/types.py` & `tap_airtable-0.1.0.dev5/tap_airtable/types.py`

 * *Files identical despite different names*

### Comparing `tap_airtable-0.1.0.dev4/PKG-INFO` & `tap_airtable-0.1.0.dev5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-airtable
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: `tap-airtable` is a Singer tap for Airtable, built with the Meltano SDK for Singer Taps.
 License: Apache 2.0
 Keywords: ELT,Airtable
 Author: Tomas Votava
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

