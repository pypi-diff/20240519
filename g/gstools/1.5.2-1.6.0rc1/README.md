# Comparing `tmp/gstools-1.5.2.tar.gz` & `tmp/gstools-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gstools-1.5.2.tar", last modified: Sun May 19 20:19:41 2024, max compression
+gzip compressed data, was "gstools-1.6.0rc1.tar", last modified: Fri Nov 10 10:48:40 2023, max compression
```

## Comparing `gstools-1.5.2.tar` & `gstools-1.6.0rc1.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.769456 gstools-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-19 20:14:12.000000 gstools-1.5.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-19 20:14:12.000000 gstools-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21842 2024-05-19 20:19:41.769456 gstools-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-05-19 20:14:12.000000 gstools-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-19 20:14:12.000000 gstools-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:19:41.769456 gstools-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 20:14:12.000000 gstools-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.753456 gstools-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.757457 gstools-1.5.2/src/gstools/
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 20:19:41.000000 gstools-1.5.2/src/gstools/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.757457 gstools-1.5.2/src/gstools/covmodel/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/covmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41882 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/covmodel/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20810 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/covmodel/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    27867 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/covmodel/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/covmodel/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    19517 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/covmodel/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    18494 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/covmodel/tpl_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.757457 gstools-1.5.2/src/gstools/field/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23833 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/cond_srf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13227 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/srf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/summator.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/field/upscaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.761457 gstools-1.5.2/src/gstools/krige/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/krige/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/krige/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/krige/krigesum.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    21042 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/krige/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/krige/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.761457 gstools-1.5.2/src/gstools/normalizer/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/normalizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/normalizer/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/normalizer/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.761457 gstools-1.5.2/src/gstools/random/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/random/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/random/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.761457 gstools-1.5.2/src/gstools/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/tools/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    22093 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/tools/geometric.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4292 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/tools/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/tools/special.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.761457 gstools-1.5.2/src/gstools/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/transform/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    20418 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/transform/field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.761457 gstools-1.5.2/src/gstools/variogram/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/variogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/variogram/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/variogram/estimator.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    18992 2024-05-19 20:14:12.000000 gstools-1.5.2/src/gstools/variogram/variogram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.765457 gstools-1.5.2/src/gstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-19 20:19:41.000000 gstools-1.5.2/src/gstools.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:19:41.765457 gstools-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_covmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_incomprrandmeth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_krige.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_latlon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_randmeth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_srf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_variogram_structured.py
--rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-05-19 20:14:12.000000 gstools-1.5.2/tests/test_variogram_unstructured.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.484378 gstools-1.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21842 2023-11-10 10:48:40.484378 gstools-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18833 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 10:48:40.484378 gstools-1.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.468378 gstools-1.6.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.472378 gstools-1.6.0rc1/src/gstools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-10 10:48:40.000000 gstools-1.6.0rc1/src/gstools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.472378 gstools-1.6.0rc1/src/gstools/covmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/covmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41881 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/covmodel/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20705 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/covmodel/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/covmodel/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/covmodel/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19517 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/covmodel/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18493 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/covmodel/tpl_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.472378 gstools-1.6.0rc1/src/gstools/field/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23829 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/cond_srf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27093 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13499 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/srf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/summator.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/field/upscaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.476378 gstools-1.6.0rc1/src/gstools/krige/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/krige/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29420 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/krige/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/krige/krigesum.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    21041 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/krige/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/krige/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.476378 gstools-1.6.0rc1/src/gstools/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/normalizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/normalizer/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/normalizer/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.476378 gstools-1.6.0rc1/src/gstools/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/random/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/random/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.476378 gstools-1.6.0rc1/src/gstools/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/tools/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22104 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/tools/geometric.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4291 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/tools/special.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.476378 gstools-1.6.0rc1/src/gstools/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/transform/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20441 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/transform/field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.476378 gstools-1.6.0rc1/src/gstools/variogram/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/variogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/variogram/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/variogram/estimator.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    18829 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/src/gstools/variogram/variogram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.480378 gstools-1.6.0rc1/src/gstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-10 10:48:40.000000 gstools-1.6.0rc1/src/gstools.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:48:40.480378 gstools-1.6.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_covmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_fouriergen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_incomprrandmeth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_krige.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_latlon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_randmeth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12969 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_srf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_variogram_structured.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15024 2023-11-10 10:42:50.000000 gstools-1.6.0rc1/tests/test_variogram_unstructured.py
```

### Comparing `gstools-1.5.2/AUTHORS.md` & `gstools-1.6.0rc1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/LICENSE` & `gstools-1.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/PKG-INFO` & `gstools-1.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gstools
-Version: 1.5.2
+Version: 1.6.0rc1
 Summary: GSTools: A geostatistical toolbox.
 Author-email: "Sebastian Müller, Lennart Schüler" <info@geostat-framework.org>
 License: LGPL-3.0
 Project-URL: Changelog, https://github.com/GeoStat-Framework/GSTools/blob/main/CHANGELOG.md
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/gstools
 Project-URL: Documentation, https://gstools.readthedocs.io
 Project-URL: Homepage, https://geostat-framework.org/#gstools
@@ -36,37 +36,37 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: emcee>=3.0.0
 Requires-Dist: hankel>=1.0.0
 Requires-Dist: meshio>=5.1.0
-Requires-Dist: numpy>=1.20.0
+Requires-Dist: numpy>=1.14.5
 Requires-Dist: pyevtk>=1.1.1
 Requires-Dist: scipy>=1.1.0
 Provides-Extra: doc
 Requires-Dist: m2r2>=0.2.8; extra == "doc"
-Requires-Dist: matplotlib>=3.7; extra == "doc"
+Requires-Dist: matplotlib>=3; extra == "doc"
 Requires-Dist: meshzoo>=0.7; extra == "doc"
 Requires-Dist: numpydoc>=1.1; extra == "doc"
 Requires-Dist: pykrige<2,>=1.5; extra == "doc"
-Requires-Dist: pyvista>=0.40; extra == "doc"
-Requires-Dist: sphinx>=7; extra == "doc"
+Requires-Dist: pyvista>=0.29; extra == "doc"
+Requires-Dist: sphinx>=4; extra == "doc"
 Requires-Dist: sphinx-gallery>=0.8; extra == "doc"
-Requires-Dist: sphinx-rtd-theme>=2; extra == "doc"
+Requires-Dist: sphinx-rtd-theme<1.1,>=1; extra == "doc"
 Requires-Dist: sphinxcontrib-youtube>=1.1; extra == "doc"
 Provides-Extra: plotting
-Requires-Dist: matplotlib>=3.7; extra == "plotting"
-Requires-Dist: pyvista>=0.40; extra == "plotting"
+Requires-Dist: matplotlib>=3; extra == "plotting"
+Requires-Dist: pyvista>=0.29; extra == "plotting"
 Provides-Extra: rust
 Requires-Dist: gstools_core<1,>=0.2.0; extra == "rust"
 Provides-Extra: test
 Requires-Dist: pytest-cov>=3; extra == "test"
 Provides-Extra: lint
-Requires-Dist: black>=24; extra == "lint"
+Requires-Dist: black; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: isort[colors]; extra == "lint"
 Requires-Dist: cython-lint; extra == "lint"
 
 # Welcome to GSTools
 [![GMD](https://img.shields.io/badge/GMD-10.5194%2Fgmd--15--3161--2022-orange)](https://doi.org/10.5194/gmd-15-3161-2022)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1313628.svg)](https://doi.org/10.5281/zenodo.1313628)
@@ -410,15 +410,15 @@
 <p align="center">
 <img src="https://raw.githubusercontent.com/GeoStat-Framework/GSTools/main/docs/source/pics/pyvista_export.png" alt="pyvista export" width="600px"/>
 </p>
 
 
 ## Requirements:
 
-- [NumPy >= 1.20.0](https://www.numpy.org)
+- [NumPy >= 1.14.5](https://www.numpy.org)
 - [SciPy >= 1.1.0](https://www.scipy.org/scipylib)
 - [hankel >= 1.0.0](https://github.com/steven-murray/hankel)
 - [emcee >= 3.0.0](https://github.com/dfm/emcee)
 - [pyevtk >= 1.1.1](https://github.com/pyscience-projects/pyevtk)
 - [meshio >= 5.1.0](https://github.com/nschloe/meshio)
 
 ### Optional
@@ -431,15 +431,15 @@
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[LGPLv3][license_link] © 2018-2024
+[LGPLv3][license_link] © 2018-2021
 
 [pip_link]: https://pypi.org/project/gstools
 [conda_link]: https://docs.conda.io/en/latest/miniconda.html
 [conda_forge_link]: https://github.com/conda-forge/gstools-feedstock#installing-gstools
 [conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
 [pipiflag]: https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html?highlight=i#cmdoption-i
 [winpy_link]: https://winpython.github.io/
```

### Comparing `gstools-1.5.2/README.md` & `gstools-1.6.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,15 @@
 <p align="center">
 <img src="https://raw.githubusercontent.com/GeoStat-Framework/GSTools/main/docs/source/pics/pyvista_export.png" alt="pyvista export" width="600px"/>
 </p>
 
 
 ## Requirements:
 
-- [NumPy >= 1.20.0](https://www.numpy.org)
+- [NumPy >= 1.14.5](https://www.numpy.org)
 - [SciPy >= 1.1.0](https://www.scipy.org/scipylib)
 - [hankel >= 1.0.0](https://github.com/steven-murray/hankel)
 - [emcee >= 3.0.0](https://github.com/dfm/emcee)
 - [pyevtk >= 1.1.1](https://github.com/pyscience-projects/pyevtk)
 - [meshio >= 5.1.0](https://github.com/nschloe/meshio)
 
 ### Optional
@@ -362,15 +362,15 @@
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[LGPLv3][license_link] © 2018-2024
+[LGPLv3][license_link] © 2018-2021
 
 [pip_link]: https://pypi.org/project/gstools
 [conda_link]: https://docs.conda.io/en/latest/miniconda.html
 [conda_forge_link]: https://github.com/conda-forge/gstools-feedstock#installing-gstools
 [conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
 [pipiflag]: https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html?highlight=i#cmdoption-i
 [winpy_link]: https://winpython.github.io/
```

#### html2text {}

```diff
@@ -141,23 +141,23 @@
 ```python import gstools as gs x = y = range(100) model = gs.Gaussian(dim=2,
 var=1, len_scale=10) srf = gs.SRF(model) srf((x, y), mesh_type='structured')
 srf.vtk_export("field") # Saves to a VTK file mesh = srf.to_pyvista() # Create
 a VTK/PyVista dataset in memory mesh.plot() ``` Which gives a RectilinearGrid
 VTK file ``field.vtr`` or creates a PyVista mesh in memory for immediate 3D
 plotting in Python.
                                [pyvista export]
-## Requirements: - [NumPy >= 1.20.0](https://www.numpy.org) - [SciPy >= 1.1.0]
+## Requirements: - [NumPy >= 1.14.5](https://www.numpy.org) - [SciPy >= 1.1.0]
 (https://www.scipy.org/scipylib) - [hankel >= 1.0.0](https://github.com/steven-
 murray/hankel) - [emcee >= 3.0.0](https://github.com/dfm/emcee) - [pyevtk >=
 1.1.1](https://github.com/pyscience-projects/pyevtk) - [meshio >= 5.1.0](https:
 //github.com/nschloe/meshio) ### Optional - [GSTools-Core >= 0.2.0](https://
 github.com/GeoStat-Framework/GSTools-Core) - [matplotlib](https://
 matplotlib.org) - [pyvista](https://docs.pyvista.org/) ## Contact You can
 contact us via
-geostat-framework.org>. ## License [LGPLv3][license_link] Â© 2018-2024
+geostat-framework.org>. ## License [LGPLv3][license_link] Â© 2018-2021
 [pip_link]: https://pypi.org/project/gstools [conda_link]: https://
 docs.conda.io/en/latest/miniconda.html [conda_forge_link]: https://github.com/
 conda-forge/gstools-feedstock#installing-gstools [conda_pip]: https://
 docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-
 pkgs.html#installing-non-conda-packages [pipiflag]: https://pip-
 python3.readthedocs.io/en/latest/reference/
 pip_install.html?highlight=i#cmdoption-i [winpy_link]: https://
```

### Comparing `gstools-1.5.2/pyproject.toml` & `gstools-1.6.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = [
     "setuptools>=64",
     "setuptools_scm>=7",
-    "numpy>=2.0.0rc1,<2.3; python_version >= '3.9'",
-    "oldest-supported-numpy; python_version < '3.9'",
-    "Cython>=3.0.10,<3.1.0",
+    "oldest-supported-numpy",
+    "Cython>=3.0",
     "extension-helpers>=1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
 name = "gstools"
@@ -45,40 +44,40 @@
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Utilities",
 ]
 dependencies = [
     "emcee>=3.0.0",
     "hankel>=1.0.0",
     "meshio>=5.1.0",
-    "numpy>=1.20.0",
+    "numpy>=1.14.5",
     "pyevtk>=1.1.1",
     "scipy>=1.1.0",
 ]
 
 [project.optional-dependencies]
 doc = [
     "m2r2>=0.2.8",
-    "matplotlib>=3.7",
+    "matplotlib>=3",
     "meshzoo>=0.7",
     "numpydoc>=1.1",
     "pykrige>=1.5,<2",
-    "pyvista>=0.40",
-    "sphinx>=7",
+    "pyvista>=0.29",
+    "sphinx>=4",
     "sphinx-gallery>=0.8",
-    "sphinx-rtd-theme>=2",
+    "sphinx-rtd-theme>=1,<1.1",
     "sphinxcontrib-youtube>=1.1",
 ]
 plotting = [
-    "matplotlib>=3.7",
-    "pyvista>=0.40",
+    "matplotlib>=3",
+    "pyvista>=0.29",
 ]
 rust = ["gstools_core>=0.2.0,<1"]
 test = ["pytest-cov>=3"]
 lint = [
-    "black>=24",
+    "black",
     "pylint",
     "isort[colors]",
     "cython-lint",
 ]
 
 [project.urls]
 Changelog = "https://github.com/GeoStat-Framework/GSTools/blob/main/CHANGELOG.md"
@@ -158,11 +157,15 @@
     max-attributes = 25
     max-public-methods = 80
 
 [tool.cibuildwheel]
 # Switch to using build
 build-frontend = "build"
 # Disable building PyPy wheels on all platforms, 32bit for py3.10/11/12, musllinux builds, py3.6/7
-skip = ["cp36-*", "cp37-*", "pp*", "*-win32", "*-manylinux_i686", "*-musllinux_*"]
+skip = ["cp36-*", "cp37-*", "pp*", "cp31*-win32", "cp31*-manylinux_i686", "*-musllinux_*"]
 # Run the package tests using `pytest`
 test-extras = "test"
 test-command = "pytest -v {package}/tests"
+# Skip trying to test arm64 builds on Intel Macs
+test-skip = "*-macosx_arm64 *-macosx_universal2:arm64"
+# no wheels for linux-32bit anymore for numpy>=1.22
+environment = "PIP_PREFER_BINARY=1"
```

### Comparing `gstools-1.5.2/setup.py` & `gstools-1.6.0rc1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """GSTools: A geostatistical toolbox."""
-
 import os
 
 import numpy as np
 from Cython.Build import cythonize
 from extension_helpers import add_openmp_flags_if_available
 from setuptools import Extension, setup
 
@@ -14,21 +13,15 @@
         sources=[os.path.join("src", "gstools", *ext.split(".")) + ".pyx"],
         include_dirs=[np.get_include()],
         define_macros=[("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")],
     )
     for ext in ["field.summator", "variogram.estimator", "krige.krigesum"]
 ]
 # you can set GSTOOLS_BUILD_PARALLEL=0 or GSTOOLS_BUILD_PARALLEL=1
-open_mp = False
 if int(os.getenv("GSTOOLS_BUILD_PARALLEL", "0")):
     added = [add_openmp_flags_if_available(mod) for mod in CY_MODULES]
-    if any(added):
-        open_mp = True
-    print(f"## GSTools setup: OpenMP used: {open_mp}")
+    print(f"## GSTools setup: OpenMP used: {any(added)}")
 else:
     print("## GSTools setup: OpenMP not wanted by the user.")
 
 # setup - do not include package data to ignore .pyx files in wheels
-setup(
-    ext_modules=cythonize(CY_MODULES, compile_time_env={"OPENMP": open_mp}),
-    include_package_data=False,
-)
+setup(ext_modules=cythonize(CY_MODULES), include_package_data=False)
```

### Comparing `gstools-1.5.2/src/gstools/__init__.py` & `gstools-1.6.0rc1/src/gstools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
 
 .. autosummary::
    EARTH_RADIUS
    KM_SCALE
    DEGREE_SCALE
    RADIAN_SCALE
 """
-
 # Hooray!
 from gstools import (
     config,
     covmodel,
     field,
     krige,
     normalizer,
```

### Comparing `gstools-1.5.2/src/gstools/covmodel/__init__.py` & `gstools-1.6.0rc1/src/gstools/covmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/src/gstools/covmodel/base.py` & `gstools-1.6.0rc1/src/gstools/covmodel/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .. currentmodule:: gstools.covmodel.base
 
 The following classes are provided
 
 .. autosummary::
    CovModel
 """
-
 # pylint: disable=C0103, R0201, E1101, C0302, W0613
 import copy
 
 import numpy as np
 from hankel import SymmetricFourierTransform as SFT
 from scipy.integrate import quad as integral
```

### Comparing `gstools-1.5.2/src/gstools/covmodel/fit.py` & `gstools-1.6.0rc1/src/gstools/covmodel/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .. currentmodule:: gstools.covmodel.fit
 
 The following classes and functions are provided
 
 .. autosummary::
    fit_variogram
 """
-
 # pylint: disable=C0103, W0632
 import numpy as np
 from scipy.optimize import curve_fit
 
 from gstools.covmodel.tools import check_arg_in_bounds, default_arg_from_bounds
 from gstools.tools.geometric import great_circle_to_chordal, set_anis
 
@@ -210,15 +209,14 @@
         return fit_para, pcov, _r2_score(model, x_data, y_data, is_dir_vario)
     return fit_para, pcov
 
 
 def _pre_para(model, para_select, sill, anis):
     """Preprocess selected parameters."""
     var_last = False
-    var_tmp = 0.0  # init value
     for par in para_select:
         if par not in model.arg_bounds:
             raise ValueError(f"fit: unknown parameter in selection: {par}")
         if not isinstance(para_select[par], bool):
             if par == "var":
                 var_last = True
                 var_tmp = float(para_select[par])
@@ -306,19 +304,17 @@
     )
     # correctly handle given values for anis (need a list of values)
     init_guess["anis"] = list(set_anis(model.dim, init_guess["anis"]))
     # set optional arguments
     for opt in model.opt_arg:
         init_guess.setdefault(
             opt,
-            (
-                default_arg_from_bounds(bnd[opt])
-                if default
-                else getattr(model, opt)
-            ),
+            default_arg_from_bounds(bnd[opt])
+            if default
+            else getattr(model, opt),
         )
     # convert all init guesses to float (except "anis")
     for arg in model.iso_arg:
         init_guess[arg] = float(init_guess[arg])
     return init_guess
 
 
@@ -461,15 +457,14 @@
 
 
 def _post_fitting(model, para, popt, anis, is_dir_vario):
     """Postprocess fitting results and application to model."""
     fit_para = {}
     para_skip = 0
     opt_skip = 0
-    var_tmp = 0.0  # init value
     for par in DEFAULT_PARA:
         if para[par]:
             if par == "var":  # set variance last
                 var_tmp = popt[para_skip]
             else:
                 setattr(model, par, popt[para_skip])
             fit_para[par] = popt[para_skip]
```

### Comparing `gstools-1.5.2/src/gstools/covmodel/models.py` & `gstools-1.6.0rc1/src/gstools/covmodel/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
    Linear
    Circular
    Spherical
    HyperSpherical
    SuperSpherical
    JBessel
 """
-
 # pylint: disable=C0103, E1101, R0201
 import warnings
 
 import numpy as np
 from scipy import special as sps
 
 from gstools.covmodel.base import CovModel
@@ -456,29 +455,29 @@
     def cor(self, h):
         """Exponential Integral normalized correlation function."""
         h = np.asarray(h, dtype=np.double)
         return 0.5 * self.nu * exp_int(1.0 + 0.5 * self.nu, h**2)
 
     def spectral_density(self, k):  # noqa: D102
         k = np.asarray(k, dtype=np.double)
-        fac = (0.5 * self.len_rescaled / np.sqrt(np.pi)) ** self.dim
-        lim = fac * self.nu / (self.nu + self.dim)
+        x = (k * self.len_rescaled / 2.0) ** 2
         # for nu > 50 we just use an approximation of the gaussian model
         if self.nu > 50.0:
-            x = (k * self.len_rescaled / 2) ** 2
-            return lim * np.exp(-x) * (1 + 2 * x / (self.nu + self.dim + 2))
-        # separate calculation at origin
-        s = (self.nu + self.dim) / 2
-        res = np.empty_like(k)
-        k_gz = np.logical_not(np.isclose(k, 0))
-        x = (k[k_gz] * self.len_rescaled / 2) ** 2
-        # limit at k=0 (inc_gamma_low(s, x) / x**s -> 1/s for x -> 0)
-        res[np.logical_not(k_gz)] = lim
-        res[k_gz] = 0.5 * self.nu * fac / x**s * inc_gamma_low(s, x)
-        return res
+            return (
+                (0.5 * self.len_rescaled / np.sqrt(np.pi)) ** self.dim
+                * np.exp(-x)
+                * self.nu
+                / (self.nu + self.dim)
+                * (1.0 + 2 * x / (self.nu + self.dim + 2))
+            )
+        return (
+            self.nu
+            / (x ** (self.nu * 0.5) * 2 * (k * np.sqrt(np.pi)) ** self.dim)
+            * inc_gamma_low((self.nu + self.dim) / 2.0, x)
+        )
 
     def calc_integral_scale(self):  # noqa: D102
         return (
             self.len_rescaled * self.nu * np.sqrt(np.pi) / (2 * self.nu + 2.0)
         )
```

### Comparing `gstools-1.5.2/src/gstools/covmodel/plot.py` & `gstools-1.6.0rc1/src/gstools/covmodel/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
    plot_vario_spatial
    plot_cov_spatial
    plot_cor_spatial
    plot_spectrum
    plot_spectral_density
    plot_spectral_rad_pdf
 """
-
 # pylint: disable=C0103, C0415, E1130
 import numpy as np
 
 from gstools.tools.geometric import generate_grid
 from gstools.tools.misc import get_fig_ax
 
 __all__ = [
```

### Comparing `gstools-1.5.2/src/gstools/covmodel/tools.py` & `gstools-1.6.0rc1/src/gstools/covmodel/tools.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/src/gstools/covmodel/tpl_models.py` & `gstools-1.6.0rc1/src/gstools/covmodel/tpl_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 .. autosummary::
    TPLGaussian
    TPLExponential
    TPLStable
    TPLSimple
 """
-
 # pylint: disable=C0103, E1101
 import warnings
 
 import numpy as np
 
 from gstools.covmodel.base import CovModel
 from gstools.covmodel.tools import AttributeWarning
```

### Comparing `gstools-1.5.2/src/gstools/field/__init__.py` & `gstools-1.6.0rc1/src/gstools/field/__init__.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/src/gstools/field/base.py` & `gstools-1.6.0rc1/src/gstools/field/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .. currentmodule:: gstools.field.base
 
 The following classes are provided
 
 .. autosummary::
    Field
 """
-
 # pylint: disable=C0103, C0415
 from collections.abc import Iterable
 from copy import copy
 from functools import partial
 
 import numpy as np
 
@@ -359,15 +358,15 @@
         """
         Apply field transformation.
 
         Parameters
         ----------
         method : :class:`str`
             Method to use.
-            See :py:mod:`gstools.transform` for available transformations.
+            See :any:`gstools.transform` for available transformations.
         field : :class:`str`, optional
             Name of field to be transformed. The default is "field".
         store : :class:`str` or :class:`bool`, optional
             Whether to store field inplace (True/False) or under a given name.
             The default is True.
         process : :class:`bool`, optional
             Whether to process in/out fields with trend, normalizer and mean
```

### Comparing `gstools-1.5.2/src/gstools/field/cond_srf.py` & `gstools-1.6.0rc1/src/gstools/field/cond_srf.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .. currentmodule:: gstools.field.cond_srf
 
 The following classes are provided
 
 .. autosummary::
    CondSRF
 """
-
 # pylint: disable=C0103, W0231, W0221, W0222, E1102
 
 import numpy as np
 
 from gstools.field.base import Field
 from gstools.field.generator import Generator, RandMeth
 from gstools.krige import Krige
```

### Comparing `gstools-1.5.2/src/gstools/field/generator.py` & `gstools-1.6.0rc1/src/gstools/field/generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,34 +7,39 @@
 
 .. autosummary::
    :toctree:
 
    Generator
    RandMeth
    IncomprRandMeth
+   Fourier
 """
-
 # pylint: disable=C0103, W0222, C0412, W0231
 import warnings
 from abc import ABC, abstractmethod
 from copy import deepcopy as dcp
 
 import numpy as np
 
 from gstools import config
 from gstools.covmodel.base import CovModel
 from gstools.random.rng import RNG
+from gstools.tools.geometric import generate_grid
 
 if config.USE_RUST:  # pragma: no cover
     # pylint: disable=E0401
     from gstools_core import summate, summate_incompr
 else:
-    from gstools.field.summator import summate, summate_incompr
+    from gstools.field.summator import (
+        summate,
+        summate_incompr,
+        summate_fourier,
+    )
 
-__all__ = ["Generator", "RandMeth", "IncomprRandMeth"]
+__all__ = ["Generator", "RandMeth", "IncomprRandMeth", "Fourier"]
 
 
 SAMPLING = ["auto", "inversion", "mcmc"]
 
 
 class Generator(ABC):
     """
@@ -206,17 +211,15 @@
 
         Returns
         -------
         :class:`numpy.ndarray`
             the random modes
         """
         pos = np.asarray(pos, dtype=np.double)
-        summed_modes = summate(
-            self._cov_sample, self._z_1, self._z_2, pos, config.NUM_THREADS
-        )
+        summed_modes = summate(self._cov_sample, self._z_1, self._z_2, pos)
         nugget = self.get_nugget(summed_modes.shape) if add_nugget else 0.0
         return np.sqrt(self.model.var / self._mode_no) * summed_modes + nugget
 
     def get_nugget(self, shape):
         """
         Generate normal distributed values for the nugget simulation.
 
@@ -488,19 +491,15 @@
         Returns
         -------
         :class:`numpy.ndarray`
             the random modes
         """
         pos = np.asarray(pos, dtype=np.double)
         summed_modes = summate_incompr(
-            self._cov_sample,
-            self._z_1,
-            self._z_2,
-            pos,
-            config.NUM_THREADS,
+            self._cov_sample, self._z_1, self._z_2, pos
         )
         nugget = self.get_nugget(summed_modes.shape) if add_nugget else 0.0
         e1 = self._create_unit_vector(summed_modes.shape)
         return (
             self.mean_u * e1
             + self.mean_u
             * np.sqrt(self.model.var / self._mode_no)
@@ -528,7 +527,328 @@
         """
         shape = np.ones(len(broadcast_shape), dtype=int)
         shape[0] = self.model.dim
 
         e1 = np.zeros(shape)
         e1[axis] = 1.0
         return e1
+
+
+class Fourier(Generator):
+    r"""Fourier method for calculating isotropic random fields.
+
+    Parameters
+    ----------
+    model : :any:`CovModel`
+        Covariance model
+    mode_no : :class:`list`
+        Number of Fourier modes per dimension.
+    mode_truncation : :class:`list`
+        Cut-off values of the Fourier modes.
+    period_len : :class:`float` or :class:`list`, optional
+        Period length of the field in each dim as a factor of the domain size.
+    seed : :class:`int`, optional
+        The seed of the random number generator.
+        If "None", a random seed is used. Default: :any:`None`
+    verbose : :class:`bool`, optional
+        Be chatty during the generation.
+        Default: :any:`False`
+
+    **kwargs
+        Placeholder for keyword-args
+
+    Notes
+    -----
+    The Fourier method is used to generate isotropic
+    spatial random fields characterized by a given covariance model.
+    The calculation looks like [Hesse2014]_: # TODO check different source
+
+    .. math::
+       u\left(x\right)=
+       \sqrt{2\sigma^{2}}\cdot
+       \sum_{i=1}^{N}\sqrt{E(k_{i})}\left(
+       Z_{1,i}\cdot\cos\left(2\pi\left\langle k_{i},x\right\rangle \right)+
+       Z_{2,i}\cdot\sin\left(2\pi\left\langle k_{i},x\right\rangle \right)
+       \right) \sqrt{\Delta k}
+
+    where:
+
+        * :math:`N` : fourier mode number
+        * :math:`Z_{j,i}` : random samples from a normal distribution
+        * :math:`k_i` : the equidistant spectral density of the covariance model
+
+    References
+    ----------
+    .. [Hesse2014] Heße, F., Prykhodko, V., Schlüter, S., and Attinger, S.,
+           "Generating random fields with a truncated power-law variogram:
+           A comparison of several numerical methods",
+           Environmental Modelling & Software, 55, 32-48., (2014)
+    """
+
+    def __init__(
+        self,
+        model,
+        modes_no,
+        modes_truncation,
+        period_len=None,
+        seed=None,
+        verbose=False,
+        **kwargs,
+    ):
+        if kwargs:
+            warnings.warn("gstools.Fourier: **kwargs are ignored")
+        # initialize attributes
+        self._modes_truncation = self._fill_to_dim(
+            model.dim, modes_truncation, np.double
+        )
+        self._modes_no = self._fill_to_dim(model.dim, modes_no, int)
+        self._modes = []
+        [
+            self._modes.append(
+                np.linspace(
+                    -self._modes_truncation[d] / 2,
+                    self._modes_truncation[d] / 2,
+                    self._modes_no[d],
+                    endpoint=False,
+                ).T
+            )
+            for d in range(model.dim)
+        ]
+
+        self._period_len = self._fill_to_dim(
+            model.dim, period_len, np.double, 1.0
+        )
+        self._verbose = bool(verbose)
+        # initialize private attributes
+        self._model = None
+        self._seed = None
+        self._rng = None
+        self._z_1 = None
+        self._z_2 = None
+        self._spectral_density_sqrt = None
+        self._value_type = "scalar"
+        # set model and seed
+        self.update(model, seed)
+
+    def __call__(self, pos, add_nugget=True):
+        """Calculate the modes for the Fourier method.
+
+        This method  calls the `summate_*` Cython methods, which are the
+        heart of the randomization method.
+
+        Parameters
+        ----------
+        pos : (d, n), :class:`numpy.ndarray`
+            the position tuple with d dimensions and n points.
+        add_nugget : :class:`bool`
+            Whether to add nugget noise to the field.
+
+        Returns
+        -------
+        :class:`numpy.ndarray`
+            the random modes
+        """
+        pos = np.asarray(pos, dtype=np.double)
+        domain_size = pos.max(axis=1) - pos.min(axis=1)
+        self._modes = [
+            self._modes[d] / domain_size[d] * self._period_len[d]
+            for d in range(self._model.dim)
+        ]
+
+        self._modes = generate_grid(self._modes)
+
+        # pre calc. the spectral density for all wave numbers
+        # they are handed over to Cython
+        k_norm = np.linalg.norm(self._modes, axis=0)
+        self._spectral_density_sqrt = np.sqrt(
+            self._model.spectral_density(k_norm)
+        )
+        summed_modes = summate_fourier(
+            self._spectral_density_sqrt,
+            self._modes,
+            self._z_1,
+            self._z_2,
+            pos,
+        )
+        nugget = self.get_nugget(summed_modes.shape) if add_nugget else 0.0
+        return (
+            np.sqrt(2.0 * self.model.var / np.prod(domain_size)) * summed_modes
+            + nugget
+        )
+
+    def get_nugget(self, shape):
+        """
+        Generate normal distributed values for the nugget simulation.
+
+        Parameters
+        ----------
+        shape : :class:`tuple`
+            the shape of the summed modes
+
+        Returns
+        -------
+        nugget : :class:`numpy.ndarray`
+            the nugget in the same shape as the summed modes
+        """
+        if self.model.nugget > 0:
+            nugget = np.sqrt(self.model.nugget) * self._rng.random.normal(
+                size=shape
+            )
+        else:
+            nugget = 0.0
+        return nugget
+
+    def update(self, model=None, seed=np.nan):
+        """Update the model and the seed.
+
+        If model and seed are not different, nothing will be done.
+
+        Parameters
+        ----------
+        model : :any:`CovModel` or :any:`None`, optional
+            covariance model. Default: :any:`None`
+        seed : :class:`int` or :any:`None` or :any:`numpy.nan`, optional
+            the seed of the random number generator.
+            If :any:`None`, a random seed is used. If :any:`numpy.nan`,
+            the actual seed will be kept. Default: :any:`numpy.nan`
+        """
+        # check if a new model is given
+        if isinstance(model, CovModel):
+            if self.model != model:
+                self._model = dcp(model)
+                if seed is None or not np.isnan(seed):
+                    self.reset_seed(seed)
+                else:
+                    self.reset_seed(self._seed)
+            # just update the seed, if its a new one
+            elif seed is None or not np.isnan(seed):
+                self.seed = seed
+        # or just update the seed, when no model is given
+        elif model is None and (seed is None or not np.isnan(seed)):
+            if isinstance(self._model, CovModel):
+                self.seed = seed
+            else:
+                raise ValueError(
+                    "gstools.field.generator.RandMeth: no 'model' given"
+                )
+        # if the user tries to trick us, we beat him!
+        elif model is None and np.isnan(seed):
+            if (
+                isinstance(self._model, CovModel)
+                and self._z_1 is not None
+                and self._z_2 is not None
+                and self._spectral_density_sqrt is not None
+            ):
+                if self.verbose:
+                    print("RandMeth.update: Nothing will be done...")
+            else:
+                raise ValueError(
+                    "gstools.field.generator.RandMeth: "
+                    "neither 'model' nor 'seed' given!"
+                )
+        # wrong model type
+        else:
+            raise ValueError(
+                "gstools.field.generator.RandMeth: 'model' is not an "
+                "instance of 'gstools.CovModel'"
+            )
+
+    def reset_seed(self, seed=np.nan):
+        """
+        Recalculate the random values with the given seed.
+
+        Parameters
+        ----------
+        seed : :class:`int` or :any:`None` or :any:`numpy.nan`, optional
+            the seed of the random number generator.
+            If :any:`None`, a random seed is used. If :any:`numpy.nan`,
+            the actual seed will be kept. Default: :any:`numpy.nan`
+
+        Notes
+        -----
+        Even if the given seed is the present one, modes will be recalculated.
+        """
+        if seed is None or not np.isnan(seed):
+            self._seed = seed
+        self._rng = RNG(self._seed)
+        # normal distributed samples for randmeth
+        self._z_1 = self._rng.random.normal(size=np.prod(self._modes_no))
+        self._z_2 = self._rng.random.normal(size=np.prod(self._modes_no))
+
+    def _fill_to_dim(self, dim, values, dtype, default_value=None):
+        """Fill an array with last element up to len(dim)."""
+        r = values
+        if values is None:
+            if default_value is None:
+                raise ValueError(f"Fourier: Value has to be provided")
+            r = default_value
+        r = np.array(r, dtype=dtype)
+        r = np.atleast_1d(r)[:dim]
+        if len(r) > dim:
+            raise ValueError(f"Fourier: len(values) <= {dim=} not fulfilled")
+        # fill up values with values[-1], such that len()==dim
+        if len(r) < dim:
+            r = np.pad(r, (0, dim - len(r)), "edge")
+        return r
+
+    @property
+    def seed(self):
+        """:class:`int`: Seed of the master RNG.
+
+        Notes
+        -----
+        If a new seed is given, the setter property not only saves the
+        new seed, but also creates new random modes with the new seed.
+        """
+        return self._seed
+
+    @seed.setter
+    def seed(self, new_seed):
+        if new_seed is not self._seed:
+            self.reset_seed(new_seed)
+
+    @property
+    def model(self):
+        """:any:`CovModel`: Covariance model of the spatial random field."""
+        return self._model
+
+    @model.setter
+    def model(self, model):
+        self.update(model)
+
+    @property
+    def modes_truncation(self):
+        """:class:`list`: Cut-off values of the Fourier modes."""
+        return self._modes_truncation
+
+    @modes_truncation.setter
+    def modes_truncation(self, modes_truncation):
+        self._modes_truncation = modes_truncation
+
+    @property
+    def period_len(self):
+        """:class:`list`: Period length of the field in each dim."""
+        return self._period_len
+
+    @period_len.setter
+    def period_len(self, period_len):
+        self._period_len = self._fill_to_dim(
+            self._model.dim, period_len, np.double, 1.0
+        )
+
+    @property
+    def verbose(self):
+        """:class:`bool`: Verbosity of the generator."""
+        return self._verbose
+
+    @verbose.setter
+    def verbose(self, verbose):
+        self._verbose = bool(verbose)
+
+    @property
+    def value_type(self):
+        """:class:`str`: Type of the field values (scalar, vector)."""
+        return self._value_type
+
+    def __repr__(self):
+        """Return String representation."""
+        return f"{self.name}(model={self.model}, seed={self.seed})"
```

### Comparing `gstools-1.5.2/src/gstools/field/plot.py` & `gstools-1.6.0rc1/src/gstools/field/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 The following classes and functions are provided
 
 .. autosummary::
    plot_field
    plot_vec_field
 """
-
-# pylint: disable=C0103, W0613, E1101, E0606
+# pylint: disable=C0103, W0613, E1101
 import numpy as np
 from scipy import interpolate as inter
 from scipy.spatial import ConvexHull
 
 from gstools.tools.geometric import rotation_planes
 from gstools.tools.misc import get_fig_ax
 
@@ -228,14 +227,21 @@
     # create radio buttons
     if dim > 2:
         rax = fig.add_axes(
             [0.05, 0.85 - 2 * s_frac, 0.15, 2 * s_frac], frame_on=0, alpha=0
         )
         rax.set_title("  Plane", loc="left")
         radio = RadioButtons(rax, plane_names, activecolor="grey")
+        # make radio buttons circular
+        rpos = rax.get_position().get_points()
+        fh, fw = fig.get_figheight(), fig.get_figwidth()
+        rscale = (rpos[:, 1].ptp() / rpos[:, 0].ptp()) * (fh / fw)
+        for circ in radio.circles:
+            circ.set_radius(0.06)
+            circ.height /= rscale
     elif mesh_type == "unstructured" and convex_hull:
         # show convex hull in 2D
         hull = ConvexHull(pos.T)
         for simplex in hull.simplices:
             ax.plot(pos[0, simplex], pos[1, simplex], "k")
     # init imshow and colorbar axis
     grid = np.mgrid[0 : 1 : resolution * 1j, 0 : 1 : resolution * 1j]
@@ -280,15 +286,14 @@
             s.valinit = ax_ends[i][0] + ax_rngs[i] / 2.0
             s.valstep = ax_steps[i]
             s.ax.set_xlim(*ax_ends[i])
             # update representation
             s.vline.set_data(2 * [s.valinit], [-0.1, 1.1])
             s.reset()
         im.set_extent(ax_extents[p])
-        asp = 1.0  # init value
         if aspect == "quad":
             asp = ax_rngs[planes[p][0]] / ax_rngs[planes[p][1]]
         if aspect is not None:
             ax.set_aspect(asp if aspect == "quad" else aspect)
         ax.set_xlabel(ax_names[planes[p][0]])
         ax.set_ylabel(ax_names[planes[p][1]])
         update_field()
```

### Comparing `gstools-1.5.2/src/gstools/field/srf.py` & `gstools-1.6.0rc1/src/gstools/field/srf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 .. currentmodule:: gstools.field.srf
 
 The following classes are provided
 
 .. autosummary::
    SRF
 """
-
 # pylint: disable=C0103, W0221, E1102
 
 import numpy as np
 
 from gstools.field.base import Field
-from gstools.field.generator import Generator, IncomprRandMeth, RandMeth
+from gstools.field.generator import (
+    Generator,
+    IncomprRandMeth,
+    RandMeth,
+    Fourier,
+)
 from gstools.field.upscaling import var_coarse_graining, var_no_scaling
 
 __all__ = ["SRF"]
 
 GENERATOR = {
     "RandMeth": RandMeth,
     "IncomprRandMeth": IncomprRandMeth,
     "VectorField": IncomprRandMeth,
     "VelocityField": IncomprRandMeth,
+    "Fourier": Fourier,
 }
 """dict: Standard generators for spatial random fields."""
 
 UPSCALING = {
     "coarse_graining": var_coarse_graining,
     "no_scaling": var_no_scaling,
 }
@@ -71,14 +76,15 @@
             * "RandMeth" : The Randomization Method.
               See: :any:`RandMeth`
             * "IncomprRandMeth" : The incompressible Randomization Method.
               This is the original algorithm proposed by Kraichnan 1970
               See: :any:`IncomprRandMeth`
             * "VectorField" : an alias for "IncomprRandMeth"
             * "VelocityField" : an alias for "IncomprRandMeth"
+            * "Fourier" : the periodic Fourier method
 
         Default: "RandMeth"
     **generator_kwargs
         Keyword arguments that are forwarded to the generator in use.
         Have a look at the provided generators for further information.
     """
 
@@ -138,14 +144,19 @@
             The default is :any:`True` for default name "field".
 
         Returns
         -------
         field : :class:`numpy.ndarray`
             the SRF
         """
+        if isinstance(self.generator, Fourier) and mesh_type != "structured":
+            raise ValueError(
+                f"SRF: Fourier generator only defined for "
+                'mesh_type == "structured".'
+            )
         name, save = self.get_store_config(store)
         # update the model/seed in the generator if any changes were made
         self.generator.update(self.model, seed)
         # get isometrized positions and the resulting field-shape
         iso_pos, shape = self.pre_pos(pos, mesh_type)
         # generate the field
         field = np.reshape(self.generator(iso_pos), shape)
```

### Comparing `gstools-1.5.2/src/gstools/field/summator.pyx` & `gstools-1.6.0rc1/src/gstools/field/summator.pyx`

 * *Files 23% similar despite different names*

```diff
@@ -2,53 +2,34 @@
 """
 This is the randomization method summator, implemented in cython.
 """
 
 import numpy as np
 from cython.parallel import prange
 
-IF OPENMP:
-    cimport openmp
-
 cimport numpy as np
-from libc.math cimport cos, sin
-
-
-def set_num_threads(num_threads):
-    cdef int num_threads_c = 1
-    if num_threads is None:
-        # OPENMP set during setup
-        IF OPENMP:
-            num_threads_c = openmp.omp_get_num_procs()
-        ELSE:
-            ...
-    else:
-        num_threads_c = num_threads
-    return num_threads_c
+from libc.math cimport pi, cos, sin, sqrt
 
 
 def summate(
     const double[:, :] cov_samples,
     const double[:] z_1,
     const double[:] z_2,
-    const double[:, :] pos,
-    num_threads=None,
+    const double[:, :] pos
 ):
     cdef int i, j, d
     cdef double phase
     cdef int dim = pos.shape[0]
 
     cdef int X_len = pos.shape[1]
     cdef int N = cov_samples.shape[1]
 
     cdef double[:] summed_modes = np.zeros(X_len, dtype=float)
 
-    cdef int num_threads_c = set_num_threads(num_threads)
-
-    for i in prange(X_len, nogil=True, num_threads=num_threads_c):
+    for i in prange(X_len, nogil=True):
         for j in range(N):
             phase = 0.
             for d in range(dim):
                 phase += cov_samples[d, j] * pos[d, i]
             summed_modes[i] += z_1[j] * cos(phase) + z_2[j] * sin(phase)
 
     return np.asarray(summed_modes)
@@ -64,16 +45,15 @@
     return r
 
 
 def summate_incompr(
     const double[:, :] cov_samples,
     const double[:] z_1,
     const double[:] z_2,
-    const double[:, :] pos,
-    num_threads=None,
+    const double[:, :] pos
 ):
     cdef int i, j, d
     cdef double phase
     cdef double k_2
     cdef int dim = pos.shape[0]
 
     cdef double[:] e1 = np.zeros(dim, dtype=float)
@@ -93,7 +73,35 @@
                 phase += cov_samples[d, j] * pos[d, i]
             for d in range(dim):
                 proj[d] = e1[d] - cov_samples[d, j] * cov_samples[0, j] / k_2
                 summed_modes[d, i] += (
                     proj[d] * (z_1[j] * cos(phase) + z_2[j] * sin(phase))
                 )
     return np.asarray(summed_modes)
+
+
+def summate_fourier(
+    const double[:] spectral_density_sqrt,
+    const double[:, :] modes,
+    const double[:] z_1,
+    const double[:] z_2,
+    const double[:, :] pos
+    ):
+    cdef int i, j, d
+    cdef double phase
+    cdef int dim = pos.shape[0]
+
+    cdef int X_len = pos.shape[1]
+    cdef int N = modes.shape[1]
+
+    cdef double[:] summed_modes = np.zeros(X_len, dtype=float)
+
+    for i in prange(X_len, nogil=True):
+        for j in range(N):
+            phase = 0.
+            for d in range(dim):
+                phase += modes[d, j] * pos[d, i]
+            # OpenMP doesn't like *= after +=... seems to be a compiler specific thing
+            phase = phase * 2. * pi
+            summed_modes[i] += spectral_density_sqrt[j] * (z_1[j] * cos(phase) + z_2[j] * sin(phase))
+
+    return np.asarray(summed_modes)
```

### Comparing `gstools-1.5.2/src/gstools/field/tools.py` & `gstools-1.6.0rc1/src/gstools/field/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 The following classes and functions are provided
 
 .. autosummary::
    fmt_mean_norm_trend
    to_vtk_helper
    generate_on_mesh
 """
-
 # pylint: disable=W0212, C0415
 import meshio
 import numpy as np
 
 from gstools.normalizer import Normalizer
 from gstools.tools.export import to_vtk, vtk_export
 from gstools.tools.misc import list_format
```

### Comparing `gstools-1.5.2/src/gstools/field/upscaling.py` & `gstools-1.6.0rc1/src/gstools/field/upscaling.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 .. autosummary::
    :toctree:
 
    var_coarse_graining
    var_no_scaling
 """
-
 # pylint: disable=W0613
 import warnings
 
 import numpy as np
 
 __all__ = ["var_coarse_graining", "var_no_scaling"]
```

### Comparing `gstools-1.5.2/src/gstools/krige/base.py` & `gstools-1.6.0rc1/src/gstools/krige/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .. currentmodule:: gstools.krige.base
 
 The following classes are provided
 
 .. autosummary::
    Krige
 """
-
 # pylint: disable=C0103, W0221, E1102, R0201, C0412
 import collections
 
 import numpy as np
 import scipy.linalg as spl
 from scipy.spatial.distance import cdist
 
@@ -333,15 +332,14 @@
     def _get_krige_vecs(
         self, pos, chunk_slice=(0, None), ext_drift=None, only_mean=False
     ):
         """Calculate the RHS of the kriging equation."""
         # determine the chunk size
         chunk_size = len(pos[0]) if chunk_slice[1] is None else chunk_slice[1]
         chunk_size -= chunk_slice[0]
-        chunk_pos = None  # init value
         res = np.empty((self.krige_size, chunk_size), dtype=np.double)
         if only_mean:
             # set points to limit of the covariance to only get the mean
             res[: self.cond_no, :] = 0
         else:
             # get correct covariance functions (depending on exact values)
             cf = self.model.cov_nugget if self.exact else self.model.covariance
@@ -381,15 +379,17 @@
 
         Returns
         -------
         ext_drift : :class:`numpy.ndarray` or :any:`None`
             the drift values at the given positions
         """
         if ext_drift is not None:
-            ext_drift = np.atleast_2d(np.asarray(ext_drift, dtype=np.double))
+            ext_drift = np.array(
+                ext_drift, dtype=np.double, ndmin=2, copy=False
+            )
             if ext_drift.size == 0:  # treat empty array as no ext_drift
                 return np.array([])
             if set_cond:
                 if len(ext_drift.shape) > 2 or ext_drift.shape[1] != pnt_cnt:
                     raise ValueError("Krige: wrong number of ext. drifts.")
                 return ext_drift
             ext_shape = np.shape(ext_drift)
```

### Comparing `gstools-1.5.2/src/gstools/krige/krigesum.pyx` & `gstools-1.6.0rc1/src/gstools/krige/krigesum.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -2,83 +2,61 @@
 """
 This is a summator for the kriging routines
 """
 
 import numpy as np
 from cython.parallel import prange
 
-IF OPENMP:
-    cimport openmp
-
 cimport numpy as np
 
 
-def set_num_threads(num_threads):
-    cdef int num_threads_c = 1
-    if num_threads is None:
-        # OPENMP set during setup
-        IF OPENMP:
-            num_threads_c = openmp.omp_get_num_procs()
-        ELSE:
-            ...
-    else:
-        num_threads_c = num_threads
-    return num_threads_c
-
-
 def calc_field_krige_and_variance(
     const double[:, :] krig_mat,
     const double[:, :] krig_vecs,
-    const double[:] cond,
-    num_threads=None,
+    const double[:] cond
 ):
 
     cdef int mat_i = krig_mat.shape[0]
     cdef int res_i = krig_vecs.shape[1]
 
     cdef double[:] field = np.zeros(res_i)
     cdef double[:] error = np.zeros(res_i)
     cdef double krig_fac
 
     cdef int i, j, k
 
-    cdef int num_threads_c = set_num_threads(num_threads)
-
     # error = krig_vecs * krig_mat * krig_vecs
     # field = cond * krig_mat * krig_vecs
-    for k in prange(res_i, nogil=True, num_threads=num_threads_c):
+    for k in prange(res_i, nogil=True):
         for i in range(mat_i):
             krig_fac = 0.0
             for j in range(mat_i):
                 krig_fac += krig_mat[i, j] * krig_vecs[j, k]
             error[k] += krig_vecs[i, k] * krig_fac
             field[k] += cond[i] * krig_fac
 
     return np.asarray(field), np.asarray(error)
 
 
 def calc_field_krige(
     const double[:, :] krig_mat,
     const double[:, :] krig_vecs,
-    const double[:] cond,
-    const int num_threads=1,
+    const double[:] cond
 ):
 
     cdef int mat_i = krig_mat.shape[0]
     cdef int res_i = krig_vecs.shape[1]
 
     cdef double[:] field = np.zeros(res_i)
     cdef double krig_fac
 
     cdef int i, j, k
 
-    cdef int num_threads_c = set_num_threads(num_threads)
-
     # field = cond * krig_mat * krig_vecs
-    for k in prange(res_i, nogil=True, num_threads=num_threads_c):
+    for k in prange(res_i, nogil=True):
         for i in range(mat_i):
             krig_fac = 0.0
             for j in range(mat_i):
                 krig_fac += krig_mat[i, j] * krig_vecs[j, k]
             field[k] += cond[i] * krig_fac
 
     return np.asarray(field)
```

### Comparing `gstools-1.5.2/src/gstools/krige/methods.py` & `gstools-1.6.0rc1/src/gstools/krige/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 .. autosummary::
    Simple
    Ordinary
    Universal
    ExtDrift
    Detrended
 """
-
 # pylint: disable=C0103
 from gstools.krige.base import Krige
 
 __all__ = ["Simple", "Ordinary", "Universal", "ExtDrift", "Detrended"]
 
 
 class Simple(Krige):
```

### Comparing `gstools-1.5.2/src/gstools/krige/tools.py` & `gstools-1.6.0rc1/src/gstools/krige/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 The following classes and functions are provided
 
 .. autosummary::
    set_condition
    get_drift_functions
 """
-
 # pylint: disable=C0103
 from itertools import combinations_with_replacement
 
 import numpy as np
 
 __all__ = ["set_condition", "get_drift_functions"]
```

### Comparing `gstools-1.5.2/src/gstools/normalizer/__init__.py` & `gstools-1.6.0rc1/src/gstools/normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/src/gstools/normalizer/base.py` & `gstools-1.6.0rc1/src/gstools/normalizer/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .. currentmodule:: gstools.normalizer.base
 
 The following classes are provided
 
 .. autosummary::
    Normalizer
 """
-
 # pylint: disable=R0201
 import warnings
 
 import numpy as np
 import scipy.misc as spm
 import scipy.optimize as spo
```

### Comparing `gstools-1.5.2/src/gstools/normalizer/methods.py` & `gstools-1.6.0rc1/src/gstools/normalizer/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
    LogNormal
    BoxCox
    BoxCoxShift
    YeoJohnson
    Modulus
    Manly
 """
-
 # pylint: disable=E1101
 import numpy as np
 
 from gstools.normalizer.base import Normalizer
 
 
 class LogNormal(Normalizer):
```

### Comparing `gstools-1.5.2/src/gstools/normalizer/tools.py` & `gstools-1.6.0rc1/src/gstools/normalizer/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 The following classes and functions are provided
 
 .. autosummary::
    apply_mean_norm_trend
    remove_trend_norm_mean
 """
-
 import numpy as np
 
 from gstools.normalizer.base import Normalizer
 from gstools.tools.geometric import (
     format_struct_pos_shape,
     format_unstruct_pos_shape,
 )
```

### Comparing `gstools-1.5.2/src/gstools/random/rng.py` & `gstools-1.6.0rc1/src/gstools/random/rng.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .. currentmodule:: gstools.random.rng
 
 The following classes are provided
 
 .. autosummary::
    RNG
 """
-
 # pylint: disable=E1101
 import emcee as mc
 import numpy as np
 import numpy.random as rand
 from emcee.state import State
 
 from gstools.random.tools import MasterRNG, dist_gen
@@ -82,15 +81,15 @@
         # sample_size needs to be integer for emcee >= 3.1
         sample_size = int(sample_size)
         # initial guess
         init_guess = (
             self.random.rand(nwalkers).reshape((nwalkers, 1)) * sample_around
         )
         # initialize the sampler
-        sampler = mc.EnsembleSampler(nwalkers, 1, ln_pdf, vectorize=True)
+        sampler = mc.EnsembleSampler(nwalkers, 1, ln_pdf)
         # burn in phase with saving of last position
         initial_state = State(init_guess, copy=True)
         initial_state.random_state = self.random.get_state()
         burn_in_state = sampler.run_mcmc(
             initial_state=initial_state, nsteps=burn_in
         )
         # reset after burn_in
```

### Comparing `gstools-1.5.2/src/gstools/random/tools.py` & `gstools-1.6.0rc1/src/gstools/random/tools.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/src/gstools/tools/__init__.py` & `gstools-1.6.0rc1/src/gstools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/src/gstools/tools/export.py` & `gstools-1.6.0rc1/src/gstools/tools/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
    vtk_export
    vtk_export_structured
    vtk_export_unstructured
    to_vtk
    to_vtk_structured
    to_vtk_unstructured
 """
-
 # pylint: disable=C0103, E1101
 import numpy as np
 from pyevtk.hl import gridToVTK, pointsToVTK
 
 try:
     import pyvista as pv
 except ImportError:
```

### Comparing `gstools-1.5.2/src/gstools/tools/geometric.py` & `gstools-1.6.0rc1/src/gstools/tools/geometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
    format_unstruct_pos_shape
    ang2dir
    latlon2pos
    pos2latlon
    chordal_to_great_circle
    great_circle_to_chordal
 """
-
 # pylint: disable=C0103
 import numpy as np
 
 __all__ = [
     "set_angles",
     "set_anis",
     "no_of_angles",
@@ -380,15 +379,15 @@
     -----
         Time dimension will be the last one.
     """
     time = np.asarray(time, dtype=np.double).reshape(-1)
     if mesh_type != "unstructured":
         pos = generate_grid(pos)
     else:
-        pos = np.atleast_2d(np.asarray(pos, dtype=np.double))
+        pos = np.array(pos, dtype=np.double, ndmin=2, copy=False)
     out = [np.repeat(p.reshape(-1), np.size(time)) for p in pos]
     out.append(np.tile(time, np.size(pos[0])))
     return np.asarray(out, dtype=np.double)
 
 
 # conversion ##################################################################
 
@@ -549,15 +548,15 @@
     # some help from the given shape
     shape_size = np.prod(shape)
     stacked_shape_size = np.prod(shape[1:])
     wrong_shape = False
     # now we try to be smart
     pre_len = len(np.atleast_1d(pos))
     # care about 1D: pos can be given as 1D array here -> convert to 2D array
-    pos = np.atleast_2d(np.asarray(pos, dtype=np.double))
+    pos = np.array(pos, dtype=np.double, ndmin=2, copy=False)
     post_len = len(pos)
     # first array dimension should be spatial dimension (1D is special case)
     dim = post_len if pre_len == post_len else 1
     pnt_cnt = pos[0].size
     # case: 1D unstacked
     if dim == 1 and pos.size == shape_size:
         shape = (1, pos.size) if check_stacked_shape else (pos.size,)
@@ -603,15 +602,15 @@
 
     Returns
     -------
     :class:`numpy.ndarray`
         the array of direction vectors
     """
     pre_dim = np.asanyarray(angles).ndim
-    angles = np.atleast_2d(np.asarray(angles, dtype=dtype))
+    angles = np.array(angles, ndmin=2, dtype=dtype, copy=False)
     if len(angles.shape) > 2:
         raise ValueError(f"Can't interpret angles array {angles}")
     dim = angles.shape[1] + 1 if dim is None else dim
     if dim == 2 and angles.shape[0] == 1 and pre_dim < 2:
         # fix for 2D where only one angle per direction is given
         angles = angles.T  # can't be interpreted if dim=None is given
     if dim != angles.shape[1] + 1 or dim == 1:
```

### Comparing `gstools-1.5.2/src/gstools/tools/misc.py` & `gstools-1.6.0rc1/src/gstools/tools/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 The following functions are provided
 
 .. autosummary::
    get_fig_ax
    list_format
    eval_func
 """
-
 # pylint: disable=C0103, C0415
 import numpy as np
 
 from gstools.tools.geometric import format_struct_pos_dim, generate_grid
 
 __all__ = ["get_fig_ax", "list_format", "eval_func"]
```

### Comparing `gstools-1.5.2/src/gstools/tools/special.py` & `gstools-1.6.0rc1/src/gstools/tools/special.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
    inc_gamma_low
    exp_int
    inc_beta
    tplstable_cor
    tpl_exp_spec_dens
    tpl_gau_spec_dens
 """
-
 # pylint: disable=C0103, E1101
 import numpy as np
 from scipy import special as sps
 
 __all__ = [
     "confidence_scaling",
     "inc_gamma",
```

### Comparing `gstools-1.5.2/src/gstools/transform/__init__.py` & `gstools-1.6.0rc1/src/gstools/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/src/gstools/transform/array.py` & `gstools-1.6.0rc1/src/gstools/transform/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
    array_zinnharvey
    array_force_moments
    array_to_lognormal
    array_to_uniform
    array_to_arcsin
    array_to_uquad
 """
-
 # pylint: disable=C0103, C0123, R0911
 from warnings import warn
 
 import numpy as np
 from scipy.special import erf, erfinv
 
 __all__ = [
```

### Comparing `gstools-1.5.2/src/gstools/transform/field.py` & `gstools-1.6.0rc1/src/gstools/transform/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
    zinnharvey
    normal_force_moments
    normal_to_lognormal
    normal_to_uniform
    normal_to_arcsin
    normal_to_uquad
 """
-
 # pylint: disable=C0103, C0123, R0911, R1735
 import numpy as np
 
 from gstools.normalizer import (
     Normalizer,
     apply_mean_norm_trend,
     remove_trend_norm_mean,
@@ -108,15 +107,15 @@
 
     Parameters
     ----------
     fld : :any:`Field`
         Field class containing a generated field.
     method : :class:`str`
         Method to use.
-        See :py:mod:`gstools.transform` for available transformations.
+        See :any:`gstools.transform` for available transformations.
     field : :class:`str`, optional
         Name of field to be transformed. The default is "field".
     store : :class:`str` or :class:`bool`, optional
         Whether to store field inplace (True/False) or with a specified name.
         The default is True.
     process : :class:`bool`, optional
         Whether to process in/out fields with trend, normalizer and mean
@@ -258,15 +257,16 @@
     Returns
     -------
     :class:`numpy.ndarray`
         Transformed field.
     """
     if not process and divide is None:
         _check_for_default_normal(fld)
-    mean = 0.0 if process and not keep_mean else fld.mean
+    if divide is None:
+        mean = 0.0 if process and not keep_mean else fld.mean
     divide = mean if divide is None else divide
     upper = mean + np.sqrt(fld.model.sill) if upper is None else upper
     lower = mean - np.sqrt(fld.model.sill) if lower is None else lower
     kw = dict(
         values=[lower, upper],
         thresholds=[divide],
     )
```

### Comparing `gstools-1.5.2/src/gstools/variogram/__init__.py` & `gstools-1.6.0rc1/src/gstools/variogram/__init__.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/src/gstools/variogram/binning.py` & `gstools-1.6.0rc1/src/gstools/variogram/binning.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .. currentmodule:: gstools.variogram.binning
 
 The following functions are provided
 
 .. autosummary::
    standard_bins
 """
-
 import numpy as np
 
 from gstools.tools import RADIAN_SCALE
 from gstools.tools.geometric import (
     chordal_to_great_circle,
     format_struct_pos_dim,
     generate_grid,
```

### Comparing `gstools-1.5.2/src/gstools/variogram/estimator.pyx` & `gstools-1.6.0rc1/src/gstools/variogram/estimator.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,18 @@
 """
 This is the variogram estimater, implemented in cython.
 """
 
 import numpy as np
 from cython.parallel import parallel, prange
 
-IF OPENMP:
-    cimport openmp
-
 cimport numpy as np
 from libc.math cimport M_PI, acos, atan2, cos, fabs, isnan, pow, sin, sqrt
 
 
-def set_num_threads(num_threads):
-    cdef int num_threads_c = 1
-    if num_threads is None:
-        # OPENMP set during setup
-        IF OPENMP:
-            num_threads_c = openmp.omp_get_num_procs()
-        ELSE:
-            ...
-    else:
-        num_threads_c = num_threads
-    return num_threads_c
-
-
 cdef inline double dist_euclid(
     const int dim,
     const double[:, :] pos,
     const int i,
     const int j,
 ) nogil:
     cdef int d
@@ -112,59 +96,59 @@
 cdef inline double estimator_cressie(const double f_diff) nogil:
     return sqrt(fabs(f_diff))
 
 ctypedef double (*_estimator_func)(const double) nogil
 
 cdef inline void normalization_matheron(
     double[:] variogram,
-    np.int64_t[:] counts,
+    long[:] counts,
 ):
     cdef int i
     for i in range(variogram.shape[0]):
         # avoid division by zero
         variogram[i] /= (2. * max(counts[i], 1))
 
 cdef inline void normalization_cressie(
     double[:] variogram,
-    np.int64_t[:] counts,
+    long[:] counts,
 ):
     cdef int i
-    cdef np.int64_t cnt
+    cdef long cnt
     for i in range(variogram.shape[0]):
         # avoid division by zero
         cnt = max(counts[i], 1)
         variogram[i] = (
             0.5 * (1./cnt * variogram[i])**4 /
             (0.457 + 0.494 / cnt + 0.045 / cnt**2)
         )
 
 ctypedef void (*_normalization_func)(
     double[:],
-    np.int64_t[:],
+    long[:],
 )
 
 cdef inline void normalization_matheron_vec(
     double[:, :] variogram,
-    np.int64_t[:, :] counts,
+    long[:, :] counts,
 ):
     cdef int d
     for d in range(variogram.shape[0]):
         normalization_matheron(variogram[d, :], counts[d, :])
 
 cdef inline void normalization_cressie_vec(
     double[:, :] variogram,
-    np.int64_t[:, :] counts,
+    long[:, :] counts,
 ):
     cdef int d
     for d in range(variogram.shape[0]):
         normalization_cressie(variogram[d, :], counts[d, :])
 
 ctypedef void (*_normalization_func_vec)(
     double[:, :],
-    np.int64_t[:, :],
+    long[:, :],
 )
 
 cdef _estimator_func choose_estimator_func(str estimator_type):
     cdef _estimator_func estimator_func
     if estimator_type == 'm':
         estimator_func = estimator_matheron
     else:  # estimator_type == 'c'
@@ -193,15 +177,14 @@
     const double[:] bin_edges,
     const double[:, :] pos,
     const double[:, :] direction,  # should be normed
     const double angles_tol=M_PI/8.0,
     const double bandwidth=-1.0,  # negative values to turn of bandwidth search
     const bint separate_dirs=False,  # whether the direction bands don't overlap
     str estimator_type='m',
-    num_threads=None,
 ):
     if pos.shape[1] != f.shape[1]:
         raise ValueError(f'len(pos) = {pos.shape[1]} != len(f) = {f.shape[1])}')
 
     if bin_edges.shape[0] < 2:
         raise ValueError('len(bin_edges) too small')
 
@@ -217,21 +200,19 @@
     cdef int d_max = direction.shape[0]
     cdef int i_max = bin_edges.shape[0] - 1
     cdef int j_max = pos.shape[1] - 1
     cdef int k_max = pos.shape[1]
     cdef int f_max = f.shape[0]
 
     cdef double[:, :] variogram = np.zeros((d_max, len(bin_edges)-1))
-    cdef np.int64_t[:, :] counts = np.zeros((d_max, len(bin_edges)-1), dtype=np.int64)
+    cdef long[:, :] counts = np.zeros((d_max, len(bin_edges)-1), dtype=long)
     cdef int i, j, k, m, d
     cdef double dist
 
-    cdef int num_threads_c = set_num_threads(num_threads)
-
-    for i in prange(i_max, nogil=True, num_threads=num_threads_c):
+    for i in prange(i_max, nogil=True):
         for j in range(j_max):
             for k in range(j+1, k_max):
                 dist = dist_euclid(dim, pos, j, k)
                 if dist < bin_edges[i] or dist >= bin_edges[i+1]:
                     continue  # skip if not in current bin
                 for d in range(d_max):
                     if not dir_test(
@@ -254,15 +235,14 @@
 
 def unstructured(
     const double[:, :] f,
     const double[:] bin_edges,
     const double[:, :] pos,
     str estimator_type='m',
     str distance_type='e',
-    num_threads=None,
 ):
     cdef int dim = pos.shape[0]
     cdef _dist_func distance
 
     if distance_type == 'e':
         distance = dist_euclid
     else:
@@ -283,21 +263,19 @@
 
     cdef int i_max = bin_edges.shape[0] - 1
     cdef int j_max = pos.shape[1] - 1
     cdef int k_max = pos.shape[1]
     cdef int f_max = f.shape[0]
 
     cdef double[:] variogram = np.zeros(len(bin_edges)-1)
-    cdef np.int64_t[:] counts = np.zeros(len(bin_edges)-1, dtype=np.int64)
+    cdef long[:] counts = np.zeros(len(bin_edges)-1, dtype=long)
     cdef int i, j, k, m
     cdef double dist
 
-    cdef int num_threads_c = set_num_threads(num_threads)
-
-    for i in prange(i_max, nogil=True, num_threads=num_threads_c):
+    for i in prange(i_max, nogil=True):
         for j in range(j_max):
             for k in range(j+1, k_max):
                 dist = distance(dim, pos, j, k)
                 if dist < bin_edges[i] or dist >= bin_edges[i+1]:
                     continue  # skip if not in current bin
                 for m in range(f_max):
                     # skip no data values
@@ -305,67 +283,58 @@
                         counts[i] += 1
                         variogram[i] += estimator_func(f[m, k] - f[m, j])
 
     normalization_func(variogram, counts)
     return np.asarray(variogram), np.asarray(counts)
 
 
-def structured(
-    const double[:, :] f,
-    str estimator_type='m',
-    num_threads=None,
-):
+def structured(const double[:, :] f, str estimator_type='m'):
     cdef _estimator_func estimator_func = choose_estimator_func(estimator_type)
     cdef _normalization_func normalization_func = (
         choose_estimator_normalization(estimator_type)
     )
 
     cdef int i_max = f.shape[0] - 1
     cdef int j_max = f.shape[1]
     cdef int k_max = i_max + 1
 
     cdef double[:] variogram = np.zeros(k_max)
-    cdef np.int64_t[:] counts = np.zeros(k_max, dtype=np.int64)
+    cdef long[:] counts = np.zeros(k_max, dtype=long)
     cdef int i, j, k
 
-    cdef int num_threads_c = set_num_threads(num_threads)
-
-    with nogil, parallel(num_threads=num_threads_c):
+    with nogil, parallel():
         for i in range(i_max):
             for j in range(j_max):
                 for k in prange(1, k_max-i):
                     counts[k] += 1
                     variogram[k] += estimator_func(f[i, j] - f[i+k, j])
 
     normalization_func(variogram, counts)
     return np.asarray(variogram)
 
 
 def ma_structured(
     const double[:, :] f,
     const bint[:, :] mask,
     str estimator_type='m',
-    num_threads=None,
 ):
     cdef _estimator_func estimator_func = choose_estimator_func(estimator_type)
     cdef _normalization_func normalization_func = (
         choose_estimator_normalization(estimator_type)
     )
 
     cdef int i_max = f.shape[0] - 1
     cdef int j_max = f.shape[1]
     cdef int k_max = i_max + 1
 
     cdef double[:] variogram = np.zeros(k_max)
-    cdef np.int64_t[:] counts = np.zeros(k_max, dtype=np.int64)
+    cdef long[:] counts = np.zeros(k_max, dtype=long)
     cdef int i, j, k
 
-    cdef int num_threads_c = set_num_threads(num_threads)
-
-    with nogil, parallel(num_threads=num_threads_c):
+    with nogil, parallel():
         for i in range(i_max):
             for j in range(j_max):
                 for k in prange(1, k_max-i):
                     if not mask[i, j] and not mask[i+k, j]:
                         counts[k] += 1
                         variogram[k] += estimator_func(f[i, j] - f[i+k, j])
```

### Comparing `gstools-1.5.2/src/gstools/variogram/variogram.py` & `gstools-1.6.0rc1/src/gstools/variogram/variogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 The following functions are provided
 
 .. autosummary::
    vario_estimate
    vario_estimate_axis
 """
-
 # pylint: disable=C0412
 import numpy as np
 
 from gstools import config
 from gstools.normalizer.tools import remove_trend_norm_mean
 from gstools.tools import RADIAN_SCALE
 from gstools.tools.geometric import (
@@ -259,15 +258,15 @@
     References
     ----------
     .. [Webster2007] Webster, R. and Oliver, M. A.
            "Geostatistics for environmental scientists.",
            John Wiley & Sons. (2007)
     """
     if bin_edges is not None:
-        bin_edges = np.atleast_1d(np.asarray(bin_edges, dtype=np.double))
+        bin_edges = np.array(bin_edges, ndmin=1, dtype=np.double, copy=False)
         bin_centers = (bin_edges[:-1] + bin_edges[1:]) / 2.0
     # allow multiple fields at same positions (ndmin=2: first axis -> field ID)
     # need to convert to ma.array, since list of ma.array is not recognised
     field = np.ma.array(field, ndmin=2, dtype=np.double, copy=True)
     masked = np.ma.is_masked(field) or np.any(mask)
     # catch special case if everything is masked
     if masked and np.all(mask):
@@ -312,15 +311,15 @@
         select = mask = None  # free space
     # set no_data values
     if not np.isnan(no_data):
         field[np.isclose(field, float(no_data))] = np.nan
     # set directions
     dir_no = 0
     if direction is not None and dim > 1:
-        direction = np.atleast_2d(np.asarray(direction, dtype=np.double))
+        direction = np.array(direction, ndmin=2, dtype=np.double, copy=False)
         if len(direction.shape) > 2:
             raise ValueError(f"Can't interpret directions: {direction}")
         if direction.shape[1] != dim:
             raise ValueError(f"Can't interpret directions: {direction}")
         dir_no = direction.shape[0]
     # convert given angles to direction vector
     if angles is not None and direction is None and dim > 1:
@@ -371,27 +370,25 @@
         distance_type = "h" if latlon else "e"
         estimates, counts = unstructured(
             field,
             bin_edges,
             pos,
             estimator_type=cython_estimator,
             distance_type=distance_type,
-            num_threads=config.NUM_THREADS,
         )
     else:
         estimates, counts = directional(
             field,
             bin_edges,
             pos,
             direction,
             angles_tol,
             bandwidth,
             separate_dirs=_separate_dirs_test(direction, angles_tol),
             estimator_type=cython_estimator,
-            num_threads=config.NUM_THREADS,
         )
         if dir_no == 1:
             estimates, counts = estimates[0], counts[0]
     est_out = (estimates, counts)
     return (bin_centers,) + est_out[: 2 if return_counts else 1] + norm_out
 
 
@@ -470,30 +467,28 @@
         field = np.ma.array(field, ndmin=1, dtype=np.double)
         if missing:
             field.mask = np.logical_or(field.mask, missing_mask)
         mask = np.ma.getmaskarray(field)
         if not config.USE_RUST:
             mask = np.asarray(mask, dtype=np.int32)
     else:
-        field = np.atleast_1d(np.asarray(field, dtype=np.double))
+        field = np.array(field, ndmin=1, dtype=np.double, copy=False)
         missing_mask = None  # free space
 
     axis_to_swap = AXIS_DIR[direction] if direction in AXIS else int(direction)
     # desired axis first, convert to 2D array afterwards
     field = field.swapaxes(0, axis_to_swap)
     field = field.reshape((field.shape[0], -1))
     if masked:
         mask = mask.swapaxes(0, axis_to_swap)
         mask = mask.reshape((mask.shape[0], -1))
 
     cython_estimator = _set_estimator(estimator)
 
     if masked:
-        return ma_structured(
-            field, mask, cython_estimator, num_threads=config.NUM_THREADS
-        )
-    return structured(field, cython_estimator, num_threads=config.NUM_THREADS)
+        return ma_structured(field, mask, cython_estimator)
+    return structured(field, cython_estimator)
 
 
 # for backward compatibility
 vario_estimate_unstructured = vario_estimate
 vario_estimate_structured = vario_estimate_axis
```

### Comparing `gstools-1.5.2/src/gstools.egg-info/SOURCES.txt` & `gstools-1.6.0rc1/src/gstools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 src/gstools/variogram/binning.py
 src/gstools/variogram/estimator.pyx
 src/gstools/variogram/variogram.py
 tests/test_condition.py
 tests/test_covmodel.py
 tests/test_export.py
 tests/test_field.py
+tests/test_fouriergen.py
 tests/test_incomprrandmeth.py
 tests/test_krige.py
 tests/test_latlon.py
 tests/test_normalizer.py
 tests/test_randmeth.py
 tests/test_rng.py
 tests/test_srf.py
```

### Comparing `gstools-1.5.2/tests/test_condition.py` & `gstools-1.6.0rc1/tests/test_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """This is the unittest of CondSRF class."""
-
 import unittest
 from copy import copy
 
 import numpy as np
 
 import gstools as gs
```

### Comparing `gstools-1.5.2/tests/test_covmodel.py` & `gstools-1.6.0rc1/tests/test_covmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 This is the unittest of CovModel class.
 """
-
 import unittest
 
 import numpy as np
 
 from gstools import (
     Circular,
     CovModel,
```

### Comparing `gstools-1.5.2/tests/test_export.py` & `gstools-1.6.0rc1/tests/test_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Test the PyVista/VTK export methods"""
-
+"""Test the PyVista/VTK export methods
+"""
 import os
 import shutil
 import tempfile
 import unittest
 
 import numpy as np
```

### Comparing `gstools-1.5.2/tests/test_field.py` & `gstools-1.6.0rc1/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_incomprrandmeth.py` & `gstools-1.6.0rc1/tests/test_incomprrandmeth.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_krige.py` & `gstools-1.6.0rc1/tests/test_krige.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_latlon.py` & `gstools-1.6.0rc1/tests/test_latlon.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_normalizer.py` & `gstools-1.6.0rc1/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_randmeth.py` & `gstools-1.6.0rc1/tests/test_randmeth.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_rng.py` & `gstools-1.6.0rc1/tests/test_rng.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_srf.py` & `gstools-1.6.0rc1/tests/test_srf.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_temporal.py` & `gstools-1.6.0rc1/tests/test_temporal.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_transform.py` & `gstools-1.6.0rc1/tests/test_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """This is the unittest of the transform submodule."""
-
 import unittest
 
 import numpy as np
 
 import gstools as gs
```

### Comparing `gstools-1.5.2/tests/test_variogram_structured.py` & `gstools-1.6.0rc1/tests/test_variogram_structured.py`

 * *Files identical despite different names*

### Comparing `gstools-1.5.2/tests/test_variogram_unstructured.py` & `gstools-1.6.0rc1/tests/test_variogram_unstructured.py`

 * *Files identical despite different names*

