# Comparing `tmp/pkscreener-0.45.20240518.383.tar.gz` & `tmp/pkscreener-0.45.20240519.385.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240518.383.tar", last modified: Sat May 18 00:49:54 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240519.385.tar", last modified: Sun May 19 02:25:02 2024, max compression
```

## Comparing `pkscreener-0.45.20240518.383.tar` & `pkscreener-0.45.20240519.385.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 00:49:54.541392 pkscreener-0.45.20240518.383/
--rw-rw-rw-   0        0        0     1086 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-18 00:49:54.541392 pkscreener-0.45.20240518.383/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 00:49:54.525775 pkscreener-0.45.20240518.383/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:49:54.541392 pkscreener-0.45.20240518.383/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34249 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45624 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156140 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56423 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    84899 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-18 00:49:44.000000 pkscreener-0.45.20240518.383/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   145015 2024-05-18 00:45:53.000000 pkscreener-0.45.20240518.383/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1089 2024-05-18 00:45:54.000000 pkscreener-0.45.20240518.383/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53044 2024-05-18 00:45:54.000000 pkscreener-0.45.20240518.383/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34360 2024-05-18 00:45:54.000000 pkscreener-0.45.20240518.383/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:49:54.525775 pkscreener-0.45.20240518.383/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-18 00:49:54.000000 pkscreener-0.45.20240518.383/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-18 00:49:54.000000 pkscreener-0.45.20240518.383/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 00:49:54.000000 pkscreener-0.45.20240518.383/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-18 00:49:54.000000 pkscreener-0.45.20240518.383/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 00:49:54.000000 pkscreener-0.45.20240518.383/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-18 00:49:54.000000 pkscreener-0.45.20240518.383/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-18 00:49:54.541392 pkscreener-0.45.20240518.383/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-18 00:45:54.000000 pkscreener-0.45.20240518.383/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 02:25:02.019537 pkscreener-0.45.20240519.385/
+-rw-rw-rw-   0        0        0     1086 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-19 02:25:02.019537 pkscreener-0.45.20240519.385/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 02:25:02.003940 pkscreener-0.45.20240519.385/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 02:25:02.019537 pkscreener-0.45.20240519.385/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34249 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45624 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156140 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56423 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    84899 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-19 02:24:53.000000 pkscreener-0.45.20240519.385/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   145055 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1089 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53044 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34360 2024-05-19 02:19:16.000000 pkscreener-0.45.20240519.385/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-19 02:25:02.019537 pkscreener-0.45.20240519.385/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-19 02:25:01.000000 pkscreener-0.45.20240519.385/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-19 02:25:01.000000 pkscreener-0.45.20240519.385/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 02:25:01.000000 pkscreener-0.45.20240519.385/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-19 02:25:01.000000 pkscreener-0.45.20240519.385/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 02:25:01.000000 pkscreener-0.45.20240519.385/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-19 02:25:01.000000 pkscreener-0.45.20240519.385/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-19 02:25:02.019537 pkscreener-0.45.20240519.385/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-19 02:19:17.000000 pkscreener-0.45.20240519.385/setup.py
```

### Comparing `pkscreener-0.45.20240518.383/LICENSE` & `pkscreener-0.45.20240519.385/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/LICENSE-Others` & `pkscreener-0.45.20240519.385/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/PKG-INFO` & `pkscreener-0.45.20240519.385/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240518.383
+Version: 0.45.20240519.385
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240518.383.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240519.385.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240518.383/README.md` & `pkscreener-0.45.20240519.385/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240518.383/pkscreener/__init__.py` & `pkscreener-0.45.20240519.385/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/Barometer.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,9 +98,7 @@
         gmbPath = os.path.join(folderPath,"gmb.png")
         # gmbCombined.show()
     except: #Exception as e:
         # print(e)
         pass
     return gmbPath
 
-# getGlobalMarketBarometerValuation()
-# getBaseImage(255,255)
```

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/classes/keys.py` & `pkscreener-0.45.20240519.385/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/courbd.ttf` & `pkscreener-0.45.20240519.385/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/globals.py` & `pkscreener-0.45.20240519.385/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1540,15 +1540,15 @@
                 runOption = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 df = saveResults.copy()
                 df["LastTradeDate"], df["LastTradeTime"] = getLatestTradeDateTime(stockDictPrimary)
                 gClient.df_to_sheet(df=df,sheetName=runOption)
                 OutputControls().printOutput(f"{colorText.GREEN} => Done in {round(time.time()-begin,2)}s{colorText.END}")
     except:
         pass
-    if userPassedArgs is None or (userPassedArgs is not None and (userPassedArgs.answerdefault is None or userPassedArgs.systemlaunched)):
+    if "RUNNER" not in os.environ.keys() and (userPassedArgs is None or (userPassedArgs is not None and (userPassedArgs.answerdefault is None or userPassedArgs.systemlaunched))):
         prevOutput_results = saveResults.index if (saveResults is not None and not saveResults.empty) else []
         hasFoundStocks = len(prevOutput_results) > 0 and (("|" not in userPassedArgs.options) if (userPassedArgs is not None and userPassedArgs.options is not None) else True)
         if hasFoundStocks:
             monitorOption = userPassedArgs.systemlaunched if (userPassedArgs is not None and isinstance(userPassedArgs.systemlaunched,str) and userPassedArgs.systemlaunched is not None) else (userPassedArgs.options if (userPassedArgs is not None and userPassedArgs.options is not None) else "")
             if len(monitorOption) == 0:
                 for choice in selectedChoice.keys():
                     monitorOption = (f"{monitorOption}:" if len(monitorOption) > 0  else '') + f"{selectedChoice[choice]}"
```

### Comparing `pkscreener-0.45.20240518.383/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240519.385/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240519.385/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240519.385/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240519.385/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240518.383
+Version: 0.45.20240519.385
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240518.383.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240519.385.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240517.382/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240518.383/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240518.383/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240519.385/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240518.383/setup.py` & `pkscreener-0.45.20240519.385/setup.py`

 * *Files identical despite different names*

