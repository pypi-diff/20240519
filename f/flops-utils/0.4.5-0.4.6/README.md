# Comparing `tmp/flops_utils-0.4.5.tar.gz` & `tmp/flops_utils-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.4.5.tar", max compression
+gzip compressed data, was "flops_utils-0.4.6.tar", max compression
```

## Comparing `flops_utils-0.4.5.tar` & `flops_utils-0.4.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.5/README.md
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.5/flops_utils/logging.py
--rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.4.5/flops_utils/ml_model_flavor_wrapper.py
--rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.5/flops_utils/ml_repo_files_wrapper.py
--rw-r--r--   0        0        0     2639 2024-05-19 14:20:58.424779 flops_utils-0.4.5/flops_utils/ml_repo_templates.py
--rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.5/flops_utils/notifications.py
--rw-r--r--   0        0        0     2413 2024-05-12 07:37:56.424182 flops_utils-0.4.5/flops_utils/timer.py
--rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.5/flops_utils/types.py
--rw-r--r--   0        0        0      457 2024-05-19 14:21:18.724780 flops_utils-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.6/README.md
+-rw-r--r--   0        0        0      880 2024-05-19 15:58:32.700947 flops_utils-0.4.6/flops_utils/flops_learner_files_wrapper.py
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.6/flops_utils/logging.py
+-rw-r--r--   0        0        0      782 2024-05-19 15:58:54.496948 flops_utils-0.4.6/flops_utils/ml_model_flavor_wrapper.py
+-rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.6/flops_utils/ml_repo_files_wrapper.py
+-rw-r--r--   0        0        0     2603 2024-05-19 15:47:46.596928 flops_utils-0.4.6/flops_utils/ml_repo_templates.py
+-rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.6/flops_utils/notifications.py
+-rw-r--r--   0        0        0     2413 2024-05-12 07:37:56.424182 flops_utils-0.4.6/flops_utils/timer.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.6/flops_utils/types.py
+-rw-r--r--   0        0        0      457 2024-05-19 15:58:58.116948 flops_utils-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.4.6/PKG-INFO
```

### Comparing `flops_utils-0.4.5/flops_utils/logging.py` & `flops_utils-0.4.6/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.5/flops_utils/ml_model_flavor_wrapper.py` & `flops_utils-0.4.6/flops_utils/ml_model_flavor_wrapper.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.5/flops_utils/ml_repo_templates.py` & `flops_utils-0.4.6/flops_utils/ml_repo_templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from abc import ABC, abstractmethod
 from typing import Any, Tuple
 
 
-class LearnerDataManagerTemplate(ABC):
+class DataManagerTemplate(ABC):
 
     @abstractmethod
     def get_data(self) -> Tuple[Any, Any]:
-        """Gets the necessary data for training and evaluation.
+        """Get the necessary data for training and evaluation.
+        This data has already been prepared/preprocessed.
 
         Examples:
         - self.training_data, self.testing_data
-          which were set in the init like this: tf.keras.datasets.cifar10.load_data()
         """
 
 
 class ModelManagerTemplate(ABC):
 
     @abstractmethod
     def prepare_data(self) -> None:
-        """Gets the date from the DataManager and makes it available to the model.
+        """Gets the data from the DataManager and makes it available to the model.
         Make sure to now prepare the data in the ModelManager init function.
         This will avoid the aggregator from trying and fetch the data too.
         Data fetching is reserved for Learners.
 
         Heavily depends on the underlying model and ML library.
 
         Will be called by FLOps.
```

### Comparing `flops_utils-0.4.5/flops_utils/notifications.py` & `flops_utils-0.4.6/flops_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.5/flops_utils/timer.py` & `flops_utils-0.4.6/flops_utils/timer.py`

 * *Files identical despite different names*

