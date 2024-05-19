# Comparing `tmp/elicznik-2.1.0.tar.gz` & `tmp/elicznik-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elicznik-2.1.0.tar", last modified: Tue Apr  2 19:40:44 2024, max compression
+gzip compressed data, was "elicznik-2.2.0.tar", last modified: Sun May 19 16:09:43 2024, max compression
```

## Comparing `elicznik-2.1.0.tar` & `elicznik-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:44.667510 elicznik-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-02 19:40:38.000000 elicznik-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-02 19:40:44.667510 elicznik-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-02 19:40:38.000000 elicznik-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 19:40:44.671510 elicznik-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-02 19:40:38.000000 elicznik-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:44.667510 elicznik-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:44.667510 elicznik-2.1.0/src/elicznik/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 19:40:38.000000 elicznik-2.1.0/src/elicznik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-02 19:40:38.000000 elicznik-2.1.0/src/elicznik/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4774 2024-04-02 19:40:38.000000 elicznik-2.1.0/src/elicznik/elicznik.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-02 19:40:38.000000 elicznik-2.1.0/src/elicznik/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:44.667510 elicznik-2.1.0/src/elicznik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:09:43.009736 elicznik-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-19 16:09:39.000000 elicznik-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-19 16:09:43.009736 elicznik-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-19 16:09:39.000000 elicznik-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-19 16:09:43.009736 elicznik-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-19 16:09:39.000000 elicznik-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:09:43.005736 elicznik-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:09:43.005736 elicznik-2.2.0/src/elicznik/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-19 16:09:39.000000 elicznik-2.2.0/src/elicznik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-19 16:09:39.000000 elicznik-2.2.0/src/elicznik/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5189 2024-05-19 16:09:39.000000 elicznik-2.2.0/src/elicznik/elicznik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-19 16:09:39.000000 elicznik-2.2.0/src/elicznik/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:09:43.009736 elicznik-2.2.0/src/elicznik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-19 16:09:42.000000 elicznik-2.2.0/src/elicznik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-19 16:09:43.000000 elicznik-2.2.0/src/elicznik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 16:09:42.000000 elicznik-2.2.0/src/elicznik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 16:09:42.000000 elicznik-2.2.0/src/elicznik.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 16:09:42.000000 elicznik-2.2.0/src/elicznik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 16:09:42.000000 elicznik-2.2.0/src/elicznik.egg-info/top_level.txt
```

### Comparing `elicznik-2.1.0/LICENSE` & `elicznik-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elicznik-2.1.0/PKG-INFO` & `elicznik-2.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,65 @@
-Metadata-Version: 2.1
-Name: elicznik
-Version: 2.1.0
-Summary: Tauron eLicznik scrapper
-Home-page: https://github.com/mlesniew/elicznik
-Author: Michał Leśniewski
-Author-email: mlesniew@gmail.com
-Keywords: elicznik,tauron,scrapper
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Home Automation
-Classifier: Topic :: Internet
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: tabulate
-
 # Tauron eLicznik Scraper
 
 This Python 3 package allows to read electric energy meter reading history from the 
 [Tauron eLicznik](https://elicznik.tauron-dystrybucja.pl/) website.
 
 
 ## Installation
 
 The package can be installed using pip:
 
 ```
 $ pip3 install elicznik
 ```
 
+or alternatively:
+```
+$ pip3 install git@github.com:mlesniew/elicznik.git
+```
+
+
 
 ## Command line usage
 
 With the package installed readings can be retrieved by simply running the `elicznik` command:
 ```
-usage: elicznik [-h] [--format {table,csv}] [--api {chart,csv}] username password [start_date] [end_date]
+usage: elicznik [-h] [--format {table,csv}] [--api {chart,csv}] [--site SITE] username password [start_date] [end_date]
+
+positional arguments:
+  username              tauron-dystrybucja.pl user name
+  password              tauron-dystrybucja.pl password
+  start_date            Start date of date range to be retrieved, in ISO8601 format. If the end date is omitted, it's the only date for which measurements are retrieved.
+  end_date              End date of date range to be retrieved, inclusive, in ISO8601 format. Can be omitted to only retrieve a single day's measurements.
+
+options:
+  -h, --help            show this help message and exit
+  --format {table,csv}  Specify the output format
+  --api {chart,csv}     Specify which Tauron API to use to get the measurements
+  --site SITE           site identifier, must match '[0-9]+_[0-9]+_[0-9]+'
+(venv) ~/src/elicznik (site) $ elicznik --help | cat
+usage: elicznik [-h] [--format {table,csv}] [--api {chart,csv}] [--site SITE]
+                username password [start_date] [end_date]
 
 positional arguments:
   username              tauron-dystrybucja.pl user name
   password              tauron-dystrybucja.pl password
-  start_date            Start date of date range to be retrieved, in ISO8601 format. If the end date is omitted, it's the only date for which
-                        measurements are retrieved.
-  end_date              End date of date range to be retrieved, inclusive, in ISO8601 format. Can be omitted to only retrieve a single day's
-                        measurements.
+  start_date            Start date of date range to be retrieved, in ISO8601
+                        format. If the end date is omitted, it's the only date
+                        for which measurements are retrieved.
+  end_date              End date of date range to be retrieved, inclusive, in
+                        ISO8601 format. Can be omitted to only retrieve a
+                        single day's measurements.
 
 options:
   -h, --help            show this help message and exit
   --format {table,csv}  Specify the output format
-  --api {chart,csv}     Specify which Tauron API to use to get the measurements.
+  --api {chart,csv}     Specify which Tauron API to use to get the
+                        measurements
+  --site SITE           site identifier, must match '[0-9]+_[0-9]+_[0-9]+'
 ```
 
 
 ### Example
 
 ```
 $ elicznik freddy@example.com secretpassword 2022-07-20
@@ -92,31 +94,31 @@
 
 ## API usage
 
 ```
 import datetime
 import elicznik
 
-with elicznik.ELicznik("freddy@example.com", "secretpassword") as m:
+with elicznik.ELicznik("freddy@example.com", "secretpassword", "optional_site_identifier") as m:
     # date range
     print("July 2021")
 
     readings = m.get_readings(datetime.date(2021, 7, 1), datetime.date(2021, 7, 31))
 
-    for timestamp, consumed, produced in readings:
-        print(timestamp, consumed, produced)
+    for timestamp, consumed, produced, consumed_net, produced_net in readings:
+        print(timestamp, consumed, produced, consumed_net, produced_net)
 
     # single day
     print("Yesterday")
 
     yesterday = datetime.date.today() - datetime.timedelta(days=1)
     readings = m.get_readings(yesterday)
 
-    for timestamp, consumed, produced in readings:
-        print(timestamp, consumed, produced)
+    for timestamp, consumed, produced, consumed_net, produced_net in readings:
+        print(timestamp, consumed, produced, consumed_net, produced_net)
 ```
 
 
 ## Notes on APIs and the `--api` command line switch
 
 Tauron exposes two API endpoints for retrieving meter readings -- one for downloading CSV (and XLS) data,
 the other is a back-end supporting the charts in the Web UI.  In theory, both endpoints are equivalent.
@@ -140,15 +142,14 @@
 with elicznik.ELicznikChart("freddy@example.com", "secretpassword") as m:
     ...
 ```
 
 
 ## TODO & bugs
 
-* Add support for accounts with multiple meters
 * Convert the dates to UTC and handle switches from and to DST properly
 * Make the dependency on tabulate optional
 
 
 ## Similar projects
 
 This project is based on the excellent
```

### Comparing `elicznik-2.1.0/setup.py` & `elicznik-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='elicznik',
-    version='2.1.0',
+    version='2.2.0',
     description='Tauron eLicznik scrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mlesniew/elicznik',
     author='Michał Leśniewski',
     author_email='mlesniew@gmail.com',
     classifiers=[
```

### Comparing `elicznik-2.1.0/src/elicznik/__main__.py` & `elicznik-2.2.0/src/elicznik/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 import argparse
 import csv
 import datetime
 import sys
+import re
 
 import tabulate
 
 from .elicznik import ELicznikChart, ELicznikCSV
 
+SITE_ID_PATTERN = "[0-9]+_[0-9]+_[0-9]+"
+
+def parse_site(site):
+    match = re.match(SITE_ID_PATTERN, site)
+    if not match:
+        raise ValueError
+    return match.string
+
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--format",
         choices=["table", "csv"],
         default="table",
         help="Specify the output format",
     )
     parser.add_argument(
         "--api",
         choices=["chart", "csv"],
         default="csv",
-        help="Specify which Tauron API to use to get the measurements. ",
+        help="Specify which Tauron API to use to get the measurements",
+    )
+    parser.add_argument(
+        "--site",
+        type=parse_site,
+        default=None,
+        help=f"site identifier, must match '{SITE_ID_PATTERN}'",
     )
     parser.add_argument("username", help="tauron-dystrybucja.pl user name")
     parser.add_argument("password", help="tauron-dystrybucja.pl password")
     parser.add_argument(
         "start_date",
         nargs="?",
         type=datetime.date.fromisoformat,
@@ -43,25 +58,25 @@
         "day's measurements.",
     )
 
     args = parser.parse_args()
 
     elicznik_class = ELicznikCSV if args.api == "csv" else ELicznikChart
 
-    with elicznik_class(args.username, args.password) as elicznik:
+    with elicznik_class(args.username, args.password, args.site) as elicznik:
         result = elicznik.get_readings(args.start_date, args.end_date)
 
         if args.format == "table":
             print(
                 tabulate.tabulate(
                     result,
                     headers=[
                         "timestamp",
-                        "consumed",
-                        "produced",
+                        "consumption",
+                        "production",
                         "net consumption",
                         "net production",
                     ],
                 )
             )
         else:
             writer = csv.writer(sys.stdout)
```

### Comparing `elicznik-2.1.0/src/elicznik/elicznik.py` & `elicznik-2.2.0/src/elicznik/elicznik.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 #!/usr/bin/env python3
 
+import collections
 import csv
 import datetime
 
 from .session import Session
 
 
+Reading = collections.namedtuple("Reading", "timestamp consumption production net_consumption net_production")
+
+
 class ELicznikBase:
     LOGIN_URL = "https://logowanie.tauron-dystrybucja.pl/login"
 
-    def __init__(self, username, password):
+    def __init__(self, username, password, site=None):
         self.username = username
         self.password = password
+        self.site = site
 
     def login(self):
         self.session = Session()
         self.session.get(self.LOGIN_URL)
         self.session.post(
             self.LOGIN_URL,
             data={
                 "username": self.username,
                 "password": self.password,
                 "service": "https://elicznik.tauron-dystrybucja.pl",
             },
         )
+        if self.site is not None:
+            self.session.post(
+                "https://elicznik.tauron-dystrybucja.pl/ustaw_punkt",
+                data={
+                    "site[client]": self.site
+                },
+            )
 
     def __enter__(self):
         self.login()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
@@ -73,15 +85,15 @@
 
         timestamps = set(sum((list(v) for v in results.values()), start=[]))
 
         # TODO
         # This probably drops the data from the double hour during DST change
         # Needs to be investigated and fixed
         return sorted(
-            tuple([timestamp] + [results[name].get(timestamp) for name in COLUMNS])
+            Reading(*([timestamp] + [results[name].get(timestamp) for name in COLUMNS]))
             for timestamp in timestamps
         )
 
 
 class ELicznikCSV(ELicznikBase):
     DATA_URL = "https://elicznik.tauron-dystrybucja.pl/energia/do/dane"
 
@@ -144,13 +156,13 @@
 
         timestamps = set(sum((list(v) for v in results.values()), start=[]))
 
         # TODO
         # This probably drops the data from the double hour during DST change
         # Needs to be investigated and fixed
         return sorted(
-            tuple([timestamp] + [results[name].get(timestamp) for name in COLUMNS])
+            Reading(*([timestamp] + [results[name].get(timestamp) for name in COLUMNS]))
             for timestamp in timestamps
         )
 
 
 ELicznik = ELicznikCSV
```

### Comparing `elicznik-2.1.0/src/elicznik/session.py` & `elicznik-2.2.0/src/elicznik/session.py`

 * *Files identical despite different names*

### Comparing `elicznik-2.1.0/src/elicznik.egg-info/PKG-INFO` & `elicznik-2.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elicznik
-Version: 2.1.0
+Version: 2.2.0
 Summary: Tauron eLicznik scrapper
 Home-page: https://github.com/mlesniew/elicznik
 Author: Michał Leśniewski
 Author-email: mlesniew@gmail.com
 Keywords: elicznik,tauron,scrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -31,33 +31,58 @@
 
 The package can be installed using pip:
 
 ```
 $ pip3 install elicznik
 ```
 
+or alternatively:
+```
+$ pip3 install git@github.com:mlesniew/elicznik.git
+```
+
+
 
 ## Command line usage
 
 With the package installed readings can be retrieved by simply running the `elicznik` command:
 ```
-usage: elicznik [-h] [--format {table,csv}] [--api {chart,csv}] username password [start_date] [end_date]
+usage: elicznik [-h] [--format {table,csv}] [--api {chart,csv}] [--site SITE] username password [start_date] [end_date]
+
+positional arguments:
+  username              tauron-dystrybucja.pl user name
+  password              tauron-dystrybucja.pl password
+  start_date            Start date of date range to be retrieved, in ISO8601 format. If the end date is omitted, it's the only date for which measurements are retrieved.
+  end_date              End date of date range to be retrieved, inclusive, in ISO8601 format. Can be omitted to only retrieve a single day's measurements.
+
+options:
+  -h, --help            show this help message and exit
+  --format {table,csv}  Specify the output format
+  --api {chart,csv}     Specify which Tauron API to use to get the measurements
+  --site SITE           site identifier, must match '[0-9]+_[0-9]+_[0-9]+'
+(venv) ~/src/elicznik (site) $ elicznik --help | cat
+usage: elicznik [-h] [--format {table,csv}] [--api {chart,csv}] [--site SITE]
+                username password [start_date] [end_date]
 
 positional arguments:
   username              tauron-dystrybucja.pl user name
   password              tauron-dystrybucja.pl password
-  start_date            Start date of date range to be retrieved, in ISO8601 format. If the end date is omitted, it's the only date for which
-                        measurements are retrieved.
-  end_date              End date of date range to be retrieved, inclusive, in ISO8601 format. Can be omitted to only retrieve a single day's
-                        measurements.
+  start_date            Start date of date range to be retrieved, in ISO8601
+                        format. If the end date is omitted, it's the only date
+                        for which measurements are retrieved.
+  end_date              End date of date range to be retrieved, inclusive, in
+                        ISO8601 format. Can be omitted to only retrieve a
+                        single day's measurements.
 
 options:
   -h, --help            show this help message and exit
   --format {table,csv}  Specify the output format
-  --api {chart,csv}     Specify which Tauron API to use to get the measurements.
+  --api {chart,csv}     Specify which Tauron API to use to get the
+                        measurements
+  --site SITE           site identifier, must match '[0-9]+_[0-9]+_[0-9]+'
 ```
 
 
 ### Example
 
 ```
 $ elicznik freddy@example.com secretpassword 2022-07-20
@@ -92,31 +117,31 @@
 
 ## API usage
 
 ```
 import datetime
 import elicznik
 
-with elicznik.ELicznik("freddy@example.com", "secretpassword") as m:
+with elicznik.ELicznik("freddy@example.com", "secretpassword", "optional_site_identifier") as m:
     # date range
     print("July 2021")
 
     readings = m.get_readings(datetime.date(2021, 7, 1), datetime.date(2021, 7, 31))
 
-    for timestamp, consumed, produced in readings:
-        print(timestamp, consumed, produced)
+    for timestamp, consumed, produced, consumed_net, produced_net in readings:
+        print(timestamp, consumed, produced, consumed_net, produced_net)
 
     # single day
     print("Yesterday")
 
     yesterday = datetime.date.today() - datetime.timedelta(days=1)
     readings = m.get_readings(yesterday)
 
-    for timestamp, consumed, produced in readings:
-        print(timestamp, consumed, produced)
+    for timestamp, consumed, produced, consumed_net, produced_net in readings:
+        print(timestamp, consumed, produced, consumed_net, produced_net)
 ```
 
 
 ## Notes on APIs and the `--api` command line switch
 
 Tauron exposes two API endpoints for retrieving meter readings -- one for downloading CSV (and XLS) data,
 the other is a back-end supporting the charts in the Web UI.  In theory, both endpoints are equivalent.
@@ -140,15 +165,14 @@
 with elicznik.ELicznikChart("freddy@example.com", "secretpassword") as m:
     ...
 ```
 
 
 ## TODO & bugs
 
-* Add support for accounts with multiple meters
 * Convert the dates to UTC and handle switches from and to DST properly
 * Make the dependency on tabulate optional
 
 
 ## Similar projects
 
 This project is based on the excellent
```

