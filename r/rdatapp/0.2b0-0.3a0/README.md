# Comparing `tmp/rdatapp-0.2b0.tar.gz` & `tmp/rdatapp-0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdatapp-0.2b0.tar", last modified: Sun May 19 00:46:56 2024, max compression
+gzip compressed data, was "rdatapp-0.3a0.tar", last modified: Sun May 19 01:24:21 2024, max compression
```

## Comparing `rdatapp-0.2b0.tar` & `rdatapp-0.3a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 00:46:56.579629 rdatapp-0.2b0/
--rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-19 00:46:56.579460 rdatapp-0.2b0/PKG-INFO
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 00:46:56.578344 rdatapp-0.2b0/data_preprocessing_lib/
--rw-r--r--   0 ifozmen    (501) staff       (20)      771 2024-05-19 00:15:02.000000 rdatapp-0.2b0/data_preprocessing_lib/__init__.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1400 2024-05-18 22:29:37.000000 rdatapp-0.2b0/data_preprocessing_lib/categorical_encoder.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1067 2024-05-18 22:01:35.000000 rdatapp-0.2b0/data_preprocessing_lib/data_type_converter.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1170 2024-05-18 22:04:22.000000 rdatapp-0.2b0/data_preprocessing_lib/datetime_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)      624 2024-05-18 22:04:31.000000 rdatapp-0.2b0/data_preprocessing_lib/feature_engineer.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     2245 2024-05-18 21:48:09.000000 rdatapp-0.2b0/data_preprocessing_lib/missing_value_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)      844 2024-05-18 22:01:04.000000 rdatapp-0.2b0/data_preprocessing_lib/outlier_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1145 2024-05-18 21:56:43.000000 rdatapp-0.2b0/data_preprocessing_lib/scaler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     3436 2024-05-19 00:23:55.000000 rdatapp-0.2b0/data_preprocessing_lib/test.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1212 2024-05-18 21:57:57.000000 rdatapp-0.2b0/data_preprocessing_lib/text_cleaner.py
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 00:46:56.579153 rdatapp-0.2b0/rdatapp.egg-info/
--rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-19 00:46:56.000000 rdatapp-0.2b0/rdatapp.egg-info/PKG-INFO
--rw-r--r--   0 ifozmen    (501) staff       (20)      568 2024-05-19 00:46:56.000000 rdatapp-0.2b0/rdatapp.egg-info/SOURCES.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-19 00:46:56.000000 rdatapp-0.2b0/rdatapp.egg-info/dependency_links.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       31 2024-05-19 00:46:56.000000 rdatapp-0.2b0/rdatapp.egg-info/requires.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       23 2024-05-19 00:46:56.000000 rdatapp-0.2b0/rdatapp.egg-info/top_level.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-19 00:46:56.579688 rdatapp-0.2b0/setup.cfg
--rw-rw-r--   0 ifozmen    (501) staff       (20)      822 2024-05-19 00:46:45.000000 rdatapp-0.2b0/setup.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:24:21.366704 rdatapp-0.3a0/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-19 01:24:21.366584 rdatapp-0.3a0/PKG-INFO
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:24:21.365796 rdatapp-0.3a0/rdatapp/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.3a0/rdatapp/__init__.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1407 2024-05-19 01:08:24.000000 rdatapp-0.3a0/rdatapp/categorical_encoder.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1067 2024-05-18 22:01:35.000000 rdatapp-0.3a0/rdatapp/data_type_converter.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1170 2024-05-18 22:04:22.000000 rdatapp-0.3a0/rdatapp/datetime_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)      624 2024-05-18 22:04:31.000000 rdatapp-0.3a0/rdatapp/feature_engineer.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     2245 2024-05-18 21:48:09.000000 rdatapp-0.3a0/rdatapp/missing_value_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)      844 2024-05-18 22:01:04.000000 rdatapp-0.3a0/rdatapp/outlier_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1145 2024-05-18 21:56:43.000000 rdatapp-0.3a0/rdatapp/scaler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     3436 2024-05-18 22:47:35.000000 rdatapp-0.3a0/rdatapp/test.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1212 2024-05-18 21:57:57.000000 rdatapp-0.3a0/rdatapp/text_cleaner.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:24:21.366412 rdatapp-0.3a0/rdatapp.egg-info/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/PKG-INFO
+-rw-r--r--   0 ifozmen    (501) staff       (20)      418 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/SOURCES.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/dependency_links.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       33 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/requires.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-19 01:24:21.000000 rdatapp-0.3a0/rdatapp.egg-info/top_level.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-19 01:24:21.366752 rdatapp-0.3a0/setup.cfg
+-rw-rw-r--   0 ifozmen    (501) staff       (20)      835 2024-05-19 01:24:12.000000 rdatapp-0.3a0/setup.py
```

### Comparing `rdatapp-0.2b0/PKG-INFO` & `rdatapp-0.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdatapp
-Version: 0.2b0
+Version: 0.3a0
 Summary: A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding and more.
 Home-page: https://github.com/Beegash/Recoded-Data-Processing-Library
 Author: izzettin furkan özmen, ismail cifci
 Author-email: izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/categorical_encoder.py` & `rdatapp-0.3a0/rdatapp/categorical_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         Parameters:
         df (pandas.DataFrame): The DataFrame containing the categorical column.
         column (str): The name of the categorical column to be one-hot encoded.
 
         Returns:
         pandas.DataFrame: The DataFrame with the categorical column one-hot encoded and the original column dropped.
         """
-        encoder = OneHotEncoder(sparse=False)
+        encoder = OneHotEncoder(sparse_output=False)
         encoded = encoder.fit_transform(df[[column]])
         encoded_df = pd.DataFrame(encoded, columns=encoder.get_feature_names_out([column]))
         return pd.concat([df, encoded_df], axis=1).drop(columns=[column])
 
     @staticmethod
     def label_encode(df, column):
         """
```

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/data_type_converter.py` & `rdatapp-0.3a0/rdatapp/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/datetime_handler.py` & `rdatapp-0.3a0/rdatapp/datetime_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/feature_engineer.py` & `rdatapp-0.3a0/rdatapp/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/missing_value_handler.py` & `rdatapp-0.3a0/rdatapp/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/outlier_handler.py` & `rdatapp-0.3a0/rdatapp/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/scaler.py` & `rdatapp-0.3a0/rdatapp/scaler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/test.py` & `rdatapp-0.3a0/rdatapp/test.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.2b0/data_preprocessing_lib/text_cleaner.py` & `rdatapp-0.3a0/rdatapp/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.2b0/rdatapp.egg-info/PKG-INFO` & `rdatapp-0.3a0/rdatapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdatapp
-Version: 0.2b0
+Version: 0.3a0
 Summary: A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding and more.
 Home-page: https://github.com/Beegash/Recoded-Data-Processing-Library
 Author: izzettin furkan özmen, ismail cifci
 Author-email: izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `rdatapp-0.2b0/setup.py` & `rdatapp-0.3a0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rdatapp',
-    version='0.2b',
+    version='0.3a',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
-        'nltk',
+        'nltk'
+        're'
     ],
     description='A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding and more.',
     author='izzettin furkan özmen, ismail cifci',
     author_email='izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr',
     url='https://github.com/Beegash/Recoded-Data-Processing-Library',
     classifiers=[
         'Programming Language :: Python :: 3',
```

