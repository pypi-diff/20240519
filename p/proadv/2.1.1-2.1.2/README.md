# Comparing `tmp/proadv-2.1.1.tar.gz` & `tmp/proadv-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proadv-2.1.1.tar", last modified: Mon May 13 09:01:51 2024, max compression
+gzip compressed data, was "proadv-2.1.2.tar", last modified: Sun May 19 20:47:43 2024, max compression
```

## Comparing `proadv-2.1.1.tar` & `proadv-2.1.2.tar`

### file list

```diff
@@ -1,51 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.440078 proadv-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-13 09:01:51.440078 proadv-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-13 09:01:48.000000 proadv-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.432078 proadv-2.1.1/proadv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.436078 proadv-2.1.1/proadv/filtration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.436078 proadv-2.1.1/proadv/filtration/detection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/bivariatekernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/phasespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/poincare.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/pollution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/spherical.py
--rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/detection/trivariatekernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.436078 proadv-2.1.1/proadv/filtration/replacement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/replacement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/filtration/replacement/replacements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.436078 proadv-2.1.1/proadv/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/kernel/bivariate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.436078 proadv-2.1.1/proadv/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/statistics/descriptive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.440078 proadv-2.1.1/proadv/statistics/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/statistics/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/statistics/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/statistics/moment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/statistics/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/statistics/spread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.440078 proadv-2.1.1/proadv/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.440078 proadv-2.1.1/proadv/tests/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/tests/statistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.440078 proadv-2.1.1/proadv/tests/statistics/descriptive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/tests/statistics/descriptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/tests/statistics/descriptive/test_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/tests/statistics/descriptive/test_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/tests/statistics/descriptive/test_median.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/tests/statistics/descriptive/test_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-13 09:01:48.000000 proadv-2.1.1/proadv/tests/statistics/descriptive/test_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:01:51.440078 proadv-2.1.1/proadv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-13 09:01:51.000000 proadv-2.1.1/proadv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-13 09:01:51.000000 proadv-2.1.1/proadv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:01:51.000000 proadv-2.1.1/proadv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 09:01:51.000000 proadv-2.1.1/proadv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:01:51.000000 proadv-2.1.1/proadv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:01:51.440078 proadv-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-13 09:01:48.000000 proadv-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.644482 proadv-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-19 20:47:43.644482 proadv-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-19 20:47:40.000000 proadv-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.636483 proadv-2.1.2/proadv/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.636483 proadv-2.1.2/proadv/filtration/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.640483 proadv-2.1.2/proadv/filtration/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/bivariatekernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/phasespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/poincare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/pollution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/spherical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/detection/trivariatekernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.640483 proadv-2.1.2/proadv/filtration/replacement/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/replacement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/filtration/replacement/replacements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.640483 proadv-2.1.2/proadv/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/kernel/bivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.640483 proadv-2.1.2/proadv/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/descriptive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.640483 proadv-2.1.2/proadv/statistics/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/moment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.640483 proadv-2.1.2/proadv/statistics/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.644482 proadv-2.1.2/proadv/statistics/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/signal/butter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/signal/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/signal/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/signal/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/statistics/spread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.644482 proadv-2.1.2/proadv/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.644482 proadv-2.1.2/proadv/tests/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.644482 proadv-2.1.2/proadv/tests/statistics/descriptive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/descriptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/descriptive/test_exponential_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/descriptive/test_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/descriptive/test_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/descriptive/test_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/descriptive/test_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/descriptive/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-19 20:47:40.000000 proadv-2.1.2/proadv/tests/statistics/descriptive/test_moving_average.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:47:43.644482 proadv-2.1.2/proadv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-19 20:47:43.000000 proadv-2.1.2/proadv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-19 20:47:43.000000 proadv-2.1.2/proadv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:47:43.000000 proadv-2.1.2/proadv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 20:47:43.000000 proadv-2.1.2/proadv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 20:47:43.000000 proadv-2.1.2/proadv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:47:43.644482 proadv-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-19 20:47:40.000000 proadv-2.1.2/setup.py
```

### Comparing `proadv-2.1.1/PKG-INFO` & `proadv-2.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: proadv
-Version: 2.1.1
+Version: 2.1.2
 Summary: Process Acoustic Doppler Velocimeter data with advanced despiking and analysis tools
 Home-page: https://github.com/farzadasgari/proadv
 Author: Farzad Asgari
 Author-email: std_farzad.asgari@alumni.khu.ac.ir
-Project-URL: Bug Tracker, https://github.com/farzadasgari/proadv/issues
-Project-URL: Documentation, https://github.com/farzadasgari/proadv/tree/main/docs
+Project-URL: Download URL, https://pypi.org/project/proadv/
 Project-URL: Source Code, https://github.com/farzadasgari/proadv
+Project-URL: Documentation, https://proadv.readthedocs.io/en/latest/
 Keywords: ProADV,python,signal processing,data processing,acoustic Doppler velocimeter,ADV,Denoising,Despiking
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.0
 Requires-Dist: scipy>=1.0
 Requires-Dist: fastkde
 
 # ProADV - Process Acoustic Doppler Velocimeter
 
@@ -55,14 +55,22 @@
         * **m3d-KDE (Modified Three-dimensional Kernel Density Estimation):** Further refines 3d-KDE for enhanced performance.
     * **Replacement Methods:** ProADV offers several options to replace detected spikes with more reliable values:
         * **LVD (Last Valid Data):** Replaces spikes with the last valid data point before the spike.
         *  **MV (Mean Value):** Replaces spikes with the mean value of velocity component. 
         * **LI (Linear Interpolation):** Uses linear interpolation between surrounding points to estimate the missing value.
         * **12PP (12 Points Cubic Polynomial):** Employs a 12-point cubic polynomial to fit a smoother curve and replace spikes.
 
+
+<div>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/trivariate-kernel.png" alt="trivariate-kernel" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/spectrum.png" alt="trivariate-kernel" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/phase-space.png" alt="trivariate-kernel" style="width:300px;"/>
+</div>
+
+
 * **Statistical Analysis:** ProADV equips you with essential statistical tools to characterize your ADV data:
     * **Minimum, Maximum:** Provides the range of measured velocities.
     * **Mean, Median, Mode:** Calculates central tendency measures.
     * **Skewness, Kurtosis:** Analyzes the distribution characteristics of your data.
 
 * **Advanced Analysis:** In addition to cleaning and basic statistics, ProADV offers advanced functionalities for deeper insights:
     * **Moving Average:** Smooths out data fluctuations for better visualization and trend analysis. Provided in simple moving average, exponential moving average, and weighted moving average methods. 
@@ -71,17 +79,22 @@
     * **PR (Pollution Rate) Calculation:** Estimates the level of noise or pollution within the data.
     * **Spectral Analysis:**
         * **PSD (Power Spectral Density):** Analyzes the distribution of energy across different frequencies within the data.
         * **PDF (Probability Density Function):** Provides the probability of encountering specific velocity values.
     * **Normality Test:** Evaluates whether your data follows a normal distribution.
     * **Normalization:** Scales data to a common range for further analysis or visualization.
 
+<div>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/singular-spectrum.png" alt="singular-spectrum" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/kalman.png" alt="kalman-filter" style="width:300px;"/>
+</div>
+
 ### Installation
 
-There are three convenient ways to install ProADV:
+There are two convenient ways to install ProADV:
 
 1. **Using pip (recommended):**
    ```bash
    pip install proadv
    ```
 
 2. **From source code:**
@@ -116,22 +129,24 @@
 
 1. [Exploring the role of signal pollution rate on the performance of despiking velocity time-series algorithms](https://doi.org/10.1016/j.flowmeasinst.2023.102485)
 2. [Unleashing the power of three-dimensional kernel density estimation for Doppler Velocimeter data despiking](https://doi.org/10.1016/j.measurement.2023.114053)
 
 
 ### Acknowledgment
 - This project was developed under the supervision of **[Dr. Seyed Hossein Mohaeri](https://khu.ac.ir/cv/1139/Seyed-Hossein-Mohajeri)** and **[Dr. Mojtaba Mehraein](https://khu.ac.ir/cv/279/Mojtaba-Mehraein)**.
+- We extend our deepest gratitude to **[Dr. Bimlesh Kumar](https://www.researchgate.net/profile/Bimlesh-Kumar)** and **[Dr. Luis Cea](https://www.researchgate.net/profile/Luis-Cea)** for their invaluable guidance and unwavering support throughout our journey.
 - Special thanks to [Parvaneh Yaghoubi](https://github.com/parvanehyaghoubi), [Hossein Abazari](https://github.com/HossA12), [Narges Yaghoubi](https://github.com/nargesyaghoubi), [Mojtaba Karimi](https://github.com/mojikarimi), and [Hiva Yarandi](https://github.com/Hivayrn) for their valuable contributions to this project.
 
 
 ### Contact
 For any inquiries, please contact:
 - std_farzad.asgari@alumni.khu.ac.ir
 - khufarzadasgari@gmail.com
 
+
 ### Links
 
 ##### Farzad Asgari
 [![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://farzadasgari.ir/)
 
 [![Google Scholar Badge](https://img.shields.io/badge/Google%20Scholar-4285F4?logo=googlescholar&logoColor=fff&style=for-the-badge)](https://scholar.google.com/citations?user=Rhue_kkAAAAJ&hl=en)
```

### Comparing `proadv-2.1.1/README.md` & `proadv-2.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,22 @@
         * **m3d-KDE (Modified Three-dimensional Kernel Density Estimation):** Further refines 3d-KDE for enhanced performance.
     * **Replacement Methods:** ProADV offers several options to replace detected spikes with more reliable values:
         * **LVD (Last Valid Data):** Replaces spikes with the last valid data point before the spike.
         *  **MV (Mean Value):** Replaces spikes with the mean value of velocity component. 
         * **LI (Linear Interpolation):** Uses linear interpolation between surrounding points to estimate the missing value.
         * **12PP (12 Points Cubic Polynomial):** Employs a 12-point cubic polynomial to fit a smoother curve and replace spikes.
 
+
+<div>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/trivariate-kernel.png" alt="trivariate-kernel" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/spectrum.png" alt="trivariate-kernel" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/phase-space.png" alt="trivariate-kernel" style="width:300px;"/>
+</div>
+
+
 * **Statistical Analysis:** ProADV equips you with essential statistical tools to characterize your ADV data:
     * **Minimum, Maximum:** Provides the range of measured velocities.
     * **Mean, Median, Mode:** Calculates central tendency measures.
     * **Skewness, Kurtosis:** Analyzes the distribution characteristics of your data.
 
 * **Advanced Analysis:** In addition to cleaning and basic statistics, ProADV offers advanced functionalities for deeper insights:
     * **Moving Average:** Smooths out data fluctuations for better visualization and trend analysis. Provided in simple moving average, exponential moving average, and weighted moving average methods. 
@@ -45,17 +53,22 @@
     * **PR (Pollution Rate) Calculation:** Estimates the level of noise or pollution within the data.
     * **Spectral Analysis:**
         * **PSD (Power Spectral Density):** Analyzes the distribution of energy across different frequencies within the data.
         * **PDF (Probability Density Function):** Provides the probability of encountering specific velocity values.
     * **Normality Test:** Evaluates whether your data follows a normal distribution.
     * **Normalization:** Scales data to a common range for further analysis or visualization.
 
+<div>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/singular-spectrum.png" alt="singular-spectrum" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/kalman.png" alt="kalman-filter" style="width:300px;"/>
+</div>
+
 ### Installation
 
-There are three convenient ways to install ProADV:
+There are two convenient ways to install ProADV:
 
 1. **Using pip (recommended):**
    ```bash
    pip install proadv
    ```
 
 2. **From source code:**
@@ -90,22 +103,24 @@
 
 1. [Exploring the role of signal pollution rate on the performance of despiking velocity time-series algorithms](https://doi.org/10.1016/j.flowmeasinst.2023.102485)
 2. [Unleashing the power of three-dimensional kernel density estimation for Doppler Velocimeter data despiking](https://doi.org/10.1016/j.measurement.2023.114053)
 
 
 ### Acknowledgment
 - This project was developed under the supervision of **[Dr. Seyed Hossein Mohaeri](https://khu.ac.ir/cv/1139/Seyed-Hossein-Mohajeri)** and **[Dr. Mojtaba Mehraein](https://khu.ac.ir/cv/279/Mojtaba-Mehraein)**.
+- We extend our deepest gratitude to **[Dr. Bimlesh Kumar](https://www.researchgate.net/profile/Bimlesh-Kumar)** and **[Dr. Luis Cea](https://www.researchgate.net/profile/Luis-Cea)** for their invaluable guidance and unwavering support throughout our journey.
 - Special thanks to [Parvaneh Yaghoubi](https://github.com/parvanehyaghoubi), [Hossein Abazari](https://github.com/HossA12), [Narges Yaghoubi](https://github.com/nargesyaghoubi), [Mojtaba Karimi](https://github.com/mojikarimi), and [Hiva Yarandi](https://github.com/Hivayrn) for their valuable contributions to this project.
 
 
 ### Contact
 For any inquiries, please contact:
 - std_farzad.asgari@alumni.khu.ac.ir
 - khufarzadasgari@gmail.com
 
+
 ### Links
 
 ##### Farzad Asgari
 [![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://farzadasgari.ir/)
 
 [![Google Scholar Badge](https://img.shields.io/badge/Google%20Scholar-4285F4?logo=googlescholar&logoColor=fff&style=for-the-badge)](https://scholar.google.com/citations?user=Rhue_kkAAAAJ&hl=en)
```

### Comparing `proadv-2.1.1/proadv/filtration/detection/acceleration.py` & `proadv-2.1.2/proadv/filtration/detection/acceleration.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from proadv.statistics.spread import std
 
 
 def acceleration_thresholding(velocities, frequency, tag, gravity=980, k_gravity=1.5, k_sigma=1):
     """
     Detects acceleration events based on velocity data.
 
-    This function calculates acceleration events based on velocity data, considering thresholds
+    Calculate acceleration events based on velocity data, considering thresholds
         for acceleration magnitude and velocity deviation from mean.
 
     Parameters
     ------
         velocities (array_like): Array of velocity data.
             An array-like object containing velocity values.
         frequency (float): Sampling frequency.
```

### Comparing `proadv-2.1.1/proadv/filtration/detection/bivariatekernel.py` & `proadv-2.1.2/proadv/filtration/detection/bivariatekernel.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,7 +47,17 @@
     else:
         upper_cutoff_index = profile_length - 1
 
     lower_cutoff_velocity = velocity_profile[lower_cutoff_index]
     upper_cutoff_velocity = velocity_profile[upper_cutoff_index]
 
     return lower_cutoff_velocity, upper_cutoff_velocity
+
+
+def _derivative(data):
+    data_size = data.size
+    derivative = np.zeros(data_size)
+    for i in range(1, data_size - 1):
+        backward = data[i] - data[i - 1]
+        forward = data[i + 1] - data[i]
+        derivative[i] = forward if abs(backward) > abs(forward) else backward
+    return derivative
```

### Comparing `proadv-2.1.1/proadv/filtration/detection/correlation.py` & `proadv-2.1.2/proadv/filtration/detection/correlation.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/filtration/detection/phasespace.py` & `proadv-2.1.2/proadv/filtration/detection/phasespace.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/filtration/detection/poincare.py` & `proadv-2.1.2/proadv/filtration/detection/poincare.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/filtration/detection/pollution.py` & `proadv-2.1.2/proadv/filtration/detection/pollution.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/filtration/detection/spherical.py` & `proadv-2.1.2/proadv/filtration/detection/spherical.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/filtration/detection/trivariatekernel.py` & `proadv-2.1.2/proadv/filtration/detection/trivariatekernel.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/filtration/replacement/replacements.py` & `proadv-2.1.2/proadv/filtration/replacement/replacements.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,30 +62,26 @@
         linearly interpolated values based on the nearest valid data points before
         and after each spike. If a spike occurs at the end of the data, it is replaced
         with the mean of the entire dataset. The function is robust to handle individual
         spikes as well as sequences of consecutive spikes.
 
     Parameters
     ------
-    velocities : (array_like)
-        An array-like object containing velocity values. It should be a one-dimensional
+    velocities (array_like):  An array-like object containing velocity values. It should be a one-dimensional
         array of numerical data representing velocities.
-    spike_indices : (array_like)
-        An array-like object containing the indices of detected spike events. It should
+    spike_indices (array_like): An array-like object containing the indices of detected spike events. It should
         be a one-dimensional array of integers where each integer represents the index
         in 'velocities' that corresponds to a spike.
-    decimals : int, optional
-        The number of decimal places to round the interpolated values to. This allows
+    decimals (int, optional): The number of decimal places to round the interpolated values to. This allows
         the output data to be presented with a consistent level of precision. The default
         value is 4, but this can be adjusted as needed.
 
     Returns
     ------
-    modified_data (array_like):
-        An array containing the modified velocity data with spikes replaced by
+    modified_data (array_like): An array containing the modified velocity data with spikes replaced by
         interpolated values. The shape and type of the array are the same as the
         input 'velocities' array.
 
     Notes
     ------
     The function uses linear interpolation to estimate the values of spikes based on the
         surrounding non-spike data. For spikes at the beginning or end of the data where a
```

### Comparing `proadv-2.1.1/proadv/kernel/bivariate.py` & `proadv-2.1.2/proadv/kernel/bivariate.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,22 +362,22 @@
 
 
 def bivariate_kernel(data, hx, hy, grid):
     """
     Compute the bivariate kernel density estimation.
 
     Parameters
-    ----------
+    ------
     data (array_like): Input data array.
     hx (float): Bandwidth along the x-axis.
     hy (float): Bandwidth along the y-axis.
     grid (int): Number of bins along each dimension for histogram computation.
 
     Returns
-    -------
+    ------
     density_mx (array_like): Bivariate kernel density estimation.
     x_mx (array_like): Meshgrid of x values.
     y_mx (array_like): Meshgrid of y values.
     """
     
     # Compute scaling parameters
     data_size = data.size
```

### Comparing `proadv-2.1.1/proadv/statistics/descriptive.py` & `proadv-2.1.2/proadv/statistics/descriptive.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,24 +47,23 @@
     >>> from proadv.statistics.descriptive import min 
     >>> import numpy as np
     >>> data = np.random.rand(20)
     >>> minimum = min(data)
     """
 
     for i in data:
-        if isinstance(i, str):  # isinstance returns True if the specified object is of the specified type, otherwise False.
+        if isinstance(i,
+                      str):  # isinstance returns True if the specified object is of the specified type, otherwise False
             raise TypeError("String cannot be placed as an element of an array")
     if np.isnan(data).any():
         raise ValueError("The array contains NaN values. The min function cannot be applied to arrays with NaN values.")
-    if data.ndim != 1:  # Optional check for 1D array
-        raise ValueError("Data array must be a 1D array.")   
-    if np.size(data) == 0: # The array cannot be empty
+    if np.size(data) == 0:  # The array cannot be empty
         raise ValueError("cannot calculate minimum with empty array")
-      
-    minimum = np.min(data) # Calculate the minimum
+
+    minimum = np.min(data)  # Calculate the minimum
     return minimum
 
 
 def max(data):
     """
     Calculate the maximum value in an array, handling NaN values and exceptions.
 
@@ -112,30 +111,28 @@
     >>> from proadv.statistics.descriptive import max 
     >>> import numpy as np
     >>> data = np.arange(2,10)
     >>> maximum = max(data)
     >>> maximum
     9
     """
-    
+
     for i in data:
-        if isinstance(i, str): # isinstance returns True if the specified object is of the specified type, otherwise False.
+        if isinstance(i,
+                      str):  # isinstance returns True if the specified object is of the specified type, otherwise False.
             raise TypeError("String cannot be placed as an element of an array")
 
     if np.isnan(data).any():
         raise ValueError("The array contains NaN values. The max function cannot be applied to arrays with NaN values.")
-    
-    if data.ndim != 1:  # Optional check for 1D array
-        raise ValueError("Data array must be a 1D array.")
-    
+
     if np.size(data) == 0:
         # The array cannot be empty
         raise ValueError("cannot calculate maximum with empty array")
     maximum = np.max(data)  # Calculate the maximum
-    
+
     return maximum
 
 
 def mean(array):
     """
     Calculate the mean of a dataset, handling non-numeric and numeric data.
```

### Comparing `proadv-2.1.1/proadv/statistics/moment.py` & `proadv-2.1.2/proadv/statistics/moment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from descriptive import mean
-from spread import std
+from .descriptive import mean
+from .spread import std
 
 
 def skewness(data):
     """
     Compute the sample skewness of a data set. 
 
     Parameters
```

### Comparing `proadv-2.1.1/proadv/statistics/series.py` & `proadv-2.1.2/proadv/statistics/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from .descriptive import mean
 
 
 def moving_average(data, window_size=20):
     """
     Calculates the moving average of a 1D array.
 
     Parameters
@@ -55,15 +56,15 @@
         raise ValueError("Data array size must be greater than window size.")
 
     ma = np.zeros(data.size)  # Moving Average
 
     # Calculate the initial moving average for the first window_size elements
     for i in range(window_size):
         # Calculate the average of the data points from begining up to the current index (inclusive)
-        ma[i] = np.mean(data[:i + 1])
+        ma[i] = mean(data[:i + 1])
 
     # Efficiently calculate the moving average for remaining elements using cumulative sum
     for i in range(window_size, data.size):
         """
         This loop calculates the moving average for elements from index 'window_size' onwards.
         It leverages the previously calculated moving average (ma[i-1]) and the new data point
         (data[i]) to efficiently update the moving average using the formula:
@@ -99,17 +100,18 @@
     ------
     The exponential moving average (EMA) is a type of moving average that places more weight
         on recent observations while still considering older data. It is particularly useful for
         smoothing noisy data and identifying trends.
 
     Examples
     ------
+    >>> import proadv as adv
     >>> import numpy as np
     >>> data = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
-    >>> ema = exponential_moving_average(data, alpha=0.5)
+    >>> ema = adv.statistics.series.exponential_moving_average(data, alpha=0.5)
     >>> ema
     array([1, 1, 2, 3, 4, 5, 6, 7, 8, 9])
 
     """
 
     # Check if alpha is within the valid range
     if alpha <= 0 or alpha > 1:
@@ -178,25 +180,25 @@
     >>> wma = weighted_moving_average(data)    
     """
     if period <= 0:
         raise ValueError("Period must be greater than zero.")
 
     if period > data.size:
         raise ValueError("Data array size must be greater than period.")
-    
+
     wma = []
-    
+
     for i in range(period, data.size):
         """
         We obtain weighted moving average by multiplying each number in the data set by a predetermined weight 
             and summing up the resulting values. Finally, the result value is divided to the total weights. 
         """
-        weight = np.arange(1, period+1) # Weight matrix
-        weighted_sum = (weight * data[i - period : i]).sum() / (weight.sum()) # Calculate the weighted moving average
-        wma = np.append(wma, weighted_sum) # Add to array
+        weight = np.arange(1, period + 1)  # Weight matrix
+        weighted_sum = (weight * data[i - period: i]).sum() / (weight.sum())  # Calculate the weighted moving average
+        wma = np.append(wma, weighted_sum)  # Add to array
     return wma
 
 
 def _mobility(x):
     """
     Compute the covert mobility index.
 
@@ -358,29 +360,33 @@
         given a sequence of noisy observations or measurements of the state over time.
     
     Examples
     ------
     >>> from proadv.statistics.series import kalman_filter  
     >>> import numpy as np
     >>> data = np.random.rand(300)
+    >>> initial_state = np.array([[10]])
+    >>> initial_covariance = np.array([[10]])
+    >>> process_noise = np.array([[0.001]])
+    >>> measurement_noise = np.array([[15]])
     >>> filtered_data = kalman_filter(data, initial_state, initial_covariance, process_noise, measurement_noise)
     """
     filtered_data = []
     state_estimate = initial_state
     covariance_estimate = initial_covariance
     Q = process_noise
     R = measurement_noise
-    A = np.array([[1]]) # A matrix for Prediction step 
-    H = np.array([[1]]) # A matrix for Measurement update
+    A = np.array([[1]])  # A matrix for Prediction step
+    H = np.array([[1]])  # A matrix for Measurement update
     for measurement in data:
         # Prediction step
         predicted_state = np.dot(A, state_estimate)
         predicted_covariance = np.dot(np.dot(A, covariance_estimate), A.T) + Q
         # Measurement update
-        kalman_gain = np.dot(np.dot(predicted_covariance, H.T) , np.linalg.inv(np.dot(np.dot(H, predicted_covariance), H.T) + R))
+        kalman_gain = np.dot(np.dot(predicted_covariance, H.T),
+                             np.linalg.inv(np.dot(np.dot(H, predicted_covariance), H.T) + R))
         state_estimate = predicted_state + np.dot(kalman_gain, (measurement - np.dot(H, predicted_state)))
         covariance_estimate = np.dot((np.eye(len(state_estimate)) - np.dot(kalman_gain, H)), predicted_covariance)
-                                 
+
         filtered_data.append(state_estimate)
 
     return filtered_data
-
```

### Comparing `proadv-2.1.1/proadv/statistics/spread.py` & `proadv-2.1.2/proadv/statistics/spread.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/tests/statistics/descriptive/test_max.py` & `proadv-2.1.2/proadv/tests/statistics/descriptive/test_max.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/tests/statistics/descriptive/test_mean.py` & `proadv-2.1.2/proadv/tests/statistics/descriptive/test_mean.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/tests/statistics/descriptive/test_median.py` & `proadv-2.1.2/proadv/tests/statistics/descriptive/test_median.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/tests/statistics/descriptive/test_min.py` & `proadv-2.1.2/proadv/tests/statistics/descriptive/test_min.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv/tests/statistics/descriptive/test_mode.py` & `proadv-2.1.2/proadv/tests/statistics/descriptive/test_mode.py`

 * *Files identical despite different names*

### Comparing `proadv-2.1.1/proadv.egg-info/PKG-INFO` & `proadv-2.1.2/proadv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: proadv
-Version: 2.1.1
+Version: 2.1.2
 Summary: Process Acoustic Doppler Velocimeter data with advanced despiking and analysis tools
 Home-page: https://github.com/farzadasgari/proadv
 Author: Farzad Asgari
 Author-email: std_farzad.asgari@alumni.khu.ac.ir
-Project-URL: Bug Tracker, https://github.com/farzadasgari/proadv/issues
-Project-URL: Documentation, https://github.com/farzadasgari/proadv/tree/main/docs
+Project-URL: Download URL, https://pypi.org/project/proadv/
 Project-URL: Source Code, https://github.com/farzadasgari/proadv
+Project-URL: Documentation, https://proadv.readthedocs.io/en/latest/
 Keywords: ProADV,python,signal processing,data processing,acoustic Doppler velocimeter,ADV,Denoising,Despiking
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.0
 Requires-Dist: scipy>=1.0
 Requires-Dist: fastkde
 
 # ProADV - Process Acoustic Doppler Velocimeter
 
@@ -55,14 +55,22 @@
         * **m3d-KDE (Modified Three-dimensional Kernel Density Estimation):** Further refines 3d-KDE for enhanced performance.
     * **Replacement Methods:** ProADV offers several options to replace detected spikes with more reliable values:
         * **LVD (Last Valid Data):** Replaces spikes with the last valid data point before the spike.
         *  **MV (Mean Value):** Replaces spikes with the mean value of velocity component. 
         * **LI (Linear Interpolation):** Uses linear interpolation between surrounding points to estimate the missing value.
         * **12PP (12 Points Cubic Polynomial):** Employs a 12-point cubic polynomial to fit a smoother curve and replace spikes.
 
+
+<div>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/trivariate-kernel.png" alt="trivariate-kernel" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/spectrum.png" alt="trivariate-kernel" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/phase-space.png" alt="trivariate-kernel" style="width:300px;"/>
+</div>
+
+
 * **Statistical Analysis:** ProADV equips you with essential statistical tools to characterize your ADV data:
     * **Minimum, Maximum:** Provides the range of measured velocities.
     * **Mean, Median, Mode:** Calculates central tendency measures.
     * **Skewness, Kurtosis:** Analyzes the distribution characteristics of your data.
 
 * **Advanced Analysis:** In addition to cleaning and basic statistics, ProADV offers advanced functionalities for deeper insights:
     * **Moving Average:** Smooths out data fluctuations for better visualization and trend analysis. Provided in simple moving average, exponential moving average, and weighted moving average methods. 
@@ -71,17 +79,22 @@
     * **PR (Pollution Rate) Calculation:** Estimates the level of noise or pollution within the data.
     * **Spectral Analysis:**
         * **PSD (Power Spectral Density):** Analyzes the distribution of energy across different frequencies within the data.
         * **PDF (Probability Density Function):** Provides the probability of encountering specific velocity values.
     * **Normality Test:** Evaluates whether your data follows a normal distribution.
     * **Normalization:** Scales data to a common range for further analysis or visualization.
 
+<div>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/singular-spectrum.png" alt="singular-spectrum" style="width:300px;"/>
+   <img src="https://raw.githubusercontent.com/farzadasgari/proadv/main/examples/plots/kalman.png" alt="kalman-filter" style="width:300px;"/>
+</div>
+
 ### Installation
 
-There are three convenient ways to install ProADV:
+There are two convenient ways to install ProADV:
 
 1. **Using pip (recommended):**
    ```bash
    pip install proadv
    ```
 
 2. **From source code:**
@@ -116,22 +129,24 @@
 
 1. [Exploring the role of signal pollution rate on the performance of despiking velocity time-series algorithms](https://doi.org/10.1016/j.flowmeasinst.2023.102485)
 2. [Unleashing the power of three-dimensional kernel density estimation for Doppler Velocimeter data despiking](https://doi.org/10.1016/j.measurement.2023.114053)
 
 
 ### Acknowledgment
 - This project was developed under the supervision of **[Dr. Seyed Hossein Mohaeri](https://khu.ac.ir/cv/1139/Seyed-Hossein-Mohajeri)** and **[Dr. Mojtaba Mehraein](https://khu.ac.ir/cv/279/Mojtaba-Mehraein)**.
+- We extend our deepest gratitude to **[Dr. Bimlesh Kumar](https://www.researchgate.net/profile/Bimlesh-Kumar)** and **[Dr. Luis Cea](https://www.researchgate.net/profile/Luis-Cea)** for their invaluable guidance and unwavering support throughout our journey.
 - Special thanks to [Parvaneh Yaghoubi](https://github.com/parvanehyaghoubi), [Hossein Abazari](https://github.com/HossA12), [Narges Yaghoubi](https://github.com/nargesyaghoubi), [Mojtaba Karimi](https://github.com/mojikarimi), and [Hiva Yarandi](https://github.com/Hivayrn) for their valuable contributions to this project.
 
 
 ### Contact
 For any inquiries, please contact:
 - std_farzad.asgari@alumni.khu.ac.ir
 - khufarzadasgari@gmail.com
 
+
 ### Links
 
 ##### Farzad Asgari
 [![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://farzadasgari.ir/)
 
 [![Google Scholar Badge](https://img.shields.io/badge/Google%20Scholar-4285F4?logo=googlescholar&logoColor=fff&style=for-the-badge)](https://scholar.google.com/citations?user=Rhue_kkAAAAJ&hl=en)
```

### Comparing `proadv-2.1.1/proadv.egg-info/SOURCES.txt` & `proadv-2.1.2/proadv.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,24 @@
 proadv/statistics/__init__.py
 proadv/statistics/descriptive.py
 proadv/statistics/moment.py
 proadv/statistics/series.py
 proadv/statistics/spread.py
 proadv/statistics/distributions/__init__.py
 proadv/statistics/distributions/normal.py
+proadv/statistics/optimize/__init__.py
+proadv/statistics/optimize/optimize.py
+proadv/statistics/signal/__init__.py
+proadv/statistics/signal/butter.py
+proadv/statistics/signal/fluid.py
+proadv/statistics/signal/spectrum.py
+proadv/statistics/signal/synthetic.py
 proadv/tests/__init__.py
 proadv/tests/statistics/__init__.py
 proadv/tests/statistics/descriptive/__init__.py
+proadv/tests/statistics/descriptive/test_exponential_moving_average.py
 proadv/tests/statistics/descriptive/test_max.py
 proadv/tests/statistics/descriptive/test_mean.py
 proadv/tests/statistics/descriptive/test_median.py
 proadv/tests/statistics/descriptive/test_min.py
-proadv/tests/statistics/descriptive/test_mode.py
+proadv/tests/statistics/descriptive/test_mode.py
+proadv/tests/statistics/descriptive/test_moving_average.py
```

### Comparing `proadv-2.1.1/setup.py` & `proadv-2.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Read the contents of the README file for the long description
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Setting up
 setup(
     name="proadv",
-    version="2.1.1",
+    version="2.1.2",
     author="Farzad Asgari",
     author_email="std_farzad.asgari@alumni.khu.ac.ir",
     description="Process Acoustic Doppler Velocimeter data with advanced despiking and analysis tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/farzadasgari/proadv",
     license_file="MIT",
@@ -33,19 +33,19 @@
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.12",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     project_urls={
-        "Bug Tracker": "https://github.com/farzadasgari/proadv/issues",
-        "Documentation": "https://github.com/farzadasgari/proadv/tree/main/docs",
+        "Download URL": "https://pypi.org/project/proadv/",
         "Source Code": "https://github.com/farzadasgari/proadv",
+        "Documentation": "https://proadv.readthedocs.io/en/latest/",
     },
 )
```

