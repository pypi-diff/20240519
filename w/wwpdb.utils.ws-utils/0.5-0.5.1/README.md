# Comparing `tmp/wwpdb.utils.ws_utils-0.5.tar.gz` & `tmp/wwpdb_utils_ws_utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.ws_utils-0.5.tar", last modified: Fri Sep 22 18:46:14 2023, max compression
+gzip compressed data, was "wwpdb_utils_ws_utils-0.5.1.tar", last modified: Sun May 19 19:24:05 2024, max compression
```

## Comparing `wwpdb.utils.ws_utils-0.5.tar` & `wwpdb_utils_ws_utils-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-22 18:46:14.982183 wwpdb.utils.ws_utils-0.5/
--rw-r--r--   0 vsts      (1001) docker     (127)      146 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)      930 2023-09-22 18:46:14.982183 wwpdb.utils.ws_utils-0.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      790 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2023-09-22 18:46:14.986183 wwpdb.utils.ws_utils-0.5/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2036 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-22 18:46:14.978183 wwpdb.utils.ws_utils-0.5/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-22 18:46:14.978183 wwpdb.utils.ws_utils-0.5/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-22 18:46:14.982183 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     7387 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceDataStore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7454 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceHistory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3712 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceLockFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8494 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceRequest.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14714 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceResponse.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3805 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceSessionFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5000 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceSessionState.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4153 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceSmtpUtils.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     7941 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceUploadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      733 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceUtilsMisc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6565 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceWorkerBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12559 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/TokenUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      153 2023-09-22 18:45:20.000000 wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-09-22 18:46:14.978183 wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      930 2023-09-22 18:46:14.000000 wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      880 2023-09-22 18:46:14.000000 wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-09-22 18:46:14.000000 wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-09-22 18:46:00.000000 wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       87 2023-09-22 18:46:14.000000 wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2023-09-22 18:46:14.000000 wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:24:05.058805 wwpdb_utils_ws_utils-0.5.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)      146 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      932 2024-05-19 19:24:05.058805 wwpdb_utils_ws_utils-0.5.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-19 19:24:05.058805 wwpdb_utils_ws_utils-0.5.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2036 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:24:05.050805 wwpdb_utils_ws_utils-0.5.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:24:05.054805 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:24:05.054805 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7387 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceDataStore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3712 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceLockFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8494 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14714 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceResponse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3805 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceSessionFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5000 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceSessionState.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4153 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceSmtpUtils.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     7941 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceUploadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      733 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceUtilsMisc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6565 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceWorkerBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12551 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/TokenUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-05-19 19:23:13.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:24:05.054805 wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      932 2024-05-19 19:24:04.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      880 2024-05-19 19:24:05.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-19 19:24:04.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-19 19:23:48.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-05-19 19:24:04.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-19 19:24:04.000000 wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.ws_utils-0.5/PKG-INFO` & `wwpdb_utils_ws_utils-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.ws_utils
-Version: 0.5
+Version: 0.5.1
 Summary: wwPDB remote services support library
 Home-page: https://github.com/rcsb/py-wwpdb_utils_ws_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.ws_utils-0.5/README.md` & `wwpdb_utils_ws_utils-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/setup.py` & `wwpdb_utils_ws_utils-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceDataStore.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceDataStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceHistory.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceHistory.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,15 @@
         sessionCount = 0
         submittedCount = 0
         completedCount = 0
         failedCount = 0
         sL = []
         #
         try:
+            tStart = datetime.datetime(1969, 1, 1).isoformat()  # should always have a "created" in loop
             for sId in tD:
                 sD = tD[sId]
                 deltaSeconds = 0
                 if "created" in sD:
                     sessionCount += 1
                     tStart = sD["created"]["tiso"]
                     st = "created"
```

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceLockFile.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceLockFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceRequest.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceResponse.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceResponse.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceSessionFactory.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceSessionFactory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceSessionState.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceSessionState.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceSmtpUtils.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceSmtpUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceUploadUtils.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceUploadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceUtilsMisc.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceUtilsMisc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/ServiceWorkerBase.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/ServiceWorkerBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb/utils/ws_utils/TokenUtils.py` & `wwpdb_utils_ws_utils-0.5.1/wwpdb/utils/ws_utils/TokenUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         Token utilities for registration webservice
 
         """
         super(JwtTokenUtils, self).__init__(siteId=siteId, tokenPrefix=tokenPrefix, **kwargs)
         #
         # self.__inputToken = self._reqObj.getValue('authorization').split()[1]
         #
-        serviceKey = self._cI.get("SITE_SERVICE_REGISTRATION_KEY", default=None)
+        serviceKey = self._cI.get("SITE_SERVICE_REGISTRATION_KEY", None)
         self.__serviceKey = serviceKey if serviceKey else "secretvalue"
         self.__tokenErrorCode = 401
 
     def parseAuth(self, authHeader):
         rD = {"errorCode": None, "errorMessage": None, "token": None, "errorFlag": False}
         parts = authHeader.split()
         if parts[0].lower() != "bearer":
```

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/PKG-INFO` & `wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wwpdb.utils.ws-utils
-Version: 0.5
+Name: wwpdb.utils.ws_utils
+Version: 0.5.1
 Summary: wwPDB remote services support library
 Home-page: https://github.com/rcsb/py-wwpdb_utils_ws_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.ws_utils-0.5/wwpdb.utils.ws_utils.egg-info/SOURCES.txt` & `wwpdb_utils_ws_utils-0.5.1/wwpdb.utils.ws_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

