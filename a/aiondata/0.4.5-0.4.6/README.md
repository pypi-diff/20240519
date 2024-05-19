# Comparing `tmp/aiondata-0.4.5.tar.gz` & `tmp/aiondata-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiondata-0.4.5.tar", max compression
+gzip compressed data, was "aiondata-0.4.6.tar", max compression
```

## Comparing `aiondata-0.4.5.tar` & `aiondata-0.4.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11372 2024-05-09 07:46:29.806990 aiondata-0.4.5/LICENSE
--rw-r--r--   0        0        0     4606 2024-05-09 07:46:29.806990 aiondata-0.4.5/README.md
--rw-r--r--   0        0        0      419 2024-05-09 07:46:29.806990 aiondata-0.4.5/aiondata/__init__.py
--rw-r--r--   0        0        0     5484 2024-05-09 07:46:29.806990 aiondata-0.4.5/aiondata/bindingdb.py
--rw-r--r--   0        0        0     2118 2024-05-09 07:46:29.806990 aiondata-0.4.5/aiondata/datasets.py
--rw-r--r--   0        0        0     4714 2024-05-09 07:46:29.806990 aiondata-0.4.5/aiondata/moleculenet.py
--rw-r--r--   0        0        0     8692 2024-05-09 07:46:29.806990 aiondata-0.4.5/aiondata/protein_structure.py
--rw-r--r--   0        0        0     5413 2024-05-09 07:46:29.806990 aiondata-0.4.5/aiondata/weizmann_ccca.py
--rw-r--r--   0        0        0     1505 2024-05-09 07:46:29.806990 aiondata-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11372 2024-05-19 13:00:50.817646 aiondata-0.4.6/LICENSE
+-rw-r--r--   0        0        0     4606 2024-05-19 13:00:50.817646 aiondata-0.4.6/README.md
+-rw-r--r--   0        0        0      419 2024-05-19 13:00:50.817646 aiondata-0.4.6/aiondata/__init__.py
+-rw-r--r--   0        0        0     8538 2024-05-19 13:00:50.817646 aiondata-0.4.6/aiondata/bindingdb.py
+-rw-r--r--   0        0        0     2326 2024-05-19 13:00:50.817646 aiondata-0.4.6/aiondata/datasets.py
+-rw-r--r--   0        0        0     4714 2024-05-19 13:00:50.817646 aiondata-0.4.6/aiondata/moleculenet.py
+-rw-r--r--   0        0        0     8692 2024-05-19 13:00:50.821646 aiondata-0.4.6/aiondata/protein_structure.py
+-rw-r--r--   0        0        0     5413 2024-05-19 13:00:50.821646 aiondata-0.4.6/aiondata/weizmann_ccca.py
+-rw-r--r--   0        0        0     1505 2024-05-19 13:00:50.821646 aiondata-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.6/PKG-INFO
```

### Comparing `aiondata-0.4.5/LICENSE` & `aiondata-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.5/README.md` & `aiondata-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.5/aiondata/datasets.py` & `aiondata-0.4.6/aiondata/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,13 @@
         return pl.read_parquet(self.SOURCE)
 
 
 class GeneratedDataset(CachedDataset):
     """A base class for datasets that are generated on-the-fly."""
 
     def get_df(self) -> pl.DataFrame:
-        return pl.DataFrame(self.to_generator())
+        if self.SCHEMA is None:
+            return pl.DataFrame(
+                self.to_generator(), infer_schema_length=25000, strict=False
+            )
+        else:
+            return pl.DataFrame(self.to_generator(), schema=self.SCHEMA, strict=False)
```

### Comparing `aiondata-0.4.5/aiondata/moleculenet.py` & `aiondata-0.4.6/aiondata/moleculenet.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.5/aiondata/protein_structure.py` & `aiondata-0.4.6/aiondata/protein_structure.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.5/aiondata/weizmann_ccca.py` & `aiondata-0.4.6/aiondata/weizmann_ccca.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.5/pyproject.toml` & `aiondata-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiondata"
-version = "0.4.5"
+version = "0.4.6"
 description = "A common data access layer for AI-driven drug discovery."
 authors = ["JJ Ben-Joseph <jj@tensorspace.ai>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://www.github.com/aion-labs/aiondata"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `aiondata-0.4.5/PKG-INFO` & `aiondata-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiondata
-Version: 0.4.5
+Version: 0.4.6
 Summary: A common data access layer for AI-driven drug discovery.
 Home-page: https://www.github.com/aion-labs/aiondata
 License: Apache
 Author: JJ Ben-Joseph
 Author-email: jj@tensorspace.ai
 Requires-Python: >=3.10
 Classifier: Development Status :: 3 - Alpha
```

