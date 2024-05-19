# Comparing `tmp/hftbacktest-1.8.1.tar.gz` & `tmp/hftbacktest-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.8.1.tar", last modified: Wed Apr 24 14:31:47 2024, max compression
+gzip compressed data, was "hftbacktest-1.8.2.tar", last modified: Sun May 19 13:48:08 2024, max compression
```

## Comparing `hftbacktest-1.8.1.tar` & `hftbacktest-1.8.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/LICENSE
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9133 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8022 2024-04-24 14:24:53.000000 hftbacktest-1.8.1/README.rst
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.995698 hftbacktest-1.8.1/hftbacktest/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12124 2024-04-24 13:30:16.000000 hftbacktest-1.8.1/hftbacktest/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/assettype.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16000 2024-03-19 13:08:02.000000 hftbacktest-1.8.1/hftbacktest/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.995698 hftbacktest-1.8.1/hftbacktest/data/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/data/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/hftbacktest/data/utils/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14082 2024-04-24 10:45:33.000000 hftbacktest-1.8.1/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10189 2024-03-22 14:34:52.000000 hftbacktest-1.8.1/hftbacktest/data/utils/binancehistmktdata.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7967 2023-12-10 12:15:55.000000 hftbacktest-1.8.1/hftbacktest/data/utils/difforderbooksnapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2768 2024-03-22 14:39:11.000000 hftbacktest-1.8.1/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10184 2024-04-24 14:11:01.000000 hftbacktest-1.8.1/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16544 2024-04-24 14:11:20.000000 hftbacktest-1.8.1/hftbacktest/data/validation.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-08-23 14:57:13.000000 hftbacktest-1.8.1/hftbacktest/marketdepth.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/hftbacktest/models/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/models/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12224 2023-12-10 12:16:05.000000 hftbacktest-1.8.1/hftbacktest/models/latencies.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4867 2024-02-14 09:48:00.000000 hftbacktest-1.8.1/hftbacktest/models/queue.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4856 2024-03-11 14:20:26.000000 hftbacktest-1.8.1/hftbacktest/order.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/hftbacktest/proc/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/proc/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8149 2023-12-04 12:17:36.000000 hftbacktest-1.8.1/hftbacktest/proc/local.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.8.1/hftbacktest/proc/nopartialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    30419 2024-04-14 14:19:28.000000 hftbacktest-1.8.1/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5850 2023-12-01 13:42:13.000000 hftbacktest-1.8.1/hftbacktest/proc/proc.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3332 2024-03-19 12:28:56.000000 hftbacktest-1.8.1/hftbacktest/reader.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13980 2023-12-10 12:16:12.000000 hftbacktest-1.8.1/hftbacktest/stat.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.8.1/hftbacktest/state.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7460 2023-05-26 12:41:56.000000 hftbacktest-1.8.1/hftbacktest/stats.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.8.1/hftbacktest/typing.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.995698 hftbacktest-1.8.1/hftbacktest.egg-info/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9133 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1022 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/SOURCES.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/dependency_links.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.8.1/hftbacktest.egg-info/not-zip-safe
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/requires.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1250 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/setup.cfg
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.821140 hftbacktest-1.8.2/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9133 2024-05-19 13:48:08.821140 hftbacktest-1.8.2/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8022 2024-04-24 14:24:53.000000 hftbacktest-1.8.2/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.818140 hftbacktest-1.8.2/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12124 2024-05-19 12:10:25.000000 hftbacktest-1.8.2/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16000 2024-03-19 13:08:02.000000 hftbacktest-1.8.2/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.819140 hftbacktest-1.8.2/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1766 2024-05-19 12:10:07.000000 hftbacktest-1.8.2/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.820140 hftbacktest-1.8.2/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14082 2024-04-24 10:45:33.000000 hftbacktest-1.8.2/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10189 2024-03-22 14:34:52.000000 hftbacktest-1.8.2/hftbacktest/data/utils/binancehistmktdata.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7967 2023-12-10 12:15:55.000000 hftbacktest-1.8.2/hftbacktest/data/utils/difforderbooksnapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2768 2024-05-19 12:43:38.000000 hftbacktest-1.8.2/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10184 2024-04-24 14:11:01.000000 hftbacktest-1.8.2/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    17614 2024-05-19 12:15:47.000000 hftbacktest-1.8.2/hftbacktest/data/validation.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-08-23 14:57:13.000000 hftbacktest-1.8.2/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.821140 hftbacktest-1.8.2/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12224 2023-12-10 12:16:05.000000 hftbacktest-1.8.2/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4867 2024-02-14 09:48:00.000000 hftbacktest-1.8.2/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4856 2024-03-11 14:20:26.000000 hftbacktest-1.8.2/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.821140 hftbacktest-1.8.2/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8149 2023-12-04 12:17:36.000000 hftbacktest-1.8.2/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.8.2/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    30419 2024-04-14 14:19:28.000000 hftbacktest-1.8.2/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5850 2023-12-01 13:42:13.000000 hftbacktest-1.8.2/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3332 2024-03-19 12:28:56.000000 hftbacktest-1.8.2/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13980 2023-12-10 12:16:12.000000 hftbacktest-1.8.2/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.8.2/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7460 2023-05-26 12:41:56.000000 hftbacktest-1.8.2/hftbacktest/stats.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.8.2/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.819140 hftbacktest-1.8.2/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9133 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1022 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.8.2/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1250 2024-05-19 13:48:08.822140 hftbacktest-1.8.2/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/setup.py
```

### Comparing `hftbacktest-1.8.1/LICENSE` & `hftbacktest-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/PKG-INFO` & `hftbacktest-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.8.1
+Version: 1.8.2
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
```

### Comparing `hftbacktest-1.8.1/README.rst` & `hftbacktest-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/__init__.py` & `hftbacktest-1.8.2/hftbacktest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.8.1'
+__version__ = '1.8.2'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.8.1/hftbacktest/assettype.py` & `hftbacktest-1.8.2/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/backtest.py` & `hftbacktest-1.8.2/hftbacktest/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.8.2/hftbacktest/data/utils/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/data/utils/binancehistmktdata.py` & `hftbacktest-1.8.2/hftbacktest/data/utils/binancehistmktdata.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/data/utils/difforderbooksnapshot.py` & `hftbacktest-1.8.2/hftbacktest/data/utils/difforderbooksnapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.8.2/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.8.2/hftbacktest/data/utils/tardis.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/data/validation.py` & `hftbacktest-1.8.2/hftbacktest/data/validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -442,7 +442,46 @@
         ) for rn in range(len(data))
     ]
 
     return np.array(
         tup_list,
         dtype=[('ev', 'i8'), ('exch_ts', 'i8'), ('local_ts', 'i8'), ('px', 'f4'), ('qty', 'f4')]
     )
+
+
+def convert_from_struct_arr(data: np.ndarray) -> np.ndarray:
+    r"""
+    Converts the structured array that can be used in Rust hftbacktest into the 2D ndarray currently used in Python
+    hftbacktest.
+
+    Args:
+        data: the structured array to be converted.
+
+    Returns:
+        Converted 2D ndarray.
+    """
+
+    out = np.empty((len(data), 6), np.float64)
+    for row in range(len(data)):
+        ev = data[row][0]
+
+        if ev & EXCH_EVENT == EXCH_EVENT:
+            out[row, COL_EXCH_TIMESTAMP] = data[row][1]
+        else:
+            out[row, COL_EXCH_TIMESTAMP] = -1
+
+        if ev & LOCAL_EVENT == LOCAL_EVENT:
+            out[row, COL_LOCAL_TIMESTAMP] = data[row][2]
+        else:
+            out[row, COL_LOCAL_TIMESTAMP] = -1
+
+        if ev & BUY == BUY:
+            out[row, COL_SIDE] = 1
+        elif ev & SELL == SELL:
+            out[row, COL_SIDE] = -1
+        else:
+            out[row, COL_SIDE] = 0
+
+        out[row, COL_PRICE] = data[row][3]
+        out[row, COL_QTY] = data[row][4]
+        out[row, COL_EVENT] = ev & 0xFF
+    return out
```

### Comparing `hftbacktest-1.8.1/hftbacktest/marketdepth.py` & `hftbacktest-1.8.2/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/models/latencies.py` & `hftbacktest-1.8.2/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/models/queue.py` & `hftbacktest-1.8.2/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/order.py` & `hftbacktest-1.8.2/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/proc/local.py` & `hftbacktest-1.8.2/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.8.2/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.8.2/hftbacktest/proc/partialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/proc/proc.py` & `hftbacktest-1.8.2/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/reader.py` & `hftbacktest-1.8.2/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/stat.py` & `hftbacktest-1.8.2/hftbacktest/stat.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/state.py` & `hftbacktest-1.8.2/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/stats.py` & `hftbacktest-1.8.2/hftbacktest/stats.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest/typing.py` & `hftbacktest-1.8.2/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.8.2/hftbacktest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.8.1
+Version: 1.8.2
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
```

### Comparing `hftbacktest-1.8.1/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.8.2/hftbacktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.1/setup.cfg` & `hftbacktest-1.8.2/setup.cfg`

 * *Files identical despite different names*

