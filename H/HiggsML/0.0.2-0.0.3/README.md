# Comparing `tmp/higgsml-0.0.2.tar.gz` & `tmp/higgsml-0.0.3.tar.gz`

## Comparing `higgsml-0.0.2.tar` & `higgsml-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/__init__.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/datasets.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/ingestion.py
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/score.py
--rw-r--r--   0        0        0    20116 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/systematics.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.2/HiggsML/visualization.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.2/LICENSE
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 higgsml-0.0.2/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 higgsml-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 higgsml-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/__init__.py
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/datasets.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/ingestion.py
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/score.py
+-rw-r--r--   0        0        0    20116 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/systematics.py
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/visualization.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.3/LICENSE
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 higgsml-0.0.3/README.md
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 higgsml-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 higgsml-0.0.3/PKG-INFO
```

### Comparing `higgsml-0.0.2/HiggsML/datasets.py` & `higgsml-0.0.3/HiggsML/datasets.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.2/HiggsML/ingestion.py` & `higgsml-0.0.3/HiggsML/ingestion.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.2/HiggsML/score.py` & `higgsml-0.0.3/HiggsML/score.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.2/HiggsML/systematics.py` & `higgsml-0.0.3/HiggsML/systematics.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.2/HiggsML/visualization.py` & `higgsml-0.0.3/HiggsML/visualization.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.2/.gitignore` & `higgsml-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.2/LICENSE` & `higgsml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.2/pyproject.toml` & `higgsml-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HiggsML"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ragansu Chakkappai", email="ragansu.chakkappai@universite-paris-saclay.fr"},
   { name="David Rousseau", email="david.rousseau@uijclab.in2p3.fr" },
   { name="V. Estrade", email="v.estrade@centralesupelec.fr" },
   { name="Ihsan Ullah", email="ihsan.ullah@universite-paris-saclay.fr"}
 ]
 description = "A Black Swan test package"
@@ -18,27 +18,29 @@
 dependencies = [
     "numpy",
     "pandas",
     "scikit-learn",
     "matplotlib",
     "seaborn",
     "frozendict",
+    "pyarrow",
     "setuptools"
 ]
 install_requires=["numpy>=1.26.4",
                   "sklearn>=1.4.2",
                   "pandas>=2.2.2",
                   "matplotlib>=3.8.0",
                   "seaborn>=0.13.1",
                   "frozendict>=2.4.4",
+                  "pyarrow>=15.0.0",
                   "setuptools>=58.2.0"
                   ]
 
 
 
 [build-system]
-requires = ["hatchling", "numpy", "pandas", "scikit-learn", "matplotlib", "seaborn","frozendict","setuptools"]
+requires = ["hatchling", "numpy", "pandas", "scikit-learn", "matplotlib", "seaborn", "frozendict", "pyarrow", "setuptools"]
 build-backend = "hatchling.build"
 
 [project.urls]
 Homepage = "https://github.com/blackSwanCS/black_swan_pkg"
 Issues = "https://github.com/blackSwanCS/black_swan_pkg/issues"
```

### Comparing `higgsml-0.0.2/PKG-INFO` & `higgsml-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: HiggsML
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Black Swan test package
 Project-URL: Homepage, https://github.com/blackSwanCS/black_swan_pkg
 Project-URL: Issues, https://github.com/blackSwanCS/black_swan_pkg/issues
 Author-email: Ragansu Chakkappai <ragansu.chakkappai@universite-paris-saclay.fr>, David Rousseau <david.rousseau@uijclab.in2p3.fr>, "V. Estrade" <v.estrade@centralesupelec.fr>, Ihsan Ullah <ihsan.ullah@universite-paris-saclay.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: frozendict
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: pyarrow
 Requires-Dist: scikit-learn
 Requires-Dist: seaborn
 Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 # HiggsML BlackSwan Package
```

