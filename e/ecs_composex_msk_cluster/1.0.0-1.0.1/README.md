# Comparing `tmp/ecs_composex_msk_cluster-1.0.0.tar.gz` & `tmp/ecs_composex_msk_cluster-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_composex_msk_cluster-1.0.0.tar", max compression
+gzip compressed data, was "ecs_composex_msk_cluster-1.0.1.tar", max compression
```

## Comparing `ecs_composex_msk_cluster-1.0.0.tar` & `ecs_composex_msk_cluster-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       95 2022-04-24 10:25:44.093880 ecs_composex_msk_cluster-1.0.0/AUTHORS.rst
--rw-r--r--   0        0        0    16725 2022-04-24 10:25:44.149879 ecs_composex_msk_cluster-1.0.0/LICENSE
--rw-r--r--   0        0        0      392 2022-04-24 10:25:44.055880 ecs_composex_msk_cluster-1.0.0/MANIFEST.in
--rw-r--r--   0        0        0     1165 2023-03-16 20:50:05.293054 ecs_composex_msk_cluster-1.0.0/README.rst
--rw-r--r--   0        0        0      170 2024-04-21 13:17:44.467253 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/__init__.py
--rw-r--r--   0        0        0     6556 2023-01-12 10:42:26.973223 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster.py
--rw-r--r--   0        0        0     1064 2022-11-21 21:44:03.087655 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_conditions.py
--rw-r--r--   0        0        0     1114 2022-11-21 21:44:03.103654 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_ecs.py
--rw-r--r--   0        0        0     7943 2022-11-21 21:44:03.104655 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py
--rw-r--r--   0        0        0     2816 2023-03-11 22:46:19.588524 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_logging.py
--rw-r--r--   0        0        0      501 2022-11-21 21:44:03.144654 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_module.py
--rw-r--r--   0        0        0     2843 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_params.py
--rw-r--r--   0        0        0      212 2024-04-21 13:17:44.723248 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_perms.json
--rw-r--r--   0        0        0     1731 2022-11-21 21:44:03.163654 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_stack.py
--rw-r--r--   0        0        0     9535 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_template.py
--rw-r--r--   0        0        0     1401 2022-11-21 21:44:03.186653 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_configuration.py
--rw-r--r--   0        0        0     8504 2023-03-11 22:44:53.532492 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_sg_ingress.py
--rw-r--r--   0        0        0     3144 2022-11-21 21:44:03.188653 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_storage_scaling.py
--rw-r--r--   0        0        0     8392 2024-04-21 13:17:44.723248 ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/x-msk_cluster.spec.json
--rw-r--r--   0        0        0     2319 2024-04-21 13:17:44.467253 ecs_composex_msk_cluster-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2352 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       95 2022-04-24 10:25:44.093880 ecs_composex_msk_cluster-1.0.1/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2022-04-24 10:25:44.149879 ecs_composex_msk_cluster-1.0.1/LICENSE
+-rw-r--r--   0        0        0      392 2022-04-24 10:25:44.055880 ecs_composex_msk_cluster-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     1165 2023-03-16 20:50:05.293054 ecs_composex_msk_cluster-1.0.1/README.rst
+-rw-r--r--   0        0        0      170 2024-05-19 05:46:32.865621 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/__init__.py
+-rw-r--r--   0        0        0     6556 2023-01-12 10:42:26.973223 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster.py
+-rw-r--r--   0        0        0     1064 2022-11-21 21:44:03.087655 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_conditions.py
+-rw-r--r--   0        0        0     1114 2022-11-21 21:44:03.103654 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_ecs.py
+-rw-r--r--   0        0        0     7991 2024-05-19 05:46:33.140617 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py
+-rw-r--r--   0        0        0     2816 2023-03-11 22:46:19.588524 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_logging.py
+-rw-r--r--   0        0        0      501 2022-11-21 21:44:03.144654 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_module.py
+-rw-r--r--   0        0        0     2843 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_params.py
+-rw-r--r--   0        0        0      212 2024-05-19 05:46:33.160617 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_perms.json
+-rw-r--r--   0        0        0     1731 2022-11-21 21:44:03.163654 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_stack.py
+-rw-r--r--   0        0        0     9535 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_template.py
+-rw-r--r--   0        0        0     1401 2022-11-21 21:44:03.186653 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_configuration.py
+-rw-r--r--   0        0        0     8504 2023-03-11 22:44:53.532492 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_sg_ingress.py
+-rw-r--r--   0        0        0     3144 2022-11-21 21:44:03.188653 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_storage_scaling.py
+-rw-r--r--   0        0        0     8392 2024-05-19 05:46:33.160617 ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/x-msk_cluster.spec.json
+-rw-r--r--   0        0        0     2318 2024-05-19 05:46:32.865621 ecs_composex_msk_cluster-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2352 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-1.0.1/PKG-INFO
```

### Comparing `ecs_composex_msk_cluster-1.0.0/LICENSE` & `ecs_composex_msk_cluster-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/README.rst` & `ecs_composex_msk_cluster-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_conditions.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_ecs.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,17 +198,19 @@
         cluster_arn_prefix = Select(0, Split(":cluster/", cluster_arn_id))
 
     statement: list = [
         {
             "Sid": "ConnectToCluster",
             "Effect": "Allow",
             "Resource": [
-                Ref(cluster_arn_id["ImportParameter"])
-                if resource.cfn_resource
-                else cluster_arn_id
+                (
+                    Ref(cluster_arn_id["ImportParameter"])
+                    if resource.cfn_resource
+                    else cluster_arn_id
+                )
             ],
             "Action": ["kafka-cluster:Connect"],
         }
     ]
     handle_cluster_permissions(
         resource,
         settings,
```

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_logging.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_logging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_params.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_stack.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_cluster_template.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_cluster_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_configuration.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_configuration.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_sg_ingress.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_sg_ingress.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/msk_storage_scaling.py` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/msk_storage_scaling.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/ecs_composex_msk_cluster/x-msk_cluster.spec.json` & `ecs_composex_msk_cluster-1.0.1/ecs_composex_msk_cluster/x-msk_cluster.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-1.0.0/pyproject.toml` & `ecs_composex_msk_cluster-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_composex_msk_cluster"
-version = "1.0.0"
+version = "1.0.1"
 description = "msk_cluster - AWS MSK Cluster module for ECS Compose-X"
 authors = ["johnpreston <john@compose-x.io>"]
 license = "MPL-2.0"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -27,19 +27,19 @@
   "ecs_composex/**/*.json"
 ]
 exclude = ["*.pyc", "*~", "*pycache*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ecs_composex = "^1.1"
-compose-x-common = "^1.2"
+compose-x-common = "^1.1"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3"
-isort = "^5.9.3"
+black = "^24.1"
+isort = "^5.12"
 coverage = "^7.0"
 pytest = "^7.2"
 behave = "^1.2.6"
 pre-commit = "^2.14.0"
 tbump = "^6.9"
 pyupgrade = "^3.2"
 twine = "^4.0"
@@ -76,15 +76,15 @@
   "*/cli.py"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecs_composex_msk_cluster"
 
 [tool.tbump.version]
-current = "1.0.0"
+current = "1.0.1"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `ecs_composex_msk_cluster-1.0.0/PKG-INFO` & `ecs_composex_msk_cluster-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs_composex_msk_cluster
-Version: 1.0.0
+Version: 1.0.1
 Summary: msk_cluster - AWS MSK Cluster module for ECS Compose-X
 License: MPL-2.0
 Author: johnpreston
 Author-email: john@compose-x.io
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: compose-x-common (>=1.2,<2.0)
+Requires-Dist: compose-x-common (>=1.1,<2.0)
 Requires-Dist: ecs_composex (>=1.1,<2.0)
 Project-URL: Compose-X Labs, https://labs.compose-x.io/
 Project-URL: Compose-X Blog, https://blog.compose-x.io/
 Project-URL: ECS ComposeX, https://github.com/compose-x/ecs_composex/
 Description-Content-Type: text/x-rst
```

