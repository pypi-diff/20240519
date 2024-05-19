# Comparing `tmp/arbmaster-0.1.3.tar.gz` & `tmp/arbmaster-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\239294\OneDrive - V\344ster\345s Stad\Skrivbordet\upload\dist\.tmp-1v25417p\arbmaster-0.1.3.tar", last modified: Fri May 17 17:48:07 2024, max compression
+gzip compressed data, was "C:\Users\239294\OneDrive - V\344ster\345s Stad\Skrivbordet\upload\dist\.tmp-1cazv7rw\arbmaster-0.1.4.tar", last modified: Sun May 19 12:19:51 2024, max compression
```

## Comparing `arbmaster-0.1.3.tar` & `arbmaster-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 17:48:07.482018 arbmaster-0.1.3/
--rw-rw-rw-   0        0        0     1086 2024-04-30 17:51:08.000000 arbmaster-0.1.3/LICENCE
--rw-rw-rw-   0        0        0     1912 2024-05-17 17:48:07.478640 arbmaster-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1342 2024-05-17 17:15:54.000000 arbmaster-0.1.3/README.md
--rw-rw-rw-   0        0        0      660 2024-05-17 17:44:04.000000 arbmaster-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 17:48:07.482687 arbmaster-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 17:48:07.401263 arbmaster-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 17:48:07.438112 arbmaster-0.1.3/src/arbmaster/
--rw-rw-rw-   0        0        0      467 2024-05-17 17:15:56.000000 arbmaster-0.1.3/src/arbmaster/__init__.py
--rw-rw-rw-   0        0        0     1553 2024-04-30 19:29:20.000000 arbmaster-0.1.3/src/arbmaster/calc.py
--rw-rw-rw-   0        0        0     5772 2024-05-17 17:10:13.000000 arbmaster-0.1.3/src/arbmaster/client.py
--rw-rw-rw-   0        0        0     6712 2024-05-17 16:51:26.000000 arbmaster-0.1.3/src/arbmaster/constants.py
--rw-rw-rw-   0        0        0     4380 2024-05-17 17:45:41.000000 arbmaster-0.1.3/src/arbmaster/ext.py
--rw-rw-rw-   0        0        0      527 2024-04-30 17:51:08.000000 arbmaster-0.1.3/src/arbmaster/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-17 17:48:07.474298 arbmaster-0.1.3/src/arbmaster.egg-info/
--rw-rw-rw-   0        0        0     1912 2024-05-17 17:48:07.000000 arbmaster-0.1.3/src/arbmaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      418 2024-05-17 17:48:07.000000 arbmaster-0.1.3/src/arbmaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 17:48:07.000000 arbmaster-0.1.3/src/arbmaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-17 17:48:07.000000 arbmaster-0.1.3/src/arbmaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 17:48:07.000000 arbmaster-0.1.3/src/arbmaster.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 17:48:07.469337 arbmaster-0.1.3/tests/
--rw-rw-rw-   0        0        0     1581 2024-04-30 17:51:09.000000 arbmaster-0.1.3/tests/test_calc.py
--rw-rw-rw-   0        0        0     3440 2024-04-30 17:51:09.000000 arbmaster-0.1.3/tests/test_client.py
--rw-rw-rw-   0        0        0     4542 2024-04-30 17:51:09.000000 arbmaster-0.1.3/tests/test_ext.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:19:51.124283 arbmaster-0.1.4/
+-rw-rw-rw-   0        0        0     1086 2024-04-30 17:51:08.000000 arbmaster-0.1.4/LICENCE
+-rw-rw-rw-   0        0        0     1912 2024-05-19 12:19:51.124283 arbmaster-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1342 2024-05-17 17:15:54.000000 arbmaster-0.1.4/README.md
+-rw-rw-rw-   0        0        0      660 2024-05-19 11:57:18.000000 arbmaster-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:19:51.133913 arbmaster-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 12:19:51.041078 arbmaster-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 12:19:51.085348 arbmaster-0.1.4/src/arbmaster/
+-rw-rw-rw-   0        0        0      467 2024-05-17 17:15:56.000000 arbmaster-0.1.4/src/arbmaster/__init__.py
+-rw-rw-rw-   0        0        0     1553 2024-04-30 19:29:20.000000 arbmaster-0.1.4/src/arbmaster/calc.py
+-rw-rw-rw-   0        0        0     5772 2024-05-17 17:10:13.000000 arbmaster-0.1.4/src/arbmaster/client.py
+-rw-rw-rw-   0        0        0     6712 2024-05-17 16:51:26.000000 arbmaster-0.1.4/src/arbmaster/constants.py
+-rw-rw-rw-   0        0        0     4599 2024-05-19 12:17:11.000000 arbmaster-0.1.4/src/arbmaster/ext.py
+-rw-rw-rw-   0        0        0      527 2024-04-30 17:51:08.000000 arbmaster-0.1.4/src/arbmaster/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:19:51.124283 arbmaster-0.1.4/src/arbmaster.egg-info/
+-rw-rw-rw-   0        0        0     1912 2024-05-19 12:19:50.000000 arbmaster-0.1.4/src/arbmaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2024-05-19 12:19:51.000000 arbmaster-0.1.4/src/arbmaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:19:50.000000 arbmaster-0.1.4/src/arbmaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-19 12:19:50.000000 arbmaster-0.1.4/src/arbmaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 12:19:51.000000 arbmaster-0.1.4/src/arbmaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 12:19:51.121230 arbmaster-0.1.4/tests/
+-rw-rw-rw-   0        0        0     1581 2024-04-30 17:51:09.000000 arbmaster-0.1.4/tests/test_calc.py
+-rw-rw-rw-   0        0        0     3440 2024-04-30 17:51:09.000000 arbmaster-0.1.4/tests/test_client.py
+-rw-rw-rw-   0        0        0     4542 2024-04-30 17:51:09.000000 arbmaster-0.1.4/tests/test_ext.py
```

### Comparing `arbmaster-0.1.3/LICENCE` & `arbmaster-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.3/PKG-INFO` & `arbmaster-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arbmaster
-Version: 0.1.3
+Version: 0.1.4
 Summary: Odds api automated arbitrage calculator
 Author: Rashoo18
 License: MIT License
 Project-URL: Homepage, https://github.com/Rashoo18/arbmaster
 Project-URL: Issues, https://github.com/Rashoo18/arbmaster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arbmaster-0.1.3/README.md` & `arbmaster-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.3/pyproject.toml` & `arbmaster-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arbmaster"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
   "requests-cache",
   "colorlog",
 ]
 requires-python = ">=3.8"
 authors = [
   { name = "Rashoo18" },
```

### Comparing `arbmaster-0.1.3/src/arbmaster/calc.py` & `arbmaster-0.1.4/src/arbmaster/calc.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.3/src/arbmaster/client.py` & `arbmaster-0.1.4/src/arbmaster/client.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.3/src/arbmaster/constants.py` & `arbmaster-0.1.4/src/arbmaster/constants.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.3/src/arbmaster/ext.py` & `arbmaster-0.1.4/src/arbmaster/ext.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,26 @@
     key: str
     title: str
     home_odds: float
     away_odds: float
     draw_odds: Optional[float] = None
 
     @classmethod
-    def new(cls, bm_data: Dict[str, Any]) -> "Bookmaker":
+    def new(cls, hteam: str, bm_data: Dict[str, Any]) -> "Bookmaker":
         key: str = bm_data['key']
         title: str = bm_data['title']
         outcomes = bm_data['markets'][0]['outcomes']
-        home_odds: float = outcomes[0]['price']
-        away_odds: float = outcomes[1]['price']
+        
+        if hteam == outcomes[0]['name']:
+            home_odds: float = outcomes[0]['price']
+            away_odds: float = outcomes[1]['price']
+        else:
+            home_odds: float = outcomes[1]['price']
+            away_odds: float = outcomes[0]['price']
+        
         draw_odds: Optional[float] = None
         if len(outcomes) == 3:
             draw_odds = outcomes[2]['price']
         return cls(key, title, home_odds, away_odds, draw_odds)
 
     def json(self, price) -> Dict[str, Any]:
         return {
@@ -63,15 +69,15 @@
         self.id: str = match_data['id']
         self.sport_key: str = match_data['sport_key']
         self.sport_title: str = match_data['sport_title']
         self.home_team: str = match_data['home_team']
         self.away_team: str = match_data['away_team']
         
         if match_data.get("bookmakers", None) is not None:
-            odds: Odds = Odds([Bookmaker.new(b) for b in match_data['bookmakers']])
+            odds: Odds = Odds([Bookmaker.new(self.home_team, b) for b in match_data['bookmakers']])
             commence_time: str = make_europe_time(match_data['commence_time'])
         elif match_data.get("odds", None) is not None:
             odds: Odds = Odds.new(match_data['odds'])
             commence_time: str = match_data['commence_time']
         
         self.commence_time: str = commence_time
         self.odds: Odds = odds
```

### Comparing `arbmaster-0.1.3/src/arbmaster/logger.py` & `arbmaster-0.1.4/src/arbmaster/logger.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.3/src/arbmaster.egg-info/PKG-INFO` & `arbmaster-0.1.4/src/arbmaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arbmaster
-Version: 0.1.3
+Version: 0.1.4
 Summary: Odds api automated arbitrage calculator
 Author: Rashoo18
 License: MIT License
 Project-URL: Homepage, https://github.com/Rashoo18/arbmaster
 Project-URL: Issues, https://github.com/Rashoo18/arbmaster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arbmaster-0.1.3/tests/test_calc.py` & `arbmaster-0.1.4/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.3/tests/test_client.py` & `arbmaster-0.1.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.3/tests/test_ext.py` & `arbmaster-0.1.4/tests/test_ext.py`

 * *Files identical despite different names*

