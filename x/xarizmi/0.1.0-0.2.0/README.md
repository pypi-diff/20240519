# Comparing `tmp/xarizmi-0.1.0.tar.gz` & `tmp/xarizmi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarizmi-0.1.0.tar", last modified: Sun May 19 04:37:20 2024, max compression
+gzip compressed data, was "xarizmi-0.2.0.tar", last modified: Sun May 19 07:17:51 2024, max compression
```

## Comparing `xarizmi-0.1.0.tar` & `xarizmi-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:37:20.537333 xarizmi-0.1.0/
--rw-r--r--   0 javad      (501) staff       (20)    11345 2024-05-19 03:25:40.000000 xarizmi-0.1.0/LICENSE
--rw-r--r--   0 javad      (501) staff       (20)      558 2024-05-19 04:37:20.537224 xarizmi-0.1.0/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      175 2024-05-19 03:29:04.000000 xarizmi-0.1.0/README.md
--rw-r--r--   0 javad      (501) staff       (20)       30 2024-05-19 03:25:40.000000 xarizmi-0.1.0/pyproject.toml
--rw-r--r--   0 javad      (501) staff       (20)      280 2024-05-19 04:37:20.537629 xarizmi-0.1.0/setup.cfg
--rw-r--r--   0 javad      (501) staff       (20)      849 2024-05-19 03:47:51.000000 xarizmi-0.1.0/setup.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:37:20.535945 xarizmi-0.1.0/tests/
--rw-r--r--   0 javad      (501) staff       (20)      158 2024-05-19 04:34:21.000000 xarizmi-0.1.0/tests/test_candlestick.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:37:20.536207 xarizmi-0.1.0/xarizmi/
--rw-r--r--   0 javad      (501) staff       (20)       22 2024-05-19 04:36:44.000000 xarizmi-0.1.0/xarizmi/__init__.py
--rw-r--r--   0 javad      (501) staff       (20)       28 2024-05-19 04:33:16.000000 xarizmi-0.1.0/xarizmi/candlestick.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:37:20.536939 xarizmi-0.1.0/xarizmi.egg-info/
--rw-r--r--   0 javad      (501) staff       (20)      558 2024-05-19 04:37:20.000000 xarizmi-0.1.0/xarizmi.egg-info/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      244 2024-05-19 04:37:20.000000 xarizmi-0.1.0/xarizmi.egg-info/SOURCES.txt
--rw-r--r--   0 javad      (501) staff       (20)        1 2024-05-19 04:37:20.000000 xarizmi-0.1.0/xarizmi.egg-info/dependency_links.txt
--rw-r--r--   0 javad      (501) staff       (20)        8 2024-05-19 04:37:20.000000 xarizmi-0.1.0/xarizmi.egg-info/top_level.txt
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:17:51.392846 xarizmi-0.2.0/
+-rw-r--r--   0 javad      (501) staff       (20)    11345 2024-05-19 03:25:40.000000 xarizmi-0.2.0/LICENSE
+-rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-19 07:17:51.392773 xarizmi-0.2.0/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      377 2024-05-19 06:54:11.000000 xarizmi-0.2.0/README.md
+-rw-r--r--   0 javad      (501) staff       (20)       30 2024-05-19 03:25:40.000000 xarizmi-0.2.0/pyproject.toml
+-rw-r--r--   0 javad      (501) staff       (20)      280 2024-05-19 07:17:51.393102 xarizmi-0.2.0/setup.cfg
+-rw-r--r--   0 javad      (501) staff       (20)      849 2024-05-19 07:14:04.000000 xarizmi-0.2.0/setup.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:17:51.391409 xarizmi-0.2.0/tests/
+-rw-r--r--   0 javad      (501) staff       (20)      608 2024-05-19 07:00:40.000000 xarizmi-0.2.0/tests/test_candlestick.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:17:51.391819 xarizmi-0.2.0/xarizmi/
+-rw-r--r--   0 javad      (501) staff       (20)       22 2024-05-19 07:13:05.000000 xarizmi-0.2.0/xarizmi/__init__.py
+-rw-r--r--   0 javad      (501) staff       (20)      127 2024-05-19 05:19:14.000000 xarizmi-0.2.0/xarizmi/candlestick.py
+-rw-r--r--   0 javad      (501) staff       (20)       86 2024-05-19 06:57:33.000000 xarizmi-0.2.0/xarizmi/enums.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:17:51.392538 xarizmi-0.2.0/xarizmi.egg-info/
+-rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-19 07:17:51.000000 xarizmi-0.2.0/xarizmi.egg-info/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      261 2024-05-19 07:17:51.000000 xarizmi-0.2.0/xarizmi.egg-info/SOURCES.txt
+-rw-r--r--   0 javad      (501) staff       (20)        1 2024-05-19 07:17:51.000000 xarizmi-0.2.0/xarizmi.egg-info/dependency_links.txt
+-rw-r--r--   0 javad      (501) staff       (20)        8 2024-05-19 07:17:51.000000 xarizmi-0.2.0/xarizmi.egg-info/top_level.txt
```

### Comparing `xarizmi-0.1.0/LICENSE` & `xarizmi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xarizmi-0.1.0/setup.py` & `xarizmi-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,13 +18,13 @@
         "Xarizmi (read Khwarizmi) project is an educational project that"
         "contains tools for technical analysis in Python."
     ),
     name="xarizmi",
     packages=find_packages(include=["xarizmi", "xarizmi.*"]),
     version=xarizmi.__version__,
     install_requires=[],
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     license="Apache 2.0",
     url="https://github.com/javadebadi/xarizmi",
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

