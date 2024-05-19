# Comparing `tmp/djangorestframework_hybridrouter-0.1.3.tar.gz` & `tmp/djangorestframework_hybridrouter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework_hybridrouter-0.1.3.tar", last modified: Thu May 16 13:34:06 2024, max compression
+gzip compressed data, was "djangorestframework_hybridrouter-0.1.4.tar", last modified: Sat May 18 19:25:12 2024, max compression
```

## Comparing `djangorestframework_hybridrouter-0.1.3.tar` & `djangorestframework_hybridrouter-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:34:06.551944 djangorestframework_hybridrouter-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 13:34:02.000000 djangorestframework_hybridrouter-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-16 13:34:06.551944 djangorestframework_hybridrouter-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-16 13:34:02.000000 djangorestframework_hybridrouter-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:34:06.551944 djangorestframework_hybridrouter-0.1.3/djangorestframework_hybridrouter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-16 13:34:06.000000 djangorestframework_hybridrouter-0.1.3/djangorestframework_hybridrouter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-16 13:34:06.000000 djangorestframework_hybridrouter-0.1.3/djangorestframework_hybridrouter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:34:06.000000 djangorestframework_hybridrouter-0.1.3/djangorestframework_hybridrouter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 13:34:06.000000 djangorestframework_hybridrouter-0.1.3/djangorestframework_hybridrouter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 13:34:06.000000 djangorestframework_hybridrouter-0.1.3/djangorestframework_hybridrouter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:34:06.551944 djangorestframework_hybridrouter-0.1.3/hybridrouter/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:34:02.000000 djangorestframework_hybridrouter-0.1.3/hybridrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-16 13:34:02.000000 djangorestframework_hybridrouter-0.1.3/hybridrouter/hybridrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:34:06.551944 djangorestframework_hybridrouter-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 13:34:02.000000 djangorestframework_hybridrouter-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:25:12.030407 djangorestframework_hybridrouter-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 19:25:08.000000 djangorestframework_hybridrouter-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-18 19:25:12.030407 djangorestframework_hybridrouter-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-18 19:25:08.000000 djangorestframework_hybridrouter-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:25:12.030407 djangorestframework_hybridrouter-0.1.4/djangorestframework_hybridrouter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-18 19:25:12.000000 djangorestframework_hybridrouter-0.1.4/djangorestframework_hybridrouter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-18 19:25:12.000000 djangorestframework_hybridrouter-0.1.4/djangorestframework_hybridrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:25:12.000000 djangorestframework_hybridrouter-0.1.4/djangorestframework_hybridrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-18 19:25:12.000000 djangorestframework_hybridrouter-0.1.4/djangorestframework_hybridrouter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 19:25:12.000000 djangorestframework_hybridrouter-0.1.4/djangorestframework_hybridrouter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:25:12.030407 djangorestframework_hybridrouter-0.1.4/hybridrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-18 19:25:08.000000 djangorestframework_hybridrouter-0.1.4/hybridrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-18 19:25:08.000000 djangorestframework_hybridrouter-0.1.4/hybridrouter/hybridrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 19:25:12.030407 djangorestframework_hybridrouter-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-18 19:25:08.000000 djangorestframework_hybridrouter-0.1.4/setup.py
```

### Comparing `djangorestframework_hybridrouter-0.1.3/LICENSE` & `djangorestframework_hybridrouter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework_hybridrouter-0.1.3/PKG-INFO` & `djangorestframework_hybridrouter-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-hybridrouter
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to regsiter viewsets and views in the same router
 Home-page: https://github.com/enzofrnt/djangorestframework-hybridrouter
 Author: Made by enzo_frnt from a 
 Keywords: Django,Django REST Framework,viewsets,views,router,view,viewset
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django
```

### Comparing `djangorestframework_hybridrouter-0.1.3/README.md` & `djangorestframework_hybridrouter-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `djangorestframework_hybridrouter-0.1.3/djangorestframework_hybridrouter.egg-info/PKG-INFO` & `djangorestframework_hybridrouter-0.1.4/djangorestframework_hybridrouter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-hybridrouter
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to regsiter viewsets and views in the same router
 Home-page: https://github.com/enzofrnt/djangorestframework-hybridrouter
 Author: Made by enzo_frnt from a 
 Keywords: Django,Django REST Framework,viewsets,views,router,view,viewset
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django
```

### Comparing `djangorestframework_hybridrouter-0.1.3/hybridrouter/hybridrouter.py` & `djangorestframework_hybridrouter-0.1.4/hybridrouter/hybridrouter.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 from urllib.parse import urlsplit, urlunsplit
 
 try:
     from drf_spectacular.utils import extend_schema
     DRF_SPECTACULAR = True
 except ImportError:
     DRF_SPECTACULAR = False
-
+    
 def conditionally_extend_schema(exclude=True):
     def decorator(view_func):
         if DRF_SPECTACULAR:
             return extend_schema(exclude=exclude)(view_func)
-        return view_func
     return decorator
 
 class HybridRouter(DefaultRouter):    
     def __init__(self, enable_intermediate_apiviews=False , *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._api_view_urls = {}
         self.enable_intermediate_apiviews = enable_intermediate_apiviews
@@ -30,18 +29,14 @@
         
     def register_viewset(self, prefix, viewset, basename=None):
         super().register(prefix, viewset, basename)
     
     def register(self, prefix, viewset, basename=None):
         raise NotImplementedError("The 'register' method is deprecated. Use 'register_viewset' instead.")
 
-    def remove_api_view(self, name):
-        if name in self._api_view_urls:
-            del self._api_view_urls[name]
-
     @property
     def api_view_urls(self):
         return self._api_view_urls.copy()
 
     def get_urls(self):
         urls = super().get_urls()
         urls.extend(self._api_view_urls.values())
```

### Comparing `djangorestframework_hybridrouter-0.1.3/setup.py` & `djangorestframework_hybridrouter-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='djangorestframework-hybridrouter',
-    version='0.1.3',
+    version='0.1.4',
     packages=[
         'hybridrouter',
     ],
     install_requires=[
         'Django',
         'djangorestframework',
     ],
```

