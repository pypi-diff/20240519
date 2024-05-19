# Comparing `tmp/poker_now_log_converter-0.0.8.tar.gz` & `tmp/poker_now_log_converter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poker_now_log_converter-0.0.8.tar", last modified: Thu Oct 20 15:28:28 2022, max compression
+gzip compressed data, was "poker_now_log_converter-0.0.9.tar", last modified: Tue Oct 25 16:27:32 2022, max compression
```

## Comparing `poker_now_log_converter-0.0.8.tar` & `poker_now_log_converter-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 15:28:28.546740 poker_now_log_converter-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (121)     4957 2022-10-20 15:28:28.546740 poker_now_log_converter-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-20 15:28:28.546740 poker_now_log_converter-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 15:28:28.542740 poker_now_log_converter-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 15:28:28.542740 poker_now_log_converter-0.0.8/src/poker_now_log_converter/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/action.py
--rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/card.py
--rw-r--r--   0 runner    (1001) docker     (121)    30150 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/game.py
--rw-r--r--   0 runner    (1001) docker     (121)    20595 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/hand.py
--rw-r--r--   0 runner    (1001) docker     (121)    14508 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/player.py
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/seat.py
--rw-r--r--   0 runner    (1001) docker     (121)    13815 2022-10-20 15:28:10.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 15:28:28.546740 poker_now_log_converter-0.0.8/src/poker_now_log_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4957 2022-10-20 15:28:28.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-10-20 15:28:28.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 15:28:28.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-20 15:28:28.000000 poker_now_log_converter-0.0.8/src/poker_now_log_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:27:32.975611 poker_now_log_converter-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (121)     5026 2022-10-25 16:27:32.975611 poker_now_log_converter-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4356 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-25 16:27:32.975611 poker_now_log_converter-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:27:32.975611 poker_now_log_converter-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:27:32.975611 poker_now_log_converter-0.0.9/src/poker_now_log_converter/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/action.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/card.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30150 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/game.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20595 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/hand.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14508 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/player.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/seat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13815 2022-10-25 16:27:22.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:27:32.975611 poker_now_log_converter-0.0.9/src/poker_now_log_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5026 2022-10-25 16:27:32.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-10-25 16:27:32.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 16:27:32.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-25 16:27:32.000000 poker_now_log_converter-0.0.9/src/poker_now_log_converter.egg-info/top_level.txt
```

### Comparing `poker_now_log_converter-0.0.8/LICENSE.TXT` & `poker_now_log_converter-0.0.9/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/PKG-INFO` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: poker_now_log_converter
-Version: 0.0.8
+Name: poker-now-log-converter
+Version: 0.0.9
 Summary: A simple command line utility for converting logs from Poker Now games to other formats
 Home-page: https://github.com/charlestudor/PokerNowLogConverter
 Author: Charles Tudor
 Author-email: mail@ctudor.net
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # &#127137; Poker Now Log Converter &#127137;
@@ -36,34 +37,37 @@
 This project was written for my personal use, and is not affiliated, endorsed or sponsored by the Poker Now team.
 
 ## Features
 
 - Cross platform: Windows, Mac and Linux
 - Supports log files from Poker Now version 0.1.53 (06/24/2020) to present.
 - Run from the command line, or include as a python library. (Supports >=Python 3.8)
-- Outputs log files in PokerStars format. (OpenHH Format on the way)
-- Currently supports only Texas Hold'em cash games (Omaha and tournaments on the way)
+- Outputs log files in PokerStars format.
+- Currently supports only Texas Hold'em cash games.
 - Can adjust log output settings such as currency and timezone.
 - Use **Interactive Alias Mode** from the command line to easily rename players seen during poker hands to their known aliases.
  
 ## Installation
 
-Poker Now Log Converter supports Python 3.8, 3.9 and 3.10.
+Poker Now Log Converter supports Python 3.8 to 3.11.
 
 ### 1. Install via [Pip](http://www.pip-installer.org/):
 
     $ pip install poker-now-log-converter
+    $ python -m poker_now_log_converter 
 
 ### 2. Install from Git:
     $ git clone git://github.com/charlestudor/PokerNowLogConverter
     $ python setup.py install
+    $ python -m poker_now_log_converter 
+
     
 ### 3. Use as a script without installing
     $ git clone git://github.com/charlestudor/PokerNowLogConverter
-    $ python PokerNowLogConverter
+    $ python ./PokerNowLogConverter
 
 ## Usage
 
 As a command line tool:
 
     $ python -m poker_now_log_converter -h
```

### Comparing `poker_now_log_converter-0.0.8/README.md` & `poker_now_log_converter-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,34 +20,37 @@
 This project was written for my personal use, and is not affiliated, endorsed or sponsored by the Poker Now team.
 
 ## Features
 
 - Cross platform: Windows, Mac and Linux
 - Supports log files from Poker Now version 0.1.53 (06/24/2020) to present.
 - Run from the command line, or include as a python library. (Supports >=Python 3.8)
-- Outputs log files in PokerStars format. (OpenHH Format on the way)
-- Currently supports only Texas Hold'em cash games (Omaha and tournaments on the way)
+- Outputs log files in PokerStars format.
+- Currently supports only Texas Hold'em cash games.
 - Can adjust log output settings such as currency and timezone.
 - Use **Interactive Alias Mode** from the command line to easily rename players seen during poker hands to their known aliases.
  
 ## Installation
 
-Poker Now Log Converter supports Python 3.8, 3.9 and 3.10.
+Poker Now Log Converter supports Python 3.8 to 3.11.
 
 ### 1. Install via [Pip](http://www.pip-installer.org/):
 
     $ pip install poker-now-log-converter
+    $ python -m poker_now_log_converter 
 
 ### 2. Install from Git:
     $ git clone git://github.com/charlestudor/PokerNowLogConverter
     $ python setup.py install
+    $ python -m poker_now_log_converter 
+
     
 ### 3. Use as a script without installing
     $ git clone git://github.com/charlestudor/PokerNowLogConverter
-    $ python PokerNowLogConverter
+    $ python ./PokerNowLogConverter
 
 ## Usage
 
 As a command line tool:
 
     $ python -m poker_now_log_converter -h
```

### Comparing `poker_now_log_converter-0.0.8/setup.cfg` & `poker_now_log_converter-0.0.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [metadata]
 name = poker_now_log_converter
-version = 0.0.8
+version = 0.0.9
 author = Charles Tudor
 author_email = mail@ctudor.net
 description = A simple command line utility for converting logs from Poker Now games to other formats
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/charlestudor/PokerNowLogConverter
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
```

### Comparing `poker_now_log_converter-0.0.8/setup.py` & `poker_now_log_converter-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="poker_now_log_converter",
     version=VERSION,
@@ -13,14 +13,15 @@
     description="A simple command line utility for converting logs from Poker Now games to other formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/charlestudor/PokerNowLogConverter",
     classifiers=["Programming Language :: Python :: 3.8",
                  "Programming Language :: Python :: 3.9",
                  "Programming Language :: Python :: 3.10",
+                 "Programming Language :: Python :: 3.11",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.8",
 )
```

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter/action.py` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter/action.py`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter/card.py` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter/card.py`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter/game.py` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter/game.py`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter/hand.py` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter/hand.py`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter/main.py` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter/main.py`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter/player.py` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter/player.py`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter/seat.py` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter/seat.py`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter/utils.py` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter/utils.py`

 * *Files identical despite different names*

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter.egg-info/PKG-INFO` & `poker_now_log_converter-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: poker-now-log-converter
-Version: 0.0.8
+Name: poker_now_log_converter
+Version: 0.0.9
 Summary: A simple command line utility for converting logs from Poker Now games to other formats
 Home-page: https://github.com/charlestudor/PokerNowLogConverter
 Author: Charles Tudor
 Author-email: mail@ctudor.net
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # &#127137; Poker Now Log Converter &#127137;
@@ -36,34 +37,37 @@
 This project was written for my personal use, and is not affiliated, endorsed or sponsored by the Poker Now team.
 
 ## Features
 
 - Cross platform: Windows, Mac and Linux
 - Supports log files from Poker Now version 0.1.53 (06/24/2020) to present.
 - Run from the command line, or include as a python library. (Supports >=Python 3.8)
-- Outputs log files in PokerStars format. (OpenHH Format on the way)
-- Currently supports only Texas Hold'em cash games (Omaha and tournaments on the way)
+- Outputs log files in PokerStars format.
+- Currently supports only Texas Hold'em cash games.
 - Can adjust log output settings such as currency and timezone.
 - Use **Interactive Alias Mode** from the command line to easily rename players seen during poker hands to their known aliases.
  
 ## Installation
 
-Poker Now Log Converter supports Python 3.8, 3.9 and 3.10.
+Poker Now Log Converter supports Python 3.8 to 3.11.
 
 ### 1. Install via [Pip](http://www.pip-installer.org/):
 
     $ pip install poker-now-log-converter
+    $ python -m poker_now_log_converter 
 
 ### 2. Install from Git:
     $ git clone git://github.com/charlestudor/PokerNowLogConverter
     $ python setup.py install
+    $ python -m poker_now_log_converter 
+
     
 ### 3. Use as a script without installing
     $ git clone git://github.com/charlestudor/PokerNowLogConverter
-    $ python PokerNowLogConverter
+    $ python ./PokerNowLogConverter
 
 ## Usage
 
 As a command line tool:
 
     $ python -m poker_now_log_converter -h
```

### Comparing `poker_now_log_converter-0.0.8/src/poker_now_log_converter.egg-info/SOURCES.txt` & `poker_now_log_converter-0.0.9/src/poker_now_log_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

