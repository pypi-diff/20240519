# Comparing `tmp/higgsml-0.0.1.tar.gz` & `tmp/higgsml-0.0.2.tar.gz`

## Comparing `higgsml-0.0.1.tar` & `higgsml-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.1/HiggsML/__init__.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 higgsml-0.0.1/HiggsML/datasets.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 higgsml-0.0.1/HiggsML/ingestion.py
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.1/HiggsML/score.py
--rw-r--r--   0        0        0    20116 2020-02-02 00:00:00.000000 higgsml-0.0.1/HiggsML/systematics.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.1/HiggsML/visualization.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.1/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 higgsml-0.0.1/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 higgsml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 higgsml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/__init__.py
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/datasets.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/ingestion.py
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/score.py
+-rw-r--r--   0        0        0    20116 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/systematics.py
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/visualization.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.2/LICENSE
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 higgsml-0.0.2/README.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 higgsml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 higgsml-0.0.2/PKG-INFO
```

### Comparing `higgsml-0.0.1/HiggsML/datasets.py` & `higgsml-0.0.2/HiggsML/datasets.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.1/HiggsML/ingestion.py` & `higgsml-0.0.2/HiggsML/ingestion.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.1/HiggsML/score.py` & `higgsml-0.0.2/HiggsML/score.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.1/HiggsML/systematics.py` & `higgsml-0.0.2/HiggsML/systematics.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.1/HiggsML/visualization.py` & `higgsml-0.0.2/HiggsML/visualization.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.1/.gitignore` & `higgsml-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.1/LICENSE` & `higgsml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.1/pyproject.toml` & `higgsml-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [project]
 name = "HiggsML"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Ragansu Chakkappai", email="ragansu@gamil.com" },
+  { name="Ragansu Chakkappai", email="ragansu.chakkappai@universite-paris-saclay.fr"},
+  { name="David Rousseau", email="david.rousseau@uijclab.in2p3.fr" },
+  { name="V. Estrade", email="v.estrade@centralesupelec.fr" },
+  { name="Ihsan Ullah", email="ihsan.ullah@universite-paris-saclay.fr"}
 ]
 description = "A Black Swan test package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

