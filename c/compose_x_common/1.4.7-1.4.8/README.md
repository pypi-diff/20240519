# Comparing `tmp/compose_x_common-1.4.7.tar.gz` & `tmp/compose_x_common-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose_x_common-1.4.7.tar", max compression
+gzip compressed data, was "compose_x_common-1.4.8.tar", max compression
```

## Comparing `compose_x_common-1.4.7.tar` & `compose_x_common-1.4.8.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0    16725 2022-03-11 22:14:27.945418 compose_x_common-1.4.7/LICENSE
--rw-r--r--   0        0        0      262 2022-03-11 22:14:27.945418 compose_x_common-1.4.7/MANIFEST.in
--rw-r--r--   0        0        0      739 2023-03-19 15:02:14.794099 compose_x_common-1.4.7/README.rst
--rw-r--r--   0        0        0     2225 2024-03-31 16:21:47.137329 compose_x_common-1.4.7/pyproject.toml
--rw-r--r--   0        0        0      228 2024-03-31 16:21:47.137329 compose_x_common-1.4.7/src/compose_x_common/__init__.py
--rw-r--r--   0        0        0     3574 2024-01-04 16:09:40.404251 compose_x_common-1.4.7/src/compose_x_common/aws/__init__.py
--rw-r--r--   0        0        0     1863 2024-01-04 16:09:40.390251 compose_x_common-1.4.7/src/compose_x_common/aws/acm.py
--rw-r--r--   0        0        0     1557 2024-01-04 16:09:40.421251 compose_x_common-1.4.7/src/compose_x_common/aws/application_autoscaling.py
--rw-r--r--   0        0        0      305 2024-01-04 16:09:40.424251 compose_x_common-1.4.7/src/compose_x_common/aws/aps.py
--rw-r--r--   0        0        0     5105 2024-01-04 16:28:37.364007 compose_x_common-1.4.7/src/compose_x_common/aws/arns.py
--rw-r--r--   0        0        0     1072 2024-01-04 16:09:40.418251 compose_x_common-1.4.7/src/compose_x_common/aws/cloudmap.py
--rw-r--r--   0        0        0      263 2024-01-04 16:09:40.416251 compose_x_common-1.4.7/src/compose_x_common/aws/codeguru_profiler.py
--rw-r--r--   0        0        0     2003 2024-01-04 16:09:40.407251 compose_x_common-1.4.7/src/compose_x_common/aws/cognito_userpool.py
--rw-r--r--   0        0        0      238 2024-01-04 16:09:40.402251 compose_x_common-1.4.7/src/compose_x_common/aws/dynamodb.py
--rw-r--r--   0        0        0     1106 2024-01-04 16:09:40.386252 compose_x_common-1.4.7/src/compose_x_common/aws/ec2.py
--rw-r--r--   0        0        0      471 2024-01-04 16:09:40.409251 compose_x_common-1.4.7/src/compose_x_common/aws/ecr/__init__.py
--rw-r--r--   0        0        0     4696 2024-01-04 16:09:40.440251 compose_x_common-1.4.7/src/compose_x_common/aws/ecr/images.py
--rw-r--r--   0        0        0     2168 2024-01-04 16:09:40.413251 compose_x_common-1.4.7/src/compose_x_common/aws/ecr/repositories.py
--rw-r--r--   0        0        0     6765 2024-01-04 16:09:40.373252 compose_x_common-1.4.7/src/compose_x_common/aws/ecs/__init__.py
--rw-r--r--   0        0        0     2280 2024-01-04 16:09:40.377252 compose_x_common-1.4.7/src/compose_x_common/aws/ecs/instances.py
--rw-r--r--   0        0        0     1613 2024-01-04 16:09:40.442251 compose_x_common-1.4.7/src/compose_x_common/aws/ecs/services.py
--rw-r--r--   0        0        0     1979 2024-01-04 16:09:40.398251 compose_x_common-1.4.7/src/compose_x_common/aws/ecs/tasks.py
--rw-r--r--   0        0        0     1479 2024-01-04 16:09:40.428251 compose_x_common-1.4.7/src/compose_x_common/aws/efs.py
--rw-r--r--   0        0        0      250 2024-01-04 16:09:40.430251 compose_x_common-1.4.7/src/compose_x_common/aws/elasticache.py
--rw-r--r--   0        0        0      873 2024-01-04 16:20:57.269021 compose_x_common-1.4.7/src/compose_x_common/aws/elasticloadbalancing.py
--rw-r--r--   0        0        0      338 2024-01-04 16:09:40.406251 compose_x_common-1.4.7/src/compose_x_common/aws/glue/__init__.py
--rw-r--r--   0        0        0      317 2024-01-04 16:09:40.397251 compose_x_common-1.4.7/src/compose_x_common/aws/iam.py
--rw-r--r--   0        0        0      108 2024-01-04 16:09:40.395252 compose_x_common-1.4.7/src/compose_x_common/aws/kafka.py
--rw-r--r--   0        0        0      407 2024-01-04 16:09:40.384252 compose_x_common-1.4.7/src/compose_x_common/aws/kinesis.py
--rw-r--r--   0        0        0     2934 2024-01-04 16:09:40.423251 compose_x_common-1.4.7/src/compose_x_common/aws/kms.py
--rw-r--r--   0        0        0     3208 2024-01-04 16:09:40.383252 compose_x_common-1.4.7/src/compose_x_common/aws/msk.py
--rw-r--r--   0        0        0      410 2024-01-04 16:09:40.414251 compose_x_common-1.4.7/src/compose_x_common/aws/neptune.py
--rw-r--r--   0        0        0      238 2024-01-04 16:09:40.431251 compose_x_common-1.4.7/src/compose_x_common/aws/opensearch.py
--rw-r--r--   0        0        0      556 2024-01-04 16:09:40.426251 compose_x_common-1.4.7/src/compose_x_common/aws/rds.py
--rw-r--r--   0        0        0     2427 2024-01-04 16:09:40.379252 compose_x_common-1.4.7/src/compose_x_common/aws/resourcegroupstaggingapi.py
--rw-r--r--   0        0        0     2145 2024-01-04 16:09:40.435251 compose_x_common-1.4.7/src/compose_x_common/aws/route53.py
--rw-r--r--   0        0        0      178 2024-01-04 16:09:40.388252 compose_x_common-1.4.7/src/compose_x_common/aws/s3.py
--rw-r--r--   0        0        0      882 2024-01-04 16:09:40.433251 compose_x_common-1.4.7/src/compose_x_common/aws/secrets_manager.py
--rw-r--r--   0        0        0     1601 2024-01-04 16:09:40.436251 compose_x_common-1.4.7/src/compose_x_common/aws/sns.py
--rw-r--r--   0        0        0      231 2024-01-04 16:09:40.411251 compose_x_common-1.4.7/src/compose_x_common/aws/sqs.py
--rw-r--r--   0        0        0      245 2024-01-04 16:09:40.391252 compose_x_common-1.4.7/src/compose_x_common/aws/ssm_parameter.py
--rw-r--r--   0        0        0     4548 2024-01-04 16:09:40.393252 compose_x_common-1.4.7/src/compose_x_common/aws/vpc.py
--rw-r--r--   0        0        0      541 2024-01-04 16:09:40.400251 compose_x_common-1.4.7/src/compose_x_common/aws/wafv2.py
--rw-r--r--   0        0        0     4926 2024-01-04 16:09:40.438251 compose_x_common-1.4.7/src/compose_x_common/compose_x_common.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 compose_x_common-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0      316 2022-03-11 22:14:27.944417 compose_x_common-1.4.8/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2022-03-11 22:14:27.945418 compose_x_common-1.4.8/LICENSE
+-rw-r--r--   0        0        0      262 2022-03-11 22:14:27.945418 compose_x_common-1.4.8/MANIFEST.in
+-rw-r--r--   0        0        0      739 2023-03-19 15:02:14.794099 compose_x_common-1.4.8/README.rst
+-rw-r--r--   0        0        0     2225 2024-05-19 05:53:06.467687 compose_x_common-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0      228 2024-05-19 05:53:06.467687 compose_x_common-1.4.8/src/compose_x_common/__init__.py
+-rw-r--r--   0        0        0     3574 2024-01-04 16:09:40.404251 compose_x_common-1.4.8/src/compose_x_common/aws/__init__.py
+-rw-r--r--   0        0        0     1863 2024-01-04 16:09:40.390251 compose_x_common-1.4.8/src/compose_x_common/aws/acm.py
+-rw-r--r--   0        0        0     1557 2024-01-04 16:09:40.421251 compose_x_common-1.4.8/src/compose_x_common/aws/application_autoscaling.py
+-rw-r--r--   0        0        0      305 2024-01-04 16:09:40.424251 compose_x_common-1.4.8/src/compose_x_common/aws/aps.py
+-rw-r--r--   0        0        0     5105 2024-01-04 16:28:37.364007 compose_x_common-1.4.8/src/compose_x_common/aws/arns.py
+-rw-r--r--   0        0        0     1072 2024-01-04 16:09:40.418251 compose_x_common-1.4.8/src/compose_x_common/aws/cloudmap.py
+-rw-r--r--   0        0        0      263 2024-01-04 16:09:40.416251 compose_x_common-1.4.8/src/compose_x_common/aws/codeguru_profiler.py
+-rw-r--r--   0        0        0     2003 2024-01-04 16:09:40.407251 compose_x_common-1.4.8/src/compose_x_common/aws/cognito_userpool.py
+-rw-r--r--   0        0        0      238 2024-01-04 16:09:40.402251 compose_x_common-1.4.8/src/compose_x_common/aws/dynamodb.py
+-rw-r--r--   0        0        0     1106 2024-01-04 16:09:40.386252 compose_x_common-1.4.8/src/compose_x_common/aws/ec2.py
+-rw-r--r--   0        0        0      471 2024-01-04 16:09:40.409251 compose_x_common-1.4.8/src/compose_x_common/aws/ecr/__init__.py
+-rw-r--r--   0        0        0     4696 2024-01-04 16:09:40.440251 compose_x_common-1.4.8/src/compose_x_common/aws/ecr/images.py
+-rw-r--r--   0        0        0     2168 2024-01-04 16:09:40.413251 compose_x_common-1.4.8/src/compose_x_common/aws/ecr/repositories.py
+-rw-r--r--   0        0        0     6767 2024-05-19 05:53:06.823681 compose_x_common-1.4.8/src/compose_x_common/aws/ecs/__init__.py
+-rw-r--r--   0        0        0     2280 2024-01-04 16:09:40.377252 compose_x_common-1.4.8/src/compose_x_common/aws/ecs/instances.py
+-rw-r--r--   0        0        0     1613 2024-01-04 16:09:40.442251 compose_x_common-1.4.8/src/compose_x_common/aws/ecs/services.py
+-rw-r--r--   0        0        0     1979 2024-01-04 16:09:40.398251 compose_x_common-1.4.8/src/compose_x_common/aws/ecs/tasks.py
+-rw-r--r--   0        0        0     1479 2024-01-04 16:09:40.428251 compose_x_common-1.4.8/src/compose_x_common/aws/efs.py
+-rw-r--r--   0        0        0      250 2024-01-04 16:09:40.430251 compose_x_common-1.4.8/src/compose_x_common/aws/elasticache.py
+-rw-r--r--   0        0        0      873 2024-01-04 16:20:57.269021 compose_x_common-1.4.8/src/compose_x_common/aws/elasticloadbalancing.py
+-rw-r--r--   0        0        0      338 2024-01-04 16:09:40.406251 compose_x_common-1.4.8/src/compose_x_common/aws/glue/__init__.py
+-rw-r--r--   0        0        0      317 2024-01-04 16:09:40.397251 compose_x_common-1.4.8/src/compose_x_common/aws/iam.py
+-rw-r--r--   0        0        0      108 2024-01-04 16:09:40.395252 compose_x_common-1.4.8/src/compose_x_common/aws/kafka.py
+-rw-r--r--   0        0        0      407 2024-01-04 16:09:40.384252 compose_x_common-1.4.8/src/compose_x_common/aws/kinesis.py
+-rw-r--r--   0        0        0     2934 2024-01-04 16:09:40.423251 compose_x_common-1.4.8/src/compose_x_common/aws/kms.py
+-rw-r--r--   0        0        0     3208 2024-01-04 16:09:40.383252 compose_x_common-1.4.8/src/compose_x_common/aws/msk.py
+-rw-r--r--   0        0        0      410 2024-01-04 16:09:40.414251 compose_x_common-1.4.8/src/compose_x_common/aws/neptune.py
+-rw-r--r--   0        0        0      238 2024-01-04 16:09:40.431251 compose_x_common-1.4.8/src/compose_x_common/aws/opensearch.py
+-rw-r--r--   0        0        0      556 2024-01-04 16:09:40.426251 compose_x_common-1.4.8/src/compose_x_common/aws/rds.py
+-rw-r--r--   0        0        0     2427 2024-01-04 16:09:40.379252 compose_x_common-1.4.8/src/compose_x_common/aws/resourcegroupstaggingapi.py
+-rw-r--r--   0        0        0     2145 2024-01-04 16:09:40.435251 compose_x_common-1.4.8/src/compose_x_common/aws/route53.py
+-rw-r--r--   0        0        0      178 2024-01-04 16:09:40.388252 compose_x_common-1.4.8/src/compose_x_common/aws/s3.py
+-rw-r--r--   0        0        0      882 2024-01-04 16:09:40.433251 compose_x_common-1.4.8/src/compose_x_common/aws/secrets_manager.py
+-rw-r--r--   0        0        0     1601 2024-01-04 16:09:40.436251 compose_x_common-1.4.8/src/compose_x_common/aws/sns.py
+-rw-r--r--   0        0        0      231 2024-01-04 16:09:40.411251 compose_x_common-1.4.8/src/compose_x_common/aws/sqs.py
+-rw-r--r--   0        0        0      245 2024-01-04 16:09:40.391252 compose_x_common-1.4.8/src/compose_x_common/aws/ssm_parameter.py
+-rw-r--r--   0        0        0     4548 2024-01-04 16:09:40.393252 compose_x_common-1.4.8/src/compose_x_common/aws/vpc.py
+-rw-r--r--   0        0        0      541 2024-01-04 16:09:40.400251 compose_x_common-1.4.8/src/compose_x_common/aws/wafv2.py
+-rw-r--r--   0        0        0     4926 2024-01-04 16:09:40.438251 compose_x_common-1.4.8/src/compose_x_common/compose_x_common.py
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 compose_x_common-1.4.8/PKG-INFO
```

### Comparing `compose_x_common-1.4.7/LICENSE` & `compose_x_common-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/README.rst` & `compose_x_common-1.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/pyproject.toml` & `compose_x_common-1.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "compose_x_common"
-version = "1.4.7"
+version = "1.4.8"
 description = "Common Library for Compose-X Projects"
 authors = ["John Preston <john@compose-x.io>"]
 maintainers = ["John Preston <john@compose-x.io>"]
 repository = "https://github.com/compose-x/compose-x-common-libs/"
 keywords = ["compose-x", "docker", "compose"]
 license = "MPL-2.0"
 include = [
@@ -36,27 +36,27 @@
 
 [tool.poetry.dev-dependencies]
 placebo = ">=0.9.0,<1.0"
 pytest = "^7.2"
 Sphinx = "^5.0"
 sphinx-material = "^0.0.35"
 isort = "^5.12"
-black = "^23.1"
+black = "^24.3"
 pre-commit = "^3.1"
 flake8-docstrings = "^1.6.0"
 coverage = "^7.0"
 tbump = "^6.9.0"
 pyupgrade = "^3.8"
 sphinx-rtd-theme = "^1.0.0"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/compose-x-common/"
 
 [tool.tbump.version]
-current = "1.4.7"
+current = "1.4.8"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/__init__.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/acm.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/acm.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/application_autoscaling.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/application_autoscaling.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/arns.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/arns.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/cloudmap.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/cloudmap.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/cognito_userpool.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/cognito_userpool.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/ec2.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/ecr/images.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/ecr/images.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/ecr/repositories.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/ecr/repositories.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/ecs/__init__.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/ecs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,17 @@
     for cluster_arn in clusters_to_list:
         cluster_r = client.get_resource(
             TypeName="AWS::ECS::Cluster", Identifier=cluster_arn
         )
         cluster_properties = json.loads(cluster_r["ResourceDescription"]["Properties"])
         if return_as_map:
             if use_cluster_name:
-                clusters[
-                    CLUSTER_NAME_FROM_ARN.match(cluster_arn).group("name")
-                ] = cluster_properties
+                clusters[CLUSTER_NAME_FROM_ARN.match(cluster_arn).group("name")] = (
+                    cluster_properties
+                )
             else:
                 clusters[cluster_arn] = cluster_properties
         else:
             clusters.append(cluster_properties)
     return clusters
```

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/ecs/instances.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/ecs/instances.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/ecs/services.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/ecs/services.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/ecs/tasks.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/ecs/tasks.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/efs.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/efs.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/elasticloadbalancing.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/elasticloadbalancing.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/kms.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/kms.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/msk.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/msk.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/rds.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/rds.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/resourcegroupstaggingapi.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/resourcegroupstaggingapi.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/route53.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/route53.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/secrets_manager.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/sns.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/sns.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/vpc.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/vpc.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/aws/wafv2.py` & `compose_x_common-1.4.8/src/compose_x_common/aws/wafv2.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/src/compose_x_common/compose_x_common.py` & `compose_x_common-1.4.8/src/compose_x_common/compose_x_common.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.4.7/PKG-INFO` & `compose_x_common-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose_x_common
-Version: 1.4.7
+Version: 1.4.8
 Summary: Common Library for Compose-X Projects
 Home-page: https://github.com/compose-x/compose-x-common-libs/
 License: MPL-2.0
 Keywords: compose-x,docker,compose
 Author: John Preston
 Author-email: john@compose-x.io
 Maintainer: John Preston
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: flatdict (>=4.0.1,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/compose-x/compose-x-common-libs/
 Description-Content-Type: text/x-rst
 
 =====================
```

