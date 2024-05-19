# Comparing `tmp/scidatetime-1.20.1.tar.gz` & `tmp/scidatetime-1.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scidatetime-1.20.1.tar", last modified: Wed May  8 06:23:43 2024, max compression
+gzip compressed data, was "scidatetime-1.20.2.tar", last modified: Sun May 19 12:54:07 2024, max compression
```

## Comparing `scidatetime-1.20.1.tar` & `scidatetime-1.20.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 06:23:34.000000 scidatetime-1.20.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-08 06:23:43.035148 scidatetime-1.20.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-08 06:23:34.000000 scidatetime-1.20.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.027148 scidatetime-1.20.1/scidatetime/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/DateTimeParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/MdlDateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.031148 scidatetime-1.20.1/scidatetime/dateutil/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/_common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/easter.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/easter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.031148 scidatetime-1.20.1/scidatetime/dateutil/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    58803 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/isoparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/isoparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24905 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/relativedelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/relativedelta.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    66567 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/rrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/rrule.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/scidatetime/dateutil/tz/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/_common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/_factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    62868 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/tz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/tz.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/win.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tzwin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/rebuild.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/scidatetime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:23:43.035148 scidatetime-1.20.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-08 06:23:34.000000 scidatetime-1.20.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-08 06:23:34.000000 scidatetime-1.20.1/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 06:23:34.000000 scidatetime-1.20.1/tests/test_origin_polute.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-08 06:23:34.000000 scidatetime-1.20.1/tests/test_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:54:07.786598 scidatetime-1.20.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 12:53:56.000000 scidatetime-1.20.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-19 12:54:07.786598 scidatetime-1.20.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-19 12:53:56.000000 scidatetime-1.20.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:54:07.778598 scidatetime-1.20.2/scidatetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/DateTimeParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/MdlDateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:54:07.782598 scidatetime-1.20.2/scidatetime/dateutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/_common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/easter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/easter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:54:07.782598 scidatetime-1.20.2/scidatetime/dateutil/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/parser/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    58803 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/parser/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/parser/isoparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/parser/isoparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24905 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/relativedelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/relativedelta.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    66567 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/rrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/rrule.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:54:07.782598 scidatetime-1.20.2/scidatetime/dateutil/tz/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tz/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tz/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tz/_common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tz/_factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62868 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tz/tz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tz/tz.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tz/win.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/tzwin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:54:07.786598 scidatetime-1.20.2/scidatetime/dateutil/zoneinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/zoneinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-19 12:53:56.000000 scidatetime-1.20.2/scidatetime/dateutil/zoneinfo/rebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:54:07.786598 scidatetime-1.20.2/scidatetime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-19 12:54:07.000000 scidatetime-1.20.2/scidatetime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-19 12:54:07.000000 scidatetime-1.20.2/scidatetime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:54:07.000000 scidatetime-1.20.2/scidatetime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:54:07.000000 scidatetime-1.20.2/scidatetime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 12:54:07.000000 scidatetime-1.20.2/scidatetime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 12:54:07.000000 scidatetime-1.20.2/scidatetime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:54:07.786598 scidatetime-1.20.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-19 12:53:56.000000 scidatetime-1.20.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:54:07.786598 scidatetime-1.20.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-19 12:53:56.000000 scidatetime-1.20.2/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-19 12:53:56.000000 scidatetime-1.20.2/tests/test_origin_polute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-19 12:53:56.000000 scidatetime-1.20.2/tests/test_timestamp.py
```

### Comparing `scidatetime-1.20.1/LICENSE` & `scidatetime-1.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/PKG-INFO` & `scidatetime-1.20.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scidatetime
-Version: 1.20.1
+Version: 1.20.2
 Summary: scidatetime is python module for DateTime handle.
 Home-page: https://github.com/serfend/scidatetime
 Author: serfend
 Author-email: serfend@foxmail.com
 License: MIT Licence
 Keywords: lib,utils
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scidatetime Version: 1.20.1 Summary: scidatetime is
+Metadata-Version: 2.1 Name: scidatetime Version: 1.20.2 Summary: scidatetime is
 python module for DateTime handle. Home-page: https://github.com/serfend/
 scidatetime Author: serfend Author-email: serfend@foxmail.com License: MIT
 Licence Keywords: lib,utils Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
```

### Comparing `scidatetime-1.20.1/README.md` & `scidatetime-1.20.2/README.md`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/MdlDateTime.py` & `scidatetime-1.20.2/scidatetime/MdlDateTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,17 +230,18 @@
             return f'{int(v_time * 24)}小时{suffix}'
         if v_time < 14:
             return f'{int(v_time)}天{suffix}'
         if v_time < 30:
             return f'{int(v_time/7)}周{suffix}'
 
         if v_time < 365:
-            y_month = 12*(target.year - self.year)
-            v_month = y_month + target.month - self.month + 120
-            v_month %= 12
+            y_month = 12*(self.year-target.year)
+            v_month = y_month + self.month - target.month
+            if v_month < 0:
+                v_month = -v_month
             return f'{v_month}月{suffix}'
 
         v_year = abs(self.year - target.year)
         return f'{v_year}年{suffix}'
 
     def __add__(self, other):
         t = datetime.timedelta
```

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/_common.py` & `scidatetime-1.20.2/scidatetime/dateutil/_common.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/easter.py` & `scidatetime-1.20.2/scidatetime/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/parser/__init__.py` & `scidatetime-1.20.2/scidatetime/dateutil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/parser/__init__.pyi` & `scidatetime-1.20.2/scidatetime/dateutil/parser/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/parser/_parser.py` & `scidatetime-1.20.2/scidatetime/dateutil/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/parser/isoparser.py` & `scidatetime-1.20.2/scidatetime/dateutil/parser/isoparser.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/parser/isoparser.pyi` & `scidatetime-1.20.2/scidatetime/dateutil/parser/isoparser.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/relativedelta.py` & `scidatetime-1.20.2/scidatetime/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/relativedelta.pyi` & `scidatetime-1.20.2/scidatetime/dateutil/relativedelta.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/rrule.py` & `scidatetime-1.20.2/scidatetime/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/rrule.pyi` & `scidatetime-1.20.2/scidatetime/dateutil/rrule.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/tz/_common.py` & `scidatetime-1.20.2/scidatetime/dateutil/tz/_common.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/tz/_common.pyi` & `scidatetime-1.20.2/scidatetime/dateutil/tz/_common.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/tz/_factories.py` & `scidatetime-1.20.2/scidatetime/dateutil/tz/_factories.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/tz/tz.py` & `scidatetime-1.20.2/scidatetime/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/tz/tz.pyi` & `scidatetime-1.20.2/scidatetime/dateutil/tz/tz.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/tz/win.py` & `scidatetime-1.20.2/scidatetime/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/utils.py` & `scidatetime-1.20.2/scidatetime/dateutil/utils.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/__init__.py` & `scidatetime-1.20.2/scidatetime/dateutil/zoneinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/rebuild.py` & `scidatetime-1.20.2/scidatetime/dateutil/zoneinfo/rebuild.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/scidatetime.egg-info/PKG-INFO` & `scidatetime-1.20.2/scidatetime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scidatetime
-Version: 1.20.1
+Version: 1.20.2
 Summary: scidatetime is python module for DateTime handle.
 Home-page: https://github.com/serfend/scidatetime
 Author: serfend
 Author-email: serfend@foxmail.com
 License: MIT Licence
 Keywords: lib,utils
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scidatetime Version: 1.20.1 Summary: scidatetime is
+Metadata-Version: 2.1 Name: scidatetime Version: 1.20.2 Summary: scidatetime is
 python module for DateTime handle. Home-page: https://github.com/serfend/
 scidatetime Author: serfend Author-email: serfend@foxmail.com License: MIT
 Licence Keywords: lib,utils Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
```

### Comparing `scidatetime-1.20.1/scidatetime.egg-info/SOURCES.txt` & `scidatetime-1.20.2/scidatetime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/setup.py` & `scidatetime-1.20.2/setup.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.20.1/tests/test_date.py` & `scidatetime-1.20.2/tests/test_date.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 
     x2 = DateTime.fromstring('2023-01-06 15:16:11.355789')
     assert x2.toRelativeTime(x) == '10天前'
 
     x2 = DateTime.fromstring('2023-02-01 15:16:11.355789')
     assert x2.toRelativeTime(x) == '2周后'
 
+    x2 = DateTime.fromstring('2023-12-01 15:16:11.355789')
+    assert x2.toRelativeTime(x) == '11月后'
+
+    x2 = DateTime.fromstring('2024-12-01 15:16:11.355789')
+    assert x2.toRelativeTime(x) == '1年后'
+
     x2 = DateTime.fromstring('2023-01-16 15:16:11.355789')
     assert x2.toRelativeTime(x) == '55分钟前'
 
     x2 = DateTime.fromstring('2023-01-16 16:11:07.355789')
     assert x2.toRelativeTime(x) == '10秒前'
 
     x2 = DateTime.fromstring('2023-01-16 16:11:27.355789')
```

### Comparing `scidatetime-1.20.1/tests/test_timestamp.py` & `scidatetime-1.20.2/tests/test_timestamp.py`

 * *Files identical despite different names*

