# Comparing `tmp/tenant-schemas-celery-2.2.0.tar.gz` & `tmp/tenant_schemas_celery-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenant-schemas-celery-2.2.0.tar", last modified: Fri Apr 28 11:40:09 2023, max compression
+gzip compressed data, was "tenant_schemas_celery-3.0.0.tar", last modified: Sun May 19 11:14:55 2024, max compression
```

## Comparing `tenant-schemas-celery-2.2.0.tar` & `tenant_schemas_celery-3.0.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-04-28 11:40:09.002534 tenant-schemas-celery-2.2.0/
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1076 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/LICENSE
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       34 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/MANIFEST.in
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     7184 2023-04-28 11:40:09.002534 tenant-schemas-celery-2.2.0/PKG-INFO
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     6705 2023-04-28 11:38:19.000000 tenant-schemas-celery-2.2.0/README.md
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        6 2023-04-28 11:38:26.000000 tenant-schemas-celery-2.2.0/VERSION
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       38 2023-04-28 11:40:09.002534 tenant-schemas-celery-2.2.0/setup.cfg
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1001 2022-02-04 09:43:17.000000 tenant-schemas-celery-2.2.0/setup.py
-drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-04-28 11:40:08.998534 tenant-schemas-celery-2.2.0/tenant_schemas_celery/
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        0 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/__init__.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     3246 2023-03-30 18:49:09.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/app.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      746 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/cache.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1402 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/cache_test.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      226 2023-03-30 18:49:09.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/compat.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      439 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/conftest.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5799 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/integration_test.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      562 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/registry.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1234 2021-01-04 22:35:23.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/registry_test.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     3585 2023-04-28 11:38:19.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/scheduler.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     2462 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/task.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5624 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/task_test.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      642 2023-03-30 19:19:58.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_app.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5524 2023-04-28 11:38:19.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_scheduler.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1442 2023-03-30 19:16:55.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_tasks.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      460 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_utils.py
-drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-04-28 11:40:09.002534 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     7184 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/PKG-INFO
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      827 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/SOURCES.txt
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        1 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/dependency_links.txt
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        7 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/requires.txt
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       22 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/top_level.txt
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2024-05-19 11:14:55.222846 tenant_schemas_celery-3.0.0/
+-rw-r--r--   0 mg        (1000) mg        (1000)     1076 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)       34 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/MANIFEST.in
+-rw-r--r--   0 mg        (1000) mg        (1000)     7259 2024-05-19 11:14:55.222846 tenant_schemas_celery-3.0.0/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)     6758 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/README.md
+-rw-r--r--   0 mg        (1000) mg        (1000)        6 2024-05-19 11:14:32.000000 tenant_schemas_celery-3.0.0/VERSION
+-rw-r--r--   0 mg        (1000) mg        (1000)       38 2024-05-19 11:14:55.222846 tenant_schemas_celery-3.0.0/setup.cfg
+-rw-r--r--   0 mg        (1000) mg        (1000)     1001 2024-05-19 11:13:54.000000 tenant_schemas_celery-3.0.0/setup.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2024-05-19 11:14:55.212846 tenant_schemas_celery-3.0.0/tenant_schemas_celery/
+-rw-r--r--   0 mg        (1000) mg        (1000)        0 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/__init__.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     3423 2024-05-19 11:13:37.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/app.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      716 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/app_test.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      746 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/cache.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1402 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/cache_test.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      226 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/compat.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      439 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/conftest.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     5799 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/integration_test.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      562 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/registry.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1234 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/registry_test.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     3585 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/scheduler.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     2462 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/task.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     5624 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/task_test.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      642 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/test_app.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     5524 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/test_scheduler.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1442 2024-05-19 10:58:40.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/test_tasks.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      460 2024-05-19 10:14:04.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery/test_utils.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2024-05-19 11:14:55.222846 tenant_schemas_celery-3.0.0/tenant_schemas_celery.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     7259 2024-05-19 11:14:55.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      861 2024-05-19 11:14:55.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2024-05-19 11:14:55.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        7 2024-05-19 11:14:55.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery.egg-info/requires.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       22 2024-05-19 11:14:55.000000 tenant_schemas_celery-3.0.0/tenant_schemas_celery.egg-info/top_level.txt
```

### Comparing `tenant-schemas-celery-2.2.0/LICENSE` & `tenant_schemas_celery-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/PKG-INFO` & `tenant_schemas_celery-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: tenant-schemas-celery
-Version: 2.2.0
+Version: 3.0.0
 Summary: Celery integration for django-tenant-schemas and django-tenants
 Home-page: https://github.com/maciej-gol/tenant-schemas-celery
 Author: Maciej Gol
 Author-email: 1kroolik1@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: celery
 
 tenant-schemas-celery 
 =====================
 
 Celery application implementation that allows celery tasks to cooperate with
 multi-tenancy provided by [django-tenant-schemas](https://github.com/bernardopires/django-tenant-schemas) and
 [django-tenants](https://github.com/tomturner/django-tenants) packages.
@@ -52,14 +53,15 @@
 
    * Replace your `@task` decorator with `@app.task`
 
 ```python
    from celery import shared_task
    from django.db import connection
    from myproject.celery import app
+   from tenant_schemas_celery.task import TenantTask
 
    @app.task
    def my_task():
       print(connection.schema_name)
 
    @shared_task(base=TenantTask, bind=True)
    def my_shared_task():
```

### Comparing `tenant-schemas-celery-2.2.0/README.md` & `tenant_schemas_celery-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
    * Replace your `@task` decorator with `@app.task`
 
 ```python
    from celery import shared_task
    from django.db import connection
    from myproject.celery import app
+   from tenant_schemas_celery.task import TenantTask
 
    @app.task
    def my_task():
       print(connection.schema_name)
 
    @shared_task(base=TenantTask, bind=True)
    def my_shared_task():
```

### Comparing `tenant-schemas-celery-2.2.0/setup.py` & `tenant_schemas_celery-3.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         'Programming Language :: Python',
     ],
     description='Celery integration for django-tenant-schemas and django-tenants',
     install_requires=[
         'celery',
     ],
     packages=find_packages(),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     name='tenant-schemas-celery',
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/maciej-gol/tenant-schemas-celery',
     version=version,
 )
```

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/app.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,18 +72,23 @@
 task_postrun.connect(
     restore_schema, sender=None, dispatch_uid="tenant_schemas_restore_schema"
 )
 
 
 class CeleryApp(Celery):
     registry_cls = 'tenant_schemas_celery.registry:TenantTaskRegistry'
-    
+    task_cls = 'tenant_schemas_celery.task:TenantTask'
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("task_cls", self.task_cls)
+        super(CeleryApp, self).__init__(*args, **kwargs)
+
     def create_task_cls(self):
         return self.subclass_with_self(
-            "tenant_schemas_celery.task:TenantTask",
+            self.task_cls,
             abstract=True,
             name="TenantTask",
             attribute="_app",
         )
 
     def _update_headers(self, kw):
         kw["headers"] = kw.get("headers") or {}
```

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/cache.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/cache.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/cache_test.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/cache_test.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/integration_test.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/integration_test.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/registry.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/registry.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/registry_test.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/registry_test.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/scheduler.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/scheduler.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/task.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/task.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/task_test.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/task_test.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_app.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/test_app.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_scheduler.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_tasks.py` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery/test_tasks.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/PKG-INFO` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: tenant-schemas-celery
-Version: 2.2.0
+Version: 3.0.0
 Summary: Celery integration for django-tenant-schemas and django-tenants
 Home-page: https://github.com/maciej-gol/tenant-schemas-celery
 Author: Maciej Gol
 Author-email: 1kroolik1@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: celery
 
 tenant-schemas-celery 
 =====================
 
 Celery application implementation that allows celery tasks to cooperate with
 multi-tenancy provided by [django-tenant-schemas](https://github.com/bernardopires/django-tenant-schemas) and
 [django-tenants](https://github.com/tomturner/django-tenants) packages.
@@ -52,14 +53,15 @@
 
    * Replace your `@task` decorator with `@app.task`
 
 ```python
    from celery import shared_task
    from django.db import connection
    from myproject.celery import app
+   from tenant_schemas_celery.task import TenantTask
 
    @app.task
    def my_task():
       print(connection.schema_name)
 
    @shared_task(base=TenantTask, bind=True)
    def my_shared_task():
```

### Comparing `tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/SOURCES.txt` & `tenant_schemas_celery-3.0.0/tenant_schemas_celery.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 setup.py
 tenant_schemas_celery/__init__.py
 tenant_schemas_celery/app.py
+tenant_schemas_celery/app_test.py
 tenant_schemas_celery/cache.py
 tenant_schemas_celery/cache_test.py
 tenant_schemas_celery/compat.py
 tenant_schemas_celery/conftest.py
 tenant_schemas_celery/integration_test.py
 tenant_schemas_celery/registry.py
 tenant_schemas_celery/registry_test.py
```

