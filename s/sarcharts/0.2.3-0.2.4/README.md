# Comparing `tmp/sarcharts-0.2.3.tar.gz` & `tmp/sarcharts-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.2.3.tar", last modified: Sat May 18 13:03:03 2024, max compression
+gzip compressed data, was "sarcharts-0.2.4.tar", last modified: Sat May 18 13:58:09 2024, max compression
```

## Comparing `sarcharts-0.2.3.tar` & `sarcharts-0.2.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.508344 sarcharts-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.496344 sarcharts-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.500344 sarcharts-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 13:02:57.000000 sarcharts-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-18 13:02:57.000000 sarcharts-0.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 13:03:03.000000 sarcharts-0.2.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 13:03:03.000000 sarcharts-0.2.3/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 13:02:57.000000 sarcharts-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 13:03:03.508344 sarcharts-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 13:02:57.000000 sarcharts-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.500344 sarcharts-0.2.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 13:02:57.000000 sarcharts-0.2.3/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   109472 2024-05-18 13:02:57.000000 sarcharts-0.2.3/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-18 13:02:57.000000 sarcharts-0.2.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.500344 sarcharts-0.2.3/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.504344 sarcharts-0.2.3/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.500344 sarcharts-0.2.3/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.504344 sarcharts-0.2.3/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/css/sarcharts.css
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/css/ul-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.504344 sarcharts-0.2.3/sarcharts/html/img/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/img/chevron.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.504344 sarcharts-0.2.3/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    50650 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/chartjs-plugin-annotation.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/html/js/ul-select.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.508344 sarcharts-0.2.3/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10660 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.508344 sarcharts-0.2.3/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-18 13:02:57.000000 sarcharts-0.2.3/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:03:03.508344 sarcharts-0.2.3/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 13:03:03.000000 sarcharts-0.2.3/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-18 13:03:03.508344 sarcharts-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-18 13:02:57.000000 sarcharts-0.2.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-18 13:02:57.000000 sarcharts-0.2.3/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-18 13:02:57.000000 sarcharts-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.081965 sarcharts-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 13:58:03.000000 sarcharts-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-18 13:58:03.000000 sarcharts-0.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 13:58:09.000000 sarcharts-0.2.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 13:58:09.000000 sarcharts-0.2.4/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 13:58:03.000000 sarcharts-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 13:58:09.081965 sarcharts-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 13:58:03.000000 sarcharts-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 13:58:03.000000 sarcharts-0.2.4/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   109472 2024-05-18 13:58:03.000000 sarcharts-0.2.4/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-18 13:58:03.000000 sarcharts-0.2.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.077965 sarcharts-0.2.4/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.077965 sarcharts-0.2.4/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/css/sarcharts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/css/ul-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.077965 sarcharts-0.2.4/sarcharts/html/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/img/chevron.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.077965 sarcharts-0.2.4/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50650 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/chartjs-plugin-annotation.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/ul-select.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.081965 sarcharts-0.2.4/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.081965 sarcharts-0.2.4/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.081965 sarcharts-0.2.4/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-18 13:58:09.081965 sarcharts-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-18 13:58:03.000000 sarcharts-0.2.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-18 13:58:03.000000 sarcharts-0.2.4/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-18 13:58:03.000000 sarcharts-0.2.4/tox.ini
```

### Comparing `sarcharts-0.2.3/.github/workflows/python-publish.yml` & `sarcharts-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/.pylintrc` & `sarcharts-0.2.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/LICENSE` & `sarcharts-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/PKG-INFO` & `sarcharts-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.2.3
+Version: 0.2.4
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.2.3/README.md` & `sarcharts-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/doc/README.md` & `sarcharts-0.2.4/doc/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/doc/sarcharts.png` & `sarcharts-0.2.4/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/__init__.py` & `sarcharts-0.2.4/sarcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/css/sarcharts.css` & `sarcharts-0.2.4/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/css/ul-select.css` & `sarcharts-0.2.4/sarcharts/html/css/ul-select.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/js/chart.umd.js` & `sarcharts-0.2.4/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js` & `sarcharts-0.2.4/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/js/chartjs-plugin-annotation.min.js` & `sarcharts-0.2.4/sarcharts/html/js/chartjs-plugin-annotation.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.2.4/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/js/hammer.min.js` & `sarcharts-0.2.4/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/js/jquery.js` & `sarcharts-0.2.4/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/html/js/ul-select.js` & `sarcharts-0.2.4/sarcharts/html/js/ul-select.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/lib/chartjs.py` & `sarcharts-0.2.4/sarcharts/lib/chartjs.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/lib/events.py` & `sarcharts-0.2.4/sarcharts/lib/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 from sarcharts.lib import util
 
 
 class Events:
 
     def getCSVdata(args, charts):
-        with open(args.eventfile) as csv_file:
-            csv_reader = csv.reader(csv_file, delimiter=';')
-            for row in csv_reader:
-                if row[1] not in charts.keys():
-                    util.debug(
-                        args, 'W',
-                        f"Host '{row[1]}' from '{f}' not in 'sar' data.")
-                    continue
-                charts[row[1]]['xlabels'].append(row[0])
-                if row[2] not in charts[row[1]]['events']:
-                    charts[row[1]]['events'][row[2]] = []
-                charts[row[1]]['events'][row[2]].append(
-                       {'date': row[0], 'text': row[3]})
+        if args.eventfile:
+            with open(args.eventfile) as csv_file:
+                csv_reader = csv.reader(csv_file, delimiter=';')
+                for row in csv_reader:
+                    if not row[0].startswith("#"):
+                        if row[1] not in charts.keys():
+                            util.debug(
+                                args, 'W',
+                                f"Host '{row[1]}' from '{args.eventfile}'"
+                                + " not in 'sar' data.")
+                            continue
+                        charts[row[1]]['xlabels'].append(row[0])
+                        if row[2] not in charts[row[1]]['events']:
+                            charts[row[1]]['events'][row[2]] = []
+                        charts[row[1]]['events'][row[2]].append(
+                               {'date': row[0], 'text': row[3]})
 
         return charts
```

### Comparing `sarcharts-0.2.3/sarcharts/lib/progressbar.py` & `sarcharts-0.2.4/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/lib/sadf.py` & `sarcharts-0.2.4/sarcharts/lib/sadf.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,20 @@
             jdata = self.sar_to_json(args, inputfile, '-A')
             if jdata:
                 data.append(jdata)
             else:
                 util.debug(args, 'W', f"Can't add data from {inputfile}.")
         return data
 
+    def data_normalization(self, act, data):
+        if isinstance(data, list) and isinstance(data[0], dict):
+            print(f"{act} is type 1")
+            headers = ";".join(data[0].keys())
+            print(headers)
+            
     def sar_to_chartjs(self, args, sarfiles):
         data = self.merge_sarfiles(args, sarfiles)
         linehead = "# hostname;interval;timestamp"
         pb = ProgressBar()
         pb.quiet = args.quiet
         all_entries = 0
         for idata in range(len(data)):
@@ -82,14 +88,15 @@
                         if act == "timestamp":
                             date = f"{adata['date']} {adata['time']}"
                             if (date not in charts[nodename]['xlabels']
                                     and util.in_date_range(args, date)):
                                 charts[nodename]['xlabels'].append(date)
                             linedet = f"{hdata['nodename']};{adata['interval']};{date}"
                         else:
+                            # self.data_normalization(act, adata)
                             if isinstance(adata, list):
                                 if act not in charts[nodename]['activities'].keys():
                                     line = linehead
                                     for h in adata[0].keys():
                                         line += f";{str(h)}"
                                     charts[nodename]['activities'][act] = {
                                         "content": [line.split(";")],
```

### Comparing `sarcharts-0.2.3/sarcharts/lib/util.py` & `sarcharts-0.2.4/sarcharts/lib/util.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/templates/chart.html` & `sarcharts-0.2.4/sarcharts/templates/chart.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts/templates/header.html` & `sarcharts-0.2.4/sarcharts/templates/header.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.2.4/sarcharts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.2.3
+Version: 0.2.4
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.2.3/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.2.4/sarcharts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/setup.cfg` & `sarcharts-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/setup.py` & `sarcharts-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.3/tox.ini` & `sarcharts-0.2.4/tox.ini`

 * *Files identical despite different names*

