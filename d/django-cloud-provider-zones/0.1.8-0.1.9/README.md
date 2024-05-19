# Comparing `tmp/django_cloud_provider_zones-0.1.8.tar.gz` & `tmp/django_cloud_provider_zones-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cloud_provider_zones-0.1.8.tar", max compression
+gzip compressed data, was "django_cloud_provider_zones-0.1.9.tar", max compression
```

## Comparing `django_cloud_provider_zones-0.1.8.tar` & `django_cloud_provider_zones-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     5964 2024-04-03 16:58:07.335613 django_cloud_provider_zones-0.1.8/README.md
--rw-r--r--   0        0        0      904 2024-04-03 17:31:22.062921 django_cloud_provider_zones-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1087 2024-03-27 01:00:55.837913 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/LICENSE
--rw-r--r--   0        0        0        0 2024-03-28 22:45:59.846660 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/__init__.py
--rw-r--r--   0        0        0      924 2024-03-28 22:45:59.847084 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/admin.py
--rw-r--r--   0        0        0      172 2024-03-28 22:45:59.846181 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/apps.py
--rw-r--r--   0        0        0     1343 2024-03-28 22:45:59.847084 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/cloud_short_names.py
--rw-r--r--   0        0        0    71050 2024-03-29 00:00:51.289304 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudAvailabilityZone.json
--rw-r--r--   0        0        0      294 2024-03-29 00:00:51.220544 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudProvider.json
--rw-r--r--   0        0        0    24609 2024-03-29 00:00:51.223421 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudRegion.json
--rw-r--r--   0        0        0     3826 2024-03-29 00:00:49.263242 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-28 22:45:59.846871 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/migrations/__init__.py
--rw-r--r--   0        0        0     3501 2024-04-03 17:00:23.978898 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/models.py
--rw-r--r--   0        0        0     2612 2024-03-28 22:45:59.847459 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/serializers.py
--rw-r--r--   0        0        0     5120 2024-04-03 17:31:48.737627 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/tests.py
--rw-r--r--   0        0        0      519 2024-03-28 22:45:59.846195 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/urls.py
--rw-r--r--   0        0        0      898 2024-03-28 22:45:59.846252 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/views.py
--rw-r--r--   0        0        0     6805 1970-01-01 00:00:00.000000 django_cloud_provider_zones-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5964 2024-04-03 16:58:07.335613 django_cloud_provider_zones-0.1.9/README.md
+-rw-r--r--   0        0        0      904 2024-05-19 02:33:09.651601 django_cloud_provider_zones-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1087 2024-03-27 01:00:55.837913 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:59.846660 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/__init__.py
+-rw-r--r--   0        0        0      924 2024-03-28 22:45:59.847084 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/admin.py
+-rw-r--r--   0        0        0      172 2024-03-28 22:45:59.846181 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/apps.py
+-rw-r--r--   0        0        0     1343 2024-03-28 22:45:59.847084 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/cloud_short_names.py
+-rw-r--r--   0        0        0    71050 2024-03-29 00:00:51.289304 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudAvailabilityZone.json
+-rw-r--r--   0        0        0      294 2024-03-29 00:00:51.220544 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudProvider.json
+-rw-r--r--   0        0        0    24609 2024-03-29 00:00:51.223421 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudRegion.json
+-rw-r--r--   0        0        0     3826 2024-03-29 00:00:49.263242 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:59.846871 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/migrations/__init__.py
+-rw-r--r--   0        0        0     3501 2024-04-03 17:00:23.978898 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/models.py
+-rw-r--r--   0        0        0     2612 2024-03-28 22:45:59.847459 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/serializers.py
+-rw-r--r--   0        0        0     5120 2024-04-03 17:31:48.737627 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/tests.py
+-rw-r--r--   0        0        0      519 2024-03-28 22:45:59.846195 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/urls.py
+-rw-r--r--   0        0        0      898 2024-03-28 22:45:59.846252 django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/views.py
+-rw-r--r--   0        0        0     6805 1970-01-01 00:00:00.000000 django_cloud_provider_zones-0.1.9/PKG-INFO
```

### Comparing `django_cloud_provider_zones-0.1.8/README.md` & `django_cloud_provider_zones-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/pyproject.toml` & `django_cloud_provider_zones-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cloud-provider-zones"
-version = "0.1.8"
+version = "0.1.9"
 description = "Django app providing a static list of cloud provider regions and AZs"
 authors = ["TJ <yolabingo@gmail.com>"]
 readme = "README.md"
 license = "src/django_cloud_provider_zones/LICENSE"
 packages = [{include = "django_cloud_provider_zones", from = "src"}]
 repository = "https://github.com/yolabingo/django-cloud-provider-zones"
 keywords = ["django", "cloud", "provider", "regions", "aws", "gcp"]
```

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/LICENSE` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/admin.py` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/admin.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/cloud_short_names.py` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/cloud_short_names.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudAvailabilityZone.json` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudAvailabilityZone.json`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudRegion.json` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudRegion.json`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/migrations/0001_initial.py` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/models.py` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/models.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/serializers.py` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/serializers.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/tests.py` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/tests.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/urls.py` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/urls.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/views.py` & `django_cloud_provider_zones-0.1.9/src/django_cloud_provider_zones/views.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.8/PKG-INFO` & `django_cloud_provider_zones-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloud-provider-zones
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django app providing a static list of cloud provider regions and AZs
 Home-page: https://github.com/yolabingo/django-cloud-provider-zones
 License: src/django_cloud_provider_zones/LICENSE
 Keywords: django,cloud,provider,regions,aws,gcp
 Author: TJ
 Author-email: yolabingo@gmail.com
 Requires-Python: >=3.10
```

