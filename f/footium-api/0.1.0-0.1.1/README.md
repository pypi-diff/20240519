# Comparing `tmp/footium_api-0.1.0.tar.gz` & `tmp/footium_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "footium_api-0.1.0.tar", last modified: Sat May 18 04:44:45 2024, max compression
+gzip compressed data, was "footium_api-0.1.1.tar", last modified: Sat May 18 05:24:22 2024, max compression
```

## Comparing `footium_api-0.1.0.tar` & `footium_api-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:44:45.380087 footium_api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-18 04:44:45.380087 footium_api-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 04:44:34.000000 footium_api-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:44:45.372087 footium_api-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 04:44:34.000000 footium_api-0.1.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-18 04:44:34.000000 footium_api-0.1.0/examples/setup_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-18 04:44:34.000000 footium_api-0.1.0/examples/try_best_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-18 04:44:34.000000 footium_api-0.1.0/examples/try_club_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-18 04:44:34.000000 footium_api-0.1.0/examples/try_footium_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-18 04:44:34.000000 footium_api-0.1.0/examples/try_formations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-18 04:44:34.000000 footium_api-0.1.0/examples/try_get_next_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-18 04:44:34.000000 footium_api-0.1.0/examples/try_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:44:45.372087 footium_api-0.1.0/footium_api/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/gql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/key_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:44:45.376087 footium_api-0.1.0/footium_api/mutations/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/mutations/lineups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:44:45.376087 footium_api-0.1.0/footium_api/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/queries/all_clubs_basic_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/queries/clubTournaments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/queries/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/queries/formations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/queries/lineups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/queries/players.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/queries/server_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 04:44:34.000000 footium_api-0.1.0/footium_api/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:44:45.376087 footium_api-0.1.0/footium_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-18 04:44:45.000000 footium_api-0.1.0/footium_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-18 04:44:45.000000 footium_api-0.1.0/footium_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 04:44:45.000000 footium_api-0.1.0/footium_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-18 04:44:45.000000 footium_api-0.1.0/footium_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 04:44:45.000000 footium_api-0.1.0/footium_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 04:44:34.000000 footium_api-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 04:44:45.380087 footium_api-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-18 04:44:34.000000 footium_api-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:44:45.376087 footium_api-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-18 04:44:34.000000 footium_api-0.1.0/tests/test_report_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:24:22.390615 footium_api-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-18 05:24:05.000000 footium_api-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-18 05:24:22.390615 footium_api-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 05:24:05.000000 footium_api-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:24:22.382614 footium_api-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 05:24:05.000000 footium_api-0.1.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-18 05:24:05.000000 footium_api-0.1.1/examples/setup_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-18 05:24:05.000000 footium_api-0.1.1/examples/try_best_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-18 05:24:05.000000 footium_api-0.1.1/examples/try_club_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-18 05:24:05.000000 footium_api-0.1.1/examples/try_footium_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-18 05:24:05.000000 footium_api-0.1.1/examples/try_formations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-18 05:24:05.000000 footium_api-0.1.1/examples/try_get_next_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-18 05:24:05.000000 footium_api-0.1.1/examples/try_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:24:22.386614 footium_api-0.1.1/footium_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/gql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/key_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:24:22.386614 footium_api-0.1.1/footium_api/mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/mutations/lineups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:24:22.386614 footium_api-0.1.1/footium_api/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/queries/all_clubs_basic_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/queries/clubTournaments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/queries/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/queries/formations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/queries/lineups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/queries/players.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/queries/server_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 05:24:05.000000 footium_api-0.1.1/footium_api/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:24:22.386614 footium_api-0.1.1/footium_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-18 05:24:22.000000 footium_api-0.1.1/footium_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-18 05:24:22.000000 footium_api-0.1.1/footium_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 05:24:22.000000 footium_api-0.1.1/footium_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-18 05:24:22.000000 footium_api-0.1.1/footium_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 05:24:22.000000 footium_api-0.1.1/footium_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 05:24:05.000000 footium_api-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 05:24:22.390615 footium_api-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-18 05:24:05.000000 footium_api-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:24:22.386614 footium_api-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-18 05:24:05.000000 footium_api-0.1.1/tests/test_report_strategy.py
```

### Comparing `footium_api-0.1.0/PKG-INFO` & `footium_api-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: footium_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: python api for the footium game
-Home-page: https://github.com/sohojoe/fooitum_api
+Home-page: https://github.com/Sohojoe/footium_api
 Author: SohoJoe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: python-box==7.1.1
 Requires-Dist: gql==3.5.0
 Requires-Dist: requests_toolbelt==1.0.0
 Requires-Dist: eth-account==0.12.2
 Requires-Dist: pandas==2.2.2
```

### Comparing `footium_api-0.1.0/examples/try_best_teams.py` & `footium_api-0.1.1/examples/try_best_teams.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/examples/try_club_stats.py` & `footium_api-0.1.1/examples/try_club_stats.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/examples/try_footium_api.py` & `footium_api-0.1.1/examples/try_footium_api.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/examples/try_get_next_fixtures.py` & `footium_api-0.1.1/examples/try_get_next_fixtures.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/gql_connection.py` & `footium_api-0.1.1/footium_api/gql_connection.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/key_signer.py` & `footium_api-0.1.1/footium_api/key_signer.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/mutations/lineups.py` & `footium_api-0.1.1/footium_api/mutations/lineups.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/queries/__init__.py` & `footium_api-0.1.1/footium_api/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/queries/clubTournaments.py` & `footium_api-0.1.1/footium_api/queries/clubTournaments.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/queries/fixtures.py` & `footium_api-0.1.1/footium_api/queries/fixtures.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/queries/formations.py` & `footium_api-0.1.1/footium_api/queries/formations.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/queries/lineups.py` & `footium_api-0.1.1/footium_api/queries/lineups.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/queries/players.py` & `footium_api-0.1.1/footium_api/queries/players.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api/report.py` & `footium_api-0.1.1/footium_api/report.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.0/footium_api.egg-info/PKG-INFO` & `footium_api-0.1.1/footium_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: footium_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: python api for the footium game
-Home-page: https://github.com/sohojoe/fooitum_api
+Home-page: https://github.com/Sohojoe/footium_api
 Author: SohoJoe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: python-box==7.1.1
 Requires-Dist: gql==3.5.0
 Requires-Dist: requests_toolbelt==1.0.0
 Requires-Dist: eth-account==0.12.2
 Requires-Dist: pandas==2.2.2
```

### Comparing `footium_api-0.1.0/footium_api.egg-info/SOURCES.txt` & `footium_api-0.1.1/footium_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 examples/__init__.py
 examples/setup_environment.py
 examples/try_best_teams.py
 examples/try_club_stats.py
```

### Comparing `footium_api-0.1.0/setup.py` & `footium_api-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="footium_api",
-    version="0.1.0",
+    version="0.1.1",
     author="SohoJoe",
     description="python api for the footium game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/sohojoe/fooitum_api",
+    url="https://github.com/Sohojoe/footium_api",
     packages=find_packages(),
     install_requires=[
         "python-dotenv==1.0.1",
         "pycryptodome==3.20.0",
         "python-box==7.1.1",
         "gql==3.5.0",
         "requests_toolbelt==1.0.0",
```

### Comparing `footium_api-0.1.0/tests/test_report_strategy.py` & `footium_api-0.1.1/tests/test_report_strategy.py`

 * *Files identical despite different names*

