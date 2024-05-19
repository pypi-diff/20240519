# Comparing `tmp/entity-type-local-0.0.8.tar.gz` & `tmp/entity-type-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity-type-local-0.0.8.tar", last modified: Mon Aug 14 10:53:27 2023, max compression
+gzip compressed data, was "entity-type-local-0.0.9.tar", last modified: Wed Aug 16 07:10:48 2023, max compression
```

## Comparing `entity-type-local-0.0.8.tar` & `entity-type-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 10:53:27.632630 entity-type-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-14 10:53:27.632630 entity-type-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-14 10:53:10.000000 entity-type-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 10:53:27.632630 entity-type-local-0.0.8/entity_type/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-14 10:53:10.000000 entity-type-local-0.0.8/entity_type/EntityType.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 10:53:10.000000 entity-type-local-0.0.8/entity_type/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 10:53:27.632630 entity-type-local-0.0.8/entity_type_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-14 10:53:27.000000 entity-type-local-0.0.8/entity_type_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-14 10:53:27.000000 entity-type-local-0.0.8/entity_type_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 10:53:27.000000 entity-type-local-0.0.8/entity_type_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-14 10:53:27.000000 entity-type-local-0.0.8/entity_type_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-14 10:53:10.000000 entity-type-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-14 10:53:27.632630 entity-type-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-14 10:53:10.000000 entity-type-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 10:53:27.632630 entity-type-local-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-14 10:53:10.000000 entity-type-local-0.0.8/tests/test_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 07:10:48.971823 entity-type-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-16 07:10:48.971823 entity-type-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-16 07:10:31.000000 entity-type-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 07:10:48.971823 entity-type-local-0.0.9/entity_type/
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-16 07:10:31.000000 entity-type-local-0.0.9/entity_type/EntityType.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-16 07:10:31.000000 entity-type-local-0.0.9/entity_type/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 07:10:48.971823 entity-type-local-0.0.9/entity_type_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-16 07:10:48.000000 entity-type-local-0.0.9/entity_type_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-16 07:10:48.000000 entity-type-local-0.0.9/entity_type_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-16 07:10:48.000000 entity-type-local-0.0.9/entity_type_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-16 07:10:48.000000 entity-type-local-0.0.9/entity_type_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-16 07:10:31.000000 entity-type-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-16 07:10:48.971823 entity-type-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-16 07:10:31.000000 entity-type-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 07:10:48.971823 entity-type-local-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-16 07:10:31.000000 entity-type-local-0.0.9/tests/test_entity.py
```

### Comparing `entity-type-local-0.0.8/entity_type/EntityType.py` & `entity-type-local-0.0.9/entity_type/EntityType.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from dotenv import load_dotenv
 from logger_local.LoggerLocal import logger_local
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from circles_local_database_python.connection import DatabaseFunctions
 load_dotenv()
 
 ENTITY_TYPE_COMPONENT_ID = 116
-COMPONENT_NAME = 'entity-type-local-python-package'
+ENTITY_TYPE_COMPONENT_NAME = 'entity-type-local-python-package'
 
 logger_code_init  = {
     'component_id': ENTITY_TYPE_COMPONENT_ID,
-    'component_name': COMPONENT_NAME,
+    'component_name': ENTITY_TYPE_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
-    'testing_framework': LoggerComponentEnum.testingFramework.pytest.value,
     'developer_email': 'idan.a@circ.zone'
 }
 logger_local.init(object=logger_code_init)
 database_conn = DatabaseFunctions("entityType")
 connection = database_conn.connect()
 
 class EntityType:
```

### Comparing `entity-type-local-0.0.8/setup.py` & `entity-type-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      name='entity-type-local',
-     version='0.0.8',
+     version='0.0.9',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local Entity Type Python (Currently empty package)",
      long_description="This is a package for sharing common importer function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

### Comparing `entity-type-local-0.0.8/tests/test_entity.py` & `entity-type-local-0.0.9/tests/test_entity.py`

 * *Files identical despite different names*

