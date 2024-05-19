# Comparing `tmp/phylokrr-0.4.8.tar.gz` & `tmp/phylokrr-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phylokrr-0.4.8.tar", last modified: Sun Apr 28 06:45:48 2024, max compression
+gzip compressed data, was "dist/phylokrr-0.4.9.tar", last modified: Sun May 19 01:50:59 2024, max compression
```

## Comparing `phylokrr-0.4.8.tar` & `phylokrr-0.4.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 06:45:48.000000 phylokrr-0.4.8/
--rw-r--r--   0 ulises     (502) staff       (20)      204 2024-04-28 06:45:48.000000 phylokrr-0.4.8/PKG-INFO
--rw-r--r--   0 ulises     (502) staff       (20)     3579 2024-04-27 21:04:58.000000 phylokrr-0.4.8/README.md
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 06:45:47.000000 phylokrr-0.4.8/phylokrr.egg-info/
--rw-r--r--   0 ulises     (502) staff       (20)      204 2024-04-28 06:45:47.000000 phylokrr-0.4.8/phylokrr.egg-info/PKG-INFO
--rw-r--r--   0 ulises     (502) staff       (20)      329 2024-04-28 06:45:47.000000 phylokrr-0.4.8/phylokrr.egg-info/SOURCES.txt
--rw-r--r--   0 ulises     (502) staff       (20)        1 2024-04-28 06:45:47.000000 phylokrr-0.4.8/phylokrr.egg-info/dependency_links.txt
--rw-r--r--   0 ulises     (502) staff       (20)        1 2024-04-28 05:30:36.000000 phylokrr-0.4.8/phylokrr.egg-info/not-zip-safe
--rw-r--r--   0 ulises     (502) staff       (20)        6 2024-04-28 06:45:47.000000 phylokrr-0.4.8/phylokrr.egg-info/requires.txt
--rw-r--r--   0 ulises     (502) staff       (20)        9 2024-04-28 06:45:47.000000 phylokrr-0.4.8/phylokrr.egg-info/top_level.txt
--rw-r--r--   0 ulises     (502) staff       (20)       38 2024-04-28 06:45:48.000000 phylokrr-0.4.8/setup.cfg
--rw-r--r--   0 ulises     (502) staff       (20)      656 2024-04-28 06:39:28.000000 phylokrr-0.4.8/setup.py
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 06:45:47.000000 phylokrr-0.4.8/src/
--rw-r--r--   0 ulises     (502) staff       (20)        0 2023-09-27 05:08:48.000000 phylokrr-0.4.8/src/__init__.py
--rw-r--r--   0 ulises     (502) staff       (20)     6916 2024-02-11 02:35:07.000000 phylokrr-0.4.8/src/core.py
--rw-r--r--   0 ulises     (502) staff       (20)     1381 2024-04-28 06:42:39.000000 phylokrr-0.4.8/src/datasets.py
--rw-r--r--   0 ulises     (502) staff       (20)     2650 2024-04-23 23:57:46.000000 phylokrr-0.4.8/src/inspection.py
--rw-r--r--   0 ulises     (502) staff       (20)     7245 2024-04-23 23:30:12.000000 phylokrr-0.4.8/src/kernels.py
--rw-r--r--   0 ulises     (502) staff       (20)      339 2024-02-25 06:38:58.000000 phylokrr-0.4.8/src/metrics.py
--rw-r--r--   0 ulises     (502) staff       (20)    20652 2024-04-23 23:32:36.000000 phylokrr-0.4.8/src/phylosig.py
--rw-r--r--   0 ulises     (502) staff       (20)    16152 2024-04-28 06:39:18.000000 phylokrr-0.4.8/src/utils.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-19 01:50:59.000000 phylokrr-0.4.9/
+-rw-r--r--   0 ulises     (502) staff       (20)      204 2024-05-19 01:50:59.000000 phylokrr-0.4.9/PKG-INFO
+-rw-r--r--   0 ulises     (502) staff       (20)     3913 2024-05-19 01:50:12.000000 phylokrr-0.4.9/README.md
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/
+-rw-r--r--   0 ulises     (502) staff       (20)      204 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/PKG-INFO
+-rw-r--r--   0 ulises     (502) staff       (20)      329 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/SOURCES.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        1 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/dependency_links.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        1 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/not-zip-safe
+-rw-r--r--   0 ulises     (502) staff       (20)        6 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/requires.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        9 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/top_level.txt
+-rw-r--r--   0 ulises     (502) staff       (20)       38 2024-05-19 01:50:59.000000 phylokrr-0.4.9/setup.cfg
+-rw-r--r--   0 ulises     (502) staff       (20)      656 2024-05-19 01:39:58.000000 phylokrr-0.4.9/setup.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-19 01:50:59.000000 phylokrr-0.4.9/src/
+-rw-r--r--   0 ulises     (502) staff       (20)        0 2023-09-27 05:08:48.000000 phylokrr-0.4.9/src/__init__.py
+-rw-r--r--   0 ulises     (502) staff       (20)     6916 2024-02-11 02:35:07.000000 phylokrr-0.4.9/src/core.py
+-rw-r--r--   0 ulises     (502) staff       (20)     1381 2024-04-28 06:42:39.000000 phylokrr-0.4.9/src/datasets.py
+-rw-r--r--   0 ulises     (502) staff       (20)     3106 2024-05-06 19:17:07.000000 phylokrr-0.4.9/src/inspection.py
+-rw-r--r--   0 ulises     (502) staff       (20)     8047 2024-05-19 01:09:11.000000 phylokrr-0.4.9/src/kernels.py
+-rw-r--r--   0 ulises     (502) staff       (20)      339 2024-02-25 06:38:58.000000 phylokrr-0.4.9/src/metrics.py
+-rw-r--r--   0 ulises     (502) staff       (20)    20652 2024-04-23 23:32:36.000000 phylokrr-0.4.9/src/phylosig.py
+-rw-r--r--   0 ulises     (502) staff       (20)    16152 2024-04-28 06:39:18.000000 phylokrr-0.4.9/src/utils.py
```

### Comparing `phylokrr-0.4.8/README.md` & `phylokrr-0.4.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 
 # Installation
 
 ```
 pip install phylokrr
 ```
 
-# Quick overview
+# Notebooks
 
-## Data simulation
+* [Quick Overview](https://colab.research.google.com/drive/1TrQymi-D6B4KCmWciqneMzMDfTEcTSYX?usp=sharing)
+* [Model Inspection](https://colab.research.google.com/drive/1sW67wIf7IH30zpLPe0qo8wlvBOTLYLaU?usp=sharing)
+* [Multi-output Regression](https://colab.research.google.com/drive/1wGNtyyl_0taAgUCktLr1tbTv-nDrgTa0?usp=sharing)
+
+<!-- ## Data simulation
 This simulation is based on a given covariance matrix
 
 
 ```python
 import random
 import numpy as np
 
@@ -117,12 +121,12 @@
 plt.ylabel('y')
 plt.legend()
 ```
 
 <p align="center">
 <img src="https://github.com/Ulises-Rosas/phylokrr/blob/main/data/imgs/phyloKRR_vs_PGLS_cv.png" alt="drawing" width="600px"/>
 </p>
-
+ -->
 
 # Reference
 
 Rosas-Puchuri, U., Santaquiteria, A., Khanmohammadi, S., Solis-Lemus, C., & Betancur-R, R. (2023). [Non-linear phylogenetic regression using regularized kernels](https://www.biorxiv.org/content/10.1101/2023.10.04.560983v1.abstract). bioRxiv, 2023-10.
```

### Comparing `phylokrr-0.4.8/setup.py` & `phylokrr-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "numpy"
 ]
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(name = "phylokrr",
-      version = '0.4.8',
+      version = '0.4.9',
     #   long_description = readme,
     #   long_description_content_type = 'text/markdown',
       packages = ['phylokrr'],
       package_dir = {'phylokrr': 'src'},
       python_requires='>=3.5',
       install_requires = dependencies,
       zip_safe = False,
```

### Comparing `phylokrr-0.4.8/src/core.py` & `phylokrr-0.4.9/src/core.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.8/src/datasets.py` & `phylokrr-0.4.9/src/datasets.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.8/src/inspection.py` & `phylokrr-0.4.9/src/inspection.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,14 +55,22 @@
 
     # np.any(Xpdp == Xq[1])
     return Xq    
 
 def pdp_1d(X, feature, model, quantiles = [0,1], sample = 70, integer = False):
     """
     1D partial dependence plot
+
+    feature: feature index
+    model: model
+    quantiles: quantiles to sample feature values
+    sample: number of samples
+    integer: boolean to indicate if feature is integer
+
+    returns: Xq, pdp_values
     """
 
     Xq = sample_feature(X, feature, quantiles, sample, integer)
     pdp_values = []
     for n in Xq:
         # copy original values
         X_tmp = X.copy()
@@ -79,17 +87,26 @@
     out = np.hstack((
         Xq.reshape(-1,1), 
         np.array(pdp_values).reshape(-1,1)
         ))
     
     return out
 
-def pdp_2d(X, f1_idx, f2_idx, model, quantiles, sample, integer):
+def pdp_2d(X, f1_idx, f2_idx, model, quantiles = [0, 1], sample = 10, integer = [False, False]):
     """
     2D partial dependence plot
+
+    f1_idx: feature 1 index
+    f2_idx: feature 2 index
+    model: model
+    quantiles: quantiles to sample feature values
+    sample: number of samples
+    integer: boolean list to indicate if feature is integer
+
+
     """
 
     Xq1 = sample_feature(X, f1_idx, quantiles, sample, integer[0])
     Xq2 = sample_feature(X, f2_idx, quantiles, sample, integer[1])
 
     n_xq1 = len(Xq1)
     n_xq2 = len(Xq2)
```

### Comparing `phylokrr-0.4.8/src/kernels.py` & `phylokrr-0.4.9/src/kernels.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,30 +28,36 @@
 class WKRR:
     def __init__(self, kernel='rbf', fit_intercept=True, check_cov=False) -> None:
         self.kernel = kernel
 
         if self.kernel == 'rbf':
             self.params = {'gamma': 0.1, 'lambda': 0.1}
 
-        else:
+        elif self.kernel == 'linear':
             self.params = {'c': 0.1, 'lambda': 0.1}
 
+        else:
+            self.params = {'lambda': 0.1}
+
         self.fit_intercept = fit_intercept
         self.check_cov = check_cov
         self.intercept = 0
         self.alpha = np.array([])
         self.X = np.array([])
         self.chol = False
 
     def set_params(self, **params):
         if self.kernel == 'rbf':
             self.params['gamma'] = params['gamma']
-
-        else:
+            
+        elif self.kernel == 'linear':
             self.params['c'] = params['c']
+        
+        else:
+            pass
 
         self.params['lambda'] = params['lambda']
 
     def get_params(self):
         return self.params
 
     def P_mat(self, vcv):
@@ -82,30 +88,39 @@
 
     def fit(self, X, y, vcv=None):
         self.X = X
         P = self.P_mat(vcv)
 
         if self.kernel == 'rbf':
             K_train = RBF_kernel(self.X, self.X, self.params['gamma'])
-        else:
+
+        elif self.kernel == 'linear':
             K_train = linear_kernel(self.X, self.X, self.params['c'])
 
+        else:
+            K_train = self.X
+
+
         self.alpha = self.opt_alpha(K_train, y, self.params['lambda'], P)
 
         if self.fit_intercept:
             self.intercept = np.mean(y - K_train @ self.alpha)
 
     def predict(self, X_test):
         assert len(self.alpha) > 0, "The model needs to be fitted first"
 
         if self.kernel == 'rbf':
             K_test = RBF_kernel(X_test, self.X, self.params['gamma'])
-        else:
+
+        elif self.kernel == 'linear':
             K_test = linear_kernel(X_test, self.X, self.params['c'])
 
+        else:
+            K_test = X_test            
+
         return K_test @ self.alpha + self.intercept
 
     def score(self, X_test, y_test, vcv_test, metric='rmse'):
         y_pred = self.predict(X_test)
 
         if isinstance(vcv_test, type(None)):
             P = np.eye(X_test.shape[0])
@@ -129,41 +144,57 @@
         if isinstance(P, type(None)):
             return np.linalg.solve(K + nlI, y)
         
         else:
             return P @ np.linalg.solve(P @ K @ P + nlI, P @ y)
 
 class KRR(WKRR):
+    """
+    Kernel Ridge Regression
+
+    """
 
     def __init__(self, kernel='rbf', fit_intercept=True) -> None:
+
+        """
+        Initialize the Kernel Ridge Regression model
+        kernel: str, default='rbf'. The kernel to use. Options are 'rbf', 'linear', and 'precomputed'
+                If 'precomputed', the kernel matrix is passed directly.
+        fit_intercept: bool, default=True. Whether to fit an intercept term
+        """
         super().__init__(kernel, fit_intercept)
         self.intercept = 0
         self.alpha = np.array([])
         self.X = np.array([])
 
     def fit(self, X, y):
         self.X = X
         self.y = y
 
         if self.kernel == 'rbf':
             K_train = RBF_kernel(self.X, self.X, self.params['gamma'])
-            
-        else:
+
+        elif self.kernel == 'linear':
             K_train = linear_kernel(self.X, self.X, self.params['c'])
 
+        else:
+            K_train = self.X            
+        
+
         self.alpha = self.opt_alpha(K_train, self.y, self.params['lambda'])
 
         if self.fit_intercept:
             self.intercept = np.mean(y - K_train @ self.alpha)
 
     def opt_alpha(self, K, y, reg_lam=None):
         
         n, _ = self.X.shape
         I = np.eye(K.shape[0])
         nlI = n * reg_lam * I
+        # print(K.shape, nlI.shape, y.shape)
 
         return np.linalg.solve(K + nlI, y)
         
 
     def score(self, X_test, y_test, metric='rmse'):
         y_pred = self.predict(X_test)
```

### Comparing `phylokrr-0.4.8/src/phylosig.py` & `phylokrr-0.4.9/src/phylosig.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.8/src/utils.py` & `phylokrr-0.4.9/src/utils.py`

 * *Files identical despite different names*

