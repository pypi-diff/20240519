# Comparing `tmp/diffforms-0.0.30.tar.gz` & `tmp/diffforms-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffforms-0.0.30.tar", last modified: Tue Apr 30 22:51:38 2024, max compression
+gzip compressed data, was "diffforms-0.0.31.tar", last modified: Sun May 19 20:30:32 2024, max compression
```

## Comparing `diffforms-0.0.30.tar` & `diffforms-0.0.31.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 22:51:38.364638 diffforms-0.0.30/
--rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.30/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-30 22:51:38.364221 diffforms-0.0.30/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1527 2024-04-30 22:45:27.000000 diffforms-0.0.30/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 22:51:38.360978 diffforms-0.0.30/diffforms/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.30/diffforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    24106 2024-04-30 22:47:03.000000 diffforms-0.0.30/diffforms/core.py
--rwxrwxrwx   0 root         (0) root         (0)       23 2024-04-30 22:51:28.000000 diffforms-0.0.30/diffforms/release.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 22:51:38.363778 diffforms-0.0.30/diffforms.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-30 22:51:38.000000 diffforms-0.0.30/diffforms.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-30 22:51:38.000000 diffforms-0.0.30/diffforms.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-30 22:51:38.000000 diffforms-0.0.30/diffforms.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-04-30 22:51:38.000000 diffforms-0.0.30/diffforms.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-30 22:51:38.000000 diffforms-0.0.30/diffforms.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.30/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-30 22:51:38.364728 diffforms-0.0.30/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.30/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 20:30:32.613669 diffforms-0.0.31/
+-rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.31/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-05-19 20:30:32.613222 diffforms-0.0.31/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1597 2024-05-19 20:29:36.000000 diffforms-0.0.31/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 20:30:32.610090 diffforms-0.0.31/diffforms/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.31/diffforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    34057 2024-05-19 20:27:43.000000 diffforms-0.0.31/diffforms/core.py
+-rwxrwxrwx   0 root         (0) root         (0)       23 2024-05-19 20:30:19.000000 diffforms-0.0.31/diffforms/release.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 20:30:32.612739 diffforms-0.0.31/diffforms.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-05-19 20:30:32.000000 diffforms-0.0.31/diffforms.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      272 2024-05-19 20:30:32.000000 diffforms-0.0.31/diffforms.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-19 20:30:32.000000 diffforms-0.0.31/diffforms.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-19 20:30:32.000000 diffforms-0.0.31/diffforms.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-19 20:30:32.000000 diffforms-0.0.31/diffforms.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.31/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-19 20:30:32.613759 diffforms-0.0.31/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.31/setup.py
```

### Comparing `diffforms-0.0.30/PKG-INFO` & `diffforms-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffforms
-Version: 0.0.30
+Version: 0.0.31
 Summary: Symbolic differential forms python library
 Home-page: https://github.com/Bone5505/Differential-Forms
 Author: Adam Shaw
 Keywords: differential forms,sympy,polyforms,exterior derivative
 Requires-Dist: wheel>=0.43.0
 Requires-Dist: sympy>=1.12
 Requires-Dist: ipython>=8.19.0
```

### Comparing `diffforms-0.0.30/README.md` & `diffforms-0.0.31/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 =========
 This is the list of possible implementation, in an approximate order of priority (interest to me):
 
 - [X] Differential Forms
 - [X] Exterior Product
 - [X] Simplification of Forms
 - [X] Exterior Differential Operator
-- [X] Substitution of factors/forms (Done?)
+- [X] Substitution of factors/forms
 - [X] Vector fields
 - [X] Generic tensor product
-- [X] Insertion of vector fields (Done?)
+- [X] Insertion of vector fields
+- [X] Generic Tensor Contractions
+- [ ] Implement substitution for Tensors
 - [ ] Hodge star given metric/frame (In Progress)
-- [ ] Generic Tensor Contractions
+- [ ] Solving 1-form simple linear equations
 - [ ] Vector Field Commutator
 
 Dependencies
 ============
 Make sure you have the following python packages:
 
 - wheel (needed for installing through pip)
```

### Comparing `diffforms-0.0.30/diffforms.egg-info/PKG-INFO` & `diffforms-0.0.31/diffforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffforms
-Version: 0.0.30
+Version: 0.0.31
 Summary: Symbolic differential forms python library
 Home-page: https://github.com/Bone5505/Differential-Forms
 Author: Adam Shaw
 Keywords: differential forms,sympy,polyforms,exterior derivative
 Requires-Dist: wheel>=0.43.0
 Requires-Dist: sympy>=1.12
 Requires-Dist: ipython>=8.19.0
```

### Comparing `diffforms-0.0.30/setup.py` & `diffforms-0.0.31/setup.py`

 * *Files identical despite different names*

