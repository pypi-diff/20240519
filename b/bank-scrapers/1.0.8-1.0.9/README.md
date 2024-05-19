# Comparing `tmp/bank_scrapers-1.0.8.tar.gz` & `tmp/bank_scrapers-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bank_scrapers-1.0.8.tar", last modified: Sat May 18 06:14:34 2024, max compression
+gzip compressed data, was "bank_scrapers-1.0.9.tar", last modified: Sat May 18 06:29:26 2024, max compression
```

## Comparing `bank_scrapers-1.0.8.tar` & `bank_scrapers-1.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/LICENSE
--rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.339314 bank_scrapers-1.0.8/bank_scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)      308 2024-05-18 06:14:30.000000 bank_scrapers-1.0.8/bank_scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/kraken/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/kraken/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/api_wrappers/kraken/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/cli/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/cli/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/cli/cli.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     1394 2024-05-18 06:14:01.000000 bank_scrapers-1.0.8/bank_scrapers/common/functions.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      271 2024-05-18 06:09:50.000000 bank_scrapers-1.0.8/bank_scrapers/common/log.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      169 2024-05-18 06:02:00.000000 bank_scrapers-1.0.8/bank_scrapers/common/values.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.340314 bank_scrapers-1.0.8/bank_scrapers/scrapers/becu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/becu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     7589 2024-05-18 06:13:34.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/becu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/chase/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/chase/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/chase/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/common/functions.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/fidelity_netbenefits/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/roundpoint/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/roundpoint/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/roundpoint/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/smbc_prestia/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/smbc_prestia/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/smbc_prestia/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.341313 bank_scrapers-1.0.8/bank_scrapers/scrapers/uhfcu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/uhfcu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/uhfcu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/bank_scrapers/scrapers/vanguard/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/vanguard/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/vanguard/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/bank_scrapers/scrapers/zillow/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/zillow/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2024-05-16 09:36:03.000000 bank_scrapers-1.0.8/bank_scrapers/scrapers/zillow/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/bank_scrapers.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1412 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       59 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      128 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       14 2024-05-18 06:14:34.000000 bank_scrapers-1.0.8/bank_scrapers.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      962 2024-05-18 05:07:40.000000 bank_scrapers-1.0.8/pyproject.toml
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2024-05-18 06:14:34.342314 bank_scrapers-1.0.8/setup.cfg
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.159931 bank_scrapers-1.0.9/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/LICENSE
+-rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 06:29:26.159931 bank_scrapers-1.0.9/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.155931 bank_scrapers-1.0.9/bank_scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      307 2024-05-18 06:29:23.000000 bank_scrapers-1.0.9/bank_scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.156931 bank_scrapers-1.0.9/bank_scrapers/api_wrappers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/api_wrappers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.156931 bank_scrapers-1.0.9/bank_scrapers/api_wrappers/kraken/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/api_wrappers/kraken/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/api_wrappers/kraken/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.156931 bank_scrapers-1.0.9/bank_scrapers/cli/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/cli/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/cli/cli.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.157931 bank_scrapers-1.0.9/bank_scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1394 2024-05-18 06:14:01.000000 bank_scrapers-1.0.9/bank_scrapers/common/functions.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      271 2024-05-18 06:09:50.000000 bank_scrapers-1.0.9/bank_scrapers/common/log.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      169 2024-05-18 06:02:00.000000 bank_scrapers-1.0.9/bank_scrapers/common/values.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.157931 bank_scrapers-1.0.9/bank_scrapers/scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.157931 bank_scrapers-1.0.9/bank_scrapers/scrapers/becu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/becu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7593 2024-05-18 06:27:54.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/becu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.157931 bank_scrapers-1.0.9/bank_scrapers/scrapers/chase/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/chase/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/chase/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.157931 bank_scrapers-1.0.9/bank_scrapers/scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/common/functions.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.157931 bank_scrapers-1.0.9/bank_scrapers/scrapers/fidelity_netbenefits/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.158931 bank_scrapers-1.0.9/bank_scrapers/scrapers/roundpoint/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/roundpoint/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/roundpoint/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.158931 bank_scrapers-1.0.9/bank_scrapers/scrapers/smbc_prestia/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/smbc_prestia/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/smbc_prestia/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.158931 bank_scrapers-1.0.9/bank_scrapers/scrapers/uhfcu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/uhfcu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/uhfcu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.159931 bank_scrapers-1.0.9/bank_scrapers/scrapers/vanguard/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/vanguard/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/vanguard/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.159931 bank_scrapers-1.0.9/bank_scrapers/scrapers/zillow/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/zillow/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2024-05-16 09:36:03.000000 bank_scrapers-1.0.9/bank_scrapers/scrapers/zillow/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-05-18 06:29:26.159931 bank_scrapers-1.0.9/bank_scrapers.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)    22430 2024-05-18 06:29:26.000000 bank_scrapers-1.0.9/bank_scrapers.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1412 2024-05-18 06:29:26.000000 bank_scrapers-1.0.9/bank_scrapers.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2024-05-18 06:29:26.000000 bank_scrapers-1.0.9/bank_scrapers.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       59 2024-05-18 06:29:26.000000 bank_scrapers-1.0.9/bank_scrapers.egg-info/entry_points.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      128 2024-05-18 06:29:26.000000 bank_scrapers-1.0.9/bank_scrapers.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       14 2024-05-18 06:29:26.000000 bank_scrapers-1.0.9/bank_scrapers.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      962 2024-05-18 05:07:40.000000 bank_scrapers-1.0.9/pyproject.toml
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2024-05-18 06:29:26.159931 bank_scrapers-1.0.9/setup.cfg
```

### Comparing `bank_scrapers-1.0.8/LICENSE` & `bank_scrapers-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/PKG-INFO` & `bank_scrapers-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank_scrapers
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bank_scrapers-1.0.8/README.md` & `bank_scrapers-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/api_wrappers/kraken/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/api_wrappers/kraken/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/cli/cli.py` & `bank_scrapers-1.0.9/bank_scrapers/cli/cli.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/common/functions.py` & `bank_scrapers-1.0.9/bank_scrapers/common/functions.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/becu/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/becu/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,18 +221,18 @@
     tables: List[WebElement] = wait_and_find_elements(
         driver, wait, (By.CLASS_NAME, "tablesaw-stack")
     )
 
     # Process tables
     return_tables: List = list()
     for t in tables:
+        table: pd.DataFrame = process_table(t)
         is_credit_account = any(
-            list(True for header in t.columns if "credit" in header.lower())
+            list(True for header in table.columns if "credit" in header.lower())
         )
-        table: pd.DataFrame = process_table(t)
         table.name = "credit" if is_credit_account else "deposit"
         return_tables.append(table)
 
     # Clean up
     driver.quit()
 
     # Convert to Prometheus exposition if flag is set
```

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/chase/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/chase/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/common/functions.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/common/functions.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/fidelity_netbenefits/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/fidelity_netbenefits/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/roundpoint/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/roundpoint/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/smbc_prestia/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/smbc_prestia/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/uhfcu/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/uhfcu/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/vanguard/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/vanguard/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers/scrapers/zillow/driver.py` & `bank_scrapers-1.0.9/bank_scrapers/scrapers/zillow/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/bank_scrapers.egg-info/PKG-INFO` & `bank_scrapers-1.0.9/bank_scrapers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank_scrapers
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bank_scrapers-1.0.8/bank_scrapers.egg-info/SOURCES.txt` & `bank_scrapers-1.0.9/bank_scrapers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.8/pyproject.toml` & `bank_scrapers-1.0.9/pyproject.toml`

 * *Files identical despite different names*

