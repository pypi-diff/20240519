# Comparing `tmp/crownstone-sse-2.0.4.tar.gz` & `tmp/crownstone_sse-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crownstone-sse-2.0.4.tar", last modified: Thu Sep 15 12:25:39 2022, max compression
+gzip compressed data, was "crownstone_sse-2.0.5.tar", last modified: Sun May 19 20:12:57 2024, max compression
```

## Comparing `crownstone-sse-2.0.4.tar` & `crownstone_sse-2.0.5.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)    10484 2022-09-15 12:24:39.000000 crownstone-sse-2.0.4/README.md
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       20 2021-11-26 16:24:06.000000 crownstone-sse-2.0.4/requirements.txt
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/crownstone_sse.egg-info/
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       21 2022-09-15 12:25:38.000000 crownstone-sse-2.0.4/crownstone_sse.egg-info/top_level.txt
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)    13753 2022-09-15 12:25:38.000000 crownstone-sse-2.0.4/crownstone_sse.egg-info/PKG-INFO
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     1023 2022-09-15 12:25:38.000000 crownstone-sse-2.0.4/crownstone_sse.egg-info/SOURCES.txt
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       21 2022-09-15 12:25:38.000000 crownstone-sse-2.0.4/crownstone_sse.egg-info/requires.txt
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)        1 2022-09-15 12:25:38.000000 crownstone-sse-2.0.4/crownstone_sse.egg-info/dependency_links.txt
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/crownstone_sse/
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/crownstone_sse/helpers/
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     1625 2021-08-10 09:22:38.000000 crownstone-sse-2.0.4/crownstone_sse/helpers/switch_command.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)      847 2021-08-10 09:22:38.000000 crownstone-sse-2.0.4/crownstone_sse/helpers/aiohttp_client.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       51 2021-05-03 11:30:22.000000 crownstone-sse-2.0.4/crownstone_sse/helpers/__init__.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     8358 2022-09-15 12:24:39.000000 crownstone-sse-2.0.4/crownstone_sse/events.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     3006 2022-09-15 12:24:39.000000 crownstone-sse-2.0.4/crownstone_sse/const.py
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/crownstone_sse/util/
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     2530 2021-08-10 09:22:38.000000 crownstone-sse-2.0.4/crownstone_sse/util/eventbus.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)        0 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/crownstone_sse/util/__init__.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     1698 2022-09-15 12:24:39.000000 crownstone-sse-2.0.4/crownstone_sse/exceptions.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)    11705 2022-09-15 12:24:39.000000 crownstone-sse-2.0.4/crownstone_sse/async_client.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     1148 2022-09-15 12:25:31.000000 crownstone-sse-2.0.4/crownstone_sse/__init__.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     2683 2022-09-15 12:24:39.000000 crownstone-sse-2.0.4/crownstone_sse/client.py
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)    13753 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/PKG-INFO
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       38 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/setup.cfg
--rw-rw-r--   0 vliedel   (1000) vliedel   (1000)      702 2022-09-15 12:25:31.000000 crownstone-sse-2.0.4/setup.py
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/tests/
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/tests/mock_classes/
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)        0 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mock_classes/__init__.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)      611 2020-11-10 15:20:07.000000 crownstone-sse-2.0.4/tests/mock_classes/response.py
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/tests/mocked_events/
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)     1146 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mocked_events/presence_events.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)      495 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mocked_events/system_events.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)      309 2020-10-26 16:17:24.000000 crownstone-sse-2.0.4/tests/mocked_events/switch_state_update_events.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)        0 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mocked_events/__init__.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)      317 2020-10-26 16:17:21.000000 crownstone-sse-2.0.4/tests/mocked_events/command_events.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)     3380 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mocked_events/data_change_events.py
-drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2022-09-15 12:25:39.000000 crownstone-sse-2.0.4/tests/mocked_replies/
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)      141 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mocked_replies/login_data.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)      232 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mocked_replies/stream_response.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)        0 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mocked_replies/__init__.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)      381 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/tests/mocked_replies/login_errors.py
--rw-r--r--   0 vliedel   (1000) vliedel   (1000)       24 2020-10-15 10:58:58.000000 crownstone-sse-2.0.4/MANIFEST.in
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.506754 crownstone_sse-2.0.5/
+-rw-r--r--   0 ricardo   (1000) users      (100)    10792 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/LICENSE-APACHE
+-rw-r--r--   0 ricardo   (1000) users      (100)     7651 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/LICENSE-LGPL
+-rw-r--r--   0 ricardo   (1000) users      (100)     1082 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/LICENSE-MIT
+-rw-r--r--   0 ricardo   (1000) users      (100)       24 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/MANIFEST.in
+-rw-r--r--   0 ricardo   (1000) users      (100)    12269 2024-05-19 20:12:57.506754 crownstone_sse-2.0.5/PKG-INFO
+-rw-r--r--   0 ricardo   (1000) users      (100)    11660 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/README.md
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.504754 crownstone_sse-2.0.5/crownstone_sse/
+-rw-r--r--   0 ricardo   (1000) users      (100)     1148 2024-05-19 18:37:18.000000 crownstone_sse-2.0.5/crownstone_sse/__init__.py
+-rw-r--r--   0 ricardo   (1000) users      (100)    11845 2024-05-19 18:29:13.000000 crownstone_sse-2.0.5/crownstone_sse/async_client.py
+-rw-r--r--   0 ricardo   (1000) users      (100)     2683 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/crownstone_sse/client.py
+-rw-r--r--   0 ricardo   (1000) users      (100)     3085 2024-05-10 15:18:27.000000 crownstone_sse-2.0.5/crownstone_sse/const.py
+-rw-r--r--   0 ricardo   (1000) users      (100)     8358 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/crownstone_sse/events.py
+-rw-r--r--   0 ricardo   (1000) users      (100)     1698 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/crownstone_sse/exceptions.py
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.505755 crownstone_sse-2.0.5/crownstone_sse/helpers/
+-rw-r--r--   0 ricardo   (1000) users      (100)       51 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/crownstone_sse/helpers/__init__.py
+-rw-r--r--   0 ricardo   (1000) users      (100)      847 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/crownstone_sse/helpers/aiohttp_client.py
+-rw-r--r--   0 ricardo   (1000) users      (100)     1625 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/crownstone_sse/helpers/switch_command.py
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.505755 crownstone_sse-2.0.5/crownstone_sse/util/
+-rw-r--r--   0 ricardo   (1000) users      (100)        0 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/crownstone_sse/util/__init__.py
+-rw-r--r--   0 ricardo   (1000) users      (100)     2530 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/crownstone_sse/util/eventbus.py
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.506754 crownstone_sse-2.0.5/crownstone_sse.egg-info/
+-rw-r--r--   0 ricardo   (1000) users      (100)    12269 2024-05-19 20:12:57.000000 crownstone_sse-2.0.5/crownstone_sse.egg-info/PKG-INFO
+-rw-r--r--   0 ricardo   (1000) users      (100)     1063 2024-05-19 20:12:57.000000 crownstone_sse-2.0.5/crownstone_sse.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardo   (1000) users      (100)        1 2024-05-19 20:12:57.000000 crownstone_sse-2.0.5/crownstone_sse.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardo   (1000) users      (100)       21 2024-05-19 20:12:57.000000 crownstone_sse-2.0.5/crownstone_sse.egg-info/requires.txt
+-rw-r--r--   0 ricardo   (1000) users      (100)       21 2024-05-19 20:12:57.000000 crownstone_sse-2.0.5/crownstone_sse.egg-info/top_level.txt
+-rw-r--r--   0 ricardo   (1000) users      (100)       20 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/requirements.txt
+-rw-r--r--   0 ricardo   (1000) users      (100)       38 2024-05-19 20:12:57.506754 crownstone_sse-2.0.5/setup.cfg
+-rw-r--r--   0 ricardo   (1000) users      (100)      812 2024-05-19 18:36:22.000000 crownstone_sse-2.0.5/setup.py
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.503754 crownstone_sse-2.0.5/tests/
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.505755 crownstone_sse-2.0.5/tests/mock_classes/
+-rw-r--r--   0 ricardo   (1000) users      (100)        0 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mock_classes/__init__.py
+-rw-r--r--   0 ricardo   (1000) users      (100)      611 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mock_classes/response.py
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.506754 crownstone_sse-2.0.5/tests/mocked_events/
+-rw-r--r--   0 ricardo   (1000) users      (100)        0 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_events/__init__.py
+-rw-r--r--   0 ricardo   (1000) users      (100)      317 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_events/command_events.py
+-rw-r--r--   0 ricardo   (1000) users      (100)     3380 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_events/data_change_events.py
+-rw-r--r--   0 ricardo   (1000) users      (100)     1146 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_events/presence_events.py
+-rw-r--r--   0 ricardo   (1000) users      (100)      309 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_events/switch_state_update_events.py
+-rw-r--r--   0 ricardo   (1000) users      (100)      495 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_events/system_events.py
+drwxr-xr-x   0 ricardo   (1000) users      (100)        0 2024-05-19 20:12:57.506754 crownstone_sse-2.0.5/tests/mocked_replies/
+-rw-r--r--   0 ricardo   (1000) users      (100)        0 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_replies/__init__.py
+-rw-r--r--   0 ricardo   (1000) users      (100)      141 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_replies/login_data.py
+-rw-r--r--   0 ricardo   (1000) users      (100)      381 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_replies/login_errors.py
+-rw-r--r--   0 ricardo   (1000) users      (100)      232 2024-05-10 14:54:11.000000 crownstone_sse-2.0.5/tests/mocked_replies/stream_response.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `crownstone-sse-2.0.4/README.md` & `crownstone_sse-2.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -349,7 +349,37 @@
 Tests are not available yet for this version. The client has however been live tested on the following:
 1. Logging in with Crownstone credentials.
 2. Establishing a connection to the Crownstone SSE server.
 3. Tested the connection staying alive for longer than 10 minutes (no total timeout).
 4. Tested client reconnection by manually disabling internet, waiting over 35 seconds, and turning it back on.
 5. Tested access token renewal by providing a short TTL on the access token when logging in.
 6. Safely closing the connection and exiting the loop after a manual stop is called, both and running and reconnecting state.
+
+# License
+
+## Open-source license
+
+This software is provided under a noncontagious open-source license towards the open-source community. It's available under three open-source licenses:
+ 
+* License: LGPL v3+, Apache, MIT
+
+<p align="center">
+  <a href="http://www.gnu.org/licenses/lgpl-3.0">
+    <img src="https://img.shields.io/badge/License-LGPL%20v3-blue.svg" alt="License: LGPL v3" />
+  </a>
+  <a href="https://opensource.org/licenses/MIT">
+    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT" />
+  </a>
+  <a href="https://opensource.org/licenses/Apache-2.0">
+    <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License: Apache 2.0" />
+  </a>
+</p>
+
+## Commercial license
+
+This software can also be provided under a commercial license. If you are not an open-source developer or are not planning to release adaptations to the code under one or multiple of the mentioned licenses, contact us to obtain a commercial license.
+
+* License: Crownstone commercial license
+
+# Contact
+
+For any question contact us at <https://crownstone.rocks/contact/> or on our discord server through <https://crownstone.rocks/forum/>.
```

### Comparing `crownstone-sse-2.0.4/crownstone_sse.egg-info/SOURCES.txt` & `crownstone_sse-2.0.5/crownstone_sse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+LICENSE-APACHE
+LICENSE-LGPL
+LICENSE-MIT
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 crownstone_sse/__init__.py
 crownstone_sse/async_client.py
 crownstone_sse/client.py
```

### Comparing `crownstone-sse-2.0.4/crownstone_sse/helpers/switch_command.py` & `crownstone_sse-2.0.5/crownstone_sse/helpers/switch_command.py`

 * *Files identical despite different names*

### Comparing `crownstone-sse-2.0.4/crownstone_sse/helpers/aiohttp_client.py` & `crownstone_sse-2.0.5/crownstone_sse/helpers/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `crownstone-sse-2.0.4/crownstone_sse/events.py` & `crownstone_sse-2.0.5/crownstone_sse/events.py`

 * *Files identical despite different names*

### Comparing `crownstone-sse-2.0.4/crownstone_sse/const.py` & `crownstone_sse-2.0.5/crownstone_sse/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 
 from typing import Final
 
 # Project name
 PROJECT_NAME: Final = "crownstone-lib-python-sse"
 NO_PROJECT_NAME: Final = "no_project_name"
 
-# URLs
-EVENT_BASE_URL: Final = "https://events.crownstone.rocks/sse?accessToken="
-LOGIN_URL: Final = "https://cloud.crownstone.rocks/api/users/login"
+# Addresses / suffixes
+DEFAULT_SSE_ADDR: Final = "https://events.ownstone.org/sse"
+DEFAULT_CLOUD_ADDR: Final = "https://cloud.ownstone.org/api"
+
+SSE_AUTH_SUFFIX: Final = "?accessToken="
+CLOUD_LOGIN_SUFFIX: Final = "/users/login"
 
 # Headers
 CONTENT_TYPE: Final = "text/event-stream"
 NO_CACHE: Final = "no-cache"
 
 # Connection parameters
 RECONNECTION_TIME: Final = 2
```

### Comparing `crownstone-sse-2.0.4/crownstone_sse/util/eventbus.py` & `crownstone_sse-2.0.5/crownstone_sse/util/eventbus.py`

 * *Files identical despite different names*

### Comparing `crownstone-sse-2.0.4/crownstone_sse/exceptions.py` & `crownstone_sse-2.0.5/crownstone_sse/exceptions.py`

 * *Files identical despite different names*

### Comparing `crownstone-sse-2.0.4/crownstone_sse/async_client.py` & `crownstone_sse-2.0.5/crownstone_sse/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """
 Asynchronous iterator class that connects to the Crownstone Cloud,
 and returns received events in data containers.
 
 This class must be used in the event loop.
 """
+
 from __future__ import annotations
 
 import asyncio
 import hashlib
 import json
 import logging
 from enum import Enum, auto
 from typing import Any
 
 import aiohttp
 
 import crownstone_sse
 from crownstone_sse.const import (
+    CLOUD_LOGIN_SUFFIX,
     CONNECTION_TIMEOUT,
     CONTENT_TYPE,
-    EVENT_BASE_URL,
+    DEFAULT_CLOUD_ADDR,
+    DEFAULT_SSE_ADDR,
     EVENT_SYSTEM_NO_CONNECTION,
     EVENT_SYSTEM_TOKEN_EXPIRED,
     EVENT_SYSTEM_TOKEN_INVALID,
     LOGIN_FAILED,
     LOGIN_FAILED_EMAIL_NOT_VERIFIED,
-    LOGIN_URL,
     NO_CACHE,
     NO_PROJECT_NAME,
     PROJECT_NAME,
     RECONNECTION_TIME,
+    SSE_AUTH_SUFFIX,
 )
 from crownstone_sse.events import Event, SystemEvent, parse_event
 from crownstone_sse.exceptions import (
     AuthError,
     ClientError,
     ConnectError,
     CrownstoneAuthException,
@@ -200,15 +203,17 @@
         hashed_password = sha_hash.hexdigest()
 
         # Create JSON object with login credentials
         login_data = {"email": self._email, "password": hashed_password}
 
         try:
             # login
-            response = await self.websession.post(LOGIN_URL, json=login_data)
+            response = await self.websession.post(
+                f"{DEFAULT_CLOUD_ADDR}{CLOUD_LOGIN_SUFFIX}", json=login_data
+            )
             data: dict[str, Any] = await response.json()
             # success
             if response.status == 200:
                 self._access_token = data["id"]
                 _LOGGER.debug("Login successful")
             # auth error
             elif response.status == 401:
@@ -253,15 +258,15 @@
             hasattr(self, "_client_response")
             and getattr(self, "_client_response") is not None
         ):
             self._client_response.close()
 
         try:
             response = await self.websession.get(
-                url=f"{EVENT_BASE_URL}{self._access_token}&projectName={self._project_name}",
+                url=f"{DEFAULT_SSE_ADDR}{SSE_AUTH_SUFFIX}{self._access_token}&projectName={self._project_name}",
                 headers=headers,
                 timeout=sse_timeout,
             )
             # Raises ClientResponseError
             response.raise_for_status()
 
             # aiohttp.ClientResponse instance
```

### Comparing `crownstone-sse-2.0.4/crownstone_sse/__init__.py` & `crownstone_sse-2.0.5/crownstone_sse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     EVENT_SYSTEM_TOKEN_EXPIRED,
     OPERATION_CREATE,
     OPERATION_DELETE,
     OPERATION_UPDATE,
 )
 from crownstone_sse.util.eventbus import EventBus
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
```

### Comparing `crownstone-sse-2.0.4/crownstone_sse/client.py` & `crownstone_sse-2.0.5/crownstone_sse/client.py`

 * *Files identical despite different names*

### Comparing `crownstone-sse-2.0.4/setup.py` & `crownstone_sse-2.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='crownstone-sse',
-    version="2.0.4",
-    url='https://github.com/crownstone/crownstone-lib-python-sse',
+    version="2.0.5",
+    url='https://github.com/Crownstone-Community/crownstone-lib-python-sse',
     author='Crownstone B.V.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['examples', 'tests']),
     install_requires=list(package.strip() for package in open('requirements.txt')),
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12'
     ],
     python_requires='>=3.8',
 )
```

### Comparing `crownstone-sse-2.0.4/tests/mock_classes/response.py` & `crownstone_sse-2.0.5/tests/mock_classes/response.py`

 * *Files identical despite different names*

### Comparing `crownstone-sse-2.0.4/tests/mocked_events/presence_events.py` & `crownstone_sse-2.0.5/tests/mocked_events/presence_events.py`

 * *Files identical despite different names*

### Comparing `crownstone-sse-2.0.4/tests/mocked_events/data_change_events.py` & `crownstone_sse-2.0.5/tests/mocked_events/data_change_events.py`

 * *Files identical despite different names*

