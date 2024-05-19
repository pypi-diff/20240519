# Comparing `tmp/PKDevTools-0.13.20240518.123.tar.gz` & `tmp/PKDevTools-0.13.20240519.124.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240518.123.tar", last modified: Sat May 18 01:39:31 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240519.124.tar", last modified: Sun May 19 10:06:54 2024, max compression
```

## Comparing `PKDevTools-0.13.20240518.123.tar` & `PKDevTools-0.13.20240519.124.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 01:39:31.765231 PKDevTools-0.13.20240518.123/
--rw-rw-rw-   0        0        0     1086 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-18 01:39:31.749591 PKDevTools-0.13.20240518.123/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 01:39:31.765231 PKDevTools-0.13.20240518.123/PKDevTools/classes/
--rw-rw-rw-   0        0        0     4960 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6376 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2608 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/FunctionTimeouts.py
--rw-rw-rw-   0        0        0    11963 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2860 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    15627 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5243 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    11651 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-18 01:39:27.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-18 01:39:31.765231 PKDevTools-0.13.20240518.123/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-18 01:39:31.000000 PKDevTools-0.13.20240518.123/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2024-05-18 01:39:31.000000 PKDevTools-0.13.20240518.123/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 01:39:31.000000 PKDevTools-0.13.20240518.123/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-18 01:39:31.000000 PKDevTools-0.13.20240518.123/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 01:39:25.000000 PKDevTools-0.13.20240518.123/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-05-18 01:39:31.000000 PKDevTools-0.13.20240518.123/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 01:39:31.000000 PKDevTools-0.13.20240518.123/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-18 01:39:31.765231 PKDevTools-0.13.20240518.123/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/README.md
--rw-rw-rw-   0        0        0       86 2024-05-18 01:39:31.765231 PKDevTools-0.13.20240518.123/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-18 01:37:30.000000 PKDevTools-0.13.20240518.123/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:06:54.555067 PKDevTools-0.13.20240519.124/
+-rw-rw-rw-   0        0        0     1086 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-19 10:06:54.539447 PKDevTools-0.13.20240519.124/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:06:54.555067 PKDevTools-0.13.20240519.124/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     4960 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2608 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/FunctionTimeouts.py
+-rw-rw-rw-   0        0        0    11963 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     5072 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/NSEMarketStatus.py
+-rw-rw-rw-   0        0        0     2860 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    16184 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5243 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    12875 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-19 10:06:49.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:06:54.555067 PKDevTools-0.13.20240519.124/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-19 10:06:54.000000 PKDevTools-0.13.20240519.124/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1199 2024-05-19 10:06:54.000000 PKDevTools-0.13.20240519.124/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 10:06:54.000000 PKDevTools-0.13.20240519.124/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-05-19 10:06:54.000000 PKDevTools-0.13.20240519.124/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 10:06:47.000000 PKDevTools-0.13.20240519.124/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      189 2024-05-19 10:06:54.000000 PKDevTools-0.13.20240519.124/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 10:06:54.000000 PKDevTools-0.13.20240519.124/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-05-19 10:06:54.555067 PKDevTools-0.13.20240519.124/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-19 10:06:54.555067 PKDevTools-0.13.20240519.124/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-05-19 10:05:12.000000 PKDevTools-0.13.20240519.124/setup.py
```

### Comparing `PKDevTools-0.13.20240518.123/LICENSE` & `PKDevTools-0.13.20240519.124/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/__init__.py` & `PKDevTools-0.13.20240519.124/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/FunctionTimeouts.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/FunctionTimeouts.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/PKDateUtilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import datetime
 import requests
 from datetime import timezone
 from PKDevTools.classes.Fetcher import fetcher
 from PKDevTools.classes.PKPickler import PKPickler
 from PKDevTools.classes.Utils import random_user_agent
 from PKDevTools.classes.FunctionTimeouts import exit_after
+from PKDevTools.classes.NSEMarketStatus import NSEMarketStatus
 
 class PKDateUtilities:
     def utc_to_ist(utc_dt):
         return (
             pytz.utc.localize(utc_dt)
             .replace(tzinfo=timezone.utc)
             .astimezone(tz=pytz.timezone("Asia/Kolkata"))
@@ -170,47 +171,59 @@
         if "simulation" in os.environ.keys():
             simulatedEnvs = json.loads(os.environ["simulation"])
             if "isTrading" in simulatedEnvs.keys():
                 return simulatedEnvs["isTrading"]
         curr = PKDateUtilities.currentDateTime()
         openTime = curr.replace(hour=9, minute=15)
         closeTime = curr.replace(hour=15, minute=30)
-        return ((openTime <= curr <= closeTime) and PKDateUtilities.isTradingWeekday()) #or str(PKDateUtilities.onlineTradingStatus()[0]) == "Open"
+        if NSEMarketStatus().status == "Open":
+            return True
+        elif NSEMarketStatus().status == "Close":
+            return False
+        return ((openTime <= curr <= closeTime) and PKDateUtilities.isTradingWeekday())
 
+    def wasTradedOn(checkDate=None):
+        if checkDate is None:
+            checkDate = PKDateUtilities.currentDateTime()
+        tradeDate = NSEMarketStatus().tradeDate
+        if tradeDate is not None and "-" in str(tradeDate):
+            tradeDate = PKDateUtilities.dateFromdbYString(tradeDate.split(" ")[0])
+            tradeDateEqualsCheckDate = (tradeDate.date() == (checkDate.date() if isinstance(checkDate,datetime.datetime) else checkDate))
+            if tradeDateEqualsCheckDate:
+                return True
+        return False
+
+    def nextTradingBellDate():
+        next_bell = NSEMarketStatus().next_bell
+        if next_bell is not None and "T" in str(next_bell):
+            next_bell = PKDateUtilities.dateFromYmdString(next_bell.split("T")[0])
+            return next_bell.date()
+        return None
+    
+    def willNextTradeOnDate(checkDate=None):
+        if checkDate is None:
+            checkDate = PKDateUtilities.currentDateTime()
+        next_bell = PKDateUtilities.nextTradingBellDate()
+        if next_bell is not None:
+            nextBellEqualsCheckDate = (next_bell == (checkDate.date() if isinstance(checkDate,datetime.datetime) else checkDate))
+            if nextBellEqualsCheckDate:
+                return True
+        return False
+    
     def isTradingWeekday(checkDate=None):
         if checkDate is None:
             checkDate = PKDateUtilities.currentDateTime()
+        if NSEMarketStatus().status == "Open":
+            return True
+        if PKDateUtilities.wasTradedOn(checkDate) or PKDateUtilities.willNextTradeOnDate(checkDate):
+            return True
         if 0 <= checkDate.weekday() <= 4:
             return True
-        # else:
-        #     tradeDate = PKDateUtilities.onlineTradingStatus()[1]
-        #     if tradeDate is not None:
-        #         return (tradeDate.date() == (checkDate.date() if isinstance(checkDate,datetime.datetime) else checkDate))
-        return False
 
-    def onlineTradingStatus():
-        url = "https://www.nseindia.com/api/marketStatus"
-        headers = {"user-agent": random_user_agent()}
-        f = fetcher()
-        try:
-            status = None
-            tradeDate = None
-            res = f.fetchURL(url, headers=headers, timeout=10)
-            if res is None or res.status_code != 200:
-                return None, None
-            marketResp = res.json()
-            marketStates = marketResp["marketState"]
-            for mktState in marketStates:
-                if mktState["market"].lower() == "capital market":
-                    status = mktState["marketStatus"]
-                    tradeDate = PKDateUtilities.dateFromdbYString(mktState["tradeDate"].split(" ")[0])
-                    break
-        except:
-            pass
-        return status, tradeDate
+        return False
         
     def nextWeekday(forDate=None):
         if forDate is None:
             forDate = PKDateUtilities.currentDateTime()
         nextWeekday = forDate + datetime.timedelta(days=1)
         while not PKDateUtilities.isTradingWeekday(nextWeekday):
             nextWeekday = nextWeekday + datetime.timedelta(days=1)
```

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,41 +49,43 @@
 from PKDevTools.classes.multiprocessing_logging import SubProcessLogHandler
 from PKDevTools.classes import Archiver
 
 class PKMultiProcessorClient(multiprocessing.Process):
     def __init__(
         self,
         processorMethod,
-        task_queue,
-        result_queue,
-        logging_queue,
-        processingCounter,
-        processingResultsCounter,
-        objectDictionaryPrimary,
-        objectDictionarySecondary,
-        proxyServer,
-        keyboardInterruptEvent,
-        defaultLogger,
+        task_queue=None,
+        result_queue=None,
+        logging_queue=None,
+        processingCounter=None,
+        processingResultsCounter=None,
+        objectDictionaryPrimary=None,
+        objectDictionarySecondary=None,
+        proxyServer=None,
+        keyboardInterruptEvent=None,
+        defaultLogger=None,
         fetcher=None,
         configManager=None,
         candlePatterns=None,
         screener=None,
         dbFileNamePrimary=None,
         dbFileNameSecondary=None,
         stockList=None,
         dataCallbackHandler=None,
         progressCallbackHandler=None,
+        processorArgs=None
     ):
         multiprocessing.Process.__init__(self)
         self.multiprocessingForWindows()
         assert (
             processorMethod is not None
         ), "processorMethod argument must not be None. This is the meyhod that will do the processing."
-        assert task_queue is not None, "task_queue argument must not be None."
-        assert (result_queue is not None or dataCallbackHandler is not None), "result_queue or dataCallbackHandler argument must not be None."
+        # assert keyboardInterruptEvent is not None, "keyboardInterruptEvent argument must not be None."
+        # assert task_queue is not None, "task_queue argument must not be None."
+        # assert (result_queue is not None or dataCallbackHandler is not None), "result_queue or dataCallbackHandler argument must not be None."
         self.processorMethod = processorMethod
         self.task_queue = task_queue
         self.result_queue = result_queue
         self.logging_queue = logging_queue
         # processingCounter and processingResultsCounter
         # are sunchronized counters that can be used within
         # processorMethod via hostRef.processingCounter
@@ -101,40 +103,44 @@
         # and can be accessed using hostRef.proxyServer
         # within processorMethod
         self.proxyServer = proxyServer
         # A logger that can contain logger reference
         # and can be accessed using hostRef.default_logger
         # within processorMethod
         self.default_logger = None
-        self.logLevel = defaultLogger.level
+        self.logLevel = defaultLogger.level if defaultLogger is not None else logging.NOTSET
 
         self.keyboardInterruptEvent = keyboardInterruptEvent
         self.stockList = stockList
         self.dataCallbackHandler = dataCallbackHandler
         self.progressCallbackHandler = progressCallbackHandler
         self.fetcher = fetcher
         self.intradayNSEFetcher = None
         self.configManager = configManager
         self.candlePatterns = candlePatterns
         self.screener = screener
-        self.refreshDatabase = True
+        self.refreshDatabase = (self.dbFileNamePrimary is not None) or (self.dbFileNameSecondary is not None)
         self.paused = False
+        self.processorArgs = processorArgs
+        self.queueProcessingMode = (self.task_queue is not None) and (self.result_queue is not None)
 
     def _clear(self):
         self.paused = True
         try:
-            while True:
-                self.task_queue.get_nowait()
+            if self.queueProcessingMode:
+                while True:
+                    self.task_queue.get_nowait()
         except Empty:
             if self.default_logger is not None:
                 self.default_logger.debug("task_queue empty.")
             pass
         try:
-            while True:
-                self.result_queue.get_nowait()
+            if self.queueProcessingMode:
+                while True:
+                    self.result_queue.get_nowait()
         except Empty:
             if self.default_logger is not None:
                 self.default_logger.debug("result_queue empty.")
             pass
         self.paused = False
 
     def _setupLogger(self):
@@ -186,50 +192,67 @@
                         self.objectDictionarySecondary = pickle.load(f)
 
             except:
                 self.objectDictionarySecondary = multiprocessing.Manager().dict()
                 pass
         self.refreshDatabase = False
 
+    def processQueueItems(self):
+        while not self.keyboardInterruptEvent.is_set():
+            try:
+                if self.refreshDatabase:
+                    # Maybe the database pickle file changed/re-saved.
+                    # We'd need to reload again
+                    self._reloadDatabase()
+
+                next_task = None
+                answer = None
+                if self.task_queue is not None:
+                    next_task = self.task_queue.get()
+                    if next_task is not None:
+                        # Inject a reference to this instance of the client
+                        # so that the task can still get access back to it.
+                        next_task = (*(next_task), self)
+            except Empty as e:
+                self.default_logger.debug(e, exc_info=True)
+                continue
+            except KeyboardInterrupt as e:
+                self.default_logger.debug(e, exc_info=True)
+                sys.exit(0)
+            if next_task is None:
+                self.default_logger.info("No next task in queue")
+                if self.task_queue is not None:
+                    self.task_queue.task_done()
+                break
+            if self.processorMethod is not None and not self.paused:
+                answer = self.processorMethod(*(next_task))
+            if self.task_queue is not None:
+                self.task_queue.task_done()
+            # self.default_logger.info(f"Task done. Result:{answer}")
+            if self.result_queue is not None and not self.paused:
+                self.result_queue.put(answer)
+
     def run(self):
         try:
             self._setupLogger()
-            while not self.keyboardInterruptEvent.is_set():
-                try:
-                    if self.refreshDatabase:
-                        # Maybe the database pickle file changed/re-saved.
-                        # We'd need to reload again
-                        self._reloadDatabase()
-
-                    next_task = None
-                    answer = None
-                    if self.task_queue is not None:
-                        next_task = self.task_queue.get()
-                        if next_task is not None:
-                            # Inject a reference to this instance of the client
-                            # so that the task can still get access back to it.
-                            next_task = (*(next_task), self)
-                except Empty as e:
-                    self.default_logger.debug(e, exc_info=True)
-                    continue
-                except KeyboardInterrupt as e:
-                    self.default_logger.debug(e, exc_info=True)
-                    sys.exit(0)
-                if next_task is None:
-                    self.default_logger.info("No next task in queue")
-                    if self.task_queue is not None:
-                        self.task_queue.task_done()
-                    break
-                if self.processorMethod is not None and not self.paused:
-                    answer = self.processorMethod(*(next_task))
-                if self.task_queue is not None:
-                    self.task_queue.task_done()
-                # self.default_logger.info(f"Task done. Result:{answer}")
-                if self.result_queue is not None and not self.paused:
-                    self.result_queue.put(answer)
+            if self.queueProcessingMode:
+                self.processQueueItems()
+            else:
+                if self.keyboardInterruptEvent is not None:
+                    while not self.keyboardInterruptEvent.is_set():
+                        try:
+                            if self.processorMethod is not None and not self.paused:
+                                self.processorMethod(self.processorArgs)
+                        except KeyboardInterrupt:
+                            try:
+                                self.terminate()
+                            finally:
+                                sys.exit(0)
+                elif self.processorMethod is not None:
+                    self.processorMethod(self.processorArgs)
         except Exception as e:
             self.default_logger.debug(e, exc_info=True)
             sys.exit(0)
 
     def multiprocessingForWindows(self):
         if sys.platform.startswith("win"):
             # First define a modified version of Popen.
```

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240519.124/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240519.124/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240518.123
+Version: 0.13.20240519.124
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240518.123.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240519.124.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240518.123/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240519.124/PKDevTools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 PKDevTools/classes/Archiver.py
 PKDevTools/classes/ColorText.py
 PKDevTools/classes/Committer.py
 PKDevTools/classes/CookieHelper.py
 PKDevTools/classes/Fetcher.py
 PKDevTools/classes/FunctionTimeouts.py
 PKDevTools/classes/MenuOptions.py
+PKDevTools/classes/NSEMarketStatus.py
 PKDevTools/classes/OutputControls.py
 PKDevTools/classes/PKDateUtilities.py
 PKDevTools/classes/PKGitFolderDownloader.py
 PKDevTools/classes/PKJoinableQueue.py
 PKDevTools/classes/PKMultiProcessorClient.py
 PKDevTools/classes/PKPickler.py
 PKDevTools/classes/PKTimer.py
```

### Comparing `PKDevTools-0.13.20240518.123/PKG-INFO` & `PKDevTools-0.13.20240519.124/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240518.123
+Version: 0.13.20240519.124
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240518.123.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240519.124.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240518.123/README.md` & `PKDevTools-0.13.20240519.124/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240518.123/setup.py` & `PKDevTools-0.13.20240519.124/setup.py`

 * *Files identical despite different names*

