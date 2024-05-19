# Comparing `tmp/pydiscovergy-3.0.0.tar.gz` & `tmp/pydiscovergy-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiscovergy-3.0.0.tar", max compression
+gzip compressed data, was "pydiscovergy-3.0.1.tar", max compression
```

## Comparing `pydiscovergy-3.0.0.tar` & `pydiscovergy-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1081 2024-02-24 18:38:21.190957 pydiscovergy-3.0.0/LICENSE
--rw-r--r--   0        0        0     4933 2024-02-24 18:38:21.190957 pydiscovergy-3.0.0/README.md
--rw-r--r--   0        0        0      102 2024-02-24 18:38:21.190957 pydiscovergy-3.0.0/pydiscovergy/__init__.py
--rw-r--r--   0        0        0      330 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/authentication/__init__.py
--rw-r--r--   0        0        0      565 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/authentication/base.py
--rw-r--r--   0        0        0      720 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/authentication/basicauth.py
--rw-r--r--   0        0        0     7484 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/authentication/token.py
--rw-r--r--   0        0        0      680 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/const.py
--rw-r--r--   0        0        0     6660 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/discovergy.py
--rw-r--r--   0        0        0      593 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/error.py
--rw-r--r--   0        0        0     3273 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/models.py
--rw-r--r--   0        0        0        0 2024-02-24 18:38:21.194957 pydiscovergy-3.0.0/pydiscovergy/py.typed
--rw-r--r--   0        0        0     3860 2024-02-24 18:38:32.242978 pydiscovergy-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 pydiscovergy-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/LICENSE
+-rw-r--r--   0        0        0     4956 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/README.md
+-rw-r--r--   0        0        0      103 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/__init__.py
+-rw-r--r--   0        0        0      330 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/authentication/__init__.py
+-rw-r--r--   0        0        0      566 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/authentication/base.py
+-rw-r--r--   0        0        0      720 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/authentication/basicauth.py
+-rw-r--r--   0        0        0     7453 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/authentication/token.py
+-rw-r--r--   0        0        0      678 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/const.py
+-rw-r--r--   0        0        0     6661 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/discovergy.py
+-rw-r--r--   0        0        0      593 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/error.py
+-rw-r--r--   0        0        0     3274 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/models.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:10:34.810541 pydiscovergy-3.0.1/pydiscovergy/py.typed
+-rw-r--r--   0        0        0     3861 2024-05-19 18:10:55.174665 pydiscovergy-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 pydiscovergy-3.0.1/PKG-INFO
```

### Comparing `pydiscovergy-3.0.0/LICENSE` & `pydiscovergy-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiscovergy-3.0.0/README.md` & `pydiscovergy-3.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE.md)
 
 [![Build Status][build-shield]][build]
 [![Code Coverage][codecov-shield]][codecov]
 
-Asynchronous Python client for Discovergy smart meter using their API.
+Asynchronous Python client for inexogy (former Discovergy) smart meter using their API.
 
 ## About
 
-This package allows you to fetch data from api.discovergy.com.
+This package allows you to fetch data from api.inexogy.com.
 
 ## Installation
 
 ```bash
 pip install pydiscovergy
 ```
 
@@ -30,15 +30,15 @@
 
 async def main():
     discovergy = Discovergy(email="demo@example.com", password="demo")
     meters = await discovergy.meters()
 
     for meter in meters:
         if meter.meter_id == "abc123":
-            reading = await discovergy.meter_last_reading(meter.meter_id)
+            reading = await discovergy.meter_last_reading(meter_id=meter.meter_id)
             print(f"Last reading: {reading.values['energy']} kWh")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## Changelog & Releases
```

### Comparing `pydiscovergy-3.0.0/pydiscovergy/authentication/base.py` & `pydiscovergy-3.0.1/pydiscovergy/authentication/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base authentication module for Discovergy API."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
 from httpx import AsyncClient  # noqa: TCH002
```

### Comparing `pydiscovergy-3.0.0/pydiscovergy/authentication/basicauth.py` & `pydiscovergy-3.0.1/pydiscovergy/authentication/basicauth.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-3.0.0/pydiscovergy/authentication/token.py` & `pydiscovergy-3.0.1/pydiscovergy/authentication/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Authentication module for token auth."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 import json
 from urllib.parse import parse_qs
 
 from authlib.integrations.httpx_client import AsyncOAuth1Client
@@ -154,15 +155,15 @@
                 oauth_token_response = await client.fetch_request_token(
                     API_REQUEST_TOKEN,
                 )
                 return RequestToken(
                     oauth_token_response.get("oauth_token"),
                     oauth_token_response.get("oauth_token_secret"),
                 )
-            except Exception as exc:  # noqa: BLE001
+            except Exception as exc:
                 msg = f"Request failed: {exc}"
                 raise HTTPError(msg) from exc
 
     async def _authorize_request_token(
         self,
         email: str,
         password: str,
@@ -214,10 +215,10 @@
                     API_ACCESS_TOKEN,
                     verifier,
                 )
                 return AccessToken(
                     access_token_response.get("oauth_token"),
                     access_token_response.get("oauth_token_secret"),
                 )
-            except Exception as exc:  # noqa: BLE001
+            except Exception as exc:
                 msg = f"Request failed: {exc}"
                 raise HTTPError(msg) from exc
```

### Comparing `pydiscovergy-3.0.0/pydiscovergy/discovergy.py` & `pydiscovergy-3.0.1/pydiscovergy/discovergy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Discovergy API."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import UTC, datetime
 from typing import Any
 
 import httpx
```

### Comparing `pydiscovergy-3.0.0/pydiscovergy/error.py` & `pydiscovergy-3.0.1/pydiscovergy/error.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-3.0.0/pydiscovergy/models.py` & `pydiscovergy-3.0.1/pydiscovergy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Models for Discovergy API."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from datetime import UTC, datetime
 from typing import Any, Self
 
 from mashumaro.config import BaseConfig
```

### Comparing `pydiscovergy-3.0.0/pyproject.toml` & `pydiscovergy-3.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiscovergy"
-version = "3.0.0"
+version = "3.0.1"
 description = "Async Python 3 library for interacting with Discovergy smart meters API"
 authors = ["Jan-Philipp Benecke <jan-philipp@bnck.me>"]
 repository = "https://github.com/jpbede/pydiscovergy"
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "pydiscovergy" }
@@ -28,26 +28,26 @@
 pytz = ">=2023.3"
 mashumaro = ">=3.11"
 orjson = ">=3.9.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
-coverage = {version = "7.4.3", extras = ["toml"]}
-pre-commit = "3.6.2"
-pre-commit-hooks = "4.5.0"
-pylint = "3.0.4"
+coverage = {version = "7.5.1", extras = ["toml"]}
+pre-commit = "3.7.1"
+pre-commit-hooks = "4.6.0"
+pylint = "3.1.0"
 pytest = "7.4.4"
-pytest-asyncio = "==0.23.5"
-pytest-cov = "4.1.0"
-respx = "0.20.2"
+pytest-asyncio = "==0.23.6"
+pytest-cov = "5.0.0"
+respx = "0.21.1"
 pytest-httpx = "0.30.0"
-mypy = "1.8.0"
-ruff = "0.2.2"
-safety = "3.0.1"
+mypy = "1.10.0"
+ruff = "0.4.2"
+safety = "3.1.0"
 yamllint = "1.35.1"
 types-pytz = "^2023.3.1.1"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/jpbede/pydiscovergy/issues"
 Changelog = "https://github.com/jpbede/pydiscovergy/releases"
```

### Comparing `pydiscovergy-3.0.0/PKG-INFO` & `pydiscovergy-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiscovergy
-Version: 3.0.0
+Version: 3.0.1
 Summary: Async Python 3 library for interacting with Discovergy smart meters API
 Home-page: https://github.com/jpbede/pydiscovergy
 License: MIT
 Keywords: discovergy,smart meter,smart home
 Author: Jan-Philipp Benecke
 Author-email: jan-philipp@bnck.me
 Requires-Python: >=3.11,<4.0
@@ -34,19 +34,19 @@
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE.md)
 
 [![Build Status][build-shield]][build]
 [![Code Coverage][codecov-shield]][codecov]
 
-Asynchronous Python client for Discovergy smart meter using their API.
+Asynchronous Python client for inexogy (former Discovergy) smart meter using their API.
 
 ## About
 
-This package allows you to fetch data from api.discovergy.com.
+This package allows you to fetch data from api.inexogy.com.
 
 ## Installation
 
 ```bash
 pip install pydiscovergy
 ```
 
@@ -59,15 +59,15 @@
 
 async def main():
     discovergy = Discovergy(email="demo@example.com", password="demo")
     meters = await discovergy.meters()
 
     for meter in meters:
         if meter.meter_id == "abc123":
-            reading = await discovergy.meter_last_reading(meter.meter_id)
+            reading = await discovergy.meter_last_reading(meter_id=meter.meter_id)
             print(f"Last reading: {reading.values['energy']} kWh")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## Changelog & Releases
```

