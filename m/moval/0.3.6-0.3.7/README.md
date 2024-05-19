# Comparing `tmp/moval-0.3.6.tar.gz` & `tmp/moval-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-r02e0gw1/moval-0.3.6.tar", last modified: Thu May 16 14:35:32 2024, max compression
+gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-bbbrcw60/moval-0.3.7.tar", last modified: Sun May 19 15:24:16 2024, max compression
```

## Comparing `moval-0.3.6.tar` & `moval-0.3.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.533845 moval-0.3.6/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-05-16 14:35:32.533788 moval-0.3.6/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.6/README.md
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.527877 moval-0.3.6/moval/
--rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-05-16 14:34:58.000000 moval-0.3.6/moval/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.529120 moval-0.3.6/moval/integrations/
--rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.6/moval/integrations/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.529737 moval-0.3.6/moval/integrations/sklearn/
--rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.6/moval/integrations/sklearn/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    41330 2024-05-16 14:33:33.000000 moval-0.3.6/moval/integrations/sklearn/moval.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.531831 moval-0.3.6/moval/models/
--rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.6/moval/models/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.6/moval/models/confidences.py
--rw-r--r--   0 zejuli     (501) staff       (20)    44866 2024-04-21 15:22:16.000000 moval-0.3.6/moval/models/model.py
--rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.6/moval/models/solver_temperature.py
--rw-r--r--   0 zejuli     (501) staff       (20)    10804 2024-04-20 02:13:02.000000 moval-0.3.6/moval/models/utils.py
--rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.6/moval/registry.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.533244 moval-0.3.6/moval/solvers/
--rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.6/moval/solvers/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.6/moval/solvers/criterions.py
--rw-r--r--   0 zejuli     (501) staff       (20)    28881 2024-05-16 14:34:21.000000 moval-0.3.6/moval/solvers/solver.py
--rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.6/moval/solvers/utils.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.533545 moval-0.3.6/moval.egg-info/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/SOURCES.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/dependency_links.txt
--rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/requires.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/top_level.txt
--rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.6/pyproject.toml
--rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-05-16 14:35:32.534187 moval-0.3.6/setup.cfg
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-19 15:24:16.696199 moval-0.3.7/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-05-19 15:24:16.696125 moval-0.3.7/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.7/README.md
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-19 15:24:16.692751 moval-0.3.7/moval/
+-rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-05-19 15:23:21.000000 moval-0.3.7/moval/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-19 15:24:16.693649 moval-0.3.7/moval/integrations/
+-rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.7/moval/integrations/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-19 15:24:16.693962 moval-0.3.7/moval/integrations/sklearn/
+-rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.7/moval/integrations/sklearn/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    41330 2024-05-19 15:16:21.000000 moval-0.3.7/moval/integrations/sklearn/moval.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-19 15:24:16.694932 moval-0.3.7/moval/models/
+-rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.7/moval/models/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.7/moval/models/confidences.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    44866 2024-04-21 15:22:16.000000 moval-0.3.7/moval/models/model.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.7/moval/models/solver_temperature.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    10828 2024-05-19 14:24:05.000000 moval-0.3.7/moval/models/utils.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.7/moval/registry.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-19 15:24:16.695690 moval-0.3.7/moval/solvers/
+-rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.7/moval/solvers/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.7/moval/solvers/criterions.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    29073 2024-05-19 15:20:02.000000 moval-0.3.7/moval/solvers/solver.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.7/moval/solvers/utils.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-19 15:24:16.695886 moval-0.3.7/moval.egg-info/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-05-19 15:24:16.000000 moval-0.3.7/moval.egg-info/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-05-19 15:24:16.000000 moval-0.3.7/moval.egg-info/SOURCES.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-05-19 15:24:16.000000 moval-0.3.7/moval.egg-info/dependency_links.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-05-19 15:24:16.000000 moval-0.3.7/moval.egg-info/requires.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-05-19 15:24:16.000000 moval-0.3.7/moval.egg-info/top_level.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.7/pyproject.toml
+-rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-05-19 15:24:16.696535 moval-0.3.7/setup.cfg
```

### Comparing `moval-0.3.6/PKG-INFO` & `moval-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.6
+Version: 0.3.7
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.6 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.7 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.6/README.md` & `moval-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/moval/__init__.py` & `moval-0.3.7/moval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from moval.integrations.sklearn.moval import MOVAL
 except ImportError as e:
     # silently fail for now
     pass
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 __all__ = ["MOVAL"]
 
 def __getattr__(key):
     """Lazy import of moval submodules and -packages.
 
     Once :py:mod:`moval` is imported, it is possible to lazy import
```

### Comparing `moval-0.3.6/moval/integrations/sklearn/moval.py` & `moval-0.3.7/moval/integrations/sklearn/moval.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/moval/models/confidences.py` & `moval-0.3.7/moval/models/confidences.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/moval/models/model.py` & `moval-0.3.7/moval/models/model.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/moval/models/solver_temperature.py` & `moval-0.3.7/moval/models/solver_temperature.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/moval/models/utils.py` & `moval-0.3.7/moval/models/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     """Calculation of soft sensitivity.
 
     Args:
         x: The predicted probability of shape ``(n, d, (H), (W), (D))``.
         y: The manual label of shape ``(n, (H), (W), (D))``.
     
     Returns:
-        dice_score: Average class-wise dice of shape ``(d, )``
+        sensitivity_score: Average class-wise sensitivity of shape ``(d, )``
 
     """
     assert len(x.shape) == len(y.shape) + 1
 
     shp_x = x.shape
     square = False
 
@@ -196,15 +196,15 @@
     """Calculation of soft precision score.
 
     Args:
         x: The predicted probability of shape ``(n, d, (H), (W), (D))``.
         y: The manual label of shape ``(n, (H), (W), (D))``.
     
     Returns:
-        dice_score: Average class-wise dice of shape ``(d, )``
+        precision_score: Average class-wise precision of shape ``(d, )``
 
     """
     assert len(x.shape) == len(y.shape) + 1
 
     shp_x = x.shape
     square = False
```

### Comparing `moval-0.3.6/moval/registry.py` & `moval-0.3.7/moval/registry.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/moval/solvers/criterions.py` & `moval-0.3.7/moval/solvers/criterions.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/moval/solvers/solver.py` & `moval-0.3.7/moval/solvers/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         """Generate a list of kcls, such that the predicted samples are in descending order.
 
         Args:
             inp: The network output (logits) of shape ``(n, d)`` for classification and a list of n ``(d, H, W, (D))`` for segmentation. 
             exclusive_background: If ``False``, we exclude the background class (the most majority class).
         
         Return:
-            kcls_list: a list of class index. The first element should correspond to the most minority class.
+            kcls_list: a list of class index. The first element should correspond to the most major class.
 
         """
         kcls_sample = np.zeros(self.opt_class)
         if self.model.mode == "classification":
             pred = np.argmax(inp, axis = 1)
             for opt_kcls in range(self.opt_class):
                 for kcls in range(self.batch * opt_kcls, np.min((self.batch * (opt_kcls + 1), self.model.num_class))):
@@ -256,14 +256,17 @@
             print(f"Opitimizing with {len(inp)} samples...")
             print("Be patient, it should take a while...")
             if self.metric != "accuracy":
                 exclusive_background = True # leave the background class uncalibrated.
 
         # generate a list of length kcls, from high to low
         kcls_list = self.kcls_order_list(self.inp, exclusive_background)
+        if self.metric == "auc" or self.metric == "precision":
+            # these two largely depends on FP, threfore we optimize from the minority class
+            kcls_list = kcls_list[::-1]
 
         if self.class_specific:
             
             if self.model.mode == "classification":
                 pred = np.argmax(inp, axis = 1)
             else:
                 preds = []
```

### Comparing `moval-0.3.6/moval/solvers/utils.py` & `moval-0.3.7/moval/solvers/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/moval.egg-info/PKG-INFO` & `moval-0.3.7/moval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.6
+Version: 0.3.7
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.6 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.7 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.6/moval.egg-info/SOURCES.txt` & `moval-0.3.7/moval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/pyproject.toml` & `moval-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moval-0.3.6/setup.cfg` & `moval-0.3.7/setup.cfg`

 * *Files identical despite different names*

