# Comparing `tmp/ecs_files_composer-2.1.3.tar.gz` & `tmp/ecs_files_composer-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_files_composer-2.1.3.tar", max compression
+gzip compressed data, was "ecs_files_composer-2.1.4.tar", max compression
```

## Comparing `ecs_files_composer-2.1.3.tar` & `ecs_files_composer-2.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       95 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.3/AUTHORS.rst
--rw-r--r--   0        0        0    16725 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.3/LICENSE
--rw-r--r--   0        0        0     3280 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.3/README.rst
--rw-r--r--   0        0        0      223 2024-05-06 07:04:37.394686 ecs_files_composer-2.1.3/ecs_files_composer/__init__.py
--rw-r--r--   0        0        0     7798 2024-05-06 06:14:50.630407 ecs_files_composer-2.1.3/ecs_files_composer/aws_mgmt.py
--rw-r--r--   0        0        0     4182 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.3/ecs_files_composer/certificates_mgmt.py
--rw-r--r--   0        0        0     4804 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.3/ecs_files_composer/cli.py
--rw-r--r--   0        0        0     1605 2023-08-20 14:53:24.555417 ecs_files_composer-2.1.3/ecs_files_composer/common.py
--rw-r--r--   0        0        0     5025 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.3/ecs_files_composer/ecs_files_composer.py
--rw-r--r--   0        0        0     1669 2022-07-27 07:35:08.374630 ecs_files_composer-2.1.3/ecs_files_composer/envsubst.py
--rw-r--r--   0        0        0    13688 2023-10-19 08:22:36.090481 ecs_files_composer-2.1.3/ecs_files_composer/files_mgmt.py
--rw-r--r--   0        0        0     3550 2023-10-19 08:22:36.090481 ecs_files_composer-2.1.3/ecs_files_composer/input.py
--rw-r--r--   0        0        0     3300 2024-02-02 10:43:08.348929 ecs_files_composer-2.1.3/ecs_files_composer/jinja2_filters/__init__.py
--rw-r--r--   0        0        0     1340 2024-02-02 11:02:22.316616 ecs_files_composer-2.1.3/ecs_files_composer/jinja2_functions/__init__.py
--rw-r--r--   0        0        0     6077 2024-02-02 11:02:22.316616 ecs_files_composer-2.1.3/ecs_files_composer/jinja2_functions/aws.py
--rw-r--r--   0        0        0     3062 2024-05-06 07:04:37.394686 ecs_files_composer-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 ecs_files_composer-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0       95 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.4/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.4/LICENSE
+-rw-r--r--   0        0        0     3280 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.4/README.rst
+-rw-r--r--   0        0        0      223 2024-05-19 05:55:05.657889 ecs_files_composer-2.1.4/ecs_files_composer/__init__.py
+-rw-r--r--   0        0        0     7798 2024-05-06 06:14:50.630407 ecs_files_composer-2.1.4/ecs_files_composer/aws_mgmt.py
+-rw-r--r--   0        0        0     4182 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.4/ecs_files_composer/certificates_mgmt.py
+-rw-r--r--   0        0        0     4804 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.4/ecs_files_composer/cli.py
+-rw-r--r--   0        0        0     1605 2023-08-20 14:53:24.555417 ecs_files_composer-2.1.4/ecs_files_composer/common.py
+-rw-r--r--   0        0        0     5025 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.4/ecs_files_composer/ecs_files_composer.py
+-rw-r--r--   0        0        0     1669 2022-07-27 07:35:08.374630 ecs_files_composer-2.1.4/ecs_files_composer/envsubst.py
+-rw-r--r--   0        0        0    13688 2023-10-19 08:22:36.090481 ecs_files_composer-2.1.4/ecs_files_composer/files_mgmt.py
+-rw-r--r--   0        0        0     3550 2023-10-19 08:22:36.090481 ecs_files_composer-2.1.4/ecs_files_composer/input.py
+-rw-r--r--   0        0        0     3300 2024-02-02 10:43:08.348929 ecs_files_composer-2.1.4/ecs_files_composer/jinja2_filters/__init__.py
+-rw-r--r--   0        0        0     1340 2024-02-02 11:02:22.316616 ecs_files_composer-2.1.4/ecs_files_composer/jinja2_functions/__init__.py
+-rw-r--r--   0        0        0     6077 2024-02-02 11:02:22.316616 ecs_files_composer-2.1.4/ecs_files_composer/jinja2_functions/aws.py
+-rw-r--r--   0        0        0     3062 2024-05-19 05:55:05.657889 ecs_files_composer-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 ecs_files_composer-2.1.4/PKG-INFO
```

### Comparing `ecs_files_composer-2.1.3/LICENSE` & `ecs_files_composer-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/README.rst` & `ecs_files_composer-2.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/aws_mgmt.py` & `ecs_files_composer-2.1.4/ecs_files_composer/aws_mgmt.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/certificates_mgmt.py` & `ecs_files_composer-2.1.4/ecs_files_composer/certificates_mgmt.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/cli.py` & `ecs_files_composer-2.1.4/ecs_files_composer/cli.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/common.py` & `ecs_files_composer-2.1.4/ecs_files_composer/common.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/ecs_files_composer.py` & `ecs_files_composer-2.1.4/ecs_files_composer/ecs_files_composer.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/envsubst.py` & `ecs_files_composer-2.1.4/ecs_files_composer/envsubst.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/files_mgmt.py` & `ecs_files_composer-2.1.4/ecs_files_composer/files_mgmt.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/input.py` & `ecs_files_composer-2.1.4/ecs_files_composer/input.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/jinja2_filters/__init__.py` & `ecs_files_composer-2.1.4/ecs_files_composer/jinja2_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/jinja2_functions/__init__.py` & `ecs_files_composer-2.1.4/ecs_files_composer/jinja2_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/ecs_files_composer/jinja2_functions/aws.py` & `ecs_files_composer-2.1.4/ecs_files_composer/jinja2_functions/aws.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.3/pyproject.toml` & `ecs_files_composer-2.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_files_composer"
-version = "2.1.3"
+version = "2.1.4"
 description = "Files and configuration handler to inject configuration files into volumes for ECS containers"
 authors = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
@@ -94,15 +94,15 @@
 
 omit = ["ecs_files_composer/cli.py"]
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecs-files-composer"
 
 [tool.tbump.version]
-current = "2.1.3"
+current = "2.1.4"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `ecs_files_composer-2.1.3/PKG-INFO` & `ecs_files_composer-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs_files_composer
-Version: 2.1.3
+Version: 2.1.4
 Summary: Files and configuration handler to inject configuration files into volumes for ECS containers
 License: MPL-2.0
 Keywords: aws,ecs,k8s,secrets
 Author: John Preston
 Author-email: john@compose-x.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

