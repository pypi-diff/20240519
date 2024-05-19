# Comparing `tmp/monzopy-1.1.0.tar.gz` & `tmp/monzopy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monzopy-1.1.0.tar", last modified: Mon Apr 22 16:08:49 2024, max compression
+gzip compressed data, was "monzopy-1.2.0.tar", last modified: Sun May 19 12:09:26 2024, max compression
```

## Comparing `monzopy-1.1.0.tar` & `monzopy-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:49.440962 monzopy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 16:08:45.000000 monzopy-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 16:08:49.440962 monzopy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 16:08:45.000000 monzopy-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:49.440962 monzopy-1.1.0/monzopy/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 16:08:45.000000 monzopy-1.1.0/monzopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-22 16:08:45.000000 monzopy-1.1.0/monzopy/monzopy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:45.000000 monzopy-1.1.0/monzopy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:49.440962 monzopy-1.1.0/monzopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 16:08:49.000000 monzopy-1.1.0/monzopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 16:08:49.000000 monzopy-1.1.0/monzopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:08:49.000000 monzopy-1.1.0/monzopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 16:08:49.000000 monzopy-1.1.0/monzopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-22 16:08:45.000000 monzopy-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:08:49.440962 monzopy-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:09:26.491517 monzopy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 12:09:15.000000 monzopy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-19 12:09:26.491517 monzopy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-19 12:09:15.000000 monzopy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:09:26.491517 monzopy-1.2.0/monzopy/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-19 12:09:15.000000 monzopy-1.2.0/monzopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-19 12:09:15.000000 monzopy-1.2.0/monzopy/monzopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:09:15.000000 monzopy-1.2.0/monzopy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:09:26.491517 monzopy-1.2.0/monzopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-19 12:09:26.000000 monzopy-1.2.0/monzopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-19 12:09:26.000000 monzopy-1.2.0/monzopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:09:26.000000 monzopy-1.2.0/monzopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 12:09:26.000000 monzopy-1.2.0/monzopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-19 12:09:15.000000 monzopy-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:09:26.491517 monzopy-1.2.0/setup.cfg
```

### Comparing `monzopy-1.1.0/LICENSE` & `monzopy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monzopy-1.1.0/PKG-INFO` & `monzopy-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monzopy
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple async python wrapper for the Monzo API, used primarily by the Monzo Home Assistant integration.
 Author-email: Jake Martin <jake_martin_@outlook.com>
 Project-URL: Homepage, https://github.com/JakeMartin-ICL/monzopy
 Project-URL: Bug Tracker, https://github.com/JakeMartin-ICL/monzopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `monzopy-1.1.0/monzopy/monzopy.py` & `monzopy-1.2.0/monzopy/monzopy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-"""API for Monzo bound to Home Assistant OAuth."""
+"""API for Monzo."""
+
 from abc import ABC, abstractmethod
 from collections.abc import Awaitable, Callable
 from datetime import datetime
 from typing import Any
 
 from aiohttp import ClientSession
 
 API_URL_BASE = "https://api.monzo.com"
 
 
 class AbstractMonzoApi(ABC):  # pylint: disable=too-few-public-methods
-    """Define an object to work with the AirVisual Cloud API."""
+    """An abstract class for accessing the Monzo API."""
 
     def __init__(self, session: ClientSession) -> None:
         """Initialize.
 
         Args:
             api_key: An API key.
             session: An optional aiohttp ClientSession.
@@ -69,21 +70,23 @@
     CURRENT_ACCOUNT: "Current Account",
     "uk_retail_joint": "Joint Account",
     "uk_monzo_flex": "Flex",
     "uk_business": "Business Account",
     "uk_rewards": "Cashback",
 }
 
+TOKEN_EXPIRY_CODE = "unauthorized.bad_access_token.expired"
+CODE = "code"
 
 class UserAccount:
     """Define an object representing a Monzo account holder."""
 
-    def __init__(self, request: Callable[..., Awaitable]) -> None:
+    def __init__(self, request: Callable[..., Awaitable[dict[str, Any]]]) -> None:
         """Initialise the account."""
-        self._request = request
+        self._request: Callable[..., Awaitable[dict[str, Any]]] = request
         self._account_ids: set[str] = set()
         self._webhook_ids: list[str] = []
 
     async def accounts(self) -> list[dict[str, Any]]:
         """List accounts and their balances."""
         result = []
 
@@ -116,27 +119,27 @@
         for account_id in self._account_ids:
             pots = await self._request(
                 "get", "pots", params={"current_account_id": account_id}
             )
             try:
                 valid_pots += [pot for pot in pots["pots"] if pot["deleted"] is False]
             except KeyError:
-                raise InvalidMonzoAPIResponseError
+                _raise_auth_or_response_error(pots)
         return valid_pots
 
     async def _get_accounts(self) -> list[dict[str, Any]]:
         res = await self._request("get", "accounts")
         valid_accounts = []
         try:
             for acc in res["accounts"]:
                 if acc["type"] not in INVALID_ACCOUNT_TYPES:
                     self._account_ids.add(acc["id"])
                     valid_accounts.append(acc)
         except KeyError:
-            raise InvalidMonzoAPIResponseError
+            _raise_auth_or_response_error(res)
         return valid_accounts
 
     async def pot_deposit(self, account_id: str, pot_id: str, amount: int) -> bool:
         """Deposit money into a pot from the specified account."""
         res = await self._request(
             "put",
             f"pots/{pot_id}/deposit",
@@ -191,14 +194,28 @@
         return webhook_ids
 
     async def unregister_webhooks(self) -> None:
         """Unregister all webhooks."""
         for webhook_id in await self.list_webhooks():
             await self._request("delete", f"webhooks/{webhook_id}")
 
+async def _authorisation_expired(response: dict[str, Any]) -> bool:
+    return CODE in response and response[CODE] == TOKEN_EXPIRY_CODE
+
+async def _raise_auth_or_response_error(response: dict[str, Any]) -> None:
+    if _authorisation_expired(response):
+        raise AuthorisationExpiredError
+    raise InvalidMonzoAPIResponseError
 
 class InvalidMonzoAPIResponseError(Exception):
     """Error thrown when the external Monzo API returns an invalid response."""
 
     def __init__(self, *args: object) -> None:
         """Initialise error."""
         super().__init__(*args)
+
+class AuthorisationExpiredError(Exception):
+    """Error thrown when the external Monzo API authentication has expired."""
+
+    def __init__(self, *args: object) -> None:
+        """Initialise error."""
+        super().__init__(*args)
```

### Comparing `monzopy-1.1.0/monzopy.egg-info/PKG-INFO` & `monzopy-1.2.0/monzopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monzopy
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple async python wrapper for the Monzo API, used primarily by the Monzo Home Assistant integration.
 Author-email: Jake Martin <jake_martin_@outlook.com>
 Project-URL: Homepage, https://github.com/JakeMartin-ICL/monzopy
 Project-URL: Bug Tracker, https://github.com/JakeMartin-ICL/monzopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `monzopy-1.1.0/pyproject.toml` & `monzopy-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "monzopy"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Jake Martin", email="jake_martin_@outlook.com" },
 ]
 description = "A simple async python wrapper for the Monzo API, used primarily by the Monzo Home Assistant integration."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

