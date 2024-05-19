# Comparing `tmp/plum_project-1.0.0.tar.gz` & `tmp/plum_project-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plum_project-1.0.0.tar", last modified: Sat May 18 01:58:59 2024, max compression
+gzip compressed data, was "plum_project-1.0.1.tar", last modified: Sun May 19 19:28:11 2024, max compression
```

## Comparing `plum_project-1.0.0.tar` & `plum_project-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.596816 plum_project-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 01:58:54.000000 plum_project-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-18 01:58:59.596816 plum_project-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-18 01:58:54.000000 plum_project-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.592816 plum_project-1.0.0/plum/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.592816 plum_project-1.0.0/plum/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.592816 plum_project-1.0.0/plum/clients/postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/postgresql/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.592816 plum_project-1.0.0/plum/clients/postgresql/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/postgresql/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/postgresql/connectors/base_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/postgresql/connectors/sql_login_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.592816 plum_project-1.0.0/plum/clients/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/s3/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.592816 plum_project-1.0.0/plum/clients/s3/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/s3/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/s3/connectors/access_key_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/clients/s3/connectors/base_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.592816 plum_project-1.0.0/plum/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/jobs/base_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.596816 plum_project-1.0.0/plum/jobs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:54.000000 plum_project-1.0.0/plum/jobs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:59.596816 plum_project-1.0.0/plum_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-18 01:58:59.000000 plum_project-1.0.0/plum_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-18 01:58:59.000000 plum_project-1.0.0/plum_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:58:59.000000 plum_project-1.0.0/plum_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-18 01:58:59.000000 plum_project-1.0.0/plum_project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 01:58:59.000000 plum_project-1.0.0/plum_project.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 01:58:59.596816 plum_project-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-18 01:58:54.000000 plum_project-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.422636 plum_project-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 19:28:07.000000 plum_project-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-19 19:28:11.422636 plum_project-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 19:28:07.000000 plum_project-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.418636 plum_project-1.0.1/plum/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.418636 plum_project-1.0.1/plum/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.418636 plum_project-1.0.1/plum/clients/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/postgresql/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.418636 plum_project-1.0.1/plum/clients/postgresql/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/postgresql/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/postgresql/connectors/base_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/postgresql/connectors/sql_login_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.418636 plum_project-1.0.1/plum/clients/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/s3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.418636 plum_project-1.0.1/plum/clients/s3/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/s3/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/s3/connectors/access_key_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/clients/s3/connectors/base_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.418636 plum_project-1.0.1/plum/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/jobs/base_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.422636 plum_project-1.0.1/plum/jobs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/jobs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.422636 plum_project-1.0.1/plum/jobs/utils/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/jobs/utils/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-19 19:28:07.000000 plum_project-1.0.1/plum/jobs/utils/execution/recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:11.422636 plum_project-1.0.1/plum_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-19 19:28:11.000000 plum_project-1.0.1/plum_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 19:28:11.000000 plum_project-1.0.1/plum_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:28:11.000000 plum_project-1.0.1/plum_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-19 19:28:11.000000 plum_project-1.0.1/plum_project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-19 19:28:11.000000 plum_project-1.0.1/plum_project.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:28:11.422636 plum_project-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-19 19:28:07.000000 plum_project-1.0.1/setup.py
```

### Comparing `plum_project-1.0.0/LICENSE` & `plum_project-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plum_project-1.0.0/README.md` & `plum_project-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `plum_project-1.0.0/plum/clients/postgresql/client.py` & `plum_project-1.0.1/plum/clients/postgresql/client.py`

 * *Files identical despite different names*

### Comparing `plum_project-1.0.0/plum/clients/postgresql/connectors/sql_login_connector.py` & `plum_project-1.0.1/plum/clients/postgresql/connectors/sql_login_connector.py`

 * *Files identical despite different names*

### Comparing `plum_project-1.0.0/plum/clients/s3/client.py` & `plum_project-1.0.1/plum/clients/s3/client.py`

 * *Files identical despite different names*

### Comparing `plum_project-1.0.0/plum/clients/s3/connectors/access_key_connector.py` & `plum_project-1.0.1/plum/clients/s3/connectors/access_key_connector.py`

 * *Files identical despite different names*

### Comparing `plum_project-1.0.0/plum/clients/s3/connectors/base_connector.py` & `plum_project-1.0.1/plum/clients/s3/connectors/base_connector.py`

 * *Files identical despite different names*

### Comparing `plum_project-1.0.0/plum/jobs/base_job.py` & `plum_project-1.0.1/plum/jobs/base_job.py`

 * *Files identical despite different names*

### Comparing `plum_project-1.0.0/plum_project.egg-info/SOURCES.txt` & `plum_project-1.0.1/plum_project.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 plum/clients/s3/client.py
 plum/clients/s3/connectors/__init__.py
 plum/clients/s3/connectors/access_key_connector.py
 plum/clients/s3/connectors/base_connector.py
 plum/jobs/__init__.py
 plum/jobs/base_job.py
 plum/jobs/utils/__init__.py
+plum/jobs/utils/execution/__init__.py
+plum/jobs/utils/execution/recorder.py
 plum_project.egg-info/PKG-INFO
 plum_project.egg-info/SOURCES.txt
 plum_project.egg-info/dependency_links.txt
 plum_project.egg-info/requires.txt
 plum_project.egg-info/top_level.txt
```

### Comparing `plum_project-1.0.0/setup.py` & `plum_project-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'plum-project',
-    version = '1.0.0',
+    version = '1.0.1',
     description = 'A python data job framework to simplify development and operations.',
     long_description = 'A python data job framework to simplify development and operations.',
     long_description_content_type = "text/markdown",
     keywords = ['data', 'etl', 'jobs'],
     packages = find_packages(),
     install_requires = [
         'psycopg[binary]==3.1.16',
```

