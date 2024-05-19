# Comparing `tmp/sarcharts-0.2.4.tar.gz` & `tmp/sarcharts-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.2.4.tar", last modified: Sat May 18 13:58:09 2024, max compression
+gzip compressed data, was "sarcharts-0.2.5.tar", last modified: Sun May 19 06:54:14 2024, max compression
```

## Comparing `sarcharts-0.2.4.tar` & `sarcharts-0.2.5.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.081965 sarcharts-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 13:58:03.000000 sarcharts-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-18 13:58:03.000000 sarcharts-0.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 13:58:09.000000 sarcharts-0.2.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 13:58:09.000000 sarcharts-0.2.4/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 13:58:03.000000 sarcharts-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 13:58:09.081965 sarcharts-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 13:58:03.000000 sarcharts-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-18 13:58:03.000000 sarcharts-0.2.4/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   109472 2024-05-18 13:58:03.000000 sarcharts-0.2.4/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-18 13:58:03.000000 sarcharts-0.2.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.077965 sarcharts-0.2.4/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.073965 sarcharts-0.2.4/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.077965 sarcharts-0.2.4/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/css/sarcharts.css
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/css/ul-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.077965 sarcharts-0.2.4/sarcharts/html/img/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/img/chevron.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.077965 sarcharts-0.2.4/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    50650 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/chartjs-plugin-annotation.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/html/js/ul-select.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.081965 sarcharts-0.2.4/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.081965 sarcharts-0.2.4/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-18 13:58:03.000000 sarcharts-0.2.4/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:58:09.081965 sarcharts-0.2.4/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 13:58:09.000000 sarcharts-0.2.4/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-18 13:58:09.081965 sarcharts-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-18 13:58:03.000000 sarcharts-0.2.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-18 13:58:03.000000 sarcharts-0.2.4/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-18 13:58:03.000000 sarcharts-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.054914 sarcharts-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.042914 sarcharts-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.046914 sarcharts-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 06:54:05.000000 sarcharts-0.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-19 06:54:05.000000 sarcharts-0.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 06:54:14.000000 sarcharts-0.2.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-19 06:54:13.000000 sarcharts-0.2.5/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 06:54:05.000000 sarcharts-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-19 06:54:14.054914 sarcharts-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-19 06:54:05.000000 sarcharts-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.046914 sarcharts-0.2.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-19 06:54:05.000000 sarcharts-0.2.5/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   109472 2024-05-19 06:54:05.000000 sarcharts-0.2.5/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-19 06:54:05.000000 sarcharts-0.2.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.050914 sarcharts-0.2.5/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.050914 sarcharts-0.2.5/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.046914 sarcharts-0.2.5/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.050914 sarcharts-0.2.5/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/css/sarcharts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/css/ul-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.050914 sarcharts-0.2.5/sarcharts/html/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/img/chevron.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.054914 sarcharts-0.2.5/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50650 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/js/chartjs-plugin-annotation.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/js/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/html/js/ul-select.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.054914 sarcharts-0.2.5/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/lib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.054914 sarcharts-0.2.5/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-19 06:54:05.000000 sarcharts-0.2.5/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:54:14.054914 sarcharts-0.2.5/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-19 06:54:14.000000 sarcharts-0.2.5/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-19 06:54:14.000000 sarcharts-0.2.5/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 06:54:14.000000 sarcharts-0.2.5/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-19 06:54:14.000000 sarcharts-0.2.5/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 06:54:14.000000 sarcharts-0.2.5/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 06:54:14.000000 sarcharts-0.2.5/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 06:54:14.000000 sarcharts-0.2.5/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 06:54:14.000000 sarcharts-0.2.5/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 06:54:14.054914 sarcharts-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 06:54:05.000000 sarcharts-0.2.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-19 06:54:05.000000 sarcharts-0.2.5/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-19 06:54:05.000000 sarcharts-0.2.5/tox.ini
```

### Comparing `sarcharts-0.2.4/.github/workflows/python-publish.yml` & `sarcharts-0.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/.pylintrc` & `sarcharts-0.2.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/LICENSE` & `sarcharts-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/PKG-INFO` & `sarcharts-0.2.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.2.4
+Version: 0.2.5
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -27,33 +27,35 @@
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
 ### Installation
 `pip install sarcharts`
 
 ### Usage
 ~~~
-usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
+usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-m METRICFILE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
   sarfilespaths         `sa` file/s to parse. Default: `./sa??`.
 
 optional arguments:
   -h, --help            show this help message and exit
   -d {D,I,W,E}, --debug {D,I,W,E}
                         Set debug level. Default `W`.
   -e EVENTFILE, --eventfile EVENTFILE
                         Add events csv file. Header: # date;hostname;event_name;event_description
   -f FROMDATE, --fromdate FROMDATE
-                        Include metrics from this date.
+                        Include metrics/events from this date.
+  -m METRICFILE, --metricfile METRICFILE
+                        Add metrics csv file. Header: # date;hostname;metric_name;metric_value
   -o OUTPUTPATH, --outputpath OUTPUTPATH
                         Path to put output files. Default `./sarcharts`.
   -t TODATE, --todate TODATE
-                        Discard metrics after this date.
+                        Include metrics/events before this date.
   -q, --quiet           Don't show progress.
 ~~~
 
 | Example Chart |
 | --- |
 | ![](/doc/sarcharts.png) |
```

### Comparing `sarcharts-0.2.4/README.md` & `sarcharts-0.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
 ### Installation
 `pip install sarcharts`
 
 ### Usage
 ~~~
-usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
+usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-m METRICFILE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
   sarfilespaths         `sa` file/s to parse. Default: `./sa??`.
 
 optional arguments:
   -h, --help            show this help message and exit
   -d {D,I,W,E}, --debug {D,I,W,E}
                         Set debug level. Default `W`.
   -e EVENTFILE, --eventfile EVENTFILE
                         Add events csv file. Header: # date;hostname;event_name;event_description
   -f FROMDATE, --fromdate FROMDATE
-                        Include metrics from this date.
+                        Include metrics/events from this date.
+  -m METRICFILE, --metricfile METRICFILE
+                        Add metrics csv file. Header: # date;hostname;metric_name;metric_value
   -o OUTPUTPATH, --outputpath OUTPUTPATH
                         Path to put output files. Default `./sarcharts`.
   -t TODATE, --todate TODATE
-                        Discard metrics after this date.
+                        Include metrics/events before this date.
   -q, --quiet           Don't show progress.
 ~~~
 
 | Example Chart |
 | --- |
 | ![](/doc/sarcharts.png) |
```

### Comparing `sarcharts-0.2.4/doc/README.md` & `sarcharts-0.2.5/doc/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
 ### Installation
 `pip install sarcharts`
 
 ### Usage
 ~~~
-usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
+usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-m METRICFILE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
   sarfilespaths         `sa` file/s to parse. Default: `./sa??`.
 
 optional arguments:
   -h, --help            show this help message and exit
   -d {D,I,W,E}, --debug {D,I,W,E}
                         Set debug level. Default `W`.
   -e EVENTFILE, --eventfile EVENTFILE
                         Add events csv file. Header: # date;hostname;event_name;event_description
   -f FROMDATE, --fromdate FROMDATE
-                        Include metrics from this date.
+                        Include metrics/events from this date.
+  -m METRICFILE, --metricfile METRICFILE
+                        Add metrics csv file. Header: # date;hostname;metric_name;metric_value
   -o OUTPUTPATH, --outputpath OUTPUTPATH
                         Path to put output files. Default `./sarcharts`.
   -t TODATE, --todate TODATE
-                        Discard metrics after this date.
+                        Include metrics/events before this date.
   -q, --quiet           Don't show progress.
 ~~~
 
 | Example Chart |
 | --- |
 | ![](/doc/sarcharts.png) |
```

### Comparing `sarcharts-0.2.4/doc/sarcharts.png` & `sarcharts-0.2.5/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/__init__.py` & `sarcharts-0.2.5/sarcharts/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import argparse
 import fnmatch
 import shutil
 import webbrowser
 
 from sarcharts.lib.chartjs import ChartJS
 from sarcharts.lib.events import Events
+from sarcharts.lib.metrics import Metrics
 from sarcharts.lib.sadf import Sadf
 from sarcharts.lib import util
 
 
 class SarCharts:
     args = ()
     cwd = os.getcwd()
@@ -63,28 +64,35 @@
             help='Add events csv file. Header: '
                  + '# date;hostname;event_name;event_description',
             type=self.valid_path
             )
         self.parser.add_argument(
             '-f',
             '--fromdate',
-            help='Include metrics from this date.',
+            help='Include metrics/events from this date.',
             default=datetime.datetime.strptime('1970-01-01', '%Y-%m-%d'),
             type=self.valid_date
             )
         self.parser.add_argument(
+            '-m',
+            '--metricfile',
+            help='Add metrics csv file. Header: '
+                 + '# date;hostname;metric_name;metric_value',
+            type=self.valid_path
+            )
+        self.parser.add_argument(
             '-o',
             '--outputpath',
             help='Path to put output files. Default `./sarcharts`.',
             default='.'
             )
         self.parser.add_argument(
             '-t',
             '--todate',
-            help='Discard metrics after this date.',
+            help='Include metrics/events before this date.',
             default=datetime.datetime.strptime('2039-01-01', '%Y-%m-%d'),
             type=self.valid_date
             )
         self.parser.add_argument(
             '-q',
             '--quiet',
             help="Don't show progress.",
@@ -113,15 +121,16 @@
 
     def main(self):
         if len(self.args.sarfilespaths) > 0:
             sarfiles = util.get_filelist(self.args.sarfilespaths)
             if len(sarfiles) > 0:
                 util.debug(self.args, 'D', "sarfiles: " + str(sarfiles))
                 charts = Sadf().sar_to_chartjs(self.args, sarfiles)
-                charts = Events.getCSVdata(self.args, charts)
+                #charts = Events.getCSVdata(self.args, charts)
+                # charts = Metrics.getCSVdata(self.args, charts)
                 ChartJS().write_files(self.args, charts)
                 util.debug(self.args, '', "Open SarCharts in default browser.")
                 webbrowser.open(self.args.outputpath, 0, True)
             else:
                 self.parser.print_help()
                 util.debug(
                     self.args, 'E',
```

### Comparing `sarcharts-0.2.4/sarcharts/html/css/sarcharts.css` & `sarcharts-0.2.5/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/html/css/ul-select.css` & `sarcharts-0.2.5/sarcharts/html/css/ul-select.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/html/js/chart.umd.js` & `sarcharts-0.2.5/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js` & `sarcharts-0.2.5/sarcharts/html/js/chartjs-adapter-date-fns.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/html/js/chartjs-plugin-annotation.min.js` & `sarcharts-0.2.5/sarcharts/html/js/chartjs-plugin-annotation.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.2.5/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/html/js/hammer.min.js` & `sarcharts-0.2.5/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/html/js/jquery.js` & `sarcharts-0.2.5/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/html/js/ul-select.js` & `sarcharts-0.2.5/sarcharts/html/js/ul-select.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/lib/chartjs.py` & `sarcharts-0.2.5/sarcharts/lib/chartjs.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/lib/events.py` & `sarcharts-0.2.5/sarcharts/lib/events.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/lib/progressbar.py` & `sarcharts-0.2.5/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/lib/sadf.py` & `sarcharts-0.2.5/sarcharts/lib/sadf.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return data
 
     def data_normalization(self, act, data):
         if isinstance(data, list) and isinstance(data[0], dict):
             print(f"{act} is type 1")
             headers = ";".join(data[0].keys())
             print(headers)
-            
+
     def sar_to_chartjs(self, args, sarfiles):
         data = self.merge_sarfiles(args, sarfiles)
         linehead = "# hostname;interval;timestamp"
         pb = ProgressBar()
         pb.quiet = args.quiet
         all_entries = 0
         for idata in range(len(data)):
@@ -88,15 +88,14 @@
                         if act == "timestamp":
                             date = f"{adata['date']} {adata['time']}"
                             if (date not in charts[nodename]['xlabels']
                                     and util.in_date_range(args, date)):
                                 charts[nodename]['xlabels'].append(date)
                             linedet = f"{hdata['nodename']};{adata['interval']};{date}"
                         else:
-                            # self.data_normalization(act, adata)
                             if isinstance(adata, list):
                                 if act not in charts[nodename]['activities'].keys():
                                     line = linehead
                                     for h in adata[0].keys():
                                         line += f";{str(h)}"
                                     charts[nodename]['activities'][act] = {
                                         "content": [line.split(";")],
@@ -105,65 +104,82 @@
                                 for d in adata:
                                     line = linedet
                                     for v in d.values():
                                         line += f";{str(v)}"
                                     charts[nodename]['activities'][act][
                                         'content'].append(line.split(";"))
                             elif isinstance(adata, dict):
-                                for subact, subdata in adata.items():
-                                    nact = f"{act}_{subact}"
-                                    if isinstance(subdata, float) or isinstance(subdata, int):
-                                        if (act not in charts[nodename][
-                                                'activities'].keys()):
-                                            line = linehead
-                                            for h in adata.keys():
-                                                line += f";{str(h)}"
-                                            charts[nodename]['activities'][act] = {
-                                                "content": [line.split(";")],
-                                                "multiple": False
-                                                }
-                                        line = linedet
-                                        line += f";{str(subdata)}"
-                                        charts[nodename]['activities'][act][
-                                            'content'].append(line.split(";"))
-                                    elif isinstance(subdata, list):
-                                        if (nact not in charts[nodename][
-                                                'activities'].keys()):
-                                            line = linehead
-                                            for h in subdata[0].keys():
-                                                line += f";{str(h)}"
-                                            charts[nodename]['activities'][nact] = {
-                                                "content": [line.split(";")],
-                                                "multiple": True
-                                                }
-                                        for sv in subdata:
+                                d = adata[list(adata.keys())[1]]
+                                if isinstance(d, float) or isinstance(d, int):
+                                    if (act not in charts[nodename][
+                                            'activities'].keys()):
+                                        line = linehead
+                                        for h in adata.keys():
+                                            line += f";{str(h)}"
+                                        charts[nodename]['activities'][act] = {
+                                            "content": [line.split(";")],
+                                            "multiple": False
+                                            }
+                                    line = linedet
+                                    for v in adata.values():
+                                        line += f";{str(v)}"
+                                    charts[nodename]['activities'][act][
+                                        'content'].append(line.split(";"))
+                                else:
+                                    for subact, subdata in adata.items():
+                                        nact = f"{act}_{subact}"
+                                        if isinstance(subdata, list):
+                                            if (nact not in charts[nodename][
+                                                    'activities'].keys()):
+                                                line = linehead
+                                                for h in subdata[0].keys():
+                                                    line += f";{str(h)}"
+                                                charts[nodename]['activities'][nact] = {
+                                                    "content": [line.split(";")],
+                                                    "multiple": True
+                                                    }
+                                            for sv in subdata:
+                                                line = linedet
+                                                for v in sv.values():
+                                                    line += f";{str(v)}"
+                                                charts[nodename]['activities'][nact]['content'].append(line.split(";"))                                        
+                                        elif isinstance(subdata, dict):
+                                            if nact not in charts[nodename]['activities'].keys():
+                                                line = linehead
+                                                for h in subdata.keys():
+                                                    line += f";{str(h)}"
+                                                charts[nodename]['activities'][nact] = {
+                                                    "content": [line.split(";")],
+                                                    "multiple": False
+                                                    }
                                             line = linedet
-                                            for v in sv.values():
+                                            for v in subdata.values():
                                                 line += f";{str(v)}"
                                             charts[nodename]['activities'][nact]['content'].append(line.split(";"))                                        
-                                    else:
-                                        if nact not in charts[nodename]['activities'].keys():
-                                            line = linehead
-                                            for h in subdata.keys():
-                                                line += f";{str(h)}"
-                                            charts[nodename]['activities'][nact] = {
-                                                "content": [line.split(";")],
-                                                "multiple": False
-                                                }
-                                        line = linedet
-                                        for v in subdata.values():
-                                            line += f";{str(v)}"
-                                        charts[nodename]['activities'][nact]['content'].append(line.split(";"))                                        
+
+                                        elif isinstance(subdata, float) or isinstance(subdata, int):
+                                            if (nact not in charts[nodename][
+                                                    'activities'].keys()):
+                                                line = f"{linehead};{nact}"
+                                                charts[nodename]['activities'][nact] = {
+                                                    "content": [line.split(";")],
+                                                    "multiple": False
+                                                    }
+                                            line = f"{linedet};{str(subdata)}"
+                                            charts[nodename]['activities'][nact][
+                                                'content'].append(line.split(";"))
 
         pb.finish("  Get data.")
         # write csv files
         for nodename, nodecharts in charts.items():
             for activity, csvdata in charts[nodename]['activities'].items():
                 with open(f"{args.outputpath}/sar/{nodename}_{activity}.csv", "w") as f:
-                    f.write(";".join(csvdata['content'][0]) + "\n")
+                    # workaround for io.cs headers (maybe other activities)
+                    n = len(csvdata['content'][1])
+                    f.write(";".join(csvdata['content'][0][:n]) + "\n")
                     csvdata['content'].pop(0)
                     csvdata['content'].sort(key=lambda x: x[2])
                     for line in csvdata['content']:
                         if util.in_date_range(args, line[2]):
                             f.write(";".join(line) + "\n")
 
         # build the chartjs dict
@@ -180,23 +196,23 @@
                     # get first stats date
                     pos = f.tell()
                     line = f.readline().split(";")
                     # seek file to first stats line
                     f.seek(pos)
                     for line in f:
                         fields = line.strip().split(";")
-                        # set fake item on non multiple nodecharts
+                        # insert a fake item on non multiple nodecharts
                         item = fields[3] if csvdata['multiple'] else ""
                         if item not in charts[nodename]['activities'][activity]['datasets'].keys():
                             charts[nodename]['activities'][activity]['datasets'][item] = []
                             for h in headers:
                                 charts[nodename]['activities'][activity]['datasets'][item].append({
                                     "label": h,
                                     "values": []
                                     })
-                        
+
                         for f in range(len(fields[datastart:])):
                             charts[nodename]['activities'][activity]['datasets'][item][f]['values'].append({
                                     'x': fields[2],
                                     'y': fields[f+datastart]
                                     })
         return charts
```

### Comparing `sarcharts-0.2.4/sarcharts/lib/util.py` & `sarcharts-0.2.5/sarcharts/lib/util.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts/templates/chart.html` & `sarcharts-0.2.5/sarcharts/templates/chart.html`

 * *Files 6% similar despite different names*

```diff
@@ -102,21 +102,29 @@
               'hour': 'yyyy:LL:dd HH:mm:ss',
               'day': 'yyyy:LL:dd HH:mm:ss',
               'week': 'yyyy:LL:dd HH:mm:ss',
               'month': 'yyyy:LL:dd HH:mm:ss',
               'quarter': 'yyyy LL:dd HH:mm:ss',
               'year': 'yyyy:LL:dd HH:mm:ss'
             }
+          },
+          ticks: {
+            source: 'auto'
           }
         },
         y: {
           title: {
             display: false,
             text: 'value'
           }
+        },
+        y1: {
+        type: 'linear',
+        display: true,
+        position: 'right'
         }
       },
       plugins: {
         legend: {
           position: 'top'
         },
         annotation: { annotations: { 
@@ -148,21 +156,25 @@
 }
 
 var myCharts = {
   {% for item, data in details['datasets'].items() %}
   '{{ item }}': {
     'datasets': [
     {% for i in range(data|length) %}
-      {
-      {{ "hidden: true," if data[i]['label'] in details['hidden'] else "" }}
-      label: '{{ data[i]['label'] }}',
-      data: {{ data[i]['values'] }},
-      borderColor: 'rgb({{ colors[i] }} 0.3)',
-      backgroundColor: 'rgb({{ colors[i] }})'
-      }{{ ", " if not loop.last else "" }}
+      {% if data[i]['values']|length > 0 %}
+        {
+        {{ "hidden: true," if data[i]['label'] in details['hidden'] else "" }}
+        label: '{{ data[i]['label'] }}',
+        yAxisID: '{{ data[i]['yAxisID']|default('y') }}',
+        type: '{{ data[i]['type']|default('bar') }}',
+        data: {{ data[i]['values'] }},
+        borderColor: 'rgb({{ colors[i] }})',
+        backgroundColor: 'rgb({{ colors[i] }})'
+        }{{ ", " if not loop.last else "" }}
+      {% endif %}
     {% endfor %}
     ]
   }{{ ", " if not loop.last else "" }}
   {% endfor %}
 }
 
 var ctx = document.getElementById('chartcanvas').getContext('2d');
```

### Comparing `sarcharts-0.2.4/sarcharts/templates/header.html` & `sarcharts-0.2.5/sarcharts/templates/header.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.2.5/sarcharts.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.2.4
+Version: 0.2.5
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -27,33 +27,35 @@
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
 ### Installation
 `pip install sarcharts`
 
 ### Usage
 ~~~
-usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
+usage: sarcharts [-h] [-d {D,I,W,E}] [-e EVENTFILE] [-f FROMDATE] [-m METRICFILE] [-o OUTPUTPATH] [-t TODATE] [-q] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
   sarfilespaths         `sa` file/s to parse. Default: `./sa??`.
 
 optional arguments:
   -h, --help            show this help message and exit
   -d {D,I,W,E}, --debug {D,I,W,E}
                         Set debug level. Default `W`.
   -e EVENTFILE, --eventfile EVENTFILE
                         Add events csv file. Header: # date;hostname;event_name;event_description
   -f FROMDATE, --fromdate FROMDATE
-                        Include metrics from this date.
+                        Include metrics/events from this date.
+  -m METRICFILE, --metricfile METRICFILE
+                        Add metrics csv file. Header: # date;hostname;metric_name;metric_value
   -o OUTPUTPATH, --outputpath OUTPUTPATH
                         Path to put output files. Default `./sarcharts`.
   -t TODATE, --todate TODATE
-                        Discard metrics after this date.
+                        Include metrics/events before this date.
   -q, --quiet           Don't show progress.
 ~~~
 
 | Example Chart |
 | --- |
 | ![](/doc/sarcharts.png) |
```

### Comparing `sarcharts-0.2.4/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.2.5/sarcharts.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,12 +30,13 @@
 sarcharts/html/js/chartjs-plugin-annotation.min.js
 sarcharts/html/js/chartjs-plugin-zoom.min.js
 sarcharts/html/js/hammer.min.js
 sarcharts/html/js/jquery.js
 sarcharts/html/js/ul-select.js
 sarcharts/lib/chartjs.py
 sarcharts/lib/events.py
+sarcharts/lib/metrics.py
 sarcharts/lib/progressbar.py
 sarcharts/lib/sadf.py
 sarcharts/lib/util.py
 sarcharts/templates/chart.html
 sarcharts/templates/header.html
```

### Comparing `sarcharts-0.2.4/setup.cfg` & `sarcharts-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/setup.py` & `sarcharts-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.2.4/tox.ini` & `sarcharts-0.2.5/tox.ini`

 * *Files identical despite different names*

