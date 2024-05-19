# Comparing `tmp/py_alpaca_api-0.4.0.tar.gz` & `tmp/py_alpaca_api-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.4.0.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.4.4.tar", max compression
```

## Comparing `py_alpaca_api-0.4.0.tar` & `py_alpaca_api-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.4.0/LICENSE
--rw-r--r--   0        0        0    17299 2024-05-15 03:25:08.684820 py_alpaca_api-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.4.0/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2326 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-14 02:56:26.383431 py_alpaca_api-0.4.0/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     3025 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     2494 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    20501 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     7736 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2102 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    18665 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0    14954 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0    21192 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1279 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    18060 1970-01-01 00:00:00.000000 py_alpaca_api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.4.4/LICENSE
+-rw-r--r--   0        0        0    17299 2024-05-15 03:25:08.684820 py_alpaca_api-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 07:55:50.214840 py_alpaca_api-0.4.4/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2460 2024-05-18 15:10:11.299597 py_alpaca_api-0.4.4/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-18 07:55:40.234842 py_alpaca_api-0.4.4/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     3025 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     3711 2024-05-18 15:10:11.299597 py_alpaca_api-0.4.4/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    20501 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.4/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7736 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2102 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    18665 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0    14954 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     6403 2024-05-18 15:10:11.299597 py_alpaca_api-0.4.4/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    21192 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1279 2024-05-18 15:10:11.299597 py_alpaca_api-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    18060 1970-01-01 00:00:00.000000 py_alpaca_api-0.4.4/PKG-INFO
```

### Comparing `py_alpaca_api-0.4.0/LICENSE` & `py_alpaca_api-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/README.md` & `py_alpaca_api-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.4.4/py_alpaca_api/alpaca.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .src.account import Account
 from .src.asset import Asset
 from .src.history import History
 from .src.market import Market
 from .src.order import Order
 from .src.position import Position
+from .src.screener import Screener
 from .src.watchlist import Watchlist
 
 
 # PyAlpacaApi class
 class PyAlpacaApi:
     def __init__(self, api_key: str, api_secret: str, api_paper: bool = True):
         """Initialize PyAlpacaApi class
@@ -57,7 +58,8 @@
         self.account = Account(trade_url=self.trade_url, headers=self.headers)
         self.asset = Asset(trade_url=self.trade_url, headers=self.headers)
         self.history = History(data_url=self.data_url, headers=self.headers, asset=self.asset)
         self.position = Position(trade_url=self.trade_url, headers=self.headers, account=self.account)
         self.order = Order(trade_url=self.trade_url, headers=self.headers)
         self.market = Market(trade_url=self.trade_url, headers=self.headers)
         self.watchlist = Watchlist(trade_url=self.trade_url, headers=self.headers)
+        self.screener = Screener(data_url=self.data_url, headers=self.headers, asset=self.asset)
```

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/src/account.py` & `py_alpaca_api-0.4.4/py_alpaca_api/src/account.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.4.4/py_alpaca_api/src/asset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 
+import pandas as pd
 import requests
 
 from .data_classes import AssetClass, asset_class_from_dict
 
 
 class Asset:
     def __init__(self, trade_url: str, headers: object) -> None:
@@ -23,14 +24,43 @@
 
         ValueError: If headers are not provided
         """  # noqa
 
         self.trade_url = trade_url
         self.headers = headers
 
+    def get_all(self, status: str = "active", asset_class: str = "us_equity", exchange: str = "") -> pd.DataFrame:
+        # Alpaca API URL for asset information
+        url = f"{self.trade_url}/assets"
+
+        params = {
+            "status": status,
+            "asset_class": asset_class,
+            "exchange": exchange,
+        }
+
+        # Get request to Alpaca API for asset information
+        response = requests.get(url, headers=self.headers, params=params)
+        # Check if response is successful
+        if response.status_code == 200:
+            # Convert JSON response to dictionary
+            res_df = pd.json_normalize(json.loads(response.text))
+
+            res_df = res_df[res_df["status"] == "active"]
+            res_df = res_df[res_df["fractionable"]]
+            res_df = res_df[res_df["tradable"]]
+            res_df = res_df[res_df["exchange"] != "OTC"]
+            res_df.reset_index(drop=True, inplace=True)
+
+            # Return asset information as an AssetClass object
+            return res_df
+        # If response is not successful, raise an exception
+        else:
+            raise ValueError(f"Failed to get asset information. Response: {response.text}")
+
     #####################################################
     # \\\\\\\\\\\\\\\\\\\  Get Asset ////////////////////#
     #####################################################
     def get(self, symbol: str) -> AssetClass:
         """Get asset information from Alpaca API
 
         Parameters:
```

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.4.4/py_alpaca_api/src/data_classes.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/src/history.py` & `py_alpaca_api-0.4.4/py_alpaca_api/src/history.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/src/market.py` & `py_alpaca_api-0.4.4/py_alpaca_api/src/market.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/src/order.py` & `py_alpaca_api-0.4.4/py_alpaca_api/src/order.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/src/position.py` & `py_alpaca_api-0.4.4/py_alpaca_api/src/position.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.4.4/py_alpaca_api/src/watchlist.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.0/pyproject.toml` & `py_alpaca_api-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.4.0"
+version = "0.4.4"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.4.0/PKG-INFO` & `py_alpaca_api-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.4.0
+Version: 0.4.4
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

