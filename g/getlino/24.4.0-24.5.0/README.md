# Comparing `tmp/getlino-24.4.0.tar.gz` & `tmp/getlino-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getlino-24.4.0.tar", last modified: Fri Apr 12 23:15:52 2024, max compression
+gzip compressed data, was "getlino-24.5.0.tar", last modified: Sun May 19 07:15:05 2024, max compression
```

## Comparing `getlino-24.4.0.tar` & `getlino-24.5.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.971992 getlino-24.4.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:36.000000 getlino-24.4.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)       59 2019-10-25 15:17:06.000000 getlino-24.4.0/MANIFEST.in
--rw-r--r--   0 luc       (1000) www-data    (33)     1559 2024-04-12 23:15:52.971992 getlino-24.4.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      692 2021-06-11 08:29:48.000000 getlino-24.4.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.967992 getlino-24.4.0/getlino/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      322 2024-02-14 17:37:21.000000 getlino-24.4.0/getlino/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      816 2024-02-14 17:37:21.000000 getlino-24.4.0/getlino/cli.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    20445 2024-04-01 09:56:59.000000 getlino-24.4.0/getlino/configure.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      971 2024-04-01 15:27:49.000000 getlino-24.4.0/getlino/list.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1788 2024-04-12 23:15:26.000000 getlino-24.4.0/getlino/setup_info.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7794 2024-03-11 13:29:19.000000 getlino-24.4.0/getlino/startproject.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    25754 2024-04-01 09:53:27.000000 getlino-24.4.0/getlino/startsite.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.967992 getlino-24.4.0/getlino/templates/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2021-02-12 13:40:30.000000 getlino-24.4.0/getlino/templates/apache.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)      214 2022-09-10 15:27:38.000000 getlino-24.4.0/getlino/templates/asgi.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1678 2024-02-22 15:57:56.000000 getlino-24.4.0/getlino/templates/daphne_supervisor.conf
--rw-rw-r--   0 luc       (1000) www-data    (33)      852 2023-01-01 07:07:06.000000 getlino-24.4.0/getlino/templates/django_settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      371 2023-07-01 18:31:56.000000 getlino-24.4.0/getlino/templates/healthcheck.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)      308 2023-01-15 18:29:24.000000 getlino-24.4.0/getlino/templates/lino.ini
--rwxrwxr-x   0 luc       (1000) www-data    (33)     2074 2022-09-15 06:25:41.000000 getlino-24.4.0/getlino/templates/make_snapshot.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)      329 2023-11-05 18:22:29.000000 getlino-24.4.0/getlino/templates/manage.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1671 2023-07-16 11:11:44.000000 getlino-24.4.0/getlino/templates/nginx.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1543 2022-09-10 15:27:38.000000 getlino-24.4.0/getlino/templates/nginx_asgi.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1558 2023-10-08 06:14:57.000000 getlino-24.4.0/getlino/templates/pull.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)     1472 2024-04-05 03:44:20.000000 getlino-24.4.0/getlino/templates/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2021-02-10 17:53:35.000000 getlino-24.4.0/getlino/templates/uwsgi.ini
--rw-rw-rw-   0 luc       (1000) www-data    (33)      664 2019-10-25 14:15:15.000000 getlino-24.4.0/getlino/templates/uwsgi_params
--rw-rw-rw-   0 luc       (1000) www-data    (33)      251 2019-10-25 14:30:31.000000 getlino-24.4.0/getlino/templates/wsgi.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    20855 2024-03-30 09:04:06.000000 getlino-24.4.0/getlino/utils.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.971992 getlino-24.4.0/getlino.egg-info/
--rw-r--r--   0 luc       (1000) www-data    (33)     1559 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      983 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/entry_points.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-06-20 10:29:13.000000 getlino-24.4.0/getlino.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-04-12 23:15:52.971992 getlino-24.4.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2020-07-10 08:02:46.000000 getlino-24.4.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      313 2024-02-14 17:37:21.000000 getlino-24.4.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.971992 getlino-24.4.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-03-02 11:04:28.000000 getlino-24.4.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2106 2024-02-14 17:37:21.000000 getlino-24.4.0/tests/test_case.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10812 2024-02-14 17:37:21.000000 getlino-24.4.0/tests/test_docker.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:37:21.000000 getlino-24.4.0/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2024-02-14 17:37:21.000000 getlino-24.4.0/tests/test_packages.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-19 07:15:05.898691 getlino-24.5.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:36.000000 getlino-24.5.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       59 2019-10-25 15:17:06.000000 getlino-24.5.0/MANIFEST.in
+-rw-r--r--   0 luc       (1000) www-data    (33)     1559 2024-05-19 07:15:05.898691 getlino-24.5.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      692 2021-06-11 08:29:48.000000 getlino-24.5.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-19 07:15:05.894691 getlino-24.5.0/getlino/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      322 2024-02-14 17:37:21.000000 getlino-24.5.0/getlino/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      816 2024-02-14 17:37:21.000000 getlino-24.5.0/getlino/cli.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20464 2024-04-16 07:54:19.000000 getlino-24.5.0/getlino/configure.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      971 2024-04-01 15:27:49.000000 getlino-24.5.0/getlino/list.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1788 2024-05-19 07:14:50.000000 getlino-24.5.0/getlino/setup_info.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7794 2024-03-11 13:29:19.000000 getlino-24.5.0/getlino/startproject.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    25761 2024-05-18 16:49:07.000000 getlino-24.5.0/getlino/startsite.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-19 07:15:05.898691 getlino-24.5.0/getlino/templates/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2021-02-12 13:40:30.000000 getlino-24.5.0/getlino/templates/apache.conf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      214 2022-09-10 15:27:38.000000 getlino-24.5.0/getlino/templates/asgi.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1678 2024-02-22 15:57:56.000000 getlino-24.5.0/getlino/templates/daphne_supervisor.conf
+-rw-rw-r--   0 luc       (1000) www-data    (33)      852 2023-01-01 07:07:06.000000 getlino-24.5.0/getlino/templates/django_settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      371 2023-07-01 18:31:56.000000 getlino-24.5.0/getlino/templates/healthcheck.sh
+-rw-rw-r--   0 luc       (1000) www-data    (33)      308 2023-01-15 18:29:24.000000 getlino-24.5.0/getlino/templates/lino.ini
+-rwxrwxr-x   0 luc       (1000) www-data    (33)     2074 2022-09-15 06:25:41.000000 getlino-24.5.0/getlino/templates/make_snapshot.sh
+-rw-rw-r--   0 luc       (1000) www-data    (33)      329 2023-11-05 18:22:29.000000 getlino-24.5.0/getlino/templates/manage.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1671 2023-07-16 11:11:44.000000 getlino-24.5.0/getlino/templates/nginx.conf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1543 2022-09-10 15:27:38.000000 getlino-24.5.0/getlino/templates/nginx_asgi.conf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1558 2023-10-08 06:14:57.000000 getlino-24.5.0/getlino/templates/pull.sh
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1472 2024-04-05 03:44:20.000000 getlino-24.5.0/getlino/templates/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2021-02-10 17:53:35.000000 getlino-24.5.0/getlino/templates/uwsgi.ini
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      664 2019-10-25 14:15:15.000000 getlino-24.5.0/getlino/templates/uwsgi_params
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      251 2019-10-25 14:30:31.000000 getlino-24.5.0/getlino/templates/wsgi.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20855 2024-04-16 05:53:33.000000 getlino-24.5.0/getlino/utils.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-19 07:15:05.898691 getlino-24.5.0/getlino.egg-info/
+-rw-r--r--   0 luc       (1000) www-data    (33)     1559 2024-05-19 07:15:05.000000 getlino-24.5.0/getlino.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      983 2024-05-19 07:15:05.000000 getlino-24.5.0/getlino.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-05-19 07:15:05.000000 getlino-24.5.0/getlino.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2024-05-19 07:15:05.000000 getlino-24.5.0/getlino.egg-info/entry_points.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-06-20 10:29:13.000000 getlino-24.5.0/getlino.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2024-05-19 07:15:05.000000 getlino-24.5.0/getlino.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2024-05-19 07:15:05.000000 getlino-24.5.0/getlino.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-05-19 07:15:05.898691 getlino-24.5.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2020-07-10 08:02:46.000000 getlino-24.5.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      313 2024-02-14 17:37:21.000000 getlino-24.5.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-19 07:15:05.898691 getlino-24.5.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-03-02 11:04:28.000000 getlino-24.5.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2106 2024-02-14 17:37:21.000000 getlino-24.5.0/tests/test_case.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10812 2024-02-14 17:37:21.000000 getlino-24.5.0/tests/test_docker.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:37:21.000000 getlino-24.5.0/tests/test_docs.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2024-02-14 17:37:21.000000 getlino-24.5.0/tests/test_packages.py
```

### Comparing `getlino-24.4.0/COPYING` & `getlino-24.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/PKG-INFO` & `getlino-24.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getlino
-Version: 24.4.0
+Version: 24.5.0
 Summary: A command-line tool for installing Lino in different environments.
 Home-page: https://gitlab.com/lino-framework/getlino
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `getlino-24.4.0/README.rst` & `getlino-24.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/cli.py` & `getlino-24.5.0/getlino/cli.py`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/configure.py` & `getlino-24.5.0/getlino/configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# Copyright 2019-2022 Rumma & Ko Ltd
+# Copyright 2019-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 import os
+from os.path import join
 import sys
 import stat
 import shutil
 import distro
 import configparser
 import subprocess
 import click
 import collections
 from pathlib import Path
 from contextlib import contextmanager
 
-from os.path import join
+from synodal import KNOWN_REPOS, FRONT_ENDS
 
 from .utils import CONFIG, CONF_FILES, DEFAULTSECTION
-from .utils import KNOWN_REPOS, DB_ENGINES, BATCH_HELP, FRONT_ENDS
+from .utils import DB_ENGINES, BATCH_HELP
 from .utils import Installer, ifroot, default_db_engine, resolve_db_engine
 from .utils import which_certbot
 from .utils import WEB_SERVERS, resolve_web_server, GITLAB_CI
 
 HEALTHCHECK_NAME = '/usr/local/bin/healthcheck.sh'
 
 CERTBOT_AUTO_RENEW = """\
```

### Comparing `getlino-24.4.0/getlino/list.py` & `getlino-24.5.0/getlino/list.py`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/setup_info.py` & `getlino-24.5.0/getlino/setup_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 SETUP_INFO = dict(
     name='getlino',
-    version='24.4.0',
+    version='24.5.0',
     install_requires=[
         'click', 'virtualenv', 'jinja2', 'distro', 'synodal',
         'GitPython', 'rstgen'
     ],
     # tests_require=['docker', 'atelier'],
     # test_suite='tests',
     description=
```

### Comparing `getlino-24.4.0/getlino/startproject.py` & `getlino-24.5.0/getlino/startproject.py`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/startsite.py` & `getlino-24.5.0/getlino/startsite.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from urllib.parse import urlparse
 
 logger = getLogger(__file__)
 
 from os.path import join
 
 from synodal import REPOS_DICT, KNOWN_REPOS, FRONT_ENDS
-from .utils import KNOWN_REPOS, DEFAULTSECTION
+from .utils import DEFAULTSECTION
 from .utils import DB_ENGINES, BATCH_HELP
 from .utils import Installer, ifroot, has_usergroup
 from .utils import default_db_engine, resolve_db_engine
 from .utils import which_certbot, resolve_web_server
 from .utils import JINJA_ENV
 from .utils import GITLAB_CI
 
@@ -632,16 +632,17 @@
             db_engine.setup_user(i, context)
         db_engine.setup_database(i, prjname, db_user, db_host)
 
     os.chdir(project_dir)
     i.run_in_env(envdir, "python manage.py install --noinput")
 
     if linod and not asgi_server and ifroot():
-        i.write_file(join(project_dir, 'linod.sh'), LINOD_SH.format(**context))
-        i.check_permissions(executable=True, writeable=False)
+        fn = join(project_dir, 'linod.sh')
+        i.write_file(fn, LINOD_SH.format(**context))
+        i.check_permissions(fn, executable=True, writeable=False)
         i.write_supervisor_conf('linod_{}.conf'.format(prjname),
                                 LINOD_SUPERVISOR_CONF.format(**context))
         i.must_restart('supervisor')
 
     if not reinstall:
         # i.run_in_env(envdir, "python manage.py migrate --noinput")  # Not necessary, prep does it from initdb.
         i.run_in_env(envdir, "python manage.py prep --noinput")
```

### Comparing `getlino-24.4.0/getlino/templates/apache.conf` & `getlino-24.5.0/getlino/templates/apache.conf`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/daphne_supervisor.conf` & `getlino-24.5.0/getlino/templates/daphne_supervisor.conf`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/django_settings.py` & `getlino-24.5.0/getlino/templates/django_settings.py`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/make_snapshot.sh` & `getlino-24.5.0/getlino/templates/make_snapshot.sh`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/nginx.conf` & `getlino-24.5.0/getlino/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/nginx_asgi.conf` & `getlino-24.5.0/getlino/templates/nginx_asgi.conf`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/pull.sh` & `getlino-24.5.0/getlino/templates/pull.sh`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/settings.py` & `getlino-24.5.0/getlino/templates/settings.py`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/uwsgi.ini` & `getlino-24.5.0/getlino/templates/uwsgi.ini`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/templates/uwsgi_params` & `getlino-24.5.0/getlino/templates/uwsgi_params`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino/utils.py` & `getlino-24.5.0/getlino/utils.py`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/getlino.egg-info/PKG-INFO` & `getlino-24.5.0/getlino.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getlino
-Version: 24.4.0
+Version: 24.5.0
 Summary: A command-line tool for installing Lino in different environments.
 Home-page: https://gitlab.com/lino-framework/getlino
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `getlino-24.4.0/getlino.egg-info/SOURCES.txt` & `getlino-24.5.0/getlino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/tests/test_case.py` & `getlino-24.5.0/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `getlino-24.4.0/tests/test_docker.py` & `getlino-24.5.0/tests/test_docker.py`

 * *Files identical despite different names*

