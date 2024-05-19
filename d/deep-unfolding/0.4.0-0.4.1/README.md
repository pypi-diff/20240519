# Comparing `tmp/deep_unfolding-0.4.0.tar.gz` & `tmp/deep_unfolding-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_unfolding-0.4.0.tar", last modified: Sun May 19 19:50:36 2024, max compression
+gzip compressed data, was "deep_unfolding-0.4.1.tar", last modified: Sun May 19 21:18:59 2024, max compression
```

## Comparing `deep_unfolding-0.4.0.tar` & `deep_unfolding-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:36.774307 deep_unfolding-0.4.0/
--rw-rw-rw-   0        0        0    35823 2024-05-16 09:14:53.000000 deep_unfolding-0.4.0/LICENSE
--rw-rw-rw-   0        0        0        0 2024-05-19 19:26:15.000000 deep_unfolding-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3595 2024-05-19 19:50:36.773297 deep_unfolding-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2024-05-16 09:14:53.000000 deep_unfolding-0.4.0/README.md
--rw-rw-rw-   0        0        0       82 2024-05-19 19:48:27.000000 deep_unfolding-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1070 2024-05-19 19:50:36.777846 deep_unfolding-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:36.728334 deep_unfolding-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:36.771648 deep_unfolding-0.4.0/src/deep_unfolding.egg-info/
--rw-rw-rw-   0        0        0     3595 2024-05-19 19:50:36.000000 deep_unfolding-0.4.0/src/deep_unfolding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-19 19:50:36.000000 deep_unfolding-0.4.0/src/deep_unfolding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:50:36.000000 deep_unfolding-0.4.0/src/deep_unfolding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-19 19:50:36.000000 deep_unfolding-0.4.0/src/deep_unfolding.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:50:36.000000 deep_unfolding-0.4.0/src/deep_unfolding.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:36.769397 deep_unfolding-0.4.0/tests/
--rw-rw-rw-   0        0        0     2374 2024-05-16 09:14:53.000000 deep_unfolding-0.4.0/tests/testNet.py
--rw-rw-rw-   0        0        0     1713 2024-05-16 09:14:53.000000 deep_unfolding-0.4.0/tests/test_iterative.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:18:59.385987 deep_unfolding-0.4.1/
+-rw-rw-rw-   0        0        0    35823 2024-05-16 09:14:53.000000 deep_unfolding-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-05-19 19:26:15.000000 deep_unfolding-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2062 2024-05-19 21:18:59.385987 deep_unfolding-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2024-05-19 21:13:48.000000 deep_unfolding-0.4.1/README.md
+-rw-rw-rw-   0        0        0       95 2024-05-19 21:17:23.000000 deep_unfolding-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1070 2024-05-19 21:18:59.400822 deep_unfolding-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-19 21:15:31.000000 deep_unfolding-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:18:59.281669 deep_unfolding-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 21:18:59.354272 deep_unfolding-0.4.1/src/deep_unfolding.egg-info/
+-rw-rw-rw-   0        0        0     2062 2024-05-19 21:18:59.000000 deep_unfolding-0.4.1/src/deep_unfolding.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-19 21:18:59.000000 deep_unfolding-0.4.1/src/deep_unfolding.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 21:18:59.000000 deep_unfolding-0.4.1/src/deep_unfolding.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-19 21:18:59.000000 deep_unfolding-0.4.1/src/deep_unfolding.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 21:18:59.000000 deep_unfolding-0.4.1/src/deep_unfolding.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 21:18:59.385987 deep_unfolding-0.4.1/tests/
+-rw-rw-rw-   0        0        0     2374 2024-05-16 09:14:53.000000 deep_unfolding-0.4.1/tests/testNet.py
+-rw-rw-rw-   0        0        0     1713 2024-05-16 09:14:53.000000 deep_unfolding-0.4.1/tests/test_iterative.py
```

### Comparing `deep_unfolding-0.4.0/LICENSE` & `deep_unfolding-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_unfolding-0.4.0/README.md` & `deep_unfolding-0.4.1/src/deep_unfolding.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,44 @@
+Metadata-Version: 2.1
+Name: deep-unfolding
+Version: 0.4.1
+Summary: deep unfolding of iterative methods to solve linear equations
+Home-page: https://github.com/Salahberra2022/deep_unfolding
+Author: Salah Berra
+Author-email: salahberra39@gmail.com
+Project-URL: Bug Tracker, https://github.com/Salahberra2022/deep_unfolding/-/issues
+Project-URL: repository, https://github.com/Salahberra2022/deep_unfolding
+Keywords: deep unfolding,iterative methods,trainable parameters,linear equation,optimization parameters,deep learning
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Deep unfolding of iterative method
 
 The package includes iterative methods for solving linear equations. However, due to the various parameters and performance of the iterative approach, it is necessary to optimize these parameters to improve the convergence rate. Such a proposed tool called **deep_unfolding**, which takes an iterative algorithm with a fixed number of iterations T, unravels its structure and adds trainable parameters. These parameters are then trained using deep learning techniques such as loss functions, stochastic gradient descent, and back-propagation.
-The package contains two different Iterative methods. The first package is called **Iterative**, which contains the conventional iterative method. The other package is called **IterativeNet**, which contains the deep unfolding of the iterative method.
+The package contains two different Iterative methods. The first package is called **methods**, which contains the conventional iterative method. The other package is called **train_methods**, which contains the deep unfolding of the iterative method.
 
 ### Installation 
 ```python
 pip install --upgrade pip
 pip install deep_unfolding
 ```
 ### Quick start
 
-```python
-from deep_unfolding.Iterative import main
-list_iterative=['RI', 'SOR', 'GS']
-main(list_iterative)
-```
-<p align="center">
-   <img src="https://github.com/Salahberra2022/deep_unfolding/assets/119638218/c5e53af3-445a-4607-8cec-b9ba33400f26" width="500" height="400">
- <p>
- 
-```python
-from deep_unfolding.IterativeNet import main
-list_iterative=['RINet', 'RI', 'SORNet', 'SOR', 'GS']
-main(list_iterative)
-```
-
-<p align="center">
- <img src="https://github.com/Salahberra2022/deep_unfolding/assets/119638218/c53ceec4-458f-44e8-b6cb-72e559b69ffc" width="500" height="400">
- <p>
-
 ### The diagram of the Deep unfolded network (DUN)
 
-In this example of the diagram, it can show that **$\omega_{l}$** can be unfolded throughout this network and can be the optimum parameter based on the input of the matrix.
-
-![sorNet](https://github.com/Salahberra2022/deep_unfolding/assets/119638218/d6d6af2b-89a6-4414-82af-2861e68c69a2)
-
 
   
 ### The Rest of package
 
-The package includes several conventional iterative methods for solving the linear equation (**Ax=b**), such as 
-<h4> The iterative methods</h4>
-<ul>
-  <li>Accelerated Over-relaxation (AOR)</li>
-  <li>Successive Over-relaxation (SOR)</li>
-  <li>Jacobi (JA)</li>
-  <li>gauss seidel (GS)</li>
-  <li>Richardson iteration (RI)</li>
-</ul>
-
-
-The package includes the following deep unfolded iterative methods:
-<h4> deep unfolded iterative methods </h4>
-<ul>
-  <li>AORNet</li>
-  <li>SORNet</li>
-  <li>ChebySORNet</li>
-  <li>ChebyAORNet</li>
-  <li>RINet</li>
-</ul>
-
 ### Reference
 If you use this software, please cite the following reference:
 
 
 
 ### License
```

### Comparing `deep_unfolding-0.4.0/setup.cfg` & `deep_unfolding-0.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6565 705f 756e 666f 6c64 696e   = deep_unfoldin
 00000020: 670d 0a76 6572 7369 6f6e 203d 2030 2e34  g..version = 0.4
-00000030: 2e30 0d0a 6175 7468 6f72 203d 2053 616c  .0..author = Sal
+00000030: 2e31 0d0a 6175 7468 6f72 203d 2053 616c  .1..author = Sal
 00000040: 6168 2042 6572 7261 0d0a 6175 7468 6f72  ah Berra..author
 00000050: 5f65 6d61 696c 203d 2073 616c 6168 6265  _email = salahbe
 00000060: 7272 6133 3940 676d 6169 6c2e 636f 6d0d  rra39@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2064  .description = d
 00000080: 6565 7020 756e 666f 6c64 696e 6720 6f66  eep unfolding of
 00000090: 2069 7465 7261 7469 7665 206d 6574 686f   iterative metho
 000000a0: 6473 2074 6f20 736f 6c76 6520 6c69 6e65  ds to solve line
```

### Comparing `deep_unfolding-0.4.0/tests/testNet.py` & `deep_unfolding-0.4.1/tests/testNet.py`

 * *Files identical despite different names*

### Comparing `deep_unfolding-0.4.0/tests/test_iterative.py` & `deep_unfolding-0.4.1/tests/test_iterative.py`

 * *Files identical despite different names*

