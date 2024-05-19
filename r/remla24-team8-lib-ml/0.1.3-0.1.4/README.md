# Comparing `tmp/remla24_team8_lib_ml-0.1.3.tar.gz` & `tmp/remla24_team8_lib_ml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla24_team8_lib_ml-0.1.3.tar", max compression
+gzip compressed data, was "remla24_team8_lib_ml-0.1.4.tar", max compression
```

## Comparing `remla24_team8_lib_ml-0.1.3.tar` & `remla24_team8_lib_ml-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1544 2024-05-15 17:17:48.345610 remla24_team8_lib_ml-0.1.3/README.md
--rw-r--r--   0        0        0      724 2024-05-15 17:17:48.345610 remla24_team8_lib_ml-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 17:17:48.345610 remla24_team8_lib_ml-0.1.3/src/lib_ml/__init__.py
--rw-r--r--   0        0        0     4307 2024-05-15 17:17:48.345610 remla24_team8_lib_ml-0.1.3/src/lib_ml/process_data.py
--rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 remla24_team8_lib_ml-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1544 2024-05-19 10:44:13.229499 remla24_team8_lib_ml-0.1.4/README.md
+-rw-r--r--   0        0        0      740 2024-05-19 10:44:13.229499 remla24_team8_lib_ml-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 10:44:13.229499 remla24_team8_lib_ml-0.1.4/src/lib_ml/__init__.py
+-rw-r--r--   0        0        0     4483 2024-05-19 10:44:13.229499 remla24_team8_lib_ml-0.1.4/src/lib_ml/process_data.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 remla24_team8_lib_ml-0.1.4/PKG-INFO
```

### Comparing `remla24_team8_lib_ml-0.1.3/README.md` & `remla24_team8_lib_ml-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `remla24_team8_lib_ml-0.1.3/pyproject.toml` & `remla24_team8_lib_ml-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remla24-team8-lib-ml"
-version = "0.1.3"
+version = "0.1.4"
 description = "Pre-processing logic used for both model-training and model-service."
 authors = [
     "Tip ten Brink <T.M.tenBrink@student.tudelft.nl>", 
     "Felipe Bononi Bello <bello2001felipe@gmail.com>", 
     "Dielof van Loon <d.i.vanloon@student.tudelft.nl>", 
     "Sayf El Kaddouri <sayfgmaul@gmail.com>"
 ]
@@ -15,14 +15,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pandas = "^2.2.2"
 joblib = "^1.4.2"
 scikit-learn = "^1.4.2"
 tensorflow = "^2.16.1"
+gdown = "4.5.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 
 
 [build-system]
```

### Comparing `remla24_team8_lib_ml-0.1.3/src/lib_ml/process_data.py` & `remla24_team8_lib_ml-0.1.4/src/lib_ml/process_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 """This module contains the DataProcessor class for processing data for the model."""
 
 import pandas as pd
 from tensorflow.keras.preprocessing.text import Tokenizer
 from tensorflow.keras.preprocessing.sequence import pad_sequences
 from sklearn.preprocessing import LabelEncoder
 import joblib
-
+import gdown
 
 class DataProcessor:
     """
     Class to process data for the model
 
     """
-    def __init__(self, token_path=None, enc_path=None, sequence_length=200):
+    def __init__(self, tokenizer_url=None, enc_path=None, sequence_length=200):
         self.sequence_length = sequence_length
 
         if enc_path:
             self.encoder = joblib.load(enc_path)
         else:
             self.encoder = LabelEncoder()
 
-        if token_path:
-            self.tokenizer = joblib.load(token_path)
+        if tokenizer_url:
+            
+            gdown.download_folder(tokenizer_url, output="tokenizer")
+
+            tokenizer_path = "tokenizer/tokenizer.joblib"
+            self.tokenizer = joblib.load(tokenizer_path)
+            
         else:
             self.tokenizer = Tokenizer(char_level=True,lower=True, oov_token = '-n-')
 
 
     @staticmethod
     def raw_to_df(content):
         """
```

### Comparing `remla24_team8_lib_ml-0.1.3/PKG-INFO` & `remla24_team8_lib_ml-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: remla24-team8-lib-ml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pre-processing logic used for both model-training and model-service.
 Author: Tip ten Brink
 Author-email: T.M.tenBrink@student.tudelft.nl
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: gdown (==4.5.1)
 Requires-Dist: joblib (>=1.4.2,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: tensorflow (>=2.16.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # lib-ml
```

