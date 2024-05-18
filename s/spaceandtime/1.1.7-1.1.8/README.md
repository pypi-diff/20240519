# Comparing `tmp/spaceandtime-1.1.7.tar.gz` & `tmp/spaceandtime-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceandtime-1.1.7.tar", last modified: Thu Oct 12 22:47:47 2023, max compression
+gzip compressed data, was "spaceandtime-1.1.8.tar", last modified: Sun Oct 15 19:43:37 2023, max compression
```

## Comparing `spaceandtime-1.1.7.tar` & `spaceandtime-1.1.8.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2023-10-12 22:47:47.856509 spaceandtime-1.1.7/
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     1071 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/LICENSE
--rw-r--r--   0 stephen.hilton   (501) staff       (20)       41 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/MANIFEST.in
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     9794 2023-10-12 22:47:47.856252 spaceandtime-1.1.7/PKG-INFO
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     7439 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/README.md
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     1356 2023-10-12 22:47:19.000000 spaceandtime-1.1.7/pyproject.toml
--rw-r--r--   0 stephen.hilton   (501) staff       (20)       38 2023-10-12 22:47:47.856543 spaceandtime-1.1.7/setup.cfg
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     1258 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/setup.py
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2023-10-12 22:47:47.852186 spaceandtime-1.1.7/src/
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2023-10-12 22:47:47.854959 spaceandtime-1.1.7/src/spaceandtime/
--rw-r--r--   0 stephen.hilton   (501) staff       (20)      312 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/__init__.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)      557 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/__main__.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     1546 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/apiversions.json
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    16576 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/spaceandtime.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    30288 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/sxtbaseapi.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    18274 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/sxtbiscuits.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     1666 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/sxtenums.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     1309 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/sxtexceptions.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    13106 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/sxtkeymanager.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    38820 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/sxtresource.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    13401 2023-10-12 22:46:04.000000 spaceandtime-1.1.7/src/spaceandtime/sxtuser.py
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2023-10-12 22:47:47.855824 spaceandtime-1.1.7/src/spaceandtime.egg-info/
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     9794 2023-10-12 22:47:47.000000 spaceandtime-1.1.7/src/spaceandtime.egg-info/PKG-INFO
--rw-r--r--   0 stephen.hilton   (501) staff       (20)      640 2023-10-12 22:47:47.000000 spaceandtime-1.1.7/src/spaceandtime.egg-info/SOURCES.txt
--rw-r--r--   0 stephen.hilton   (501) staff       (20)        1 2023-10-12 22:47:47.000000 spaceandtime-1.1.7/src/spaceandtime.egg-info/dependency_links.txt
--rw-r--r--   0 stephen.hilton   (501) staff       (20)       56 2023-10-12 22:47:47.000000 spaceandtime-1.1.7/src/spaceandtime.egg-info/entry_points.txt
--rw-r--r--   0 stephen.hilton   (501) staff       (20)       98 2023-10-12 22:47:47.000000 spaceandtime-1.1.7/src/spaceandtime.egg-info/requires.txt
--rw-r--r--   0 stephen.hilton   (501) staff       (20)       13 2023-10-12 22:47:47.000000 spaceandtime-1.1.7/src/spaceandtime.egg-info/top_level.txt
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2023-10-15 19:43:37.798830 spaceandtime-1.1.8/
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     1071 2023-10-12 22:46:04.000000 spaceandtime-1.1.8/LICENSE
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)       41 2023-10-12 22:46:04.000000 spaceandtime-1.1.8/MANIFEST.in
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     9642 2023-10-15 19:43:37.798576 spaceandtime-1.1.8/PKG-INFO
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     7439 2023-10-12 22:46:04.000000 spaceandtime-1.1.8/README.md
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     1356 2023-10-15 19:42:34.000000 spaceandtime-1.1.8/pyproject.toml
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)       38 2023-10-15 19:43:37.798866 spaceandtime-1.1.8/setup.cfg
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2023-10-15 19:43:37.793631 spaceandtime-1.1.8/src/
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2023-10-15 19:43:37.797399 spaceandtime-1.1.8/src/spaceandtime/
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)      312 2023-10-12 22:46:04.000000 spaceandtime-1.1.8/src/spaceandtime/__init__.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)      557 2023-10-12 22:46:04.000000 spaceandtime-1.1.8/src/spaceandtime/__main__.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     1546 2023-10-12 22:46:04.000000 spaceandtime-1.1.8/src/spaceandtime/apiversions.json
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    16571 2023-10-15 18:08:14.000000 spaceandtime-1.1.8/src/spaceandtime/spaceandtime.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    32091 2023-10-15 19:41:17.000000 spaceandtime-1.1.8/src/spaceandtime/sxtbaseapi.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    18271 2023-10-15 18:01:51.000000 spaceandtime-1.1.8/src/spaceandtime/sxtbiscuits.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     1666 2023-10-12 22:46:04.000000 spaceandtime-1.1.8/src/spaceandtime/sxtenums.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     1309 2023-10-12 22:46:04.000000 spaceandtime-1.1.8/src/spaceandtime/sxtexceptions.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    13104 2023-10-15 18:01:59.000000 spaceandtime-1.1.8/src/spaceandtime/sxtkeymanager.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    42744 2023-10-15 19:41:17.000000 spaceandtime-1.1.8/src/spaceandtime/sxtresource.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    13398 2023-10-15 18:02:06.000000 spaceandtime-1.1.8/src/spaceandtime/sxtuser.py
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2023-10-15 19:43:37.798201 spaceandtime-1.1.8/src/spaceandtime.egg-info/
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     9642 2023-10-15 19:43:37.000000 spaceandtime-1.1.8/src/spaceandtime.egg-info/PKG-INFO
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)      631 2023-10-15 19:43:37.000000 spaceandtime-1.1.8/src/spaceandtime.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)        1 2023-10-15 19:43:37.000000 spaceandtime-1.1.8/src/spaceandtime.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)       56 2023-10-15 19:43:37.000000 spaceandtime-1.1.8/src/spaceandtime.egg-info/entry_points.txt
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)       98 2023-10-15 19:43:37.000000 spaceandtime-1.1.8/src/spaceandtime.egg-info/requires.txt
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)       13 2023-10-15 19:43:37.000000 spaceandtime-1.1.8/src/spaceandtime.egg-info/top_level.txt
```

### Comparing `spaceandtime-1.1.7/LICENSE` & `spaceandtime-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spaceandtime-1.1.7/PKG-INFO` & `spaceandtime-1.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Metadata-Version: 2.1
 Name: spaceandtime
-Version: 1.1.7
+Version: 1.1.8
 Summary: SDK for Space and Time verifiable database
-Home-page: https://github.com/spaceandtimelabs/SxT-Python-SDK
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
-Author: Stephen Hilton
 Author-email: Stephen Hilton <stephen.hilton@spaceandtime.io>
 License: MIT License
         
         Copyright (c) 2023 Space and Time
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `spaceandtime-1.1.7/README.md` & `spaceandtime-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `spaceandtime-1.1.7/pyproject.toml` & `spaceandtime-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spaceandtime"
-version = "1.1.7"
+version = "1.1.8"
 description = "SDK for Space and Time verifiable database"
 authors = [{ name = "Stephen Hilton", email = "stephen.hilton@spaceandtime.io" }]
 readme = "README.md"
 requires-python = ">=3.11"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `spaceandtime-1.1.7/src/spaceandtime/__main__.py` & `spaceandtime-1.1.8/src/spaceandtime/__main__.py`

 * *Files identical despite different names*

### Comparing `spaceandtime-1.1.7/src/spaceandtime/apiversions.json` & `spaceandtime-1.1.8/src/spaceandtime/apiversions.json`

 * *Files identical despite different names*

### Comparing `spaceandtime-1.1.7/src/spaceandtime/spaceandtime.py` & `spaceandtime-1.1.8/src/spaceandtime/spaceandtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging, random, time, json
 from datetime import datetime
 from pathlib import Path
-from .sxtuser import SXTUser
-from .sxtresource import SXTTable, SXTView
-from .sxtkeymanager import SXTKeyManager
-from .sxtenums import *
-from .sxtexceptions import *
+from sxtuser import SXTUser
+from sxtresource import SXTTable, SXTView
+from sxtkeymanager import SXTKeyManager
+from sxtenums import *
+from sxtexceptions import *
 
 class SpaceAndTime:
 
     user: SXTUser = None 
     application_name: str = 'SxT-SDK'
     network_calls_enabled:bool = True
     discovery = None
```

### Comparing `spaceandtime-1.1.7/src/spaceandtime/sxtbaseapi.py` & `spaceandtime-1.1.8/src/spaceandtime/sxtbaseapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .sxtbiscuits import SXTBiscuit
 
 
 class SXTBaseAPI():
     api_url = 'https://api.spaceandtime.app'
     access_token = ''
     logger: logging.Logger
+    network_calls_enabled:bool = True
     standard_headers = {
                     "accept": "application/json",
                     "content-type": "application/json"
                     }
     versions = {}
 
 
@@ -161,15 +162,29 @@
             match request_type:
                 case SXTApiCallTypes.POST   : callfunc = requests.post
                 case SXTApiCallTypes.GET    : callfunc = requests.get
                 case SXTApiCallTypes.PUT    : callfunc = requests.put
                 case SXTApiCallTypes.DELETE : callfunc = requests.delete
                 case _: raise SxTArgumentError('Call type must be SXTApiCallTypes enum.', logger=self.logger)
 
-            response = callfunc(url=url, data=json.dumps(data_parms), headers=headers)
+            if self.network_calls_enabled:
+                response = callfunc(url=url, data=json.dumps(data_parms), headers=headers)
+            else:
+                if endpoint in ['sql','sql/dql']:
+                    rtn = [{'id':'1', 'str':'a','this_record':'is a test'}]
+                    rtn.append( {'id':'2', 'str':'b','this_record':'is a test'} )
+                    rtn.append( {'id':'3', 'str':'c','this_record':'is a test'} )
+                    return True, rtn
+                else:
+                    return True, {'authCode':'469867d9660b67f8aa12b2'
+                                ,'accessToken':'eyJ0eXBlIjoiYWNjZXNzIiwia2lkIjUxNDVkYmQtZGNmYi00ZjI4LTg3NzItZjVmNjNlMzcwM2JlIiwiYWxnIjoiRVMyNTYifQ.eyJpYXQiOjE2OTczOTM1MDIsIm5iZiI6MTY5NzM5MzUwMiwiZXhwIjoxNjk3Mzk1MDAyLCJ0eXBlIjoiYWNjZXNzIiwidXNlciI6InN0ZXBoZW4iLCJzdWJzY3JpcHRpb24iOiIzMWNiMGI0Yi0xMjZlLTRlM2MtYTdhMS1lNWRmNDc4YTBjMDUiLCJzZXNzaW9uIjoiMzNiNGRhMzYxZjZiNTM3MjZlYmYyNzU4Iiwic3NuX2V4cCI6MTY5NzQ3OTkwMjMxNSwiaXRlcmF0aW9uIjoiNDEwY2YyZTgyYWZlODdmNDRiMzE4NDFiIn0.kpvrG-ro13P1YeMF6sjLh8wn1rO3jpCVeTrzhDe16ZmJu4ik1amcYz9uQff_XQcwBDrpnCeD5ZZ9mHqb_basew'
+                                ,'refreshToken':'eyJ0eXBlIjoicmVmcmVzaCIsImtpZCITQ1ZGJkLWRjZmItNGYyOC04NzcyLWY1ZjYzZTM3MDNiZSIsImFsZyI6IkVTMjU2In0.eyJpYXQiOjE2OTczOTM1MDIsIm5iZiI6MTY5NzM5MzUwMiwiZXhwIjoxNjk3Mzk1MzAyLCJ0eXBlIjoicmVmcmVzaCIsInVzZXIiOiJzdGVwaGVuIiwic3Vic2NyaXB0aW9uIjoiMzFjYjBiNGItMTI2ZS00ZTNjLWE3YTEtZTVkZjQ3OGEwYzA1Iiwic2Vzc2lvbiI6IjMzYjRkYTM2MWY2YjUzNzI2ZWJmMjc1OCIsInNzbl9leHAiOjE2OTc0Nzk5MDIzMTUsIml0ZXJhdGlvbiI6IjQxMGNmMmU4MmFmZTg3ZjQ0YjMxODQxYiJ9.3vVYpTGBjXIejlaacaZOh_59O9ETfbvTCWvldoi0ojyXTRkTmENVpQRbw7av7yMM2jA7SRdEPQGGjYmThCfk9w'
+                                ,'accessTokenExpires':1973950023160
+                                ,'refreshTokenExpires':1973953023160
+                                }
             txt = 'response.text not available'
             txt = response.text
             response.raise_for_status()
 
             try:
                 rtn = response.json()
             except json.decoder.JSONDecodeError as ex:
@@ -452,15 +467,14 @@
 
         Args: 
             sql_text (str): SQL query text to execute. Note, there is NO placeholder replacement.
             resources (list): List of Resources ("schema.table_name") in the sql_text. 
             biscuits (list): (optional) List of biscuit tokens for permissioned tables. If only querying public tables, this is not needed.
             app_name (str): (optional) Name that will appear in querylog, used for bucketing workload.
 
-
         Returns:
             bool: Success flag (True/False) indicating the api call worked as expected.
             object: Response information from the Space and Time network, as list or dict(json). 
         """
         if type(resources) != list: resources = [resources]
         headers = { 'originApp': app_name } if app_name else {}
         sql_text = self.prep_sql(sql_text=sql_text)
```

### Comparing `spaceandtime-1.1.7/src/spaceandtime/sxtbiscuits.py` & `spaceandtime-1.1.8/src/spaceandtime/sxtbiscuits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging, json
 from pathlib import Path
 from datetime import datetime
 from biscuit_auth import KeyPair, PrivateKey, PublicKey, Authorizer, Biscuit, BiscuitBuilder, BlockBuilder, Rule, DataLogError
-from .sxtexceptions import SxTArgumentError, SxTFileContentError, SxTBiscuitError, SxTKeyEncodingError
-from .sxtenums import SXTPermission, SXTKeyEncodings
-from .sxtkeymanager import SXTKeyManager
+from sxtexceptions import SxTArgumentError, SxTFileContentError, SxTBiscuitError, SxTKeyEncodingError
+from sxtenums import SXTPermission, SXTKeyEncodings
+from sxtkeymanager import SXTKeyManager
 
 
 
 class SXTBiscuit():
     """Definition of a single biscuit."""
 
     logger: logging.Logger = None
```

### Comparing `spaceandtime-1.1.7/src/spaceandtime/sxtenums.py` & `spaceandtime-1.1.8/src/spaceandtime/sxtenums.py`

 * *Files identical despite different names*

### Comparing `spaceandtime-1.1.7/src/spaceandtime/sxtexceptions.py` & `spaceandtime-1.1.8/src/spaceandtime/sxtexceptions.py`

 * *Files identical despite different names*

### Comparing `spaceandtime-1.1.7/src/spaceandtime/sxtkeymanager.py` & `spaceandtime-1.1.8/src/spaceandtime/sxtkeymanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging, base64
 from pathlib import Path 
 import nacl.signing
 from biscuit_auth import KeyPair, PrivateKey 
-from .sxtexceptions import SxTKeyEncodingError, SxTArgumentError, SxTBiscuitError
-from .sxtenums import SXTPermission, SXTKeyEncodings
+from sxtexceptions import SxTKeyEncodingError, SxTArgumentError, SxTBiscuitError
+from sxtenums import SXTPermission, SXTKeyEncodings
 
 
 
 ####
 #### SXT KEY MANAGER
 ####
 class SXTKeyManager():
```

### Comparing `spaceandtime-1.1.7/src/spaceandtime/sxtresource.py` & `spaceandtime-1.1.8/src/spaceandtime/sxtresource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging, datetime, json, random
 from pathlib import Path
-from .sxtenums import SXTResourceType, SXTPermission, SXTKeyEncodings, SXTTableAccessType
+from sxtenums import SXTResourceType, SXTPermission, SXTKeyEncodings, SXTTableAccessType
 from .sxtexceptions import SxTArgumentError, SxTFileContentError
 from .sxtbiscuits import SXTBiscuit
 from .sxtkeymanager import SXTKeyManager
 from .sxtuser import SXTUser
 
 class SXTResource():
     # child objects should override: self.__with__, has_with_statement(), self.resource_type
@@ -580,29 +580,102 @@
     def table_name(self) ->str:
         return self.resource_name
     @table_name.setter
     def table_name(self, value):
         self.resource_name = value
 
 
+    def get_column_names(self) -> dict:
+        """Returns a dictonary of column_name : data_type as defined in the create_ddl.
+        
+        Useful when an iterable list of columns (and types) is required, such as building 
+        INSERT statements or view SELECT lists.  Order should be preserved, although as a dict 
+        object type, this is technically not gauranteed.
+        """
+        rtn = {}
+
+        # prep ddl to isolate columns 
+        ddl = str(self.create_ddl).replace('\t',' ').replace('\n',' ').strip()
+        while '  ' in ddl: ddl = ddl.replace('  ',' ')
+        first_paren = ddl.find('(')+1
+        for i in range(len(ddl), 1, -1):
+            if ddl[i:i+1] == ')': 
+                last_paren = i 
+                break
+        
+        # process columns
+        cols = [c.strip() for c in ddl[first_paren:last_paren].split(',') ]
+        for col in cols:
+            if col.lower().startswith('primary key'): continue
+            colname = col.split(' ')[0]
+            coltype = col.split(' ')[1]
+            rtn[colname] = coltype
+
+        return rtn 
+
+
     def insert(self, sql_text:str = None, columns:list = None, data:list = None, user:SXTUser = None, biscuits:list = None):
+        """-----------------
+        Inserts records into the table, in one DML request per 1000 rows.
+
+        The process uses a column list and data list (rather than a single dictionary) because the multi-row 
+        insert syntax requires a single column definition, with all data rows expected to follow that same 
+        order and completeness. This also adheres better to common high-volumn analytic formats like CSV, 
+        where repeating column definitions becomes onerous.  NOTE: this submits in 1000 row transactions, 
+        so it is possible to have partially successful loads (in 1000 row chunks). Once any part insert fails
+        the holistic process stops and reports an error, and reports Success = False.
+
+        Args:
+            sql_text (str): If set, columns and data are ignored and this SQL text is simply passed thru to the network directly as a DML request.
+            columns (list): List of columns to build the INSERT statement. Order must match the data list.
+            data (list): List of data that matches the columns order.  
+            user (SXTUser): User who will execute the request. Defaults to the default user.
+            biscuits (list): List of biscuits required to authorize this request. 
+
+        Returns: 
+            bool: Success flag, True if the data was fully inserted, False if any of the records failed.
+            object: Row output of the SQL request, in JSON format, or if error, details returned from the request.
+        """
         user = self.get_first_valid_user(user)
         if not biscuits: biscuits = list(self.biscuits) 
         if biscuits == []: 
             raise SxTArgumentError('A biscuit with INSERT permissions must be included.', logger=self.logger)
         if not sql_text:
-            sql_text_prefix = f"INSERT INTO {self.table_name} ({ ', '.join(columns) }) VALUES \n"
-            sql_text_rows = []
-            for row in data:
-                sql_text_rows.append( "('" + str("', '").join([str(val) for val in row]) + "')" )
-            sql_text = sql_text_prefix + ',\n'.join(sql_text_rows)
-        return user.base_api.sql_dml(sql_text=sql_text, biscuits=biscuits, app_name=self.application_name,resources=[self.table_name])
+            while data !=[]:
+                sql_text_prefix = f"INSERT INTO {self.table_name} ({ ', '.join(columns) }) VALUES \n"
+                sql_text_rows = []
+                for row in data[:999]:
+                    sql_text_rows.append( "('" + str("', '").join([str(val) for val in row]) + "')" )
+                sql_text = sql_text_prefix + ',\n'.join(sql_text_rows)
+                success, response = user.base_api.sql_dml(sql_text=sql_text, biscuits=biscuits, app_name=self.application_name,resources=[self.table_name])
+                data = data[999:]
+            if not success: 
+                msg = 'NOTE: data may have been left in a partially inserted state.'
+                response['warning'] = msg
+                self.logger.error(msg)
+                return success, response
+        return success, response
 
 
     def delete(self, sql_text:str = None, where:str = '0=1', user:SXTUser = None, biscuits:list = None):
+        """--------------------
+        Deletes records from the table, with a required WHERE statement.
+
+        Note, some tables in the space and time network are immutable and cannot be changed.
+
+        Args: 
+            sql_text (str): If set, the sql_text is simply passed thru to the network directly as a DML request.
+            where (str): A WHERE statement to limit rows deleted. This defaults to a zero-delete statement, so must be overriden to execute a meaningful delete. 
+            user (SXTUser): User who will execute the request. Defaults to the default user.
+            biscuits (list): List of biscuits required to authorize this request. 
+
+        Returns: 
+            bool: Success flag, True if the data was fully inserted, False if any of the records failed.
+            object: Row output of the SQL request, in JSON format, or if error, details returned from the request.
+        """
         user = self.get_first_valid_user(user)
         if not biscuits: biscuits = list(self.biscuits) 
         if biscuits == []: 
             raise SxTArgumentError('A biscuit with DELETE permissions must be included.', logger=self.logger)
         if len(where) >0 and not str(where).strip().startswith('where'): where = f' WHERE {where} '
         if not sql_text: sql_text = f"DELETE FROM {self.table_name} {where}"
         return user.base_api.sql_dml(sql_text=sql_text, biscuits=biscuits, app_name=self.application_name, resources=[self.table_name])
@@ -758,14 +831,16 @@
         CREATE TABLE {table_name} 
         ( MyID         int
         , MyName       varchar
         , MyDate       date
         , Primary Key  (MyID) 
         )  
     """
+    print( tableA.get_column_names() )
+
     tableA.save()  # save to local file, to prevent lost keys
     success, results = tableA.create()  # Create table on Space and Time network
     
 
     if success:
 
         # generate some dummy data
```

### Comparing `spaceandtime-1.1.7/src/spaceandtime/sxtuser.py` & `spaceandtime-1.1.8/src/spaceandtime/sxtuser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os, logging, datetime 
-from .sxtexceptions import SxTAuthenticationError, SxTArgumentError
-from .sxtkeymanager import SXTKeyManager, SXTKeyEncodings
-from .sxtbaseapi import SXTBaseAPI, SXTApiCallTypes 
+from sxtexceptions import SxTAuthenticationError, SxTArgumentError
+from sxtkeymanager import SXTKeyManager, SXTKeyEncodings
+from sxtbaseapi import SXTBaseAPI, SXTApiCallTypes 
 from pathlib import Path
 from dotenv import load_dotenv
 
 class SXTUser():
     user_id: str = ''
     api_url: str = ''
     logger: logging.Logger = None
```

### Comparing `spaceandtime-1.1.7/src/spaceandtime.egg-info/PKG-INFO` & `spaceandtime-1.1.8/src/spaceandtime.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Metadata-Version: 2.1
 Name: spaceandtime
-Version: 1.1.7
+Version: 1.1.8
 Summary: SDK for Space and Time verifiable database
-Home-page: https://github.com/spaceandtimelabs/SxT-Python-SDK
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
-Author: Stephen Hilton
 Author-email: Stephen Hilton <stephen.hilton@spaceandtime.io>
 License: MIT License
         
         Copyright (c) 2023 Space and Time
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `spaceandtime-1.1.7/src/spaceandtime.egg-info/SOURCES.txt` & `spaceandtime-1.1.8/src/spaceandtime.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.py
 src/spaceandtime/__init__.py
 src/spaceandtime/__main__.py
 src/spaceandtime/apiversions.json
 src/spaceandtime/spaceandtime.py
 src/spaceandtime/sxtbaseapi.py
 src/spaceandtime/sxtbiscuits.py
 src/spaceandtime/sxtenums.py
```

