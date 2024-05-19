# Comparing `tmp/iam_actions-1.2.20240517.tar.gz` & `tmp/iam_actions-1.2.20240518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240517.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240518.tar", max compression
```

## Comparing `iam_actions-1.2.20240517.tar` & `iam_actions-1.2.20240518.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/README.md
--rw-r--r--   0        0        0      228 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/__init__.py
--rw-r--r--   0        0        0  4837373 2024-05-17 02:22:25.579774 iam_actions-1.2.20240517/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-17 02:21:17.603372 iam_actions-1.2.20240517/iam_actions/generate/services.py
--rw-r--r--   0        0        0   629260 2024-05-17 02:22:25.579774 iam_actions-1.2.20240517/iam_actions/policies.json
--rw-r--r--   0        0        0   209717 2024-05-17 02:22:25.579774 iam_actions-1.2.20240517/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   610645 2024-05-17 02:22:25.579774 iam_actions-1.2.20240517/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-17 02:22:26.235777 iam_actions-1.2.20240517/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240517/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240517/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/README.md
+-rw-r--r--   0        0        0      228 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4837373 2024-05-18 02:23:17.746312 iam_actions-1.2.20240518/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-18 02:21:25.415650 iam_actions-1.2.20240518/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   629260 2024-05-18 02:23:17.746312 iam_actions-1.2.20240518/iam_actions/policies.json
+-rw-r--r--   0        0        0   209717 2024-05-18 02:23:17.746312 iam_actions-1.2.20240518/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   610645 2024-05-18 02:23:17.746312 iam_actions-1.2.20240518/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-18 02:23:18.454303 iam_actions-1.2.20240518/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240518/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240518/PKG-INFO
```

### Comparing `iam_actions-1.2.20240517/LICENSE` & `iam_actions-1.2.20240518/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/README.md` & `iam_actions-1.2.20240518/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/actions.json` & `iam_actions-1.2.20240518/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4442,217 +4442,217 @@
             "resources": [
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appfabric": {
-        "UntagResource": {
+        "DeleteIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestionDestination": {
+        "UpdateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "CreateIngestionDestination",
+            "action": "UpdateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionDestination": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetIngestionDestination",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ConnectAppAuthorization": {
+        "CreateAppBundle": {
             "access_level": "Undocumented",
-            "action": "ConnectAppAuthorization",
+            "action": "CreateAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteAppBundle": {
             "access_level": "Undocumented",
             "action": "DeleteAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionDestinations": {
+        "GetAppBundle": {
             "access_level": "Undocumented",
-            "action": "ListIngestionDestinations",
+            "action": "GetAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestion": {
+        "ListAppAuthorizations": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestion",
+            "action": "ListAppAuthorizations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestions": {
+        "DeleteIngestion": {
             "access_level": "Undocumented",
-            "action": "ListIngestions",
+            "action": "DeleteIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppAuthorization": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateAppAuthorization",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppBundles": {
+        "StopIngestion": {
             "access_level": "Undocumented",
-            "action": "ListAppBundles",
+            "action": "StopIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestionDestination": {
+        "CreateIngestion": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestionDestination",
+            "action": "CreateIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppAuthorization": {
+        "ConnectAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "UpdateAppAuthorization",
+            "action": "ConnectAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopIngestion": {
+        "GetIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "StopIngestion",
+            "action": "GetIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppBundle": {
+        "BatchGetUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "GetAppBundle",
+            "action": "BatchGetUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAuthorizations": {
+        "ListIngestionDestinations": {
             "access_level": "Undocumented",
-            "action": "ListAppAuthorizations",
+            "action": "ListIngestionDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestion": {
+        "ListIngestions": {
             "access_level": "Undocumented",
-            "action": "StartIngestion",
+            "action": "ListIngestions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestion": {
+        "UpdateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "GetIngestion",
+            "action": "UpdateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteAppAuthorization": {
             "access_level": "Undocumented",
             "action": "DeleteAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartUserAccessTasks": {
+        "ListAppBundles": {
             "access_level": "Undocumented",
-            "action": "StartUserAccessTasks",
+            "action": "ListAppBundles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetUserAccessTasks": {
+        "CreateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "BatchGetUserAccessTasks",
+            "action": "CreateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestion": {
+        "StartUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "CreateIngestion",
+            "action": "StartUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppBundle": {
+        "StartIngestion": {
             "access_level": "Undocumented",
-            "action": "CreateAppBundle",
+            "action": "StartIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppAuthorization": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetAppAuthorization",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetIngestion": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIngestionDestination": {
+        "GetAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "UpdateIngestionDestination",
+            "action": "GetAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "appflow": {
@@ -5170,121 +5170,121 @@
             "condition_keys": [],
             "description": "Grants permission to update an existing Application Cost Profiler Report configuration",
             "orphan": false,
             "resources": []
         }
     },
     "application-transformation": {
-        "GetGroupingAssessment": {
+        "StartDeployment": {
             "access_level": "Undocumented",
-            "action": "GetGroupingAssessment",
+            "action": "StartDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMetricData": {
+        "StartPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "PutMetricData",
+            "action": "StartPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeployment": {
+        "StartRuntimeAssessment": {
             "access_level": "Undocumented",
-            "action": "GetDeployment",
+            "action": "StartRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingCompatibilityAssessment": {
+        "GetPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "StartPortingCompatibilityAssessment",
+            "action": "GetPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRuntimeAssessment": {
+        "GetContainerization": {
             "access_level": "Undocumented",
-            "action": "GetRuntimeAssessment",
+            "action": "GetContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingRecommendationAssessment": {
+        "StartPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "GetPortingRecommendationAssessment",
+            "action": "StartPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutLogData": {
+        "GetPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "PutLogData",
+            "action": "GetPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartGroupingAssessment": {
+        "GetDeployment": {
             "access_level": "Undocumented",
-            "action": "StartGroupingAssessment",
+            "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRuntimeAssessment": {
+        "GetGroupingAssessment": {
             "access_level": "Undocumented",
-            "action": "StartRuntimeAssessment",
+            "action": "GetGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingRecommendationAssessment": {
+        "PutMetricData": {
             "access_level": "Undocumented",
-            "action": "StartPortingRecommendationAssessment",
+            "action": "PutMetricData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartContainerization": {
             "access_level": "Undocumented",
             "action": "StartContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingCompatibilityAssessment": {
+        "StartGroupingAssessment": {
             "access_level": "Undocumented",
-            "action": "GetPortingCompatibilityAssessment",
+            "action": "StartGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContainerization": {
+        "PutLogData": {
             "access_level": "Undocumented",
-            "action": "GetContainerization",
+            "action": "PutLogData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDeployment": {
+        "GetRuntimeAssessment": {
             "access_level": "Undocumented",
-            "action": "StartDeployment",
+            "action": "GetRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "applicationinsights": {
@@ -11773,25 +11773,25 @@
             "condition_keys": [],
             "description": "Grants permission to view a seller dashboard",
             "orphan": false,
             "resources": [
                 "SellerDashboard"
             ]
         },
-        "PutDeploymentParameter": {
+        "ListPrivateListings": {
             "access_level": "Undocumented",
-            "action": "PutDeploymentParameter",
+            "action": "ListPrivateListings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivateListings": {
+        "PutDeploymentParameter": {
             "access_level": "Undocumented",
-            "action": "ListPrivateListings",
+            "action": "PutDeploymentParameter",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "aws-marketplace-management": {
@@ -11997,225 +11997,225 @@
             "condition_keys": [],
             "description": "Validates Server Migration Connector Id that was registered with AWS Connector Service.",
             "orphan": false,
             "resources": []
         }
     },
     "b2bi": {
-        "GetTransformer": {
+        "GetPartnership": {
             "access_level": "Undocumented",
-            "action": "GetTransformer",
+            "action": "GetPartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdatePartnership": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTransformers": {
             "access_level": "Undocumented",
             "action": "ListTransformers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestMapping": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TestMapping",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCapability": {
+        "UpdateTransformer": {
             "access_level": "Undocumented",
-            "action": "UpdateCapability",
+            "action": "UpdateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProfile": {
+        "StartTransformerJob": {
             "access_level": "Undocumented",
-            "action": "UpdateProfile",
+            "action": "StartTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteProfile": {
             "access_level": "Undocumented",
             "action": "DeleteProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCapability": {
+        "DeleteTransformer": {
             "access_level": "Undocumented",
-            "action": "DeleteCapability",
+            "action": "DeleteTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePartnership": {
+        "GetCapability": {
             "access_level": "Undocumented",
-            "action": "CreatePartnership",
+            "action": "GetCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCapabilities": {
+        "GetProfile": {
             "access_level": "Undocumented",
-            "action": "ListCapabilities",
+            "action": "GetProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfiles": {
+        "GetTransformer": {
             "access_level": "Undocumented",
-            "action": "ListProfiles",
+            "action": "GetTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCapability": {
+        "ListCapabilities": {
             "access_level": "Undocumented",
-            "action": "CreateCapability",
+            "action": "ListCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreatePartnership": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestParsing": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TestParsing",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapability": {
+        "CreateProfile": {
             "access_level": "Undocumented",
-            "action": "GetCapability",
+            "action": "CreateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransformerJob": {
+        "DeletePartnership": {
             "access_level": "Undocumented",
-            "action": "GetTransformerJob",
+            "action": "DeletePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTransformer": {
+        "ListProfiles": {
             "access_level": "Undocumented",
-            "action": "CreateTransformer",
+            "action": "ListProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTransformer": {
+        "GetTransformerJob": {
             "access_level": "Undocumented",
-            "action": "DeleteTransformer",
+            "action": "GetTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePartnership": {
+        "TestParsing": {
             "access_level": "Undocumented",
-            "action": "DeletePartnership",
+            "action": "TestParsing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTransformer": {
+        "UpdateProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateTransformer",
+            "action": "UpdateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProfile": {
+        "ListPartnerships": {
             "access_level": "Undocumented",
-            "action": "CreateProfile",
+            "action": "ListPartnerships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnership": {
+        "DeleteCapability": {
             "access_level": "Undocumented",
-            "action": "GetPartnership",
+            "action": "DeleteCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfile": {
+        "UpdateCapability": {
             "access_level": "Undocumented",
-            "action": "GetProfile",
+            "action": "UpdateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerships": {
+        "CreateTransformer": {
             "access_level": "Undocumented",
-            "action": "ListPartnerships",
+            "action": "CreateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnership": {
+        "TestMapping": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnership",
+            "action": "TestMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTransformerJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartTransformerJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateCapability": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "backup": {
@@ -13849,97 +13849,97 @@
             "orphan": false,
             "resources": [
                 "scheduling-policy"
             ]
         }
     },
     "bcm-data-exports": {
-        "UntagResource": {
+        "ListExports": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListExports",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateExport": {
             "access_level": "Undocumented",
             "action": "UpdateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "GetTable": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "GetTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExport": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "DeleteExport",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExports": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListExports",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetExecution": {
             "access_level": "Undocumented",
             "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTables": {
+        "CreateExport": {
             "access_level": "Undocumented",
-            "action": "ListTables",
+            "action": "CreateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExport": {
+        "GetExport": {
             "access_level": "Undocumented",
-            "action": "CreateExport",
+            "action": "GetExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTable": {
+        "DeleteExport": {
             "access_level": "Undocumented",
-            "action": "GetTable",
+            "action": "DeleteExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExport": {
+        "ListTables": {
             "access_level": "Undocumented",
-            "action": "GetExport",
+            "action": "ListTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
@@ -13947,827 +13947,827 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "bedrock": {
-        "GetAgentVersion": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetAgentVersion",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEvaluationJob": {
+        "AssociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetEvaluationJob",
+            "action": "AssociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "CreateModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "CreateModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKnowledgeBase": {
+        "PutFoundationModelEntitlement": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "PutFoundationModelEntitlement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrailVersion": {
+        "StartIngestionJob": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrailVersion",
+            "action": "StartIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUseCaseForModelAccess": {
+        "CreateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "GetUseCaseForModelAccess",
+            "action": "CreateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteModelInvocationLoggingConfiguration": {
+        "GetCustomModel": {
             "access_level": "Undocumented",
-            "action": "DeleteModelInvocationLoggingConfiguration",
+            "action": "GetCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentAlias": {
+        "ListAgentAliases": {
             "access_level": "Undocumented",
-            "action": "CreateAgentAlias",
+            "action": "ListAgentAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Retrieve": {
+        "InvokeModel": {
             "access_level": "Undocumented",
-            "action": "Retrieve",
+            "action": "InvokeModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProvisionedModelThroughput": {
+        "GetAgentVersion": {
             "access_level": "Undocumented",
-            "action": "CreateProvisionedModelThroughput",
+            "action": "GetAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentActionGroups": {
+        "ListGuardrails": {
             "access_level": "Undocumented",
-            "action": "ListAgentActionGroups",
+            "action": "ListGuardrails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgent": {
+        "UpdateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "DeleteAgent",
+            "action": "UpdateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModelAvailability": {
+        "GetFoundationModel": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModelAvailability",
+            "action": "GetFoundationModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrail": {
+        "ListProvisionedModelThroughputs": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrail",
+            "action": "ListProvisionedModelThroughputs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModelWithResponseStream": {
+        "DisassociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "InvokeModelWithResponseStream",
+            "action": "DisassociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgent": {
+        "GetModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetAgent",
+            "action": "GetModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateThirdPartyKnowledgeBase": {
+        "GetAgentAlias": {
             "access_level": "Undocumented",
-            "action": "AssociateThirdPartyKnowledgeBase",
+            "action": "GetAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGuardrails": {
+        "InvokeAgent": {
             "access_level": "Undocumented",
-            "action": "ListGuardrails",
+            "action": "InvokeAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModels": {
+        "CreateAgent": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModels",
+            "action": "CreateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "ListModelInvocationJobs": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "ListModelInvocationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBase": {
+        "GetModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBase",
+            "action": "GetModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgents": {
+        "GetGuardrail": {
             "access_level": "Undocumented",
-            "action": "ListAgents",
+            "action": "GetGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopEvaluationJob": {
+        "GetUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "StopEvaluationJob",
+            "action": "GetUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGuardrail": {
+        "StopModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "GetGuardrail",
+            "action": "StopModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProvisionedModelThroughput": {
+        "DeleteProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "UpdateProvisionedModelThroughput",
+            "action": "DeleteProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "CreateModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "CreateModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutModelInvocationLoggingConfiguration": {
+        "ListCustomModels": {
             "access_level": "Undocumented",
-            "action": "PutModelInvocationLoggingConfiguration",
+            "action": "ListCustomModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProvisionedModelThroughput": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetProvisionedModelThroughput",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedModelThroughputs": {
+        "GetAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedModelThroughputs",
+            "action": "GetAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentAlias": {
+        "CreateEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentAlias",
+            "action": "CreateEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelInvocationJob": {
+        "UpdateGuardrail": {
             "access_level": "Undocumented",
-            "action": "StopModelInvocationJob",
+            "action": "UpdateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentKnowledgeBase": {
+        "DeleteModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetAgentKnowledgeBase",
+            "action": "DeleteModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ApplyGuardrail": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ApplyGuardrail",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFoundationModelAgreement": {
+        "InvokeModelWithResponseStream": {
             "access_level": "Undocumented",
-            "action": "DeleteFoundationModelAgreement",
+            "action": "InvokeModelWithResponseStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentActionGroup": {
+        "DeleteCustomModel": {
             "access_level": "Undocumented",
-            "action": "GetAgentActionGroup",
+            "action": "DeleteCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProvisionedModelThroughput": {
+        "DeleteAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteProvisionedModelThroughput",
+            "action": "DeleteAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentVersions": {
+        "DetectGeneratedContent": {
             "access_level": "Undocumented",
-            "action": "ListAgentVersions",
+            "action": "DetectGeneratedContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionJob": {
+        "GetProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "GetIngestionJob",
+            "action": "GetProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUseCaseForModelAccess": {
+        "CreateGuardrail": {
             "access_level": "Undocumented",
-            "action": "PutUseCaseForModelAccess",
+            "action": "CreateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "DeleteGuardrail": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "DeleteGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFoundationModelAgreement": {
+        "ListAgentVersions": {
             "access_level": "Undocumented",
-            "action": "CreateFoundationModelAgreement",
+            "action": "ListAgentVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCustomModels": {
+        "ListModelEvaluationJobs": {
             "access_level": "Undocumented",
-            "action": "ListCustomModels",
+            "action": "ListModelEvaluationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelInvocationJob": {
+        "DeleteFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "CreateModelInvocationJob",
+            "action": "DeleteFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModel": {
+        "CreateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModel",
+            "action": "CreateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelCustomizationJob": {
+        "ListAgentActionGroups": {
             "access_level": "Undocumented",
-            "action": "CreateModelCustomizationJob",
+            "action": "ListAgentActionGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentAliases": {
+        "ListAgentKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "ListAgentAliases",
+            "action": "ListAgentKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFoundationModelEntitlement": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "PutFoundationModelEntitlement",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEvaluationJob": {
+        "PrepareAgent": {
             "access_level": "Undocumented",
-            "action": "CreateEvaluationJob",
+            "action": "PrepareAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentActionGroup": {
+        "DeleteAgentAlias": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentActionGroup",
+            "action": "DeleteAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgent": {
+        "StopEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "CreateAgent",
+            "action": "StopEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGuardrail": {
+        "StopModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteGuardrail",
+            "action": "StopModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListFoundationModels": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListFoundationModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentAlias": {
+        "ListFoundationModelAgreementOffers": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentAlias",
+            "action": "ListFoundationModelAgreementOffers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelInvocationJobs": {
+        "ListModelCustomizationJobs": {
             "access_level": "Undocumented",
-            "action": "ListModelInvocationJobs",
+            "action": "ListModelCustomizationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomModel": {
+        "RetrieveAndGenerate": {
             "access_level": "Undocumented",
-            "action": "GetCustomModel",
+            "action": "RetrieveAndGenerate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentActionGroup": {
+        "GetAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentActionGroup",
+            "action": "GetAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModelAgreementOffers": {
+        "AssociateThirdPartyKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModelAgreementOffers",
+            "action": "AssociateThirdPartyKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PrepareAgent": {
+        "GetModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "PrepareAgent",
+            "action": "GetModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationLoggingConfiguration": {
+        "Retrieve": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationLoggingConfiguration",
+            "action": "Retrieve",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgent": {
+        "GetAgent": {
             "access_level": "Undocumented",
-            "action": "UpdateAgent",
+            "action": "GetAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentVersion": {
+        "PutModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentVersion",
+            "action": "PutModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetectGeneratedContent": {
+        "UpdateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "DetectGeneratedContent",
+            "action": "UpdateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "ListEvaluationJobs": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "ListEvaluationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RetrieveAndGenerate": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "RetrieveAndGenerate",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelEvaluationJobs": {
+        "GetModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "ListModelEvaluationJobs",
+            "action": "GetModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeAgent": {
+        "PutUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "InvokeAgent",
+            "action": "PutUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestionJob": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "StartIngestionJob",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGuardrail": {
+        "CreateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "UpdateGuardrail",
+            "action": "CreateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEvaluationJobs": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListEvaluationJobs",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelEvaluationJob": {
+        "CreateModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "CreateModelEvaluationJob",
+            "action": "CreateModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelCustomizationJob": {
+        "GetFoundationModelAvailability": {
             "access_level": "Undocumented",
-            "action": "StopModelCustomizationJob",
+            "action": "GetFoundationModelAvailability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModel": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "InvokeModel",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelEvaluationJob": {
+        "DeleteAgentVersion": {
             "access_level": "Undocumented",
-            "action": "GetModelEvaluationJob",
+            "action": "DeleteAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionJobs": {
+        "CreateFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "ListIngestionJobs",
+            "action": "CreateFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelCustomizationJobs": {
+        "ApplyGuardrail": {
             "access_level": "Undocumented",
-            "action": "ListModelCustomizationJobs",
+            "action": "ApplyGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentKnowledgeBases": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "ListAgentKnowledgeBases",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelCustomizationJob": {
+        "UpdateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetModelCustomizationJob",
+            "action": "UpdateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAgentKnowledgeBase": {
+        "ListAgents": {
             "access_level": "Undocumented",
-            "action": "AssociateAgentKnowledgeBase",
+            "action": "ListAgents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentKnowledgeBase": {
+        "UpdateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentKnowledgeBase",
+            "action": "UpdateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationJob": {
+        "DeleteAgent": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationJob",
+            "action": "DeleteAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCustomModel": {
+        "GetIngestionJob": {
             "access_level": "Undocumented",
-            "action": "DeleteCustomModel",
+            "action": "GetIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAgentKnowledgeBase": {
+        "CreateGuardrailVersion": {
             "access_level": "Undocumented",
-            "action": "DisassociateAgentKnowledgeBase",
+            "action": "CreateGuardrailVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentActionGroup": {
+        "UpdateAgent": {
             "access_level": "Undocumented",
-            "action": "CreateAgentActionGroup",
+            "action": "UpdateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentAlias": {
+        "GetEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "GetAgentAlias",
+            "action": "GetEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListIngestionJobs": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListIngestionJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billing": {
-        "GetCredits": {
+        "GetContractInformation": {
             "access_level": "Undocumented",
-            "action": "GetCredits",
+            "action": "GetContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingNotifications": {
+        "UpdateBillingPreferences": {
             "access_level": "Undocumented",
-            "action": "GetBillingNotifications",
+            "action": "UpdateBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RedeemCredits": {
+        "GetSellerOfRecord": {
             "access_level": "Undocumented",
-            "action": "RedeemCredits",
+            "action": "GetSellerOfRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContractInformation": {
+        "ListBillingViews": {
             "access_level": "Undocumented",
-            "action": "GetContractInformation",
+            "action": "ListBillingViews",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingPreferences": {
+        "RedeemCredits": {
             "access_level": "Undocumented",
-            "action": "GetBillingPreferences",
+            "action": "RedeemCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutContractInformation": {
+        "GetBillingPreferences": {
             "access_level": "Undocumented",
-            "action": "PutContractInformation",
+            "action": "GetBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetBillingDetails": {
             "access_level": "Undocumented",
             "action": "GetBillingDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIAMAccessPreference": {
+        "GetBillingNotifications": {
             "access_level": "Undocumented",
-            "action": "GetIAMAccessPreference",
+            "action": "GetBillingNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateBillingPreferences": {
+        "GetCredits": {
             "access_level": "Undocumented",
-            "action": "UpdateBillingPreferences",
+            "action": "GetCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSellerOfRecord": {
+        "GetIAMAccessPreference": {
             "access_level": "Undocumented",
-            "action": "GetSellerOfRecord",
+            "action": "GetIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingData": {
+        "PutContractInformation": {
             "access_level": "Undocumented",
-            "action": "GetBillingData",
+            "action": "PutContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIAMAccessPreference": {
+        "GetBillingData": {
             "access_level": "Undocumented",
-            "action": "UpdateIAMAccessPreference",
+            "action": "GetBillingData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBillingViews": {
+        "UpdateIAMAccessPreference": {
             "access_level": "Undocumented",
-            "action": "ListBillingViews",
+            "action": "UpdateIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billingconductor": {
@@ -19939,715 +19939,715 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "GetMembership": {
+        "GetConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "GetConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgets": {
+        "ListAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgets",
+            "action": "ListAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationAnalysisTemplates": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationAnalysisTemplates",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationConfiguredAudienceModelAssociations": {
+        "DeleteConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationConfiguredAudienceModelAssociations",
+            "action": "DeleteConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnalysisTemplates": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListAnalysisTemplates",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetCollaborationAnalysisTemplate": {
+        "ListPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "BatchGetCollaborationAnalysisTemplate",
+            "action": "ListPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "ListCollaborationPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "ListCollaborationPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePrivacyBudgetTemplate": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdatePrivacyBudgetTemplate",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModelAssociation": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModelAssociation",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnalysisTemplate": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "DeleteAnalysisTemplate",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationPrivacyBudgetTemplate": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationPrivacyBudgetTemplate",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "GetCollaborationConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "GetCollaborationConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnalysisTemplate": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "GetAnalysisTemplate",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "BatchGetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "BatchGetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "UpdateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "UpdateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgets": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgets",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "UpdateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "UpdateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PreviewPrivacyImpact": {
+        "UpdatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "PreviewPrivacyImpact",
+            "action": "UpdatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "CreatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "CreatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivacyBudgetTemplate": {
+        "CreateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "CreatePrivacyBudgetTemplate",
+            "action": "CreateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModelAssociation": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModelAssociation",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivacyBudgetTemplate": {
+        "ListCollaborationConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "DeletePrivacyBudgetTemplate",
+            "action": "ListCollaborationConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "ListCollaborationPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "ListCollaborationPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "ListConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "ListConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelAssociation": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelAssociation",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "DeletePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "DeletePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "DeleteAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "DeleteAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchemaAnalysisRule": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchemaAnalysisRule",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "CreateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "CreateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationAnalysisTemplate": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationAnalysisTemplate",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationConfiguredAudienceModelAssociation": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationConfiguredAudienceModelAssociation",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "GetPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "GetPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "GetAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "GetAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "ListPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "ListPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgetTemplates": {
+        "GetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgetTemplates",
+            "action": "GetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredAudienceModelAssociations": {
+        "BatchGetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredAudienceModelAssociations",
+            "action": "BatchGetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnalysisTemplate": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "CreateAnalysisTemplate",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgetTemplates": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgetTemplates",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnalysisTemplate": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdateAnalysisTemplate",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTables": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "ListCollaborationAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "ListCollaborationAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivacyBudgetTemplate": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "GetPrivacyBudgetTemplate",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelAssociation": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelAssociation",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "GetCollaborationPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "GetCollaborationPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "PreviewPrivacyImpact": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "PreviewPrivacyImpact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms-ml": {
-        "DeleteConfiguredAudienceModelPolicy": {
+        "UnTagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelPolicy",
+            "action": "UnTagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrainingDataset": {
+        "StartAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteTrainingDataset",
+            "action": "StartAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UnTagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UnTagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceGenerationJobs": {
+        "GetAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListAudienceGenerationJobs",
+            "action": "GetAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModel": {
+        "CreateAudienceModel": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModel",
+            "action": "CreateAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceGenerationJob": {
+        "DeleteAudienceModel": {
             "access_level": "Undocumented",
-            "action": "StartAudienceGenerationJob",
+            "action": "DeleteAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModel": {
+        "DeleteConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModel",
+            "action": "DeleteConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAudienceModel": {
+        "ListConfiguredAudienceModels": {
             "access_level": "Undocumented",
-            "action": "CreateAudienceModel",
+            "action": "ListConfiguredAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceGenerationJob": {
+        "ListAudienceExportJobs": {
             "access_level": "Undocumented",
-            "action": "GetAudienceGenerationJob",
+            "action": "ListAudienceExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrainingDataset": {
+        "ListAudienceGenerationJobs": {
             "access_level": "Undocumented",
-            "action": "CreateTrainingDataset",
+            "action": "ListAudienceGenerationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceModel": {
+        "ListAudienceModels": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceModel",
+            "action": "ListAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelPolicy": {
+        "PutConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelPolicy",
+            "action": "PutConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceGenerationJob": {
+        "DeleteTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceGenerationJob",
+            "action": "DeleteTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceModel": {
+        "GetConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "GetAudienceModel",
+            "action": "GetConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceModels": {
+        "GetAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "ListAudienceModels",
+            "action": "GetAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrainingDataset": {
+        "GetConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetTrainingDataset",
+            "action": "GetConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModel": {
+        "DeleteAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModel",
+            "action": "DeleteAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceExportJobs": {
+        "StartAudienceExportJob": {
             "access_level": "Undocumented",
-            "action": "ListAudienceExportJobs",
+            "action": "StartAudienceExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutConfiguredAudienceModelPolicy": {
+        "CreateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "PutConfiguredAudienceModelPolicy",
+            "action": "CreateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModel": {
+        "CreateTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModel",
+            "action": "CreateTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTrainingDatasets": {
             "access_level": "Undocumented",
             "action": "ListTrainingDatasets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceExportJob": {
+        "UpdateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "StartAudienceExportJob",
+            "action": "UpdateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredAudienceModels": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredAudienceModels",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -23634,33 +23634,33 @@
             "orphan": false,
             "resources": [
                 "streaming-distribution"
             ]
         }
     },
     "cloudfront-keyvaluestore": {
-        "PutKey": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "PutKey",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeKeyValueStore": {
+        "PutKey": {
             "access_level": "Undocumented",
-            "action": "DescribeKeyValueStore",
+            "action": "PutKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "UpdateKeys": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "UpdateKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteKey": {
             "access_level": "Undocumented",
@@ -23674,17 +23674,17 @@
             "access_level": "Undocumented",
             "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKeys": {
+        "DescribeKeyValueStore": {
             "access_level": "Undocumented",
-            "action": "UpdateKeys",
+            "action": "DescribeKeyValueStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloudhsm": {
@@ -27836,305 +27836,305 @@
             "orphan": false,
             "resources": [
                 "repository"
             ]
         }
     },
     "codeconnections": {
-        "ListSyncConfigurations": {
+        "GetInstallationUrl": {
             "access_level": "Undocumented",
-            "action": "ListSyncConfigurations",
+            "action": "GetInstallationUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteHost": {
+        "PassRepository": {
             "access_level": "Undocumented",
-            "action": "DeleteHost",
+            "action": "PassRepository",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListHosts": {
+        "UpdateHost": {
             "access_level": "Undocumented",
-            "action": "ListHosts",
+            "action": "UpdateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositoryLinks": {
+        "GetResourceSyncStatus": {
             "access_level": "Undocumented",
-            "action": "ListRepositoryLinks",
+            "action": "GetResourceSyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSyncConfiguration": {
+        "RegisterAppCode": {
             "access_level": "Undocumented",
-            "action": "CreateSyncConfiguration",
+            "action": "RegisterAppCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateHost": {
+        "DeleteSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateHost",
+            "action": "DeleteSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseConnection": {
+        "GetSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "UseConnection",
+            "action": "GetSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSyncConfiguration": {
+        "UpdateSyncBlocker": {
             "access_level": "Undocumented",
-            "action": "DeleteSyncConfiguration",
+            "action": "UpdateSyncBlocker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetIndividualAccessToken": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetIndividualAccessToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnection": {
+        "ListRepositoryLinks": {
             "access_level": "Undocumented",
-            "action": "DeleteConnection",
+            "action": "ListRepositoryLinks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstallationUrl": {
+        "CreateConnection": {
             "access_level": "Undocumented",
-            "action": "GetInstallationUrl",
+            "action": "CreateConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnection": {
+        "GetConnection": {
             "access_level": "Undocumented",
-            "action": "CreateConnection",
+            "action": "GetConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndividualAccessToken": {
+        "GetRepositorySyncStatus": {
             "access_level": "Undocumented",
-            "action": "GetIndividualAccessToken",
+            "action": "GetRepositorySyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppRegistrationHandshake": {
+        "CreateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartAppRegistrationHandshake",
+            "action": "CreateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRepositoryLink": {
+        "UpdateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteRepositoryLink",
+            "action": "UpdateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRepository": {
+        "GetSyncBlockerSummary": {
             "access_level": "Undocumented",
-            "action": "PassRepository",
+            "action": "GetSyncBlockerSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstallationTargets": {
+        "DeleteRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "ListInstallationTargets",
+            "action": "DeleteRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRepositoryLink": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateRepositoryLink",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateRepositoryLink": {
             "access_level": "Undocumented",
             "action": "UpdateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSyncBlockerSummary": {
+        "StartOAuthHandshake": {
             "access_level": "Undocumented",
-            "action": "GetSyncBlockerSummary",
+            "action": "StartOAuthHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConnection": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetConnection",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "PassConnection": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "PassConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSyncBlocker": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSyncBlocker",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHost": {
+        "UpdateConnectionInstallation": {
             "access_level": "Undocumented",
-            "action": "GetHost",
+            "action": "UpdateConnectionInstallation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConnectionInstallation": {
+        "ListSyncConfigurations": {
             "access_level": "Undocumented",
-            "action": "UpdateConnectionInstallation",
+            "action": "ListSyncConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceSyncStatus": {
+        "StartAppRegistrationHandshake": {
             "access_level": "Undocumented",
-            "action": "GetResourceSyncStatus",
+            "action": "StartAppRegistrationHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositorySyncDefinitions": {
+        "ListConnections": {
             "access_level": "Undocumented",
-            "action": "ListRepositorySyncDefinitions",
+            "action": "ListConnections",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartOAuthHandshake": {
+        "UseConnection": {
             "access_level": "Undocumented",
-            "action": "StartOAuthHandshake",
+            "action": "UseConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConnections": {
+        "CreateHost": {
             "access_level": "Undocumented",
-            "action": "ListConnections",
+            "action": "CreateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositoryLink": {
+        "ListHosts": {
             "access_level": "Undocumented",
-            "action": "GetRepositoryLink",
+            "action": "ListHosts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositorySyncStatus": {
+        "DeleteHost": {
             "access_level": "Undocumented",
-            "action": "GetRepositorySyncStatus",
+            "action": "DeleteHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassConnection": {
+        "DeleteConnection": {
             "access_level": "Undocumented",
-            "action": "PassConnection",
+            "action": "DeleteConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterAppCode": {
+        "ListInstallationTargets": {
             "access_level": "Undocumented",
-            "action": "RegisterAppCode",
+            "action": "ListInstallationTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSyncConfiguration": {
+        "GetRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "GetSyncConfiguration",
+            "action": "GetRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSyncConfiguration": {
+        "CreateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "UpdateSyncConfiguration",
+            "action": "CreateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateHost": {
+        "GetHost": {
             "access_level": "Undocumented",
-            "action": "CreateHost",
+            "action": "GetHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListRepositorySyncDefinitions": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListRepositorySyncDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codedeploy": {
@@ -29066,129 +29066,129 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "UntagResource": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "BatchGetFindings": {
             "access_level": "Undocumented",
             "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteScansByCategory": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountConfiguration": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricsSummary": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindingsMetrics": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -37765,69 +37765,69 @@
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         }
     },
     "consoleapp": {
-        "GetDeviceIdentity": {
+        "ListDeviceIdentities": {
             "access_level": "Undocumented",
-            "action": "GetDeviceIdentity",
+            "action": "ListDeviceIdentities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceIdentities": {
+        "GetDeviceIdentity": {
             "access_level": "Undocumented",
-            "action": "ListDeviceIdentities",
+            "action": "GetDeviceIdentity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
-        "ListLinkedAccounts": {
+        "GetAccountBillingRole": {
             "access_level": "Undocumented",
-            "action": "ListLinkedAccounts",
+            "action": "GetAccountBillingRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountBillingRole": {
+        "ListLinkedAccounts": {
             "access_level": "Undocumented",
-            "action": "GetAccountBillingRole",
+            "action": "ListLinkedAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controlcatalog": {
-        "ListObjectives": {
+        "ListCommonControls": {
             "access_level": "Undocumented",
-            "action": "ListObjectives",
+            "action": "ListCommonControls",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCommonControls": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "ListCommonControls",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "ListObjectives": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "ListObjectives",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controltower": {
@@ -38377,65 +38377,65 @@
             "orphan": false,
             "resources": [
                 "LandingZone"
             ]
         }
     },
     "cost-optimization-hub": {
-        "UpdateEnrollmentStatus": {
+        "UpdatePreferences": {
             "access_level": "Undocumented",
-            "action": "UpdateEnrollmentStatus",
+            "action": "UpdatePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePreferences": {
+        "UpdateEnrollmentStatus": {
             "access_level": "Undocumented",
-            "action": "UpdatePreferences",
+            "action": "UpdateEnrollmentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendations": {
+        "GetPreferences": {
             "access_level": "Undocumented",
-            "action": "ListRecommendations",
+            "action": "GetPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnrollmentStatuses": {
+        "GetRecommendation": {
             "access_level": "Undocumented",
-            "action": "ListEnrollmentStatuses",
+            "action": "GetRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPreferences": {
+        "ListEnrollmentStatuses": {
             "access_level": "Undocumented",
-            "action": "GetPreferences",
+            "action": "ListEnrollmentStatuses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListRecommendationSummaries": {
             "access_level": "Undocumented",
             "action": "ListRecommendationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecommendation": {
+        "ListRecommendations": {
             "access_level": "Undocumented",
-            "action": "GetRecommendation",
+            "action": "ListRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cur": {
@@ -38554,33 +38554,33 @@
             "condition_keys": [],
             "description": "Grants permission to validates if the s3 bucket exists with appropriate permissions for CUR delivery",
             "orphan": false,
             "resources": []
         }
     },
     "customer-verification": {
-        "UpdateCustomerVerificationDetails": {
+        "GetCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "UpdateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
             "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationDetails": {
+        "UpdateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationDetails",
+            "action": "UpdateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetCustomerVerificationEligibility": {
             "access_level": "Undocumented",
@@ -40272,1065 +40272,1065 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "UpdateEnvironmentBlueprint": {
+        "DeleteProjectMembership": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentBlueprint",
+            "action": "DeleteProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentBlueprint": {
+        "StartDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentBlueprint",
+            "action": "StartDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjectMemberships": {
+        "ListNotifications": {
             "access_level": "Undocumented",
-            "action": "ListProjectMemberships",
+            "action": "ListNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMetadataGenerationRun": {
+        "CancelSubscription": {
             "access_level": "Undocumented",
-            "action": "StartMetadataGenerationRun",
+            "action": "CancelSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentDeploymentStatus": {
+        "UpdateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentDeploymentStatus",
+            "action": "UpdateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTimeSeriesDataPoints": {
+        "GetAssetType": {
             "access_level": "Undocumented",
-            "action": "ListTimeSeriesDataPoints",
+            "action": "GetAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroupProfile": {
+        "GetEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateGroupProfile",
+            "action": "GetEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWarehouseMetadata": {
+        "ListEnvironmentBlueprintConfigurationSummaries": {
             "access_level": "Undocumented",
-            "action": "ListWarehouseMetadata",
+            "action": "ListEnvironmentBlueprintConfigurationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionTarget": {
+        "CreateFormType": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionTarget",
+            "action": "CreateFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RefreshToken": {
+        "GetDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "RefreshToken",
+            "action": "GetDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "RejectPredictions": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "RejectPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ProvisionDomain": {
+        "GetSubscription": {
             "access_level": "Undocumented",
-            "action": "ProvisionDomain",
+            "action": "GetSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "CreateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "CreateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossary": {
+        "GetEnvironmentCredentials": {
             "access_level": "Undocumented",
-            "action": "GetGlossary",
+            "action": "GetEnvironmentCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchUserProfiles": {
+        "ListPolicyGrants": {
             "access_level": "Undocumented",
-            "action": "SearchUserProfiles",
+            "action": "ListPolicyGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProjectMembership": {
+        "GetTimeSeriesDataPoint": {
             "access_level": "Undocumented",
-            "action": "DeleteProjectMembership",
+            "action": "GetTimeSeriesDataPoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionRequestDetails": {
+        "DeleteEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionRequestDetails",
+            "action": "DeleteEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionGrant": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionGrant",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroupProfile": {
+        "ListAssetRevisions": {
             "access_level": "Undocumented",
-            "action": "UpdateGroupProfile",
+            "action": "ListAssetRevisions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "ListProjectMemberships": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "ListProjectMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemovePolicyGrant": {
+        "ListDataSourceRunActivities": {
             "access_level": "Undocumented",
-            "action": "RemovePolicyGrant",
+            "action": "ListDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRuns": {
+        "GetGlossary": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRuns",
+            "action": "GetGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "CreateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "CreateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionTargets": {
+        "DeleteSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionTargets",
+            "action": "DeleteSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Search": {
+        "GetAsset": {
             "access_level": "Undocumented",
-            "action": "Search",
+            "action": "GetAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossaryTerm": {
+        "GetDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossaryTerm",
+            "action": "GetDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataGenerationRun": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "GetMetadataGenerationRun",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprintConfiguration": {
+        "UpdateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprintConfiguration",
+            "action": "UpdateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchListings": {
+        "GetFormType": {
             "access_level": "Undocumented",
-            "action": "SearchListings",
+            "action": "GetFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceRun": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceRun",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionRequests": {
+        "ListSubscriptionTargets": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionRequests",
+            "action": "ListSubscriptionTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAsset": {
+        "UpdateGlossary": {
             "access_level": "Undocumented",
-            "action": "DeleteAsset",
+            "action": "UpdateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "DeleteSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "DeleteSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossary": {
+        "SsoLogin": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossary",
+            "action": "SsoLogin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprint": {
+        "UpdateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprint",
+            "action": "UpdateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "PostTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "PostTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFormType": {
+        "CreateAsset": {
             "access_level": "Undocumented",
-            "action": "GetFormType",
+            "action": "CreateAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDomain": {
+        "GetEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreateDomain",
+            "action": "GetEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDomains": {
             "access_level": "Undocumented",
             "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionRequest": {
+        "DeleteProject": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionRequest",
+            "action": "DeleteProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePassRole": {
+        "RemovePolicyGrant": {
             "access_level": "Undocumented",
-            "action": "ValidatePassRole",
+            "action": "RemovePolicyGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTypes": {
+        "DeleteAssetType": {
             "access_level": "Undocumented",
-            "action": "SearchTypes",
+            "action": "DeleteAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionGrant": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionGrant",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDomain": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "UpdateDomain",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionRequest": {
+        "CreateAssetType": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionRequest",
+            "action": "CreateAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceRun": {
+        "GetSubscriptionEligibility": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceRun",
+            "action": "GetSubscriptionEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossary": {
+        "DeleteAsset": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossary",
+            "action": "DeleteAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogin": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "SsoLogin",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogout": {
+        "DeleteGlossary": {
             "access_level": "Undocumented",
-            "action": "SsoLogout",
+            "action": "DeleteGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptPredictions": {
+        "ListSubscriptionRequests": {
             "access_level": "Undocumented",
-            "action": "AcceptPredictions",
+            "action": "ListSubscriptionRequests",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAccountEnvironments": {
             "access_level": "Undocumented",
             "action": "ListAccountEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFormType": {
+        "SearchTypes": {
             "access_level": "Undocumented",
-            "action": "CreateFormType",
+            "action": "SearchTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUserProfile": {
+        "AddPolicyGrant": {
             "access_level": "Undocumented",
-            "action": "CreateUserProfile",
+            "action": "AddPolicyGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionGrants": {
+        "DeleteGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionGrants",
+            "action": "DeleteGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionRequest": {
+        "GetMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionRequest",
+            "action": "GetMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptSubscriptionRequest": {
+        "DeleteEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "AcceptSubscriptionRequest",
+            "action": "DeleteEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossary": {
+        "DeleteListing": {
             "access_level": "Undocumented",
-            "action": "CreateGlossary",
+            "action": "DeleteListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetListing": {
+        "GetEnvironmentActionLink": {
             "access_level": "Undocumented",
-            "action": "GetListing",
+            "action": "GetEnvironmentActionLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionGrant": {
+        "GetSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionGrant",
+            "action": "GetSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomain": {
+        "GetIamPortalLoginUrl": {
             "access_level": "Undocumented",
-            "action": "DeleteDomain",
+            "action": "GetIamPortalLoginUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentProfile": {
+        "DeleteDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentProfile",
+            "action": "DeleteDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateProjectMembership": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRunActivities": {
+        "ListEnvironmentProfiles": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRunActivities",
+            "action": "ListEnvironmentProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotifications": {
+        "PutEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNotifications",
+            "action": "PutEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTimeSeriesDataPoints": {
+        "CreateListingChangeSet": {
             "access_level": "Undocumented",
-            "action": "DeleteTimeSeriesDataPoints",
+            "action": "CreateListingChangeSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetType": {
+        "SearchListings": {
             "access_level": "Undocumented",
-            "action": "GetAssetType",
+            "action": "SearchListings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetRevision": {
+        "AcceptSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "CreateAssetRevision",
+            "action": "AcceptSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProject": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "CreateProject",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProject": {
+        "GetEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteProject",
+            "action": "GetEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectPredictions": {
+        "ListEnvironmentBlueprintConfigurations": {
             "access_level": "Undocumented",
-            "action": "RejectPredictions",
+            "action": "ListEnvironmentBlueprintConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentProfile": {
+        "GetUserProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentProfile",
+            "action": "GetUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentActionLink": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentActionLink",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupProfile": {
+        "GetSubscriptionRequestDetails": {
             "access_level": "Undocumented",
-            "action": "GetGroupProfile",
+            "action": "GetSubscriptionRequestDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprint": {
+        "CreateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprint",
+            "action": "CreateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurationSummaries": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurationSummaries",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataGenerationRuns": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "ListMetadataGenerationRuns",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSubscription": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "CancelSubscription",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprints": {
+        "ValidatePassRole": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprints",
+            "action": "ValidatePassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUserProfile": {
+        "DeleteDomain": {
             "access_level": "Undocumented",
-            "action": "UpdateUserProfile",
+            "action": "DeleteDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetGlossaryTerm": {
             "access_level": "Undocumented",
             "action": "GetGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentProfile": {
+        "ListSubscriptions": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentProfile",
+            "action": "ListSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscription": {
+        "UpdateProject": {
             "access_level": "Undocumented",
-            "action": "GetSubscription",
+            "action": "UpdateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionTarget": {
+        "CreateAssetRevision": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionTarget",
+            "action": "CreateAssetRevision",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProject": {
+        "GetListing": {
             "access_level": "Undocumented",
-            "action": "UpdateProject",
+            "action": "GetListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchGroupProfiles": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "SearchGroupProfiles",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "ListTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "ListTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDomainSharingPolicy": {
+        "CreateGlossary": {
             "access_level": "Undocumented",
-            "action": "PutDomainSharingPolicy",
+            "action": "CreateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAsset": {
+        "DeleteSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "GetAsset",
+            "action": "DeleteSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssetRevisions": {
+        "ListSubscriptionGrants": {
             "access_level": "Undocumented",
-            "action": "ListAssetRevisions",
+            "action": "ListSubscriptionGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionEligibility": {
+        "DeleteEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionEligibility",
+            "action": "DeleteEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "CreateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "CreateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSourceRunActivities": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSourceRunActivities",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentCredentials": {
+        "UpdateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentCredentials",
+            "action": "UpdateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMetadataGenerationRun": {
+        "UpdateUserProfile": {
             "access_level": "Undocumented",
-            "action": "CancelMetadataGenerationRun",
+            "action": "UpdateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "GetSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "GetSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurations": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurations",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionGrantStatus": {
+        "StartMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionGrantStatus",
+            "action": "StartMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentConfiguration": {
+        "UpdateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentConfiguration",
+            "action": "UpdateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentProfile": {
+        "DeleteTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentProfile",
+            "action": "DeleteTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListing": {
+        "PutDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteListing",
+            "action": "PutDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFormType": {
+        "SearchUserProfiles": {
             "access_level": "Undocumented",
-            "action": "DeleteFormType",
+            "action": "SearchUserProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossaryTerm": {
+        "SsoLogout": {
             "access_level": "Undocumented",
-            "action": "CreateGlossaryTerm",
+            "action": "SsoLogout",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "CreateProject": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "CreateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptions": {
+        "ListWarehouseMetadata": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptions",
+            "action": "ListWarehouseMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopMetadataGenerationRun": {
+        "ProvisionDomain": {
             "access_level": "Undocumented",
-            "action": "StopMetadataGenerationRun",
+            "action": "ProvisionDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "UpdateDomain": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "UpdateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprintConfiguration": {
+        "RejectSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprintConfiguration",
+            "action": "RejectSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyGrants": {
+        "ListMetadataGenerationRuns": {
             "access_level": "Undocumented",
-            "action": "ListPolicyGrants",
+            "action": "ListMetadataGenerationRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionTarget": {
+        "CreateUserProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionTarget",
+            "action": "CreateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyGrant": {
+        "UpdateEnvironmentConfiguration": {
             "access_level": "Undocumented",
-            "action": "AddPolicyGrant",
+            "action": "UpdateEnvironmentConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentProfiles": {
+        "CreateSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentProfiles",
+            "action": "CreateSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectSubscriptionRequest": {
+        "StopMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "RejectSubscriptionRequest",
+            "action": "StopMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAsset": {
+        "GetGroupProfile": {
             "access_level": "Undocumented",
-            "action": "CreateAsset",
+            "action": "GetGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssetType": {
+        "ListDataSourceRuns": {
             "access_level": "Undocumented",
-            "action": "DeleteAssetType",
+            "action": "ListDataSourceRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomainSharingPolicy": {
+        "RevokeSubscription": {
             "access_level": "Undocumented",
-            "action": "DeleteDomainSharingPolicy",
+            "action": "RevokeSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RevokeSubscription": {
+        "AcceptPredictions": {
             "access_level": "Undocumented",
-            "action": "RevokeSubscription",
+            "action": "AcceptPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PostTimeSeriesDataPoints": {
+        "RefreshToken": {
             "access_level": "Undocumented",
-            "action": "PostTimeSeriesDataPoints",
+            "action": "RefreshToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionTarget": {
+        "UpdateDataSourceRunActivities": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionTarget",
+            "action": "UpdateDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "DeleteFormType": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "DeleteFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIamPortalLoginUrl": {
+        "UpdateEnvironmentDeploymentStatus": {
             "access_level": "Undocumented",
-            "action": "GetIamPortalLoginUrl",
+            "action": "UpdateEnvironmentDeploymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTimeSeriesDataPoint": {
+        "CreateDomain": {
             "access_level": "Undocumented",
-            "action": "GetTimeSeriesDataPoint",
+            "action": "CreateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserProfile": {
+        "CreateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "GetUserProfile",
+            "action": "CreateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "CancelMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "CancelMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossaryTerm": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossaryTerm",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProjectMembership": {
+        "SearchGroupProfiles": {
             "access_level": "Undocumented",
-            "action": "CreateProjectMembership",
+            "action": "SearchGroupProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListingChangeSet": {
+        "UpdateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "CreateListingChangeSet",
+            "action": "UpdateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomainSharingPolicy": {
+        "ListEnvironmentBlueprints": {
             "access_level": "Undocumented",
-            "action": "GetDomainSharingPolicy",
+            "action": "ListEnvironmentBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "UpdateSubscriptionGrantStatus": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "UpdateSubscriptionGrantStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetType": {
+        "Search": {
             "access_level": "Undocumented",
-            "action": "CreateAssetType",
+            "action": "Search",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutEnvironmentBlueprintConfiguration": {
+        "CreateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "PutEnvironmentBlueprintConfiguration",
+            "action": "CreateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -41724,833 +41724,833 @@
             "condition_keys": [],
             "description": "Grants permission to update query tab",
             "orphan": false,
             "resources": []
         }
     },
     "deadline": {
-        "DeleteWorker": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "DeleteWorker",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLicenseEndpoint": {
+        "DisassociateMemberFromFarm": {
             "access_level": "Undocumented",
-            "action": "DeleteLicenseEndpoint",
+            "action": "DisassociateMemberFromFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFarm": {
+        "ListFleets": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFarm",
+            "action": "ListFleets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionActions": {
+        "AssumeFleetRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "ListSessionActions",
+            "action": "AssumeFleetRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetQueue": {
             "access_level": "Undocumented",
             "action": "GetQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueFleetAssociation": {
+        "ListStorageProfilesForQueue": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueFleetAssociation",
+            "action": "ListStorageProfilesForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetJob": {
+        "CreateQueue": {
             "access_level": "Undocumented",
-            "action": "GetJob",
+            "action": "CreateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSessionsStatisticsAggregation": {
+        "CreateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "StartSessionsStatisticsAggregation",
+            "action": "CreateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForRead": {
+        "ListTasks": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForRead",
+            "action": "ListTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStorageProfile": {
+        "UpdateStep": {
             "access_level": "Undocumented",
-            "action": "CreateStorageProfile",
+            "action": "UpdateStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorker": {
+        "CreateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateWorker",
+            "action": "CreateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueEnvironment": {
+        "ListStepConsumers": {
             "access_level": "Undocumented",
-            "action": "CreateQueueEnvironment",
+            "action": "ListStepConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarms": {
+        "GetJob": {
             "access_level": "Undocumented",
-            "action": "ListFarms",
+            "action": "GetJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFarm": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFarm",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWorkers": {
+        "UpdateQueue": {
             "access_level": "Undocumented",
-            "action": "SearchWorkers",
+            "action": "UpdateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicenseEndpoint": {
+        "UpdateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateLicenseEndpoint",
+            "action": "UpdateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateJob": {
+        "GetFleet": {
             "access_level": "Undocumented",
-            "action": "UpdateJob",
+            "action": "GetFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "CopyJobTemplate": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "CopyJobTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFarm": {
+        "DeleteQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateFarm",
+            "action": "DeleteQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorker": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetWorker",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplicationVersion": {
+        "GetSessionAction": {
             "access_level": "Undocumented",
-            "action": "GetApplicationVersion",
+            "action": "GetSessionAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateBudget": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionsStatisticsAggregation": {
+        "BatchGetJobEntity": {
             "access_level": "Undocumented",
-            "action": "GetSessionsStatisticsAggregation",
+            "action": "BatchGetJobEntity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSteps": {
+        "DisassociateMemberFromJob": {
             "access_level": "Undocumented",
-            "action": "SearchSteps",
+            "action": "DisassociateMemberFromJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueFleetAssociations": {
+        "CreateJob": {
             "access_level": "Undocumented",
-            "action": "ListQueueFleetAssociations",
+            "action": "CreateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "ListJobMembers": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "ListJobMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFleet": {
+        "ListSessionActions": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFleet",
+            "action": "ListSessionActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarmMembers": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListFarmMembers",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTask": {
+        "AssumeQueueRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "GetTask",
+            "action": "AssumeQueueRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFleet": {
+        "DisassociateMemberFromQueue": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFleet",
+            "action": "DisassociateMemberFromQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueFleetAssociation": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "GetQueueFleetAssociation",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "GetApplicationVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "GetApplicationVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueue": {
+        "CreateLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "CreateQueue",
+            "action": "CreateLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "StartSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "StartSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAvailableMeteredProducts": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListAvailableMeteredProducts",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueEnvironment": {
+        "ListFarms": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueEnvironment",
+            "action": "ListFarms",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFleet": {
+        "AssociateMemberToQueue": {
             "access_level": "Undocumented",
-            "action": "DeleteFleet",
+            "action": "AssociateMemberToQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStep": {
+        "GetQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateStep",
+            "action": "GetQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyJobTemplate": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "CopyJobTemplate",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromQueue": {
+        "GetStorageProfile": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromQueue",
+            "action": "GetStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForRead": {
+        "GetWorker": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForRead",
+            "action": "GetWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfile": {
+        "UpdateWorker": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfile",
+            "action": "UpdateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepDependencies": {
+        "ListQueueFleetAssociations": {
             "access_level": "Undocumented",
-            "action": "ListStepDependencies",
+            "action": "ListQueueFleetAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMeteredProduct": {
+        "ListSessionsForWorker": {
             "access_level": "Undocumented",
-            "action": "PutMeteredProduct",
+            "action": "ListSessionsForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueues": {
+        "ListBudgets": {
             "access_level": "Undocumented",
-            "action": "ListQueues",
+            "action": "ListBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobMembers": {
+        "AssumeQueueRoleForRead": {
             "access_level": "Undocumented",
-            "action": "ListJobMembers",
+            "action": "AssumeQueueRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueEnvironment": {
+        "ListJobs": {
             "access_level": "Undocumented",
-            "action": "GetQueueEnvironment",
+            "action": "ListJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetJobEntity": {
+        "AssumeFleetRoleForRead": {
             "access_level": "Undocumented",
-            "action": "BatchGetJobEntity",
+            "action": "AssumeFleetRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueEnvironments": {
+        "DeleteMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "ListQueueEnvironments",
+            "action": "DeleteMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueMembers": {
+        "AssociateMemberToJob": {
             "access_level": "Undocumented",
-            "action": "ListQueueMembers",
+            "action": "AssociateMemberToJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchJobs": {
+        "AssumeQueueRoleForUser": {
             "access_level": "Undocumented",
-            "action": "SearchJobs",
+            "action": "AssumeQueueRoleForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFleet": {
+        "AssociateMemberToFarm": {
             "access_level": "Undocumented",
-            "action": "CreateFleet",
+            "action": "AssociateMemberToFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTasks": {
+        "UpdateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "SearchTasks",
+            "action": "UpdateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobs": {
+        "DisassociateMemberFromFleet": {
             "access_level": "Undocumented",
-            "action": "ListJobs",
+            "action": "DisassociateMemberFromFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateBudget": {
             "access_level": "Undocumented",
             "action": "UpdateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfilesForQueue": {
+        "UpdateFarm": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfilesForQueue",
+            "action": "UpdateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "SearchTasks": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "SearchTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTask": {
+        "GetQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateTask",
+            "action": "GetQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMonitor": {
+        "ListStepDependencies": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "ListStepDependencies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueFleetAssociation": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueFleetAssociation",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicenseEndpoint": {
+        "CreateFleet": {
             "access_level": "Undocumented",
-            "action": "GetLicenseEndpoint",
+            "action": "CreateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfileForQueue": {
+        "AssociateMemberToFleet": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfileForQueue",
+            "action": "AssociateMemberToFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFleet": {
+        "GetStorageProfileForQueue": {
             "access_level": "Undocumented",
-            "action": "UpdateFleet",
+            "action": "GetStorageProfileForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueue": {
+        "UpdateTask": {
             "access_level": "Undocumented",
-            "action": "DeleteQueue",
+            "action": "UpdateTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessions": {
+        "UpdateWorkerSchedule": {
             "access_level": "Undocumented",
-            "action": "ListSessions",
+            "action": "UpdateWorkerSchedule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForUser": {
+        "GetTask": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForUser",
+            "action": "GetTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueEnvironment": {
+        "CreateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueEnvironment",
+            "action": "CreateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLicenseEndpoints": {
+        "PutMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "ListLicenseEndpoints",
+            "action": "PutMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFarm": {
+        "UpdateJob": {
             "access_level": "Undocumented",
-            "action": "DeleteFarm",
+            "action": "UpdateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBudgets": {
+        "ListQueueMembers": {
             "access_level": "Undocumented",
-            "action": "ListBudgets",
+            "action": "ListQueueMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForWorker": {
+        "CreateWorker": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForWorker",
+            "action": "CreateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMeteredProducts": {
+        "CreateFarm": {
             "access_level": "Undocumented",
-            "action": "ListMeteredProducts",
+            "action": "CreateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSteps": {
+        "UpdateFleet": {
             "access_level": "Undocumented",
-            "action": "ListSteps",
+            "action": "UpdateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFarm": {
+        "ListAvailableMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "CreateFarm",
+            "action": "ListAvailableMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleets": {
+        "DeleteLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListFleets",
+            "action": "DeleteLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFleet": {
+        "ListQueues": {
             "access_level": "Undocumented",
-            "action": "GetFleet",
+            "action": "ListQueues",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "DeleteFarm": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "DeleteFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepConsumers": {
+        "GetSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "ListStepConsumers",
+            "action": "GetSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStep": {
+        "ListFarmMembers": {
             "access_level": "Undocumented",
-            "action": "GetStep",
+            "action": "ListFarmMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromJob": {
+        "GetLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromJob",
+            "action": "GetLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStorageProfile": {
+        "ListSteps": {
             "access_level": "Undocumented",
-            "action": "DeleteStorageProfile",
+            "action": "ListSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueFleetAssociation": {
+        "DeleteBudget": {
             "access_level": "Undocumented",
-            "action": "CreateQueueFleetAssociation",
+            "action": "DeleteBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForWorker": {
+        "DeleteQueue": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForWorker",
+            "action": "DeleteQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateJob": {
+        "UpdateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateJob",
+            "action": "UpdateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFarm": {
+        "ListSessions": {
             "access_level": "Undocumented",
-            "action": "GetFarm",
+            "action": "ListSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionsForWorker": {
+        "GetMonitor": {
             "access_level": "Undocumented",
-            "action": "ListSessionsForWorker",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "GetStep": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "GetStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBudget": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "DeleteBudget",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetBudget": {
             "access_level": "Undocumented",
             "action": "GetBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfiles": {
+        "ListFleetMembers": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfiles",
+            "action": "ListFleetMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueue": {
+        "SearchJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateQueue",
+            "action": "SearchJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMeteredProduct": {
+        "SearchSteps": {
             "access_level": "Undocumented",
-            "action": "DeleteMeteredProduct",
+            "action": "SearchSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBudget": {
+        "DeleteFleet": {
             "access_level": "Undocumented",
-            "action": "CreateBudget",
+            "action": "DeleteFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStorageProfile": {
+        "ListLicenseEndpoints": {
             "access_level": "Undocumented",
-            "action": "UpdateStorageProfile",
+            "action": "ListLicenseEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleetMembers": {
+        "DeleteQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "ListFleetMembers",
+            "action": "DeleteQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorker": {
+        "GetFarm": {
             "access_level": "Undocumented",
-            "action": "CreateWorker",
+            "action": "GetFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToJob": {
+        "DeleteWorker": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToJob",
+            "action": "DeleteWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkerSchedule": {
+        "DeleteStorageProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkerSchedule",
+            "action": "DeleteStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkers": {
+        "ListMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "ListWorkers",
+            "action": "ListMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToQueue": {
+        "ListQueueEnvironments": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToQueue",
+            "action": "ListQueueEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTasks": {
+        "ListStorageProfiles": {
             "access_level": "Undocumented",
-            "action": "ListTasks",
+            "action": "ListStorageProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionAction": {
+        "ListWorkers": {
             "access_level": "Undocumented",
-            "action": "GetSessionAction",
+            "action": "ListWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "SearchWorkers": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "SearchWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "deepcomposer": {
@@ -65131,305 +65131,305 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "DescribeTrustStoreAssociations": {
+        "DeleteTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreAssociations",
+            "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroup": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroup",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "DeleteTrustStore": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "DeleteTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyListener": {
+        "DescribeTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "ModifyListener",
+            "action": "DescribeTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRule": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "GetTrustStoreCaCertificatesBundle": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "GetTrustStoreCaCertificatesBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreCaCertificatesBundle": {
+        "RemoveListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreCaCertificatesBundle",
+            "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTrustStoreRevocations": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "AddTrustStoreRevocations",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetGroup": {
+        "CreateTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetGroup",
+            "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrustStore": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DeleteTrustStore",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "RemoveTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "RemoveTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "ModifyTrustStore": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "ModifyTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreRevocationContent": {
+        "CreateTrustStore": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreRevocationContent",
+            "action": "CreateTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveListenerCertificates": {
+        "DescribeTrustStoreAssociations": {
             "access_level": "Undocumented",
-            "action": "RemoveListenerCertificates",
+            "action": "DescribeTrustStoreAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSubnets": {
+        "DescribeTrustStores": {
             "access_level": "Undocumented",
-            "action": "SetSubnets",
+            "action": "DescribeTrustStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreRevocations": {
+        "ModifyListener": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreRevocations",
+            "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTrustStore": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "ModifyTrustStore",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroupAttributes": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroupAttributes",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "SetSubnets": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTrustStoreRevocations": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "RemoveTrustStoreRevocations",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroupAttributes": {
+        "GetTrustStoreRevocationContent": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "GetTrustStoreRevocationContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "AddTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "AddTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterTargets": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "RegisterTargets",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "ModifyTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetGroup": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "CreateTargetGroup",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrustStore": {
+        "RegisterTargets": {
             "access_level": "Undocumented",
-            "action": "CreateTrustStore",
+            "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStores": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStores",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -67130,305 +67130,305 @@
             "orphan": false,
             "resources": [
                 "application"
             ]
         }
     },
     "entityresolution": {
-        "DeleteSchemaMapping": {
+        "CreateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteSchemaMapping",
+            "action": "CreateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaMapping": {
+        "ListIdMappingWorkflows": {
             "access_level": "Undocumented",
-            "action": "GetSchemaMapping",
+            "action": "ListIdMappingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIdMappingJob": {
+        "AddPolicyStatement": {
             "access_level": "Undocumented",
-            "action": "StartIdMappingJob",
+            "action": "AddPolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseIdNamespace": {
+        "StartIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "UseIdNamespace",
+            "action": "StartIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchId": {
+        "UpdateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "GetMatchId",
+            "action": "UpdateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdNamespace": {
+        "ListSchemaMappings": {
             "access_level": "Undocumented",
-            "action": "GetIdNamespace",
+            "action": "ListSchemaMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProviderService": {
+        "ListMatchingJobs": {
             "access_level": "Undocumented",
-            "action": "GetProviderService",
+            "action": "ListMatchingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProviderServices": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "ListProviderServices",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingWorkflow": {
+        "DeleteIdNamespace": {
             "access_level": "Undocumented",
-            "action": "GetMatchingWorkflow",
+            "action": "DeleteIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPolicy": {
+        "GetProviderService": {
             "access_level": "Undocumented",
-            "action": "PutPolicy",
+            "action": "GetProviderService",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdMappingWorkflow": {
+        "StartMatchingJob": {
             "access_level": "Undocumented",
-            "action": "UpdateIdMappingWorkflow",
+            "action": "StartMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingJob": {
+        "GetMatchId": {
             "access_level": "Undocumented",
-            "action": "GetMatchingJob",
+            "action": "GetMatchId",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyStatement": {
+        "CreateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "AddPolicyStatement",
+            "action": "CreateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdMappingWorkflow": {
+        "ListIdNamespaces": {
             "access_level": "Undocumented",
-            "action": "CreateIdMappingWorkflow",
+            "action": "ListIdNamespaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemaMappings": {
+        "ListIdMappingJobs": {
             "access_level": "Undocumented",
-            "action": "ListSchemaMappings",
+            "action": "ListIdMappingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingWorkflows": {
+        "UpdateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListMatchingWorkflows",
+            "action": "UpdateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMatchingWorkflow": {
+        "GetIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "CreateMatchingWorkflow",
+            "action": "GetIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdNamespace": {
+        "ListProviderServices": {
             "access_level": "Undocumented",
-            "action": "UpdateIdNamespace",
+            "action": "ListProviderServices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMatchingWorkflow": {
+        "CreateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteMatchingWorkflow",
+            "action": "CreateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSchemaMapping": {
+        "GetMatchingJob": {
             "access_level": "Undocumented",
-            "action": "UpdateSchemaMapping",
+            "action": "GetMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingJobs": {
+        "UpdateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingJobs",
+            "action": "UpdateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdMappingWorkflow": {
+        "DeleteSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "DeleteIdMappingWorkflow",
+            "action": "DeleteSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingWorkflow": {
+        "GetIdNamespace": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingWorkflow",
+            "action": "GetIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSchemaMapping": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateSchemaMapping",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingWorkflows": {
+        "DeleteIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingWorkflows",
+            "action": "DeleteIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMatchingJob": {
+        "UseIdNamespace": {
             "access_level": "Undocumented",
-            "action": "StartMatchingJob",
+            "action": "UseIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStatement": {
+        "GetSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStatement",
+            "action": "GetSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMatchingWorkflow": {
+        "PutPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateMatchingWorkflow",
+            "action": "PutPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdNamespace": {
+        "DeleteMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteIdNamespace",
+            "action": "DeleteMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "UpdateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "UpdateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdNamespace": {
+        "CreateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "CreateIdNamespace",
+            "action": "CreateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingJobs": {
+        "ListMatchingWorkflows": {
             "access_level": "Undocumented",
-            "action": "ListMatchingJobs",
+            "action": "ListMatchingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdNamespaces": {
+        "DeletePolicyStatement": {
             "access_level": "Undocumented",
-            "action": "ListIdNamespaces",
+            "action": "DeletePolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "es": {
@@ -70159,229 +70159,229 @@
             "orphan": false,
             "resources": [
                 "deliverystream"
             ]
         }
     },
     "fis": {
-        "DeleteTargetAccountConfiguration": {
-            "access_level": "Undocumented",
-            "action": "DeleteTargetAccountConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "GetExperimentTargetAccountConfiguration": {
+        "ListExperiments": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTargetAccountConfiguration",
+            "action": "ListExperiments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTargetAccountConfiguration": {
+        "GetTargetResourceType": {
             "access_level": "Undocumented",
-            "action": "UpdateTargetAccountConfiguration",
+            "action": "GetTargetResourceType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetAccountConfigurations": {
+        "StartExperiment": {
             "access_level": "Undocumented",
-            "action": "ListTargetAccountConfigurations",
+            "action": "StartExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiInternalError": {
+        "GetExperimentTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "InjectApiInternalError",
+            "action": "GetExperimentTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperiments": {
+        "GetAction": {
             "access_level": "Undocumented",
-            "action": "ListExperiments",
+            "action": "GetAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExperiment": {
+        "GetTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartExperiment",
+            "action": "GetTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateExperimentTemplate": {
+        "CreateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateExperimentTemplate",
+            "action": "CreateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetResourceType": {
+        "ListTargetResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetTargetResourceType",
+            "action": "ListTargetResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperiment": {
+        "GetExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "GetExperiment",
+            "action": "GetExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentResolvedTargets": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListExperimentResolvedTargets",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListActions": {
+        "DeleteTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListActions",
+            "action": "DeleteTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateExperimentTemplate": {
             "access_level": "Undocumented",
             "action": "CreateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperimentTemplate": {
+        "ListTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTemplate",
+            "action": "ListTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiThrottleError": {
+        "InjectApiInternalError": {
             "access_level": "Undocumented",
-            "action": "InjectApiThrottleError",
+            "action": "InjectApiInternalError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTemplates": {
+        "DeleteExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTemplates",
+            "action": "DeleteExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetAccountConfiguration": {
+        "StopExperiment": {
             "access_level": "Undocumented",
-            "action": "GetTargetAccountConfiguration",
+            "action": "StopExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTargetAccountConfigurations": {
+        "GetExperiment": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTargetAccountConfigurations",
+            "action": "GetExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExperimentTemplate": {
+        "ListExperimentTemplates": {
             "access_level": "Undocumented",
-            "action": "DeleteExperimentTemplate",
+            "action": "ListExperimentTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetResourceTypes": {
+        "ListActions": {
             "access_level": "Undocumented",
-            "action": "ListTargetResourceTypes",
+            "action": "ListActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopExperiment": {
+        "UpdateExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "StopExperiment",
+            "action": "UpdateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "InjectApiUnavailableError": {
             "access_level": "Undocumented",
             "action": "InjectApiUnavailableError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetAccountConfiguration": {
+        "ListExperimentTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "CreateTargetAccountConfiguration",
+            "action": "ListExperimentTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAction": {
+        "ListExperimentResolvedTargets": {
             "access_level": "Undocumented",
-            "action": "GetAction",
+            "action": "ListExperimentResolvedTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
+        },
+        "InjectApiThrottleError": {
+            "access_level": "Undocumented",
+            "action": "InjectApiThrottleError",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "fms": {
         "AssociateAdminAccount": {
             "access_level": "Write",
             "action": "AssociateAdminAccount",
             "condition_keys": [],
@@ -72624,25 +72624,25 @@
             "access_level": "Undocumented",
             "action": "GetFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFreeTierAlertPreference": {
+        "GetFreeTierUsage": {
             "access_level": "Undocumented",
-            "action": "PutFreeTierAlertPreference",
+            "action": "GetFreeTierUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierUsage": {
+        "PutFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierUsage",
+            "action": "PutFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fsx": {
@@ -80893,177 +80893,177 @@
             "condition_keys": [],
             "description": "Grants permission to enable the Organizational View feature",
             "orphan": false,
             "resources": []
         }
     },
     "healthlake": {
-        "UpdateResource": {
+        "SearchWithPost": {
             "access_level": "Undocumented",
-            "action": "UpdateResource",
+            "action": "SearchWithPost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRImportJobs": {
+        "DeleteFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "ListFHIRImportJobs",
+            "action": "DeleteFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ReadResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ReadResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchEverything": {
+        "CreateResource": {
             "access_level": "Undocumented",
-            "action": "SearchEverything",
+            "action": "CreateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRDatastores": {
+        "DescribeFHIRImportJob": {
             "access_level": "Undocumented",
-            "action": "ListFHIRDatastores",
+            "action": "DescribeFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithPost": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "SearchWithPost",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRDatastore": {
+        "ListFHIRImportJobs": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRDatastore",
+            "action": "ListFHIRImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRImportJob": {
+        "UpdateResource": {
             "access_level": "Undocumented",
-            "action": "StartFHIRImportJob",
+            "action": "UpdateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFHIRDatastore": {
+        "StartFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteFHIRDatastore",
+            "action": "StartFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadResource": {
+        "SearchWithGet": {
             "access_level": "Undocumented",
-            "action": "ReadResource",
+            "action": "SearchWithGet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRImportJob": {
+        "StartFHIRImportJob": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRImportJob",
+            "action": "StartFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DescribeFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DescribeFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithGet": {
+        "ListFHIRExportJobs": {
             "access_level": "Undocumented",
-            "action": "SearchWithGet",
+            "action": "ListFHIRExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRExportJob": {
+        "CreateFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "StartFHIRExportJob",
+            "action": "CreateFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResource": {
+        "ListFHIRDatastores": {
             "access_level": "Undocumented",
-            "action": "CreateResource",
+            "action": "ListFHIRDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapabilities": {
+        "DescribeFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "GetCapabilities",
+            "action": "DescribeFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFHIRDatastore": {
+        "SearchEverything": {
             "access_level": "Undocumented",
-            "action": "CreateFHIRDatastore",
+            "action": "SearchEverything",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRExportJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRExportJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRExportJobs": {
+        "DeleteResource": {
             "access_level": "Undocumented",
-            "action": "ListFHIRExportJobs",
+            "action": "DeleteResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetCapabilities": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "honeycode": {
@@ -81329,1377 +81329,1377 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "TagServerCertificate": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccessKey": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagRole": {
             "access_level": "Undocumented",
             "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMFADevice": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "GetMFADevice",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "GetMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "GetMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -84940,25 +84940,25 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "PutInvoiceEmailDeliveryPreferences": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoiceEmailDeliveryPreferences": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListInvoiceSummaries": {
             "access_level": "Undocumented",
@@ -91139,913 +91139,913 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "ListMulticastGroups": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "UpdateMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "UpdateMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "GetMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "GetMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMetricConfiguration": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateMetricConfiguration",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricConfiguration": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetMetricConfiguration",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "GetMetrics": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "GetMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetrics": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetMetrics",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -95212,73 +95212,73 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "DescribeRescoreExecutionPlan": {
+        "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRescoreExecutionPlan": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteRescoreExecutionPlan",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRescoreExecutionPlans": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "ListRescoreExecutionPlans",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRescoreExecutionPlan": {
+        "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
@@ -95286,265 +95286,265 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "StopStreamEncryption": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RemoveTagsFromStream": {
             "access_level": "Undocumented",
             "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "GetResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "GetResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourcePolicy": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "DeleteResourcePolicy",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStream": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "CreateStream",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourcePolicy": {
+        "DeleteResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "PutResourcePolicy",
+            "action": "DeleteResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateShardCount": {
             "access_level": "Undocumented",
             "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "PutResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "PutResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicy": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicy",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -98214,273 +98214,273 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "GetDeployment": {
+        "ListResourceCostEstimates": {
             "access_level": "Undocumented",
-            "action": "GetDeployment",
+            "action": "ListResourceCostEstimates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceCostEstimates": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "ListResourceCostEstimates",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllowedResources": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListAllowedResources",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSettingsSet": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "PutSettingsSet",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSettingsSet": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkload": {
+        "ListDeployments": {
             "access_level": "Undocumented",
-            "action": "GetWorkload",
+            "action": "ListDeployments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceRecommendation": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "GetResourceRecommendation",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeployment": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "CreateDeployment",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIpAddress": {
+        "GetWorkload": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "GetWorkload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "GetSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "GetSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "DeleteDeployment": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "DeleteDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentPatterns": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentPatterns",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "GetResourceRecommendation": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "GetResourceRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeployments": {
+        "ListDeploymentEvents": {
             "access_level": "Undocumented",
-            "action": "ListDeployments",
+            "action": "ListDeploymentEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "GetDeployment": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "ListWorkloadDeploymentPatterns": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "ListWorkloadDeploymentPatterns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSettingsSet": {
+        "ListAllowedResources": {
             "access_level": "Undocumented",
-            "action": "GetSettingsSet",
+            "action": "ListAllowedResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeploymentEvents": {
+        "PutSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListDeploymentEvents",
+            "action": "PutSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeployment": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "DeleteDeployment",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "CreateDeployment": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "CreateDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "GetWorkloadAsset": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "GetWorkloadAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAsset": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAsset",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -105705,107 +105705,107 @@
             "orphan": false,
             "resources": [
                 "proposal"
             ]
         }
     },
     "managedblockchain-query": {
-        "ListTransactionEvents": {
+        "GetTransaction": {
             "access_level": "Undocumented",
-            "action": "ListTransactionEvents",
+            "action": "GetTransaction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetContract": {
+        "ListAssetContracts": {
             "access_level": "Undocumented",
-            "action": "GetAssetContract",
+            "action": "ListAssetContracts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetTokenBalance": {
+        "GetTokenBalance": {
             "access_level": "Undocumented",
-            "action": "BatchGetTokenBalance",
+            "action": "GetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTokenBalance": {
+        "BatchGetTokenBalance": {
             "access_level": "Undocumented",
-            "action": "GetTokenBalance",
+            "action": "BatchGetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransaction": {
+        "ListFilteredTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "GetTransaction",
+            "action": "ListFilteredTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFilteredTransactionEvents": {
+        "ListTokenBalances": {
             "access_level": "Undocumented",
-            "action": "ListFilteredTransactionEvents",
+            "action": "ListTokenBalances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTransactions": {
             "access_level": "Undocumented",
             "action": "ListTransactions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTokenBalances": {
+        "ListTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "ListTokenBalances",
+            "action": "ListTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssetContracts": {
+        "GetAssetContract": {
             "access_level": "Undocumented",
-            "action": "ListAssetContracts",
+            "action": "GetAssetContract",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mapcredits": {
-        "ListQuarterCredits": {
+        "ListQuarterSpend": {
             "access_level": "Undocumented",
-            "action": "ListQuarterCredits",
+            "action": "ListQuarterSpend",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuarterSpend": {
+        "ListAssociatedPrograms": {
             "access_level": "Undocumented",
-            "action": "ListQuarterSpend",
+            "action": "ListAssociatedPrograms",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssociatedPrograms": {
+        "ListQuarterCredits": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedPrograms",
+            "action": "ListQuarterCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "marketplacecommerceanalytics": {
@@ -108249,217 +108249,217 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "PutChannelPolicy": {
+        "CreateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "PutChannelPolicy",
+            "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelPolicy": {
+        "GetChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "GetChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpointPolicy": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpointPolicy",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHeadObject": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetHeadObject",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannel": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannelGroup": {
+        "GetHeadObject": {
             "access_level": "Undocumented",
-            "action": "UpdateChannelGroup",
+            "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateChannel": {
             "access_level": "Undocumented",
             "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "CreateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOriginEndpoint": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateOriginEndpoint",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListOriginEndpoints": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelGroup": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutOriginEndpointPolicy": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "PutOriginEndpointPolicy",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutObject": {
+        "PutChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "PutObject",
+            "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOriginEndpoints": {
+        "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "ListOriginEndpoints",
+            "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannelGroup": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "CreateChannelGroup",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannelGroups": {
+        "PutObject": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOriginEndpoint": {
+        "UpdateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "CreateOriginEndpoint",
+            "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannel": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
@@ -109185,161 +109185,161 @@
             "orphan": false,
             "resources": [
                 "vodSource"
             ]
         }
     },
     "medical-imaging": {
-        "UntagResource": {
+        "ListImageSetVersions": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListImageSetVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSetMetadata": {
+        "CopyImageSet": {
             "access_level": "Undocumented",
-            "action": "GetImageSetMetadata",
+            "action": "CopyImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImageSetVersions": {
+        "UpdateImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "ListImageSetVersions",
+            "action": "UpdateImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDatastore": {
+        "GetDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "CreateDatastore",
+            "action": "GetDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDICOMImportJob": {
+        "DeleteDatastore": {
             "access_level": "Undocumented",
-            "action": "StartDICOMImportJob",
+            "action": "DeleteDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImageSet": {
+        "GetImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "DeleteImageSet",
+            "action": "GetImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchImageSets": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "SearchImageSets",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDatastore": {
+        "DeleteImageSet": {
             "access_level": "Undocumented",
-            "action": "DeleteDatastore",
+            "action": "DeleteImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetDICOMInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetDICOMInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyImageSet": {
+        "GetDatastore": {
             "access_level": "Undocumented",
-            "action": "CopyImageSet",
+            "action": "GetDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageFrame": {
+        "GetImageSet": {
             "access_level": "Undocumented",
-            "action": "GetImageFrame",
+            "action": "GetImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDICOMInstance": {
+        "ListDICOMImportJobs": {
             "access_level": "Undocumented",
-            "action": "GetDICOMInstance",
+            "action": "ListDICOMImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSet": {
+        "StartDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "GetImageSet",
+            "action": "StartDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDICOMImportJob": {
+        "CreateDatastore": {
             "access_level": "Undocumented",
-            "action": "GetDICOMImportJob",
+            "action": "CreateDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDatastores": {
             "access_level": "Undocumented",
             "action": "ListDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDICOMImportJobs": {
+        "SearchImageSets": {
             "access_level": "Undocumented",
-            "action": "ListDICOMImportJobs",
+            "action": "SearchImageSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateImageSetMetadata": {
+        "GetImageFrame": {
             "access_level": "Undocumented",
-            "action": "UpdateImageSetMetadata",
+            "action": "GetImageFrame",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDatastore": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetDatastore",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "memorydb": {
@@ -113758,265 +113758,265 @@
             "orphan": false,
             "resources": [
                 "database"
             ]
         }
     },
     "neptune-graph": {
-        "GetImportTask": {
+        "GetEngineStatus": {
             "access_level": "Undocumented",
-            "action": "GetImportTask",
+            "action": "GetEngineStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueries": {
+        "GetStatisticsStatus": {
             "access_level": "Undocumented",
-            "action": "ListQueries",
+            "action": "GetStatisticsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraphSnapshot": {
+        "RestoreGraphFromSnapshot": {
             "access_level": "Undocumented",
-            "action": "DeleteGraphSnapshot",
+            "action": "RestoreGraphFromSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueryStatus": {
+        "DeleteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "GetQueryStatus",
+            "action": "DeleteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "WriteDataViaQuery": {
+        "DeletePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "WriteDataViaQuery",
+            "action": "DeletePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListGraphs": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListGraphs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraph": {
+        "DeleteGraph": {
             "access_level": "Undocumented",
-            "action": "CreateGraph",
+            "action": "DeleteGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelQuery": {
+        "ListImportTasks": {
             "access_level": "Undocumented",
-            "action": "CancelQuery",
+            "action": "ListImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivateGraphEndpoint": {
+        "WriteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "DeletePrivateGraphEndpoint",
+            "action": "WriteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphUsingImportTask": {
+        "CancelImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateGraphUsingImportTask",
+            "action": "CancelImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGraph": {
+        "CreateGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "UpdateGraph",
+            "action": "CreateGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraph": {
+        "ListGraphSnapshots": {
             "access_level": "Undocumented",
-            "action": "GetGraph",
+            "action": "ListGraphSnapshots",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSummary": {
+        "CreatePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetGraphSummary",
+            "action": "CreatePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateGraph": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEngineStatus": {
+        "CancelQuery": {
             "access_level": "Undocumented",
-            "action": "GetEngineStatus",
+            "action": "CancelQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivateGraphEndpoint": {
+        "DeleteGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "GetPrivateGraphEndpoint",
+            "action": "DeleteGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStatisticsStatus": {
+        "ListPrivateGraphEndpoints": {
             "access_level": "Undocumented",
-            "action": "GetStatisticsStatus",
+            "action": "ListPrivateGraphEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivateGraphEndpoints": {
+        "CreateGraphUsingImportTask": {
             "access_level": "Undocumented",
-            "action": "ListPrivateGraphEndpoints",
+            "action": "CreateGraphUsingImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataViaQuery": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDataViaQuery",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphs": {
+        "StartImportTask": {
             "access_level": "Undocumented",
-            "action": "ListGraphs",
+            "action": "StartImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreGraphFromSnapshot": {
+        "ReadDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "RestoreGraphFromSnapshot",
+            "action": "ReadDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportTask": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartImportTask",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraph": {
+        "GetGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "DeleteGraph",
+            "action": "GetGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphSnapshots": {
+        "GetQueryStatus": {
             "access_level": "Undocumented",
-            "action": "ListGraphSnapshots",
+            "action": "GetQueryStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetGraph": {
+        "GetImportTask": {
             "access_level": "Undocumented",
-            "action": "ResetGraph",
+            "action": "GetImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelImportTask": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CancelImportTask",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadDataViaQuery": {
+        "ListQueries": {
             "access_level": "Undocumented",
-            "action": "ReadDataViaQuery",
+            "action": "ListQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportTasks": {
+        "ResetGraph": {
             "access_level": "Undocumented",
-            "action": "ListImportTasks",
+            "action": "ResetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivateGraphEndpoint": {
+        "GetPrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "CreatePrivateGraphEndpoint",
+            "action": "GetPrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphSnapshot": {
+        "CreateGraph": {
             "access_level": "Undocumented",
-            "action": "CreateGraphSnapshot",
+            "action": "CreateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSnapshot": {
+        "GetGraph": {
             "access_level": "Undocumented",
-            "action": "GetGraphSnapshot",
+            "action": "GetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetGraphSummary": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetGraphSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "network-firewall": {
@@ -115383,163 +115383,163 @@
             "orphan": false,
             "resources": [
                 "attachment"
             ]
         }
     },
     "networkmanager-chat": {
-        "DeleteConversation": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "DeleteConversation",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMessageResponse": {
+        "DeleteConversation": {
             "access_level": "Undocumented",
-            "action": "CancelMessageResponse",
+            "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyConversationIsActive": {
+        "SendConversationMessage": {
             "access_level": "Undocumented",
-            "action": "NotifyConversationIsActive",
+            "action": "SendConversationMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "ListConversationMessages": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "ListConversationMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConversation": {
+        "NotifyConversationIsActive": {
             "access_level": "Undocumented",
-            "action": "CreateConversation",
+            "action": "NotifyConversationIsActive",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversationMessages": {
+        "CancelMessageResponse": {
             "access_level": "Undocumented",
-            "action": "ListConversationMessages",
+            "action": "CancelMessageResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendConversationMessage": {
+        "CreateConversation": {
             "access_level": "Undocumented",
-            "action": "SendConversationMessage",
+            "action": "CreateConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "networkmonitor": {
-        "GetMonitor": {
+        "CreateProbe": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "CreateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProbe": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "GetProbe",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetMonitor": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "UpdateProbe": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "UpdateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProbe": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "CreateProbe",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProbe": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "DeleteProbe",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetProbe": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProbe": {
+        "DeleteProbe": {
             "access_level": "Undocumented",
-            "action": "UpdateProbe",
+            "action": "DeleteProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "nimble": {
@@ -116107,251 +116107,251 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "RegisterNotificationHub": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventRule": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
             "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventRules": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationEvent": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "UntagResource": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SendActivationCode": {
             "access_level": "Undocumented",
             "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEmailContacts": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -116529,883 +116529,883 @@
             "orphan": false,
             "resources": [
                 "Link"
             ]
         }
     },
     "omics": {
-        "GetRunGroup": {
+        "ListVariantStores": {
             "access_level": "Undocumented",
-            "action": "GetRunGroup",
+            "action": "ListVariantStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStore": {
+        "CancelRun": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStore",
+            "action": "CancelRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceMetadata": {
+        "ListAnnotationImportJobs": {
             "access_level": "Undocumented",
-            "action": "GetReferenceMetadata",
+            "action": "ListAnnotationImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartVariantImportJob": {
+        "UpdateWorkflow": {
             "access_level": "Undocumented",
-            "action": "StartVariantImportJob",
+            "action": "UpdateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRunGroup": {
+        "DeleteReferenceStore": {
             "access_level": "Undocumented",
-            "action": "UpdateRunGroup",
+            "action": "DeleteReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStore": {
+        "BatchDeleteReadSet": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStore",
+            "action": "BatchDeleteReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantStores": {
+        "GetShare": {
             "access_level": "Undocumented",
-            "action": "ListVariantStores",
+            "action": "GetShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetMetadata": {
+        "CreateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "GetReadSetMetadata",
+            "action": "CreateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptShare": {
+        "CreateSequenceStore": {
             "access_level": "Undocumented",
-            "action": "AcceptShare",
+            "action": "CreateSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListReferenceImportJobs": {
             "access_level": "Undocumented",
             "action": "ListReferenceImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AbortMultipartReadSetUpload": {
+        "GetRunTask": {
             "access_level": "Undocumented",
-            "action": "AbortMultipartReadSetUpload",
+            "action": "GetRunTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRun": {
+        "UpdateRunGroup": {
             "access_level": "Undocumented",
-            "action": "StartRun",
+            "action": "UpdateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRuns": {
+        "GetSequenceStore": {
             "access_level": "Undocumented",
-            "action": "ListRuns",
+            "action": "GetSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetExportJob": {
+        "CreateMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "GetReadSetExportJob",
+            "action": "CreateMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceImportJob": {
+        "DeleteVariantStore": {
             "access_level": "Undocumented",
-            "action": "GetReferenceImportJob",
+            "action": "DeleteVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantImportJobs": {
+        "CompleteMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "ListVariantImportJobs",
+            "action": "CompleteMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantImportJob": {
+        "DeleteWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetVariantImportJob",
+            "action": "DeleteWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationImportJob": {
+        "CreateWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationImportJob",
+            "action": "CreateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSets": {
+        "DeleteShare": {
             "access_level": "Undocumented",
-            "action": "ListReadSets",
+            "action": "DeleteShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetImportJob": {
+        "GetReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "StartReadSetImportJob",
+            "action": "GetReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVariantStore": {
+        "DeleteAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "DeleteVariantStore",
+            "action": "DeleteAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteShare": {
+        "StartReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteShare",
+            "action": "StartReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRunGroup": {
+        "DeleteAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "DeleteRunGroup",
+            "action": "DeleteAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStoreVersion": {
+        "DeleteReference": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStoreVersion",
+            "action": "DeleteReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkflows": {
+        "ListReadSets": {
             "access_level": "Undocumented",
-            "action": "ListWorkflows",
+            "action": "ListReadSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStoreVersion": {
+        "GetReferenceMetadata": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStoreVersion",
+            "action": "GetReferenceMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSequenceStore": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSequenceStore",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateShare": {
+        "CreateReferenceStore": {
             "access_level": "Undocumented",
-            "action": "CreateShare",
+            "action": "CreateReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunGroups": {
+        "AcceptShare": {
             "access_level": "Undocumented",
-            "action": "ListRunGroups",
+            "action": "AcceptShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStore": {
+        "ListRunTasks": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStore",
+            "action": "ListRunTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetImportJobs": {
+        "DeleteRun": {
             "access_level": "Undocumented",
-            "action": "ListReadSetImportJobs",
+            "action": "DeleteRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetUploadParts": {
+        "GetRun": {
             "access_level": "Undocumented",
-            "action": "ListReadSetUploadParts",
+            "action": "GetRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReferenceImportJob": {
+        "DeleteRunGroup": {
             "access_level": "Undocumented",
-            "action": "StartReferenceImportJob",
+            "action": "DeleteRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStoreVersions": {
+        "GetWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStoreVersions",
+            "action": "GetWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReference": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteReference",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReference": {
+        "CreateRunGroup": {
             "access_level": "Undocumented",
-            "action": "GetReference",
+            "action": "CreateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRun": {
+        "ListMultipartReadSetUploads": {
             "access_level": "Undocumented",
-            "action": "GetRun",
+            "action": "ListMultipartReadSetUploads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CompleteMultipartReadSetUpload": {
+        "CreateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "CompleteMultipartReadSetUpload",
+            "action": "CreateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStore": {
+        "GetReferenceStore": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStore",
+            "action": "GetReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStores": {
+        "StartReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStores",
+            "action": "StartReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSet": {
+        "StartRun": {
             "access_level": "Undocumented",
-            "action": "GetReadSet",
+            "action": "StartRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShares": {
+        "GetReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "ListShares",
+            "action": "GetReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunTask": {
+        "ListReadSetExportJobs": {
             "access_level": "Undocumented",
-            "action": "GetRunTask",
+            "action": "ListReadSetExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSequenceStore": {
+        "GetAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "GetSequenceStore",
+            "action": "GetAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateVariantStore": {
+        "ListSequenceStores": {
             "access_level": "Undocumented",
-            "action": "UpdateVariantStore",
+            "action": "ListSequenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationImportJobs": {
+        "CreateVariantStore": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationImportJobs",
+            "action": "CreateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CancelAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CancelAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSequenceStores": {
+        "ListReferences": {
             "access_level": "Undocumented",
-            "action": "ListSequenceStores",
+            "action": "ListReferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceStore": {
+        "GetVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReferenceStore",
+            "action": "GetVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStoreVersion": {
+        "StartReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStoreVersion",
+            "action": "StartReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetActivationJobs": {
+        "UpdateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "ListReadSetActivationJobs",
+            "action": "UpdateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVariantStore": {
+        "DeleteSequenceStore": {
             "access_level": "Undocumented",
-            "action": "CreateVariantStore",
+            "action": "DeleteSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRunGroup": {
+        "UpdateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "CreateRunGroup",
+            "action": "UpdateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkflow": {
+        "GetReadSet": {
             "access_level": "Undocumented",
-            "action": "GetWorkflow",
+            "action": "GetReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStoreVersions": {
+        "GetReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStoreVersions",
+            "action": "GetReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorkflow": {
+        "GetAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "CreateWorkflow",
+            "action": "GetAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkflow": {
+        "StartAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkflow",
+            "action": "StartAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetActivationJob": {
+        "ListRuns": {
             "access_level": "Undocumented",
-            "action": "StartReadSetActivationJob",
+            "action": "ListRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAnnotationImportJob": {
+        "UpdateVariantStore": {
             "access_level": "Undocumented",
-            "action": "StartAnnotationImportJob",
+            "action": "UpdateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferences": {
+        "ListAnnotationStores": {
             "access_level": "Undocumented",
-            "action": "ListReferences",
+            "action": "ListAnnotationStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunTasks": {
+        "ListReadSetActivationJobs": {
             "access_level": "Undocumented",
-            "action": "ListRunTasks",
+            "action": "ListReadSetActivationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteReadSet": {
+        "ListVariantImportJobs": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteReadSet",
+            "action": "ListVariantImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceStores": {
+        "ListReadSetUploadParts": {
             "access_level": "Undocumented",
-            "action": "ListReferenceStores",
+            "action": "ListReadSetUploadParts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShare": {
+        "StartReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "GetShare",
+            "action": "StartReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelAnnotationImportJob": {
+        "ListRunGroups": {
             "access_level": "Undocumented",
-            "action": "CancelAnnotationImportJob",
+            "action": "ListRunGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetActivationJob": {
+        "CancelVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReadSetActivationJob",
+            "action": "CancelVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSequenceStore": {
+        "ListWorkflows": {
             "access_level": "Undocumented",
-            "action": "CreateSequenceStore",
+            "action": "ListWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorkflow": {
+        "GetReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteWorkflow",
+            "action": "GetReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReferenceStore": {
+        "AbortMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "DeleteReferenceStore",
+            "action": "AbortMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMultipartReadSetUpload": {
+        "GetVariantStore": {
             "access_level": "Undocumented",
-            "action": "CreateMultipartReadSetUpload",
+            "action": "GetVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelVariantImportJob": {
+        "ListReferenceStores": {
             "access_level": "Undocumented",
-            "action": "CancelVariantImportJob",
+            "action": "ListReferenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadReadSetPart": {
+        "GetReadSetMetadata": {
             "access_level": "Undocumented",
-            "action": "UploadReadSetPart",
+            "action": "GetReadSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMultipartReadSetUploads": {
+        "GetRunGroup": {
             "access_level": "Undocumented",
-            "action": "ListMultipartReadSetUploads",
+            "action": "GetRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateReferenceStore": {
+        "GetAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "CreateReferenceStore",
+            "action": "GetAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantStore": {
+        "StartVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "GetVariantStore",
+            "action": "StartVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetExportJob": {
+        "UploadReadSetPart": {
             "access_level": "Undocumented",
-            "action": "StartReadSetExportJob",
+            "action": "UploadReadSetPart",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelRun": {
+        "ListReadSetImportJobs": {
             "access_level": "Undocumented",
-            "action": "CancelRun",
+            "action": "ListReadSetImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetImportJob": {
+        "ListShares": {
             "access_level": "Undocumented",
-            "action": "GetReadSetImportJob",
+            "action": "ListShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRun": {
+        "CreateShare": {
             "access_level": "Undocumented",
-            "action": "DeleteRun",
+            "action": "CreateShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetExportJobs": {
+        "ListAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "ListReadSetExportJobs",
+            "action": "ListAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetReference": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "one": {
-        "DeleteAssociatedDevice": {
+        "DeleteSite": {
             "access_level": "Undocumented",
-            "action": "DeleteAssociatedDevice",
+            "action": "DeleteSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateDeviceInstance": {
             "access_level": "Undocumented",
             "action": "UpdateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListDeviceInstances": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListDeviceInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceInstance": {
+        "UpdateSiteAddress": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceInstance",
+            "action": "UpdateSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSiteAddress": {
+        "GetDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "GetSiteAddress",
+            "action": "GetDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstance": {
+        "CreateDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstance",
+            "action": "CreateDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstance": {
+        "DeleteAssociatedDevice": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstance",
+            "action": "DeleteAssociatedDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceConfigurationTemplates": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListDeviceConfigurationTemplates",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstanceConfiguration": {
+        "DeleteDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstanceConfiguration",
+            "action": "DeleteDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceInstances": {
+        "DeleteDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "ListDeviceInstances",
+            "action": "DeleteDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "GetDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "GetDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSite": {
+        "ListSites": {
             "access_level": "Undocumented",
-            "action": "GetSite",
+            "action": "ListSites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceConfigurationTemplate": {
+        "CreateDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "GetDeviceConfigurationTemplate",
+            "action": "CreateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSite": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateSite",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceConfigurationTemplate": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceConfigurationTemplate",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceActivationQrCode": {
+        "UpdateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceActivationQrCode",
+            "action": "UpdateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetSiteAddress": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSite": {
+        "RebootDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateSite",
+            "action": "RebootDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceConfigurationTemplate": {
+        "UpdateSite": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceConfigurationTemplate",
+            "action": "UpdateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstanceConfiguration": {
+        "CreateSite": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstanceConfiguration",
+            "action": "CreateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "CreateDeviceActivationQrCode": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "CreateDeviceActivationQrCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSite": {
+        "GetDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteSite",
+            "action": "GetDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSiteAddress": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "UpdateSiteAddress",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RebootDevice": {
+        "ListDeviceConfigurationTemplates": {
             "access_level": "Undocumented",
-            "action": "RebootDevice",
+            "action": "ListDeviceConfigurationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDeviceConfigurationTemplate": {
+        "GetSite": {
             "access_level": "Undocumented",
-            "action": "UpdateDeviceConfigurationTemplate",
+            "action": "GetSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSites": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListSites",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "opsworks": {
@@ -118878,129 +118878,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "UpdatePipeline": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Ingest": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPipeline": {
             "access_level": "Undocumented",
             "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePipeline": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePipeline": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelines": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelineBlueprints": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -119663,535 +119663,535 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "partnercentral-account-management": {
-        "AssociatePartnerAccount": {
+        "AssociatePartnerUser": {
             "access_level": "Undocumented",
-            "action": "AssociatePartnerAccount",
+            "action": "AssociatePartnerUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisassociatePartnerUser": {
             "access_level": "Undocumented",
             "action": "DisassociatePartnerUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociatePartnerUser": {
+        "AssociatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "AssociatePartnerUser",
+            "action": "AssociatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payment-cryptography": {
-        "ExportKey": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAlias": {
             "access_level": "Undocumented",
             "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "ListAliases": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyPinData": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "DeleteAlias": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "DeleteAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "CreateAlias": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TranslatePinData": {
             "access_level": "Undocumented",
             "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCardValidationData": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "GenerateCardValidationData",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAliases": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "ListAliases",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPublicKeyCertificate": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyMac": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "VerifyMac",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAlias": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "DeleteAlias",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAlias": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "CreateAlias",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "VerifyMac": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopKeyUsage": {
+        "GenerateCardValidationData": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "ListPaymentPreferences": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MakePayment": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePaymentInstrument": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "DeletePaymentInstrument",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePaymentPreferences": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentStatus": {
+        "DeletePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "GetPaymentStatus",
+            "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "GetPaymentStatus": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "pca-connector-ad": {
-        "UntagResource": {
+        "DeleteServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDirectoryRegistration": {
+        "DeleteConnector": {
             "access_level": "Undocumented",
-            "action": "CreateDirectoryRegistration",
+            "action": "DeleteConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplate": {
+        "CreateDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplate",
+            "action": "CreateDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplate": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateTemplate",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnector": {
+        "GetConnector": {
             "access_level": "Undocumented",
-            "action": "DeleteConnector",
+            "action": "GetConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTemplate": {
+        "CreateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplate",
+            "action": "CreateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTemplateGroupAccessControlEntry": {
+        "CreateTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplateGroupAccessControlEntry",
+            "action": "CreateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplates": {
+        "ListConnectors": {
             "access_level": "Undocumented",
-            "action": "ListTemplates",
+            "action": "ListConnectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnector": {
+        "CreateServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "CreateConnector",
+            "action": "CreateServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConnectors": {
+        "GetServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "ListConnectors",
+            "action": "GetServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplateGroupAccessControlEntry": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplateGroupAccessControlEntry",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplateGroupAccessControlEntries": {
+        "CreateConnector": {
             "access_level": "Undocumented",
-            "action": "ListTemplateGroupAccessControlEntries",
+            "action": "CreateConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDirectoryRegistration": {
+        "GetTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "DeleteDirectoryRegistration",
+            "action": "GetTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplate": {
+        "DeleteDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "GetTemplate",
+            "action": "DeleteDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListTemplateGroupAccessControlEntries": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListTemplateGroupAccessControlEntries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplateGroupAccessControlEntry": {
+        "GetDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "GetTemplateGroupAccessControlEntry",
+            "action": "GetDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDirectoryRegistrations": {
+        "ListServicePrincipalNames": {
             "access_level": "Undocumented",
-            "action": "ListDirectoryRegistrations",
+            "action": "ListServicePrincipalNames",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServicePrincipalName": {
+        "ListDirectoryRegistrations": {
             "access_level": "Undocumented",
-            "action": "DeleteServicePrincipalName",
+            "action": "ListDirectoryRegistrations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConnector": {
+        "DeleteTemplate": {
             "access_level": "Undocumented",
-            "action": "GetConnector",
+            "action": "DeleteTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplateGroupAccessControlEntry": {
+        "UpdateTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateTemplateGroupAccessControlEntry",
+            "action": "UpdateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServicePrincipalNames": {
+        "DeleteTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "ListServicePrincipalNames",
+            "action": "DeleteTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDirectoryRegistration": {
+        "ListTemplates": {
             "access_level": "Undocumented",
-            "action": "GetDirectoryRegistration",
+            "action": "ListTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServicePrincipalName": {
+        "UpdateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "GetServicePrincipalName",
+            "action": "UpdateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServicePrincipalName": {
+        "GetTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateServicePrincipalName",
+            "action": "GetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
@@ -123557,105 +123557,105 @@
             "orphan": false,
             "resources": [
                 "purchase-order"
             ]
         }
     },
     "q": {
-        "GetTroubleshootingResults": {
+        "GetConversation": {
             "access_level": "Undocumented",
-            "action": "GetTroubleshootingResults",
+            "action": "GetConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteAssignment": {
             "access_level": "Undocumented",
             "action": "DeleteAssignment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendMessage": {
+        "GetTroubleshootingResults": {
             "access_level": "Undocumented",
-            "action": "SendMessage",
+            "action": "GetTroubleshootingResults",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTroubleshootingResolutionExplanation": {
+        "PassRequest": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingResolutionExplanation",
+            "action": "PassRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConversation": {
+        "SendMessage": {
             "access_level": "Undocumented",
-            "action": "GetConversation",
+            "action": "SendMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentityMetadata": {
+        "StartTroubleshootingResolutionExplanation": {
             "access_level": "Undocumented",
-            "action": "GetIdentityMetadata",
+            "action": "StartTroubleshootingResolutionExplanation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTroubleshootingAnalysis": {
+        "CreateAssignment": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingAnalysis",
+            "action": "CreateAssignment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssignment": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "CreateAssignment",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartConversation": {
             "access_level": "Undocumented",
             "action": "StartConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRequest": {
+        "StartTroubleshootingAnalysis": {
             "access_level": "Undocumented",
-            "action": "PassRequest",
+            "action": "StartTroubleshootingAnalysis",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "UpdateTroubleshootingCommandResult": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "UpdateTroubleshootingCommandResult",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTroubleshootingCommandResult": {
+        "GetIdentityMetadata": {
             "access_level": "Undocumented",
-            "action": "UpdateTroubleshootingCommandResult",
+            "action": "GetIdentityMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qapps": {
@@ -123663,691 +123663,691 @@
             "access_level": "Undocumented",
             "action": "CreateLibraryItemReview",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateQAppFromUser": {
+        "UpdateQApp": {
             "access_level": "Undocumented",
-            "action": "DisassociateQAppFromUser",
+            "action": "UpdateQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLibraryItem": {
+        "DisassociateQAppFromUser": {
             "access_level": "Undocumented",
-            "action": "CreateLibraryItem",
+            "action": "DisassociateQAppFromUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQApp": {
+        "AssociateQAppWithUser": {
             "access_level": "Undocumented",
-            "action": "DeleteQApp",
+            "action": "AssociateQAppWithUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQApps": {
+        "StopQAppSession": {
             "access_level": "Undocumented",
-            "action": "ListQApps",
+            "action": "StopQAppSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLibraryItem": {
+        "CreateQApp": {
             "access_level": "Undocumented",
-            "action": "GetLibraryItem",
+            "action": "CreateQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportDocumentToQApp": {
+        "CreateSubscriptionToken": {
             "access_level": "Undocumented",
-            "action": "ImportDocumentToQApp",
+            "action": "CreateSubscriptionToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopQAppSession": {
+        "UpdateLibraryItem": {
             "access_level": "Undocumented",
-            "action": "StopQAppSession",
+            "action": "UpdateLibraryItem",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PredictProblemStatementFromConversation": {
+        "StartQAppSession": {
             "access_level": "Undocumented",
-            "action": "PredictProblemStatementFromConversation",
+            "action": "StartQAppSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQApp": {
+        "GetQApp": {
             "access_level": "Undocumented",
-            "action": "UpdateQApp",
+            "action": "GetQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportDocumentToQAppSession": {
+        "DeleteLibraryItem": {
             "access_level": "Undocumented",
-            "action": "ImportDocumentToQAppSession",
+            "action": "DeleteLibraryItem",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionToken": {
+        "ImportDocumentToQAppSession": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionToken",
+            "action": "ImportDocumentToQAppSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyQApp": {
+        "ListLibraryItems": {
             "access_level": "Undocumented",
-            "action": "CopyQApp",
+            "action": "ListLibraryItems",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartQAppSession": {
+        "CreateLibraryItem": {
             "access_level": "Undocumented",
-            "action": "StartQAppSession",
+            "action": "CreateLibraryItem",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLibraryItem": {
+        "GetLibraryItem": {
             "access_level": "Undocumented",
-            "action": "UpdateLibraryItem",
+            "action": "GetLibraryItem",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQApp": {
+        "CopyQApp": {
             "access_level": "Undocumented",
-            "action": "CreateQApp",
+            "action": "CopyQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLibraryItems": {
+        "ListQApps": {
             "access_level": "Undocumented",
-            "action": "ListLibraryItems",
+            "action": "ListQApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQApp": {
+        "ImportDocumentToQApp": {
             "access_level": "Undocumented",
-            "action": "GetQApp",
+            "action": "ImportDocumentToQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PredictQAppFromProblemStatement": {
+        "PredictProblemStatementFromConversation": {
             "access_level": "Undocumented",
-            "action": "PredictQAppFromProblemStatement",
+            "action": "PredictProblemStatementFromConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLibraryItem": {
+        "PredictQAppFromProblemStatement": {
             "access_level": "Undocumented",
-            "action": "DeleteLibraryItem",
+            "action": "PredictQAppFromProblemStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateQAppWithUser": {
+        "DeleteQApp": {
             "access_level": "Undocumented",
-            "action": "AssociateQAppWithUser",
+            "action": "DeleteQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qbusiness": {
-        "DeleteWebExperience": {
+        "PutGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteWebExperience",
+            "action": "PutGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRetriever": {
+        "UpdateRetriever": {
             "access_level": "Undocumented",
-            "action": "GetRetriever",
+            "action": "UpdateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPlugin": {
+        "DeleteConversation": {
             "access_level": "Undocumented",
-            "action": "GetPlugin",
+            "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRetriever": {
+        "DeleteApplication": {
             "access_level": "Undocumented",
-            "action": "DeleteRetriever",
+            "action": "DeleteApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSubscription": {
+        "GetChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "CancelSubscription",
+            "action": "GetChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndex": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "GetIndex",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApplication": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteApplication",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDocuments": {
+        "ListRetrievers": {
             "access_level": "Undocumented",
-            "action": "ListDocuments",
+            "action": "ListRetrievers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchPutDocument": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "BatchPutDocument",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApplication": {
+        "CancelSubscription": {
             "access_level": "Undocumented",
-            "action": "CreateApplication",
+            "action": "CancelSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreatePlugin": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMessages": {
+        "CreateIndex": {
             "access_level": "Undocumented",
-            "action": "ListMessages",
+            "action": "CreateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWebExperiences": {
+        "UpdateApplication": {
             "access_level": "Undocumented",
-            "action": "ListWebExperiences",
+            "action": "UpdateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "CreateSubscription": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "CreateSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPlugins": {
+        "ChatSync": {
             "access_level": "Undocumented",
-            "action": "ListPlugins",
+            "action": "ChatSync",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroup": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "PutGroup",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePlugin": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdatePlugin",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "ListWebExperiences": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "ListWebExperiences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "ListSubscriptions": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "ListSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "BatchDeleteDocument": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "BatchDeleteDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIndex": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteIndex",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApplication": {
+        "GetRetriever": {
             "access_level": "Undocumented",
-            "action": "UpdateApplication",
+            "action": "GetRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRetriever": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateRetriever",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceSyncJob": {
+        "UpdateWebExperience": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceSyncJob",
+            "action": "UpdateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChatControlsConfiguration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteChatControlsConfiguration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "CreateApplication": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "CreateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePlugin": {
+        "AddUserLicenses": {
             "access_level": "Undocumented",
-            "action": "DeletePlugin",
+            "action": "AddUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRetrievers": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListRetrievers",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChatSync": {
+        "BatchPutDocument": {
             "access_level": "Undocumented",
-            "action": "ChatSync",
+            "action": "BatchPutDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "CreateRetriever": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "CreateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplication": {
+        "DeleteIndex": {
             "access_level": "Undocumented",
-            "action": "GetApplication",
+            "action": "DeleteIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChatControlsConfiguration": {
+        "GetPlugin": {
             "access_level": "Undocumented",
-            "action": "UpdateChatControlsConfiguration",
+            "action": "GetPlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptions": {
+        "DeleteWebExperience": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptions",
+            "action": "DeleteWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWebExperience": {
+        "GetApplication": {
             "access_level": "Undocumented",
-            "action": "UpdateWebExperience",
+            "action": "GetApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "UpdateIndex": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "UpdateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicense": {
+        "UpdateChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateLicense",
+            "action": "UpdateChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserLicenses": {
+        "DeleteChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "RemoveUserLicenses",
+            "action": "DeleteChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "StopDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "StopDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRetriever": {
+        "DeletePlugin": {
             "access_level": "Undocumented",
-            "action": "CreateRetriever",
+            "action": "DeletePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteDocument": {
+        "DeleteRetriever": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteDocument",
+            "action": "DeleteRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWebExperience": {
+        "ListDataSourceSyncJobs": {
             "access_level": "Undocumented",
-            "action": "CreateWebExperience",
+            "action": "ListDataSourceSyncJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscription": {
+        "CreateWebExperience": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscription",
+            "action": "CreateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePlugin": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "CreatePlugin",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConversation": {
+        "GetLicense": {
             "access_level": "Undocumented",
-            "action": "DeleteConversation",
+            "action": "GetLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicense": {
+        "ListDocuments": {
             "access_level": "Undocumented",
-            "action": "GetLicense",
+            "action": "ListDocuments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Chat": {
+        "StartDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "Chat",
+            "action": "StartDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApplications": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "ListApplications",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceSyncJobs": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceSyncJobs",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIndex": {
+        "ListPlugins": {
             "access_level": "Undocumented",
-            "action": "CreateIndex",
+            "action": "ListPlugins",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscription": {
+        "ListApplications": {
             "access_level": "Undocumented",
-            "action": "CreateSubscription",
+            "action": "ListApplications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "RemoveUserLicenses": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "RemoveUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChatControlsConfiguration": {
+        "ListUserLicenses": {
             "access_level": "Undocumented",
-            "action": "GetChatControlsConfiguration",
+            "action": "ListUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserLicenses": {
+        "UpdatePlugin": {
             "access_level": "Undocumented",
-            "action": "AddUserLicenses",
+            "action": "UpdatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIndex": {
+        "Chat": {
             "access_level": "Undocumented",
-            "action": "UpdateIndex",
+            "action": "Chat",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFeedback": {
+        "CreateLicense": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "CreateLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "GetIndex": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "GetIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "ListMessages": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "ListMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIndices": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "ListIndices",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserLicenses": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "ListUserLicenses",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopDataSourceSyncJob": {
+        "ListIndices": {
             "access_level": "Undocumented",
-            "action": "StopDataSourceSyncJob",
+            "action": "ListIndices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "GetWebExperience": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "GetWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWebExperience": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "GetWebExperience",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateSubscription": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qldb": {
@@ -126820,281 +126820,281 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "ram": {
-        "ListPrincipals": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateResourceShare": {
             "access_level": "Undocumented",
             "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
-            "access_level": "Undocumented",
-            "action": "DeletePermission",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "ListPermissionVersions": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetResourceShareInvitations": {
             "access_level": "Undocumented",
             "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPermission": {
             "access_level": "Undocumented",
             "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateResourceShare": {
             "access_level": "Undocumented",
             "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
             "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetResourceShareAssociations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetResourcePolicies": {
+            "access_level": "Undocumented",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -132476,89 +132476,89 @@
             "orphan": false,
             "resources": [
                 "streamprocessor"
             ]
         }
     },
     "repostspace": {
-        "RegisterAdmin": {
+        "SendInvites": {
             "access_level": "Undocumented",
-            "action": "RegisterAdmin",
+            "action": "SendInvites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeregisterAdmin": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeregisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSpace": {
+        "RegisterAdmin": {
             "access_level": "Undocumented",
-            "action": "UpdateSpace",
+            "action": "RegisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSpaces": {
+        "GetSpace": {
             "access_level": "Undocumented",
-            "action": "ListSpaces",
+            "action": "GetSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterAdmin": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeregisterAdmin",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSpace": {
+        "ListSpaces": {
             "access_level": "Undocumented",
-            "action": "DeleteSpace",
+            "action": "ListSpaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendInvites": {
+        "DeleteSpace": {
             "access_level": "Undocumented",
-            "action": "SendInvites",
+            "action": "DeleteSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateSpace": {
             "access_level": "Undocumented",
             "action": "CreateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSpace": {
+        "UpdateSpace": {
             "access_level": "Undocumented",
-            "action": "GetSpace",
+            "action": "UpdateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
@@ -132566,475 +132566,475 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resiliencehub": {
-        "ImportResourcesToDraftAppVersion": {
+        "DeleteResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ImportResourcesToDraftAppVersion",
+            "action": "DeleteResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppAssessment": {
+        "AddDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "DescribeAppAssessment",
+            "action": "AddDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessmentResourceDrifts": {
+        "PublishAppVersion": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessmentResourceDrifts",
+            "action": "PublishAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchUpdateRecommendationStatus": {
+        "DeleteRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "BatchUpdateRecommendationStatus",
+            "action": "DeleteRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResource": {
+        "ResolveAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResource",
+            "action": "ResolveAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeDraftAppVersionResourcesImportStatus": {
+        "UpdateApp": {
             "access_level": "Undocumented",
-            "action": "DescribeDraftAppVersionResourcesImportStatus",
+            "action": "UpdateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddDraftAppVersionResourceMappings": {
+        "UpdateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "AddDraftAppVersionResourceMappings",
+            "action": "UpdateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionAppComponent": {
+        "DescribeDraftAppVersionResourcesImportStatus": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionAppComponent",
+            "action": "DescribeDraftAppVersionResourcesImportStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersion": {
+        "ListAppComponentRecommendations": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersion",
+            "action": "ListAppComponentRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionTemplate": {
+        "StartAppAssessment": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionTemplate",
+            "action": "StartAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersion": {
+        "ListAppInputSources": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersion",
+            "action": "ListAppInputSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResiliencyPolicy": {
+        "ListSopRecommendations": {
             "access_level": "Undocumented",
-            "action": "UpdateResiliencyPolicy",
+            "action": "ListSopRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentCompliances": {
+        "UpdateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentCompliances",
+            "action": "UpdateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResources": {
+        "CreateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResources",
+            "action": "CreateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAssessment": {
+        "DeleteAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAssessment",
+            "action": "DeleteAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAlarmRecommendations": {
+        "DescribeAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAlarmRecommendations",
+            "action": "DescribeAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUnsupportedAppVersionResources": {
+        "ListAppVersions": {
             "access_level": "Undocumented",
-            "action": "ListUnsupportedAppVersionResources",
+            "action": "ListAppVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResourcesResolutionStatus": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResourcesResolutionStatus",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTestRecommendations": {
+        "ListAppAssessmentResourceDrifts": {
             "access_level": "Undocumented",
-            "action": "ListTestRecommendations",
+            "action": "ListAppAssessmentResourceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRecommendationTemplate": {
+        "CreateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateRecommendationTemplate",
+            "action": "CreateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeApp": {
+        "DeleteAppInputSource": {
             "access_level": "Undocumented",
-            "action": "DescribeApp",
+            "action": "DeleteAppInputSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppInputSources": {
+        "ListSuggestedResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "ListAppInputSources",
+            "action": "ListSuggestedResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApp": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateApp",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResiliencyPolicy": {
+        "ListAppComponentCompliances": {
             "access_level": "Undocumented",
-            "action": "DeleteResiliencyPolicy",
+            "action": "ListAppComponentCompliances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessmentComplianceDrifts": {
+        "DescribeAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessmentComplianceDrifts",
+            "action": "DescribeAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppAssessment": {
+        "ListApps": {
             "access_level": "Undocumented",
-            "action": "StartAppAssessment",
+            "action": "ListApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionAppComponents": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionAppComponents",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResiliencyPolicies": {
+        "ListAlarmRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListResiliencyPolicies",
+            "action": "ListAlarmRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PublishAppVersion": {
+        "ListAppVersionAppComponents": {
             "access_level": "Undocumented",
-            "action": "PublishAppVersion",
+            "action": "ListAppVersionAppComponents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSopRecommendations": {
+        "ListUnsupportedAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "ListSopRecommendations",
+            "action": "ListUnsupportedAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionResource": {
+        "DeleteAppAssessment": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionResource",
+            "action": "DeleteAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSuggestedResiliencyPolicies": {
+        "DeleteAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "ListSuggestedResiliencyPolicies",
+            "action": "DeleteAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionAppComponent": {
+        "CreateApp": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionAppComponent",
+            "action": "CreateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionResource": {
+        "BatchUpdateRecommendationStatus": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionResource",
+            "action": "BatchUpdateRecommendationStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DescribeAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DescribeAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionAppComponent": {
+        "ImportResourcesToDraftAppVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionAppComponent",
+            "action": "ImportResourcesToDraftAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResourceMappings": {
+        "DescribeResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResourceMappings",
+            "action": "DescribeResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApps": {
+        "RemoveDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "ListApps",
+            "action": "RemoveDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersions": {
+        "ListResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "ListAppVersions",
+            "action": "ListResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentRecommendations": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentRecommendations",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionResource": {
+        "ListAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionResource",
+            "action": "ListAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResolveAppVersionResources": {
+        "UpdateAppVersion": {
             "access_level": "Undocumented",
-            "action": "ResolveAppVersionResources",
+            "action": "UpdateAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRecommendationTemplate": {
+        "CreateRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteRecommendationTemplate",
+            "action": "CreateRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResiliencyPolicy": {
+        "DescribeAppVersion": {
             "access_level": "Undocumented",
-            "action": "CreateResiliencyPolicy",
+            "action": "DescribeAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationTemplates": {
+        "ListAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationTemplates",
+            "action": "ListAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "PutDraftAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "PutDraftAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeResiliencyPolicy": {
+        "ListRecommendationTemplates": {
             "access_level": "Undocumented",
-            "action": "DescribeResiliencyPolicy",
+            "action": "ListRecommendationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessments": {
+        "DescribeApp": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessments",
+            "action": "DescribeApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionAppComponent": {
+        "CreateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionAppComponent",
+            "action": "CreateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApp": {
+        "DescribeAppVersionResourcesResolutionStatus": {
             "access_level": "Undocumented",
-            "action": "UpdateApp",
+            "action": "DescribeAppVersionResourcesResolutionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDraftAppVersionTemplate": {
+        "ListAppAssessments": {
             "access_level": "Undocumented",
-            "action": "PutDraftAppVersionTemplate",
+            "action": "ListAppAssessments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppInputSource": {
+        "ListAppAssessmentComplianceDrifts": {
             "access_level": "Undocumented",
-            "action": "DeleteAppInputSource",
+            "action": "ListAppAssessmentComplianceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveDraftAppVersionResourceMappings": {
+        "DescribeAppAssessment": {
             "access_level": "Undocumented",
-            "action": "RemoveDraftAppVersionResourceMappings",
+            "action": "DescribeAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTestRecommendations": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTestRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer": {
-        "ListResources": {
+        "ListTags": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "ListTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTags": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListTags",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer-2": {
@@ -135988,137 +135988,137 @@
             "condition_keys": [],
             "description": "Grants permission to get all the domain-related billing records for the current AWS account for a specified period",
             "orphan": false,
             "resources": []
         }
     },
     "route53profiles": {
-        "UntagResource": {
+        "DisassociateProfile": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DisassociateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfileResourceAssociation": {
+        "GetProfileAssociation": {
             "access_level": "Undocumented",
-            "action": "GetProfileResourceAssociation",
+            "action": "GetProfileAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceToProfile": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceToProfile",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProfile": {
+        "AssociateProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteProfile",
+            "action": "AssociateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceFromProfile": {
+        "DeleteProfile": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceFromProfile",
+            "action": "DeleteProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfiles": {
+        "GetProfile": {
             "access_level": "Undocumented",
-            "action": "ListProfiles",
+            "action": "GetProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProfileResourceAssociation": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateProfileResourceAssociation",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetProfileResourceAssociation": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetProfileResourceAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfileResourceAssociations": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListProfileResourceAssociations",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateProfile": {
+        "CreateProfile": {
             "access_level": "Undocumented",
-            "action": "DisassociateProfile",
+            "action": "CreateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListProfileAssociations": {
             "access_level": "Undocumented",
             "action": "ListProfileAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProfile": {
+        "DisassociateResourceFromProfile": {
             "access_level": "Undocumented",
-            "action": "CreateProfile",
+            "action": "DisassociateResourceFromProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfile": {
+        "ListProfiles": {
             "access_level": "Undocumented",
-            "action": "GetProfile",
+            "action": "ListProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfileAssociation": {
+        "AssociateResourceToProfile": {
             "access_level": "Undocumented",
-            "action": "GetProfileAssociation",
+            "action": "AssociateResourceToProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateProfile": {
+        "UpdateProfileResourceAssociation": {
             "access_level": "Undocumented",
-            "action": "AssociateProfile",
+            "action": "UpdateProfileResourceAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListProfileResourceAssociations": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListProfileResourceAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "route53resolver": {
@@ -141138,65 +141138,65 @@
             "orphan": false,
             "resources": [
                 "object"
             ]
         }
     },
     "s3express": {
-        "GetBucketPolicy": {
+        "DeleteBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "GetBucketPolicy",
+            "action": "DeleteBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "ListAllMyDirectoryBuckets": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "ListAllMyDirectoryBuckets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBucketPolicy": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "DeleteBucketPolicy",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteBucket": {
             "access_level": "Undocumented",
             "action": "DeleteBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutBucketPolicy": {
+        "GetBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "PutBucketPolicy",
+            "action": "GetBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllMyDirectoryBuckets": {
+        "CreateBucket": {
             "access_level": "Undocumented",
-            "action": "ListAllMyDirectoryBuckets",
+            "action": "CreateBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBucket": {
+        "PutBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateBucket",
+            "action": "PutBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sagemaker": {
@@ -145977,86 +145977,94 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "UpdateInstance": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
             "action": "CreateBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateSSOApplication": {
             "access_level": "Undocumented",
             "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
             "action": "GetBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -146065,25 +146073,25 @@
             "access_level": "Undocumented",
             "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "SendDataIntegrationEvent": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "SendDataIntegrationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateInstance": {
             "access_level": "Undocumented",
@@ -146096,22 +146104,14 @@
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
-        },
-        "SendDataIntegrationEvent": {
-            "access_level": "Undocumented",
-            "action": "SendDataIntegrationEvent",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
         }
     },
     "sdb": {
         "BatchDeleteAttributes": {
             "access_level": "Write",
             "action": "BatchDeleteAttributes",
             "condition_keys": [],
@@ -162153,129 +162153,129 @@
             "orphan": false,
             "resources": [
                 "adapter"
             ]
         }
     },
     "thinclient": {
-        "UntagResource": {
+        "ListDeviceSessions": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListDeviceSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "GetSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "GetSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDevice": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateDevice",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDevice": {
+        "UpdateSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "GetDevice",
+            "action": "UpdateSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSoftwareSet": {
+        "DeregisterDevice": {
             "access_level": "Undocumented",
-            "action": "GetSoftwareSet",
+            "action": "DeregisterDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceSessions": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDeviceSessions",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSoftwareSet": {
+        "ListDevices": {
             "access_level": "Undocumented",
-            "action": "UpdateSoftwareSet",
+            "action": "ListDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteDevice": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "GetDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "GetDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterDevice": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "DeregisterDevice",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDevice": {
+        "UpdateDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteDevice",
+            "action": "UpdateDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevices": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "ListDevices",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
@@ -162657,41 +162657,41 @@
             "orphan": false,
             "resources": [
                 "table"
             ]
         }
     },
     "timestream-influxdb": {
-        "GetDbParameterGroup": {
+        "CreateDbInstance": {
             "access_level": "Undocumented",
-            "action": "GetDbParameterGroup",
+            "action": "CreateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDbInstances": {
+        "ListDbParameterGroups": {
             "access_level": "Undocumented",
-            "action": "ListDbInstances",
+            "action": "ListDbParameterGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteDbInstance": {
             "access_level": "Undocumented",
@@ -162705,49 +162705,49 @@
             "access_level": "Undocumented",
             "action": "UpdateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDbParameterGroups": {
+        "GetDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "ListDbParameterGroups",
+            "action": "GetDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDbInstance": {
+        "GetDbInstance": {
             "access_level": "Undocumented",
-            "action": "CreateDbInstance",
+            "action": "GetDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListDbInstances": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListDbInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDbInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetDbInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDbParameterGroup": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateDbParameterGroup",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "tiros": {
@@ -162789,273 +162789,273 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "GetSolNetworkOperation": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolFunctionPackage": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -164773,41 +164773,33 @@
             "condition_keys": [],
             "description": "Grants permission to update the risk status in AWS Trusted Advisor Priority",
             "orphan": false,
             "resources": []
         }
     },
     "ts": {
-        "GetExecutionOutput": {
-            "access_level": "Undocumented",
-            "action": "GetExecutionOutput",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "UntagResource": {
+        "StartExecution": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "StartExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListExecutions": {
             "access_level": "Undocumented",
             "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExecution": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartExecution",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetExecution": {
             "access_level": "Undocumented",
@@ -164829,17 +164821,25 @@
             "access_level": "Undocumented",
             "action": "GetTool",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetExecutionOutput": {
+            "access_level": "Undocumented",
+            "action": "GetExecutionOutput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
@@ -164855,49 +164855,49 @@
             "access_level": "Undocumented",
             "action": "DeleteClaim",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserSubscriptions": {
+        "UpdateClaim": {
             "access_level": "Undocumented",
-            "action": "ListUserSubscriptions",
+            "action": "UpdateClaim",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListApplicationClaims": {
             "access_level": "Undocumented",
             "action": "ListApplicationClaims",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateClaim": {
+        "CreateClaim": {
             "access_level": "Undocumented",
-            "action": "UpdateClaim",
+            "action": "CreateClaim",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateClaim": {
+        "ListClaims": {
             "access_level": "Undocumented",
-            "action": "CreateClaim",
+            "action": "ListClaims",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListClaims": {
+        "ListUserSubscriptions": {
             "access_level": "Undocumented",
-            "action": "ListClaims",
+            "action": "ListUserSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "vendor-insights": {
@@ -165183,201 +165183,201 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "verifiedpermissions": {
-        "GetIdentitySource": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyStores": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "ListPolicyStores",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "GetPolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "UpdatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyTemplate": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyTemplate": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "GetPolicyTemplate",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
+        "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
+            "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyStore": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyStore",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdentitySource": {
+        "ListPolicyStores": {
             "access_level": "Undocumented",
-            "action": "UpdateIdentitySource",
+            "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyStore": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdentitySource": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "CreateIdentitySource",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorized": {
+        "UpdateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "IsAuthorized",
+            "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdentitySources": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyTemplate": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyTemplate",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "CreateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "IsAuthorized": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "IsAuthorized",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "ListPolicyTemplates": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "ListPolicyTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorizedWithToken": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "IsAuthorizedWithToken",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "voiceid": {
@@ -169356,385 +169356,385 @@
             "orphan": false,
             "resources": [
                 "network"
             ]
         }
     },
     "wisdom": {
-        "CreateAssistant": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "CreateAssistant",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateContentAssociation": {
+        "UpdateKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "CreateContentAssociation",
+            "action": "UpdateKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContentAssociation": {
+        "StartContentUpload": {
             "access_level": "Undocumented",
-            "action": "GetContentAssociation",
+            "action": "StartContentUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "GetRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "GetRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistant": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistant",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteContent": {
+        "StartImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteContent",
+            "action": "StartImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKnowledgeBase": {
+        "UpdateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "UpdateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "NotifyRecommendationsReceived": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "NotifyRecommendationsReceived",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQuickResponse": {
+        "GetAssistant": {
             "access_level": "Undocumented",
-            "action": "UpdateQuickResponse",
+            "action": "GetAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "DeleteContent": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "DeleteContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "QueryAssistant": {
+        "DeleteImportJob": {
             "access_level": "Undocumented",
-            "action": "QueryAssistant",
+            "action": "DeleteImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateAssistant": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateContent": {
+        "GetImportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateContent",
+            "action": "GetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListContents": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "ListContents",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQuickResponse": {
+        "CreateContent": {
             "access_level": "Undocumented",
-            "action": "DeleteQuickResponse",
+            "action": "CreateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistantAssociation": {
+        "DeleteContentAssociation": {
             "access_level": "Undocumented",
-            "action": "GetAssistantAssociation",
+            "action": "DeleteContentAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBaseTemplateUri": {
+        "SearchContent": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBaseTemplateUri",
+            "action": "SearchContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateContent": {
+        "UpdateContent": {
             "access_level": "Undocumented",
-            "action": "CreateContent",
+            "action": "UpdateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistants": {
+        "GetQuickResponse": {
             "access_level": "Undocumented",
-            "action": "ListAssistants",
+            "action": "GetQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSessions": {
+        "DeleteQuickResponse": {
             "access_level": "Undocumented",
-            "action": "SearchSessions",
+            "action": "DeleteQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistant": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "GetAssistant",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContent": {
+        "RemoveKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "GetContent",
+            "action": "RemoveKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImportJob": {
+        "GetContentSummary": {
             "access_level": "Undocumented",
-            "action": "GetImportJob",
+            "action": "GetContentSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistantAssociations": {
+        "DeleteAssistant": {
             "access_level": "Undocumented",
-            "action": "ListAssistantAssociations",
+            "action": "DeleteAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveKnowledgeBaseTemplateUri": {
+        "CreateAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "RemoveKnowledgeBaseTemplateUri",
+            "action": "CreateAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContentUpload": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartContentUpload",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportJobs": {
+        "GetContent": {
             "access_level": "Undocumented",
-            "action": "ListImportJobs",
+            "action": "GetContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyRecommendationsReceived": {
+        "SearchSessions": {
             "access_level": "Undocumented",
-            "action": "NotifyRecommendationsReceived",
+            "action": "SearchSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "DeleteAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "DeleteAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteContentAssociation": {
+        "ListAssistantAssociations": {
             "access_level": "Undocumented",
-            "action": "DeleteContentAssociation",
+            "action": "ListAssistantAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQuickResponse": {
+        "SearchQuickResponses": {
             "access_level": "Undocumented",
-            "action": "GetQuickResponse",
+            "action": "SearchQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportJob": {
+        "ListAssistants": {
             "access_level": "Undocumented",
-            "action": "StartImportJob",
+            "action": "ListAssistants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImportJob": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "DeleteImportJob",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecommendations": {
+        "CreateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "GetRecommendations",
+            "action": "CreateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistantAssociation": {
+        "ListImportJobs": {
             "access_level": "Undocumented",
-            "action": "CreateAssistantAssociation",
+            "action": "ListImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchContent": {
+        "QueryAssistant": {
             "access_level": "Undocumented",
-            "action": "SearchContent",
+            "action": "QueryAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFeedback": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "ListContents": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "ListContents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuickResponses": {
+        "GetAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "ListQuickResponses",
+            "action": "GetAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistantAssociation": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistantAssociation",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListContentAssociations": {
+        "GetContentAssociation": {
             "access_level": "Undocumented",
-            "action": "ListContentAssociations",
+            "action": "GetContentAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchQuickResponses": {
+        "CreateContentAssociation": {
             "access_level": "Undocumented",
-            "action": "SearchQuickResponses",
+            "action": "CreateContentAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQuickResponse": {
+        "ListQuickResponses": {
             "access_level": "Undocumented",
-            "action": "CreateQuickResponse",
+            "action": "ListQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContentSummary": {
+        "ListContentAssociations": {
             "access_level": "Undocumented",
-            "action": "GetContentSummary",
+            "action": "ListContentAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "workdocs": {
```

### Comparing `iam_actions-1.2.20240517/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240518/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240518/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/generate/generate.py` & `iam_actions-1.2.20240518/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240518/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240518/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/generate/services.py` & `iam_actions-1.2.20240518/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/policies.json` & `iam_actions-1.2.20240518/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240518/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/iam_actions/services.json` & `iam_actions-1.2.20240518/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240517/pyproject.toml` & `iam_actions-1.2.20240518/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240517"
+version = "1.2.20240518"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240517/setup.py` & `iam_actions-1.2.20240518/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240517',
+    'version': '1.2.20240518',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240517/PKG-INFO` & `iam_actions-1.2.20240518/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240517
+Version: 1.2.20240518
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

