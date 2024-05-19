# Comparing `tmp/rdatapp-0.3a0.tar.gz` & `tmp/rdatapp-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdatapp-0.3a0.tar", last modified: Sun May 19 01:24:21 2024, max compression
+gzip compressed data, was "rdatapp-0.4.tar", last modified: Sun May 19 01:37:46 2024, max compression
```

## Comparing `rdatapp-0.3a0.tar` & `rdatapp-0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:24:21.366704 rdatapp-0.3a0/
--rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-19 01:24:21.366584 rdatapp-0.3a0/PKG-INFO
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:24:21.365796 rdatapp-0.3a0/rdatapp/
--rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.3a0/rdatapp/__init__.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1407 2024-05-19 01:08:24.000000 rdatapp-0.3a0/rdatapp/categorical_encoder.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1067 2024-05-18 22:01:35.000000 rdatapp-0.3a0/rdatapp/data_type_converter.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1170 2024-05-18 22:04:22.000000 rdatapp-0.3a0/rdatapp/datetime_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)      624 2024-05-18 22:04:31.000000 rdatapp-0.3a0/rdatapp/feature_engineer.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     2245 2024-05-18 21:48:09.000000 rdatapp-0.3a0/rdatapp/missing_value_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)      844 2024-05-18 22:01:04.000000 rdatapp-0.3a0/rdatapp/outlier_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1145 2024-05-18 21:56:43.000000 rdatapp-0.3a0/rdatapp/scaler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     3436 2024-05-18 22:47:35.000000 rdatapp-0.3a0/rdatapp/test.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1212 2024-05-18 21:57:57.000000 rdatapp-0.3a0/rdatapp/text_cleaner.py
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:24:21.366412 rdatapp-0.3a0/rdatapp.egg-info/
--rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/PKG-INFO
--rw-r--r--   0 ifozmen    (501) staff       (20)      418 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/SOURCES.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/dependency_links.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       33 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/requires.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/top_level.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-19 01:24:21.366752 rdatapp-0.3a0/setup.cfg
--rw-rw-r--   0 ifozmen    (501) staff       (20)      835 2024-05-19 01:24:12.000000 rdatapp-0.3a0/setup.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:37:46.990837 rdatapp-0.4/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      569 2024-05-19 01:37:46.990717 rdatapp-0.4/PKG-INFO
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:37:46.989793 rdatapp-0.4/rdatapp/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.4/rdatapp/__init__.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1407 2024-05-19 01:08:24.000000 rdatapp-0.4/rdatapp/categorical_encoder.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1067 2024-05-18 22:01:35.000000 rdatapp-0.4/rdatapp/data_type_converter.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1170 2024-05-18 22:04:22.000000 rdatapp-0.4/rdatapp/datetime_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)      624 2024-05-18 22:04:31.000000 rdatapp-0.4/rdatapp/feature_engineer.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     2245 2024-05-18 21:48:09.000000 rdatapp-0.4/rdatapp/missing_value_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)      844 2024-05-18 22:01:04.000000 rdatapp-0.4/rdatapp/outlier_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1145 2024-05-18 21:56:43.000000 rdatapp-0.4/rdatapp/scaler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     3316 2024-05-19 01:24:37.000000 rdatapp-0.4/rdatapp/test.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1212 2024-05-18 21:57:57.000000 rdatapp-0.4/rdatapp/text_cleaner.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:37:46.990532 rdatapp-0.4/rdatapp.egg-info/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      569 2024-05-19 01:37:46.000000 rdatapp-0.4/rdatapp.egg-info/PKG-INFO
+-rw-r--r--   0 ifozmen    (501) staff       (20)      418 2024-05-19 01:37:46.000000 rdatapp-0.4/rdatapp.egg-info/SOURCES.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-19 01:37:46.000000 rdatapp-0.4/rdatapp.egg-info/dependency_links.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       34 2024-05-19 01:37:46.000000 rdatapp-0.4/rdatapp.egg-info/requires.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-19 01:37:46.000000 rdatapp-0.4/rdatapp.egg-info/top_level.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-19 01:37:46.990884 rdatapp-0.4/setup.cfg
+-rw-rw-r--   0 ifozmen    (501) staff       (20)      835 2024-05-19 01:37:30.000000 rdatapp-0.4/setup.py
```

### Comparing `rdatapp-0.3a0/PKG-INFO` & `rdatapp-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdatapp
-Version: 0.3a0
+Version: 0.4
 Summary: A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding and more.
 Home-page: https://github.com/Beegash/Recoded-Data-Processing-Library
 Author: izzettin furkan özmen, ismail cifci
 Author-email: izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `rdatapp-0.3a0/rdatapp/__init__.py` & `rdatapp-0.4/rdatapp/__init__.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp/categorical_encoder.py` & `rdatapp-0.4/rdatapp/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp/data_type_converter.py` & `rdatapp-0.4/rdatapp/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp/datetime_handler.py` & `rdatapp-0.4/rdatapp/datetime_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp/feature_engineer.py` & `rdatapp-0.4/rdatapp/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp/missing_value_handler.py` & `rdatapp-0.4/rdatapp/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp/outlier_handler.py` & `rdatapp-0.4/rdatapp/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp/scaler.py` & `rdatapp-0.4/rdatapp/scaler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp/test.py` & `rdatapp-0.4/rdatapp/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import data_preprocessing_lib.__init__ as dpl
+import rdatapp.__init__ as dpl
 import pandas as pd
 
 df = pd.DataFrame({'A': [1, 2, None, 4, 5]})
 print(df)
 dpl.MissingValueHandler.impute_mean(df, 'A')
 print(df)
 
 if __name__ == '__main__':
     import unittest
     unittest.main()
 import pandas as pd
-from data_preprocessing_lib.categorical_encoder import CategoricalEncoder
-from data_preprocessing_lib.data_type_converter import DataTypeConverter
-from data_preprocessing_lib.datetime_handler import DateTimeHandler
-from data_preprocessing_lib.feature_engineer import FeatureEngineer
-from data_preprocessing_lib.outlier_handler import OutlierHandler
-from data_preprocessing_lib.scaler import Scaler
-from data_preprocessing_lib.text_cleaner import TextCleaner
+from rdatapp.categorical_encoder import CategoricalEncoder
+from rdatapp.data_type_converter import DataTypeConverter
+from rdatapp.datetime_handler import DateTimeHandler
+from rdatapp.feature_engineer import FeatureEngineer
+from rdatapp.outlier_handler import OutlierHandler
+from rdatapp.scaler import Scaler
+from rdatapp.text_cleaner import TextCleaner
 
 class TestDataPreprocessing(unittest.TestCase):
     def setUp(self):
         # Set up any necessary data or objects for your tests
         pass
 
     def tearDown(self):
```

### Comparing `rdatapp-0.3a0/rdatapp/text_cleaner.py` & `rdatapp-0.4/rdatapp/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.3a0/rdatapp.egg-info/PKG-INFO` & `rdatapp-0.4/rdatapp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdatapp
-Version: 0.3a0
+Version: 0.4
 Summary: A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding and more.
 Home-page: https://github.com/Beegash/Recoded-Data-Processing-Library
 Author: izzettin furkan özmen, ismail cifci
 Author-email: izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `rdatapp-0.3a0/setup.py` & `rdatapp-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rdatapp',
-    version='0.3a',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
-        'nltk'
+        'nltk',
         're'
     ],
     description='A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding and more.',
     author='izzettin furkan özmen, ismail cifci',
     author_email='izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr',
     url='https://github.com/Beegash/Recoded-Data-Processing-Library',
     classifiers=[
```

