# Comparing `tmp/py_alpaca_api-0.4.7.tar.gz` & `tmp/py_alpaca_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.4.7.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.5.0.tar", max compression
```

## Comparing `py_alpaca_api-0.4.7.tar` & `py_alpaca_api-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.4.7/LICENSE
--rw-r--r--   0        0        0    16791 2024-05-19 11:02:34.884010 py_alpaca_api-0.4.7/README.md
--rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.4.7/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2513 2024-05-19 04:10:18.598262 py_alpaca_api-0.4.7/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.4.7/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     6009 2024-05-19 04:10:18.608262 py_alpaca_api-0.4.7/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     3750 2024-05-19 04:10:18.608262 py_alpaca_api-0.4.7/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    21161 2024-05-19 04:10:18.608262 py_alpaca_api-0.4.7/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     7736 2024-05-19 02:32:34.142337 py_alpaca_api-0.4.7/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2102 2024-05-19 02:32:34.112337 py_alpaca_api-0.4.7/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    18665 2024-05-19 02:32:34.172337 py_alpaca_api-0.4.7/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0    14954 2024-05-19 02:32:34.172337 py_alpaca_api-0.4.7/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     7359 2024-05-19 12:31:17.233892 py_alpaca_api-0.4.7/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    21397 2024-05-19 04:10:18.608262 py_alpaca_api-0.4.7/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1324 2024-05-19 12:31:17.233892 py_alpaca_api-0.4.7/pyproject.toml
--rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.0/LICENSE
+-rw-r--r--   0        0        0    16791 2024-05-19 11:02:34.884010 py_alpaca_api-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.0/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2513 2024-05-19 04:10:18.598262 py_alpaca_api-0.5.0/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.0/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     6009 2024-05-19 04:10:18.608262 py_alpaca_api-0.5.0/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     3750 2024-05-19 04:10:18.608262 py_alpaca_api-0.5.0/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    21161 2024-05-19 04:10:18.608262 py_alpaca_api-0.5.0/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7736 2024-05-19 02:32:34.142337 py_alpaca_api-0.5.0/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2102 2024-05-19 02:32:34.112337 py_alpaca_api-0.5.0/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    23670 2024-05-19 14:46:57.123704 py_alpaca_api-0.5.0/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0    14954 2024-05-19 02:32:34.172337 py_alpaca_api-0.5.0/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     7359 2024-05-19 12:31:17.233892 py_alpaca_api-0.5.0/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    21397 2024-05-19 04:10:18.608262 py_alpaca_api-0.5.0/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1324 2024-05-19 14:46:57.123704 py_alpaca_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.0/PKG-INFO
```

### Comparing `py_alpaca_api-0.4.7/LICENSE` & `py_alpaca_api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/README.md` & `py_alpaca_api-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.5.0/py_alpaca_api/alpaca.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/account.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/account.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/asset.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/data_classes.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/history.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/history.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/market.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/market.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/order.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/order.py`

 * *Files 20% similar despite different names*

```diff
@@ -232,38 +232,26 @@
 
         MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
                 submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
                 notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='market', \
                 limit_price=None, stop_price=None, status='new', side='buy', time_in_force='day', extended_hours=False)
         """  # noqa
 
-        # Alpaca API URL for submitting market order
-        url = f"{self.trade_url}/orders"
-        # Market order payload
+        # Payload for market order
         payload = {
             "symbol": symbol,
             "qty": qty if qty else None,
             "notional": round(notional, 2) if notional else None,
             "side": side if side == "buy" else "sell",
             "type": "market",
             "time_in_force": time_in_force,
             "extended_hours": extended_hours,
         }
-        # Post request to Alpaca API for submitting market order
-        response = requests.post(url, headers=self.headers, json=payload)
-        # Check if response is successful
-        if response.status_code == 200:
-            # Convert JSON response to dictionary
-            res = json.loads(response.text)
-            # Return market order information as a MarketOrderClass object
-            return order_class_from_dict(res)
-        # If response is not successful, raise an exception
-        else:
-            res = json.loads(response.text)
-            raise Exception(f'Failed to submit market order. Code: {response.status_code}, Response: {res["message"]}')
+        # Return market order using submit order method
+        return self.__submit_order(payload)
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Limit Order /////////////////#
     ########################################################
     def limit(
         self,
         symbol: str,
@@ -331,39 +319,27 @@
         MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
                 submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
                 notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='limit', \
                 limit_price=100.0, stop_price=None, status='new', side='buy', time_in_force='day', extended_hours=False)
 
         """  # noqa
 
-        # Alpaca API URL for submitting market order
-        url = f"{self.trade_url}/orders"
-        # Market order payload
+        # Payload for limit order
         payload = {
             "symbol": symbol,  # Asset symbol to buy/sell
             "limit_price": limit_price,  # Limit price for the order
             "qty": (qty if qty else None),  # Check if qty is provided, if not, set to None
             "notional": (round(notional, 2) if notional else None),  # Round notional to 2 decimal places, if notional is provided
             "side": (side if side == "buy" else "sell"),  # Check if side is buy or sell
             "type": "limit",  # Order type is limit
             "time_in_force": time_in_force,  # Time in force options, default: day
             "extended_hours": extended_hours,  # Extended hours trading, default: False
         }
-        # Post request to Alpaca API for submitting market order
-        response = requests.post(url, headers=self.headers, json=payload)
-        # Check if response is successful
-        if response.status_code == 200:
-            # Convert JSON response to dictionary
-            res = json.loads(response.text)
-            # Return market order information as a MarketOrderClass object
-            return order_class_from_dict(res)
-        # If response is not successful, raise an exception
-        else:
-            res = json.loads(response.text)
-            raise Exception(f'Failed to submit limit order. Code: {response.status_code}, Response: {res["message"]}')
+        # Return limit order using submit order method
+        return self.__submit_order(payload)
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Stop Order /////////////////#
     ########################################################
     def stop(
         self,
         symbol: str,
@@ -417,31 +393,191 @@
         MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
                 submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
                 notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='stop', \
                 limit_price=None, stop_price=100.0, status='new', side='buy', time_in_force='day', extended_hours=False)
 
         """  # noqa
 
-        # Alpaca API URL for submitting market order
-        url = f"{self.trade_url}/orders"
-        # Market order payload
+        # Payload for stop order
         payload = {
             "symbol": symbol,  # Asset symbol to buy/sell
             "stop_price": stop_price,  # Stop price for the order
             "qty": qty,  # Quantity of asset to buy/sell
             "side": (side if side == "buy" else "sell"),  # Check if side is buy or sell
             "type": "stop",  # Order type is stop
             "time_in_force": time_in_force,  # Time in force options, default: day
             "extended_hours": extended_hours,  # Extended hours trading, default: False
         }
-        # Post request to Alpaca API for submitting market order
+        # Return stop order using submit order method
+        return self.__submit_order(payload)
+
+    ########################################################
+    # \\\\\\\\\\\\\\\\  Submit Stop Order /////////////////#
+    ########################################################
+    def stop_limit(
+        self,
+        symbol: str,
+        stop_price: float,
+        limit_price: float,
+        qty: float,
+        side: str = "buy",
+        time_in_force: str = "day",
+        extended_hours: bool = False,
+    ) -> OrderClass:
+        """Submit a Stop Limit Order
+
+        Parameters:
+        -----------
+        symbol:         Asset symbol to buy/sell
+                        A valid asset symbol string required
+
+        stop_price:     Stop price for the order
+                        Stop price for the order float required
+
+        limit_price:    Limit price for the order
+                        Limit price for the order float required
+
+        qty:            Quantity of asset to buy/sell
+                        Quantity of asset to buy/sell float required
+
+        side:           Order side (buy/sell) (default: buy)
+                        Order side (buy/sell) (optional) str
+
+        time_in_force:  Time in force options (day, gtc, opg, cls, ioc, fok) (default: day)
+                        Time in force options (optional) str
+
+        extended_hours: Extended hours trading (default: False)
+                        Extended hours trading (optional) bool
+
+        Returns:
+        --------
+        MarketOrderClass: Market order information as a MarketOrderClass object with
+
+        values: id, client_order_id, created_at, submitted_at, asset_id, symbol, asset_class,
+                notional, qty, filled_qty, filled_avg_price, order_class, order_type , limit_price,
+                stop_price, filled_qty, filled_avg_price, status, type, side, time_in_force, extended_hours
+
+        Raises:
+        -------
+        Exception:
+            Exception if failed to submit stop order
+        """  # noqa
+
+        # Payload for stop order
+        payload = {
+            "symbol": symbol,  # Asset symbol to buy/sell
+            "stop_price": stop_price,  # Stop price for the order
+            "limit_price": limit_price,  # Limit price for the order
+            "qty": qty,  # Quantity of asset to buy/sell
+            "side": (side if side == "buy" else "sell"),  # Check if side is buy or sell
+            "type": "stop_limit",  # Order type is stop
+            "time_in_force": time_in_force,  # Time in force options, default: day
+            "extended_hours": extended_hours,  # Extended hours trading, default: False
+        }
+        # Return stop order using submit order method
+        return self.__submit_order(payload)
+
+    ########################################################
+    # \\\\\\\\\\\\\\\\  Submit Stop Order /////////////////#
+    ########################################################
+    def trailing_stop(
+        self,
+        symbol: str,
+        qty: float,
+        trail_percent: float = None,
+        trail_price: float = None,
+        side: str = "buy",
+        time_in_force: str = "day",
+        extended_hours: bool = False,
+    ) -> OrderClass:
+        """Submit a Trailing Stop Order
+
+        Parameters:
+        -----------
+        symbol:         Asset symbol to buy/sell
+                        A valid asset symbol string required
+
+        qty:            Quantity of asset to buy/sell
+                        Quantity of asset to buy/sell float required
+
+        trail_percent:  Trailing stop percent
+                        Trailing stop percent float optional
+
+        trail_price:    Trailing stop price
+                        Trailing stop price float optional
+
+        side:           Order side (buy/sell) (default: buy)
+                        Order side (buy/sell) (optional) str
+
+        time_in_force:  Time in force options (day, gtc, opg, cls, ioc, fok) (default: day)
+                        Time in force options (optional) str
+
+        extended_hours: Extended hours trading (default: False)
+                        Extended hours trading (optional) bool
+
+        Returns:
+        --------
+        MarketOrderClass: Market order information as a MarketOrderClass object with
+
+        values: id, client_order_id, created_at, submitted_at, asset_id, symbol, asset_class,
+                notional, qty, filled_qty, filled_avg_price, order_class, order_type , limit_price,
+                stop_price, filled_qty, filled_avg_price, status, type, side, time_in_force, extended_hours
+
+        Raises:
+        -------
+        Exception:
+            Exception if failed to submit stop order
+        """  # noqa
+
+        if trail_percent is None and trail_price is None or trail_percent and trail_price:
+            raise ValueError("Either trail_percent or trail_price must be provided, not both.")
+        if trail_percent:
+            if trail_percent < 0:
+                raise ValueError("Trail percent must be greater than 0.")
+        # Payload for stop order
+        payload = {
+            "symbol": symbol,  # Asset symbol to buy/sell
+            "trail_percent": trail_percent,  # Stop price for the order
+            "trail_price": trail_price,  # Limit price for the order
+            "qty": qty,  # Quantity of asset to buy/sell
+            "side": (side if side == "buy" else "sell"),  # Check if side is buy or sell
+            "type": "trailing_stop",  # Order type is stop
+            "time_in_force": time_in_force,  # Time in force options, default: day
+            "extended_hours": extended_hours,  # Extended hours trading, default: False
+        }
+        # Return stop order using submit order method
+        return self.__submit_order(payload)
+
+    ########################################################
+    # \\\\\\\\\\\\\\\\  Submit Order //////////////////////#
+    ########################################################
+    def __submit_order(self, payload: dict) -> OrderClass:
+        """Submit an order
+
+        Parameters:
+        -----------
+        payload:    Order payload dictionary
+                    Order payload dictionary required
+
+        Returns:
+        --------
+        OrderClass: Order information as an OrderClass object
+
+        Raises:
+        -------
+        Exception:  If failed to submit order
+        """  # noqa
+
+        # Alpaca API URL for submitting an order
+        url = f"{self.trade_url}/orders"
+        # Post request to Alpaca API for submitting an order
         response = requests.post(url, headers=self.headers, json=payload)
         # Check if response is successful
         if response.status_code == 200:
             # Convert JSON response to dictionary
             res = json.loads(response.text)
-            # Return market order information as a MarketOrderClass object
+            # Return order information as an OrderClass object
             return order_class_from_dict(res)
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise Exception(f'Failed to submit limit order. Code: {response.status_code}, Response: {res["message"]}')
+            raise Exception(f'Failed to submit order. Code: {response.status_code}, Response: {res["message"]}')
```

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/position.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/position.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/screener.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.5.0/py_alpaca_api/src/watchlist.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.7/pyproject.toml` & `py_alpaca_api-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.4.7"
+version = "0.5.0"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.4.7/PKG-INFO` & `py_alpaca_api-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.4.7
+Version: 0.5.0
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

