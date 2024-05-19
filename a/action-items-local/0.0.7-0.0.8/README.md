# Comparing `tmp/action-items-local-0.0.7.tar.gz` & `tmp/action_items_local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-items-local-0.0.7.tar", last modified: Tue Apr  9 18:15:10 2024, max compression
+gzip compressed data, was "action_items_local-0.0.8.tar", last modified: Sun May 19 12:37:28 2024, max compression
```

## Comparing `action-items-local-0.0.7.tar` & `action_items_local-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:15:10.033611 action-items-local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 18:15:10.033611 action-items-local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 18:14:50.000000 action-items-local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:15:10.029611 action-items-local-0.0.7/action_items_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:15:10.033611 action-items-local-0.0.7/action_items_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:14:50.000000 action-items-local-0.0.7/action_items_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-09 18:14:50.000000 action-items-local-0.0.7/action_items_local/src/action_items_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 18:14:50.000000 action-items-local-0.0.7/action_items_local/src/action_items_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:15:10.033611 action-items-local-0.0.7/action_items_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 18:15:10.000000 action-items-local-0.0.7/action_items_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 18:15:10.000000 action-items-local-0.0.7/action_items_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:15:10.000000 action-items-local-0.0.7/action_items_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 18:15:10.000000 action-items-local-0.0.7/action_items_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 18:15:10.000000 action-items-local-0.0.7/action_items_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 18:14:50.000000 action-items-local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:15:10.033611 action-items-local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 18:14:50.000000 action-items-local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:37:28.259864 action_items_local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-19 12:37:28.255864 action_items_local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 12:37:02.000000 action_items_local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:37:28.255864 action_items_local-0.0.8/action_items_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:37:28.255864 action_items_local-0.0.8/action_items_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:37:02.000000 action_items_local-0.0.8/action_items_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-05-19 12:37:02.000000 action_items_local-0.0.8/action_items_local/src/action_items_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 12:37:02.000000 action_items_local-0.0.8/action_items_local/src/action_items_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:37:28.255864 action_items_local-0.0.8/action_items_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-19 12:37:28.000000 action_items_local-0.0.8/action_items_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-19 12:37:28.000000 action_items_local-0.0.8/action_items_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:37:28.000000 action_items_local-0.0.8/action_items_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-19 12:37:28.000000 action_items_local-0.0.8/action_items_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 12:37:28.000000 action_items_local-0.0.8/action_items_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-19 12:37:02.000000 action_items_local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:37:28.259864 action_items_local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-19 12:37:02.000000 action_items_local-0.0.8/setup.py
```

### Comparing `action-items-local-0.0.7/PKG-INFO` & `action_items_local-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-items-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles action-items-local Python
 Home-page: https://github.com/circles-zone/action-item-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `action-items-local-0.0.7/action_items_local/src/action_items_local.py` & `action_items_local-0.0.8/action_items_local/src/action_items_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         :return: int
         """
         logger.start(object={"priority": priority})
         where_clause = "ranking >= %s AND ranking < %s"
         params = ((priority * 10000), ((priority + 1) * 10000))
         order_by = "ranking DESC"
         action_items_dicts = self.select_multi_dict_by_where(
-            schema_name=self.schema_name,
+            schema_name=self.default_schema_name,
             view_table_name="action_item_view",
             where=where_clause, params=params, order_by=order_by
         )
         if not action_items_dicts:
             ranking = priority * 10000
         else:
             ranking = action_items_dicts[0]['ranking'] + 1
```

### Comparing `action-items-local-0.0.7/action_items_local/src/action_items_local_constants.py` & `action_items_local-0.0.8/action_items_local/src/action_items_local_constants.py`

 * *Files identical despite different names*

### Comparing `action-items-local-0.0.7/action_items_local.egg-info/PKG-INFO` & `action_items_local-0.0.8/action_items_local.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-items-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles action-items-local Python
 Home-page: https://github.com/circles-zone/action-item-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `action-items-local-0.0.7/setup.py` & `action_items_local-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "action-items-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.7',  # update only the minor version each time # https://pypi.org/project/action-items-local/
+    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/action-items-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles action-items-local Python",
     long_description="PyPI Package for Circles action-items-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/action-item-local-python-package",
     packages=[package_dir],
```

