# Comparing `tmp/user_context_remote-0.0.77.tar.gz` & `tmp/user_context_remote-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_context_remote-0.0.77.tar", last modified: Thu May  9 19:58:15 2024, max compression
+gzip compressed data, was "user_context_remote-0.0.78.tar", last modified: Sun May 19 17:49:33 2024, max compression
```

## Comparing `user_context_remote-0.0.77.tar` & `user_context_remote-0.0.78.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:58:15.699817 user_context_remote-0.0.77/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-09 19:58:15.699817 user_context_remote-0.0.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-09 19:57:59.000000 user_context_remote-0.0.77/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 19:57:59.000000 user_context_remote-0.0.77/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 19:58:15.699817 user_context_remote-0.0.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-09 19:57:59.000000 user_context_remote-0.0.77/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:58:15.699817 user_context_remote-0.0.77/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:58:15.699817 user_context_remote-0.0.77/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:57:59.000000 user_context_remote-0.0.77/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18995 2024-05-09 19:57:59.000000 user_context_remote-0.0.77/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:58:15.699817 user_context_remote-0.0.77/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-09 19:58:15.000000 user_context_remote-0.0.77/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 19:58:15.000000 user_context_remote-0.0.77/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 19:58:15.000000 user_context_remote-0.0.77/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 19:58:15.000000 user_context_remote-0.0.77/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-09 19:58:15.000000 user_context_remote-0.0.77/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:33.217081 user_context_remote-0.0.78/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 17:49:33.217081 user_context_remote-0.0.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:49:33.217081 user_context_remote-0.0.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:33.213081 user_context_remote-0.0.78/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:33.213081 user_context_remote-0.0.78/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:33.217081 user_context_remote-0.0.78/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/top_level.txt
```

### Comparing `user_context_remote-0.0.77/PKG-INFO` & `user_context_remote-0.0.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.77
+Version: 0.0.78
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `user_context_remote-0.0.77/README.md` & `user_context_remote-0.0.78/README.md`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.77/pyproject.toml` & `user_context_remote-0.0.78/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.77/setup.py` & `user_context_remote-0.0.78/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.77',  # https://pypi.org/project/user-context-remote/
+    version='0.0.78',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.ai",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `user_context_remote-0.0.77/user_context_remote/src/user_context.py` & `user_context_remote-0.0.78/user_context_remote/src/user_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from http import HTTPStatus
 
 import requests
 from language_remote.lang_code import LangCode
 from python_sdk_remote.mini_logger import MiniLogger
 from python_sdk_remote.utilities import our_get_env, create_return_http_headers
 from url_remote import action_name_enum, component_name_enum, entity_name_enum
-from url_remote.url_circlez import OurUrl
+from url_remote.our_url import OurUrl
 
 # TODO Shall we use authentication-remote-python-package and not directly authentication-local-restapi-typescript?
 
 BRAND_NAME = our_get_env("BRAND_NAME")
 ENVIORNMENT_NAME = our_get_env("ENVIRONMENT_NAME")
 
 # TODO How about using AUTHENTICATION_API_VERSION_DICT per environment_name in url-remote-python-package?
@@ -259,18 +259,18 @@
                        object={"validate_user_jwt_response": authentication_login_validate_user_jwt_response})
         return authentication_login_validate_user_jwt_response
 
     # Used only in one please
     def __get_user_data_login_response(self, validate_user_jwt_response: requests.Response) -> None:
         _GET_USER_DATA_LOGIN_RESPONSE_METHOD_NAME = "get_user_data_login_response"
         # validate_user_jwt_response created in Authentication Local REST-API https://github.com/circles-zone/authentication-local-restapi-typescript-serverless-com/edit/dev/auth-restapi-serverless-com/src/services/auth-service/auth-service-impl.ts
-        data_json = validate_user_jwt_response.json()['data']
+        data_dict = validate_user_jwt_response.json()['data']
         first_name = last_name = None
-        if "userDetails" in data_json:
-            userDetails = data_json["userDetails"]
+        if "userDetails" in data_dict:
+            userDetails = data_dict["userDetails"]
 
             if "profileId" in userDetails:
                 profile_id = userDetails["profileId"]
                 self._set_real_profile_id(int(profile_id))
                 self._set_effective_profile_id(int(profile_id))
 
             if "userId" in userDetails:
```

### Comparing `user_context_remote-0.0.77/user_context_remote.egg-info/PKG-INFO` & `user_context_remote-0.0.78/user_context_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.77
+Version: 0.0.78
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

