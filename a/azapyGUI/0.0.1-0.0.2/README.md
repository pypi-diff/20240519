# Comparing `tmp/azapyGUI-0.0.1.tar.gz` & `tmp/azapygui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azapyGUI-0.0.1.tar", last modified: Tue Apr  9 20:22:54 2024, max compression
+gzip compressed data, was "azapygui-0.0.2.tar", last modified: Sun May 19 20:36:55 2024, max compression
```

## Comparing `azapyGUI-0.0.1.tar` & `azapygui-0.0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:22:54.741193 azapyGUI-0.0.1/
--rw-rw-rw-   0        0        0    35823 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4824 2024-04-09 20:22:54.738201 azapyGUI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3945 2024-04-09 08:38:06.000000 azapyGUI-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:22:54.721246 azapyGUI-0.0.1/azapyGUI/
--rw-rw-rw-   0        0        0    10189 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/AppSettingsPage.py
--rw-rw-rw-   0        0        0     4649 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/AppSettingsPageMisc.py
--rw-rw-rw-   0        0        0     1868 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/AppSettingsWindow.py
--rw-rw-rw-   0        0        0     6488 2024-04-08 03:44:30.000000 azapyGUI-0.0.1/azapyGUI/BacktestComputation.py
--rw-rw-rw-   0        0        0    14058 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/BacktestEntryWindow.py
--rw-rw-rw-   0        0        0      801 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/BacktestMenuPortfolioWindow.py
--rw-rw-rw-   0        0        0     3660 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/CloneMenuPortfolioWindow.py
--rw-rw-rw-   0        0        0     3062 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/CrossHairBCursor.py
--rw-rw-rw-   0        0        0     2694 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/DF_Window.py
--rw-rw-rw-   0        0        0    13218 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/DF_table.py
--rw-rw-rw-   0        0        0      667 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/EditMenuPortfolioWindow.py
--rw-rw-rw-   0        0        0    21277 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/EditPortfolioWindow.py
--rw-rw-rw-   0        0        0     1397 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/EntryClonePortfolioWindow.py
--rw-rw-rw-   0        0        0     2046 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/EntryNameWindow.py
--rw-rw-rw-   0        0        0     1324 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/EntryRenamePortfolioWindow.py
--rw-rw-rw-   0        0        0     3347 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/GetMktData.py
--rw-rw-rw-   0        0        0     7563 2024-03-31 05:16:17.000000 azapyGUI-0.0.1/azapyGUI/MenuApp.py
--rw-rw-rw-   0        0        0     5524 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/MktDataFrame.py
--rw-rw-rw-   0        0        0     1026 2024-04-03 06:03:10.000000 azapyGUI-0.0.1/azapyGUI/MktDataNode.py
--rw-rw-rw-   0        0        0     5721 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/ModelParamEditWindow.py
--rw-rw-rw-   0        0        0     2115 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/NrShares_table.py
--rw-rw-rw-   0        0        0     6828 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/PortAnalyseWindow.py
--rw-rw-rw-   0        0        0     5707 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/PortDataNode.py
--rw-rw-rw-   0        0        0     8002 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/PortfolioFrame.py
--rw-rw-rw-   0        0        0      809 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/RebalanceMenuPortfolioWindow.py
--rw-rw-rw-   0        0        0     1299 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/RemoveMenuPortfolioWindow.py
--rw-rw-rw-   0        0        0     1317 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/SaveMenuPortfolioWindow.py
--rw-rw-rw-   0        0        0     2175 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/Scrollable.py
--rw-rw-rw-   0        0        0     2412 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/SelectOneWindow.py
--rw-rw-rw-   0        0        0      839 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/SymbAnalyseWindow.py
--rw-rw-rw-   0        0        0     5629 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/SymbExtractWindow.py
--rw-rw-rw-   0        0        0     3422 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/SymbTableEntry.py
--rw-rw-rw-   0        0        0    21380 2024-04-03 07:39:14.000000 azapyGUI-0.0.1/azapyGUI/TimeSeriesViewWindow.py
--rw-rw-rw-   0        0        0     2382 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/ViewTip.py
--rw-rw-rw-   0        0        0    14912 2024-04-09 07:06:22.000000 azapyGUI-0.0.1/azapyGUI/WeightsWindow.py
--rw-rw-rw-   0        0        0      150 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/__init__.py
--rw-rw-rw-   0        0        0     1504 2024-04-09 05:27:14.000000 azapyGUI-0.0.1/azapyGUI/azHelper.py
--rw-rw-rw-   0        0        0     3391 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/azapyApp.py
--rw-rw-rw-   0        0        0     1318 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/config.py
--rw-rw-rw-   0        0        0     2997 2024-03-31 05:16:25.000000 azapyGUI-0.0.1/azapyGUI/configHelps.py
--rw-rw-rw-   0        0        0     9432 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/configMSG.py
--rw-rw-rw-   0        0        0    31708 2024-04-07 07:44:08.000000 azapyGUI-0.0.1/azapyGUI/configModels.py
--rw-rw-rw-   0        0        0     3314 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/configPlot.py
--rw-rw-rw-   0        0        0     9384 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/configSettings.py
--rw-rw-rw-   0        0        0     7518 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/configTips.py
--rw-rw-rw-   0        0        0     1451 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/mktDataValidation.py
--rw-rw-rw-   0        0        0    13162 2024-04-09 08:35:00.000000 azapyGUI-0.0.1/azapyGUI/modelParametersValidation.py
--rw-rw-rw-   0        0        0      794 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/serviceMasterUserConfig.py
--rw-rw-rw-   0        0        0      635 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/azapyGUI/tkHelper.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:22:54.736207 azapyGUI-0.0.1/azapyGUI.egg-info/
--rw-rw-rw-   0        0        0     4824 2024-04-09 20:22:54.000000 azapyGUI-0.0.1/azapyGUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3084 2024-04-09 20:22:54.000000 azapyGUI-0.0.1/azapyGUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:22:54.000000 azapyGUI-0.0.1/azapyGUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-09 20:22:54.000000 azapyGUI-0.0.1/azapyGUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 20:22:54.000000 azapyGUI-0.0.1/azapyGUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2024-03-31 04:41:24.000000 azapyGUI-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 20:22:54.741193 azapyGUI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1212 2024-04-09 07:18:10.000000 azapyGUI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:36:55.132413 azapygui-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-27 23:29:47.000000 azapygui-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4824 2024-05-19 20:36:55.130418 azapygui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3945 2024-04-27 23:29:47.000000 azapygui-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 20:36:55.113459 azapygui-0.0.2/azapyGUI/
+-rw-rw-rw-   0        0        0    10252 2024-05-10 02:57:05.000000 azapygui-0.0.2/azapyGUI/AppSettingsPage.py
+-rw-rw-rw-   0        0        0     4743 2024-05-10 02:56:56.000000 azapygui-0.0.2/azapyGUI/AppSettingsPageMisc.py
+-rw-rw-rw-   0        0        0     1868 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/AppSettingsWindow.py
+-rw-rw-rw-   0        0        0     6488 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/BacktestComputation.py
+-rw-rw-rw-   0        0        0    13836 2024-05-10 02:59:35.000000 azapygui-0.0.2/azapyGUI/BacktestEntryWindow.py
+-rw-rw-rw-   0        0        0      801 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/BacktestMenuPortfolioWindow.py
+-rw-rw-rw-   0        0        0     3660 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/CloneMenuPortfolioWindow.py
+-rw-rw-rw-   0        0        0     3062 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/CrossHairBCursor.py
+-rw-rw-rw-   0        0        0     2694 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/DF_Window.py
+-rw-rw-rw-   0        0        0    13218 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/DF_table.py
+-rw-rw-rw-   0        0        0      667 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/EditMenuPortfolioWindow.py
+-rw-rw-rw-   0        0        0    21513 2024-05-11 04:43:33.000000 azapygui-0.0.2/azapyGUI/EditPortfolioWindow.py
+-rw-rw-rw-   0        0        0     1397 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/EntryClonePortfolioWindow.py
+-rw-rw-rw-   0        0        0     2046 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/EntryNameWindow.py
+-rw-rw-rw-   0        0        0     1324 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/EntryRenamePortfolioWindow.py
+-rw-rw-rw-   0        0        0     3427 2024-05-10 03:23:18.000000 azapygui-0.0.2/azapyGUI/GetMktData.py
+-rw-rw-rw-   0        0        0     7563 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/MenuApp.py
+-rw-rw-rw-   0        0        0     5524 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/MktDataFrame.py
+-rw-rw-rw-   0        0        0     1026 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/MktDataNode.py
+-rw-rw-rw-   0        0        0     5721 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/ModelParamEditWindow.py
+-rw-rw-rw-   0        0        0     2115 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/NrShares_table.py
+-rw-rw-rw-   0        0        0     7125 2024-05-11 06:13:16.000000 azapygui-0.0.2/azapyGUI/PortAnalyseWindow.py
+-rw-rw-rw-   0        0        0     5707 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/PortDataNode.py
+-rw-rw-rw-   0        0        0     8002 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/PortfolioFrame.py
+-rw-rw-rw-   0        0        0      809 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/RebalanceMenuPortfolioWindow.py
+-rw-rw-rw-   0        0        0     1299 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/RemoveMenuPortfolioWindow.py
+-rw-rw-rw-   0        0        0     1317 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/SaveMenuPortfolioWindow.py
+-rw-rw-rw-   0        0        0     2175 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/Scrollable.py
+-rw-rw-rw-   0        0        0     2412 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/SelectOneWindow.py
+-rw-rw-rw-   0        0        0      839 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/SymbAnalyseWindow.py
+-rw-rw-rw-   0        0        0     5629 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/SymbExtractWindow.py
+-rw-rw-rw-   0        0        0     3422 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/SymbTableEntry.py
+-rw-rw-rw-   0        0        0    21380 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/TimeSeriesViewWindow.py
+-rw-rw-rw-   0        0        0     2382 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/ViewTip.py
+-rw-rw-rw-   0        0        0    14912 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/WeightsWindow.py
+-rw-rw-rw-   0        0        0      150 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/__init__.py
+-rw-rw-rw-   0        0        0     1504 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/azHelper.py
+-rw-rw-rw-   0        0        0     3391 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/azapyApp.py
+-rw-rw-rw-   0        0        0     1318 2024-05-10 02:52:29.000000 azapygui-0.0.2/azapyGUI/config.py
+-rw-rw-rw-   0        0        0     2997 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/configHelps.py
+-rw-rw-rw-   0        0        0     9432 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/configMSG.py
+-rw-rw-rw-   0        0        0    31708 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/configModels.py
+-rw-rw-rw-   0        0        0     3314 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/configPlot.py
+-rw-rw-rw-   0        0        0     9380 2024-05-10 02:37:18.000000 azapygui-0.0.2/azapyGUI/configSettings.py
+-rw-rw-rw-   0        0        0     7518 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/configTips.py
+-rw-rw-rw-   0        0        0     1451 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/mktDataValidation.py
+-rw-rw-rw-   0        0        0    13162 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/modelParametersValidation.py
+-rw-rw-rw-   0        0        0      794 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/serviceMasterUserConfig.py
+-rw-rw-rw-   0        0        0      635 2024-04-27 23:29:47.000000 azapygui-0.0.2/azapyGUI/tkHelper.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:36:55.128423 azapygui-0.0.2/azapyGUI.egg-info/
+-rw-rw-rw-   0        0        0     4824 2024-05-19 20:36:54.000000 azapygui-0.0.2/azapyGUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3084 2024-05-19 20:36:54.000000 azapygui-0.0.2/azapyGUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 20:36:54.000000 azapygui-0.0.2/azapyGUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-19 20:36:54.000000 azapygui-0.0.2/azapyGUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 20:36:54.000000 azapygui-0.0.2/azapyGUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2024-04-27 23:29:47.000000 azapygui-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 20:36:55.132413 azapygui-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1212 2024-05-10 02:52:51.000000 azapygui-0.0.2/setup.py
```

### Comparing `azapyGUI-0.0.1/LICENSE` & `azapygui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/PKG-INFO` & `azapygui-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azapyGUI
-Version: 0.0.1
+Version: 0.0.2
 Summary: GUI for azapy library - Financial Portfolio Optimization Algorithms
 Home-page: https://github.com/Mircea-MMXXI/azapyGUI.git
 Author: Mircea Marinescu
 Author-email: mircea.marinescu@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://azapyGUI.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/Mircea-MMXXI/azapyGUI
```

### Comparing `azapyGUI-0.0.1/README.md` & `azapygui-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/AppSettingsPage.py` & `azapygui-0.0.2/azapyGUI/AppSettingsPage.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         
         frm_view = tk.Frame(master=frm, width=150)
         frm_view.grid(row=0, column=1, padx=5, pady=5, sticky=tk.NSEW)
         frm.columnconfigure(1, weight=1)
         
         # on frm_set
         self._setDef = configSettings.settings_model[self._category]
-        self.settings = deepcopy(configSettings.MasterApplicationSettings)
+        #self.settings = deepcopy(configSettings.MasterApplicationSettings)
+        self.settings = {key: configSettings.MasterApplicationSettings[key] for key in self._setDef.keys()}
         row = 0
         self._chk_val = {}
         self._chk_btn = {}
         for param, value in self._setDef.items():
             match value["type"]:
                 case 'ButtonDir':
                     btn = tk.Button(master=frm_set, text=value['field'], width=18, 
@@ -152,15 +153,15 @@
                                                          parent=self._window, 
                                                          initialvalue=vv["default"])
                         if vpar == '':
                             vpar = configSettings.get_envkey(pp)
                             if vpar is None:
                                 msg = (configMSG._validate_provider_key_msg
                                        +'\n' 
-                                       + configSettings.get_envkey_valriable_name(pp))
+                                       + configSettings.get_envkey_vriable_name(pp))
                                 tk.messagebox.showwarning(title="Warning", message=msg, parent=self._window)
                                 del self.settings[param][pp]
                                 self._chk_btn[param][pp].deselect()
                                 return
                         self.settings[param][pp][kk] = vpar
                     case 'int':
                         vpar = tk.simpledialog.askinteger(pp, vv["field"], 
@@ -185,18 +186,17 @@
     def _btn_cancel_func(self):
         if self._master.winfo_exists():
             self._master.grab_release()
         self._master.destroy()
         
         
     def _btn_save_func(self):
-        configSettings.MasterApplicationSettings = deepcopy(self.settings)
-        _saveMasterUserConfig(configSettings.MasterApplicationSettings)
-        #self._btn_cancel_func()
-        
+        configSettings.MasterApplicationSettings.update(self.settings)
+        _saveMasterUserConfig(configSettings.MasterApplicationSettings) 
+
         
     def _btn_reset_func(self):
         for kk, vv in self._setDef.items():
             self.settings[kk] = deepcopy(vv["default"])
             match vv["type"]:
                 case "Checkbutton":
                     if self.settings[kk]:
```

### Comparing `azapyGUI-0.0.1/azapyGUI/AppSettingsPageMisc.py` & `azapygui-0.0.2/azapyGUI/AppSettingsPageMisc.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         frm_set.columnconfigure(1, weight=1)
         
         frm_btn = tk.Frame(master=self._window)
         frm_btn.grid(row=1, column=0, padx=5, pady=5, sticky=tk.EW)
         
         # on frm
         self._setDef = configSettings.settings_model[self._category]
-        self.settings = deepcopy(configSettings.MasterApplicationSettings)
+        #self.settings = deepcopy(configSettings.MasterApplicationSettings)
+        self.settings = {key: configSettings.MasterApplicationSettings[key] for key in self._setDef.keys()}
         row = 0
         self._chk_val = {}
         self._chk_btn = {}
         for param, value in self._setDef.items():
             match value["type"]:
                 case 'Checkbutton':
                     lbl = tk.Label(master=frm_set, text=value["field"], anchor=tk.W)
@@ -88,14 +89,13 @@
                     else:
                         self._chk_btn[kk].deselect()
                 case "Entry":
                     self._chk_val[kk].set(self.settings[kk])
         
         
     def _btn_save_func(self):
-        for param in self._chk_val.keys():
-            self.settings[param] = self._chk_val[param].get()
-        configSettings.MasterApplicationSettings = deepcopy(self.settings)
+        self.settings.update({key: self._chk_val[key].get() for key in self._chk_val.keys()})
+        configSettings.MasterApplicationSettings.update(self.settings)
         _saveMasterUserConfig(configSettings.MasterApplicationSettings)
         config.tiptil.turned(on=configSettings.MasterApplicationSettings["ShowTips"])
```

### Comparing `azapyGUI-0.0.1/azapyGUI/AppSettingsWindow.py` & `azapygui-0.0.2/azapyGUI/AppSettingsWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/BacktestComputation.py` & `azapygui-0.0.2/azapyGUI/BacktestComputation.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/BacktestEntryWindow.py` & `azapygui-0.0.2/azapyGUI/BacktestEntryWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,19 +146,16 @@
         frm_btn.pack(fill=tk.BOTH, expand=True, padx=5, pady=5)
         
         self._btn_cancel = tk.Button(master=frm_btn, text='Cancel', width=12, command=self._btn_cancel_func)
         self._btn_cancel.pack(side=tk.LEFT, padx=5, pady=5,)
         
         self._btn_start = tk.Button(master=frm_btn, text='Start', width=12, command=self._btn_start_func)
         self._btn_start.pack(side=tk.RIGHT, padx=5, pady=5,)
-        
-        # self._frm_progress = tk.LabelFrame(master=self._window, text="Progress", font=("Forte", 10), height=200, width=300)
-        # self._frm_progress.pack(fill=tk.X, expand=False, padx=5, pady=5)
- 
-        
+
+
     def _destroy_all_windows(self):
         for widget in self._window.winfo_children():
             if isinstance(widget, tk.Toplevel):
                 widget.destroy()
     
     
     def _on_exit(self):
```

### Comparing `azapyGUI-0.0.1/azapyGUI/BacktestMenuPortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/BacktestMenuPortfolioWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/CloneMenuPortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/CloneMenuPortfolioWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/CrossHairBCursor.py` & `azapygui-0.0.2/azapyGUI/CrossHairBCursor.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/DF_Window.py` & `azapygui-0.0.2/azapyGUI/DF_Window.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/DF_table.py` & `azapygui-0.0.2/azapyGUI/DF_table.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/EditMenuPortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/EditMenuPortfolioWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/EditPortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/EditPortfolioWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,21 +143,25 @@
         self._set_tree_menu_selector()
         self._set_tree_menu_optimizer()
         
         
     def _tree_model_write(self):
         for name, selector in self.portfolio.selectors.items():
             item = self._tree_model.insert("", selector['index'], text=name, tags=("m_selector",))
+            invisible = configModels.param_default(name, visible=False)
             for kk, vv in selector['param'].items():
-                self._tree_model.insert(item, tk.END, text=kk +" =" + str(vv)) 
+                if kk in invisible: continue
+                self._tree_model.insert(item, tk.END, text=kk +" = "+ str(vv)) 
                 
         for name, optimizer in self.portfolio.optimizer.items():
             item = self._tree_model.insert("", tk.END, text=name, tags=("m_optimizer",)) 
+            invisible = configModels.param_default(name, visible=False)
             for kk, vv in optimizer['param'].items():
-                self._tree_model.insert(item, tk.END, text=kk + " = " + str(vv))
+                if kk in invisible: continue
+                self._tree_model.insert(item, tk.END, text=kk +" = "+ str(vv))
         
         
     def _set_tree_menu_selector(self):
         self._tree_menu_selector = tk.Menu(self._tree_model, tearoff = 0) 
         self._tree_menu_selector.add_command(label ="Edit", command=self._tree_menu_selector_edit_func) 
         self._tree_menu_selector.add_command(label ="Move Up", command=self._tree_menu_selector_moveup_func) 
         self._tree_menu_selector.add_command(label ="Move Down", command=self._tree_menu_selector_movedown_func)
```

### Comparing `azapyGUI-0.0.1/azapyGUI/EntryClonePortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/EntryClonePortfolioWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/EntryNameWindow.py` & `azapygui-0.0.2/azapyGUI/EntryNameWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/EntryRenamePortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/EntryRenamePortfolioWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/GetMktData.py` & `azapygui-0.0.2/azapyGUI/GetMktData.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,26 +15,27 @@
         for kk, vv in configSettings.MasterApplicationSettings["Provider"][source].items():
             if kk == "key":
                 api_key = vv["key"]
             else:
                 param[kk] = vv
                 
         file_dir = configSettings.MasterApplicationSettings["UserMktDataDirectory"]
+        fsave, fforce = (False, True) if file_dir is None else (True, force)
         
         self._symb_req_default = {"symbol": None,
                                   "sdate": None,
                                   "edate": None,
                                   "output_format": 'dict',
                                   "source": source,
-                                  "force": force,
-                                  "save": True,
+                                  "force": fforce,
+                                  "save": fsave,
                                   "file_dir": file_dir,
                                   "file_format": 'csv',
-                                  'api_key': api_key,
-                                  'param': param,
+                                  "api_key": api_key,
+                                  "param": param,
                                   }
         self._mktr = az.MkTreader(verbose=False)
         
         
     def getMkTDataSymb(self, symbols, sdate, edate):
         # sdate and edate are assumed to be validated
         self._symb_req = deepcopy(self._symb_req_default)
```

### Comparing `azapyGUI-0.0.1/azapyGUI/MenuApp.py` & `azapygui-0.0.2/azapyGUI/MenuApp.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/MktDataFrame.py` & `azapygui-0.0.2/azapyGUI/MktDataFrame.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/MktDataNode.py` & `azapygui-0.0.2/azapyGUI/MktDataNode.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/ModelParamEditWindow.py` & `azapygui-0.0.2/azapyGUI/ModelParamEditWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/NrShares_table.py` & `azapygui-0.0.2/azapyGUI/NrShares_table.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/PortAnalyseWindow.py` & `azapygui-0.0.2/azapyGUI/PortAnalyseWindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
         
     
     def _spec_rep_summary(self, pname):
         pp = self._ports[pname]
         rep = pp.port_perf()
         cols = ['RR', 'DD', 'RoMaD']
         rep[cols] = (rep[cols] * 100).round(2)
+        rep.index = pd.Categorical(rep.index, categories=rep.index, ordered=True)
+        rep.index.name = 'Symbols'
         
         return rep, f'{pname} Summary', '400x200'
     
     
     def _spec_rep_weights(self, pname):
         pp = self._ports[pname]
         rep = pp.get_weights().set_index(['Droll', 'Dfix'])
@@ -85,14 +87,15 @@
 
 
     def _spec_rep_quarterly(self, pname):
         pp = self._ports[pname]
         rep = pp.port_quarterly_returns(withcomp=True)
         rep = (rep * 100).round(2)
         rep.rename(columns={'close': pname}, inplace=True)
+        rep.columns = pd.Categorical(rep.columns, categories=rep.columns, ordered=True)
         rep.columns.name = 'Symbols'
         
         rep.index = pd.MultiIndex.from_arrays(
                                 [rep.index.year.to_list(),
                                  ['Q' + str(k) for k in rep.index.quarter]],
                                  names= ['year', 'quarter'])
  
@@ -102,14 +105,15 @@
     
     
     def _spec_rep_monthly(self, pname):
         pp = self._ports[pname]
         rep = pp.port_monthly_returns(withcomp=True)
         rep = (rep * 100).round(2)
         rep.rename(columns={'close': pname}, inplace=True)
+        rep.columns = pd.Categorical(rep.columns, categories=rep.columns, ordered=True)
         rep.columns.name = 'Symbols'
         
         rep.index = pd.MultiIndex.from_arrays(
                                 [rep.index.year.to_list(),
                                  rep.index.month_name().to_list()],
                                  names= ['year', 'month'])
```

### Comparing `azapyGUI-0.0.1/azapyGUI/PortDataNode.py` & `azapygui-0.0.2/azapyGUI/PortDataNode.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/PortfolioFrame.py` & `azapygui-0.0.2/azapyGUI/PortfolioFrame.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/RebalanceMenuPortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/RebalanceMenuPortfolioWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/RemoveMenuPortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/RemoveMenuPortfolioWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/SaveMenuPortfolioWindow.py` & `azapygui-0.0.2/azapyGUI/SaveMenuPortfolioWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/Scrollable.py` & `azapygui-0.0.2/azapyGUI/Scrollable.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/SelectOneWindow.py` & `azapygui-0.0.2/azapyGUI/SelectOneWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/SymbAnalyseWindow.py` & `azapygui-0.0.2/azapyGUI/SymbAnalyseWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/SymbExtractWindow.py` & `azapygui-0.0.2/azapyGUI/SymbExtractWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/SymbTableEntry.py` & `azapygui-0.0.2/azapyGUI/SymbTableEntry.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/TimeSeriesViewWindow.py` & `azapygui-0.0.2/azapyGUI/TimeSeriesViewWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/ViewTip.py` & `azapygui-0.0.2/azapyGUI/ViewTip.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/WeightsWindow.py` & `azapygui-0.0.2/azapyGUI/WeightsWindow.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/azHelper.py` & `azapygui-0.0.2/azapyGUI/azHelper.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/azapyApp.py` & `azapygui-0.0.2/azapyGUI/azapyApp.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/config.py` & `azapygui-0.0.2/azapyGUI/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 MktDataDict = {}
 PortDataDict = {}
 
 appPortfolioFrame = None
 appMktDataFrame = None
```

### Comparing `azapyGUI-0.0.1/azapyGUI/configHelps.py` & `azapygui-0.0.2/azapyGUI/configHelps.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/configMSG.py` & `azapygui-0.0.2/azapyGUI/configMSG.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/configModels.py` & `azapygui-0.0.2/azapyGUI/configModels.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/configPlot.py` & `azapygui-0.0.2/azapyGUI/configPlot.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/configSettings.py` & `azapygui-0.0.2/azapyGUI/configSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,16 @@
     rout = {}
     rout["Version"] = Version
     for category in settings_model.keys():
         rout.update(get_settings_default(category))
     return rout
     
 
-def get_envkey_valriable_name(provider):
+def get_envkey_vriable_name(provider):
     return settings_model["MkTData"]["Provider"]["values"][provider]["key"]["envkey"]
 
 
 def get_envkey(provider):
-    return os.getenv(get_envkey_valriable_name(provider))
+    return os.getenv(get_envkey_vriable_name(provider))
 
 
 MasterApplicationSettings = None
```

### Comparing `azapyGUI-0.0.1/azapyGUI/configTips.py` & `azapygui-0.0.2/azapyGUI/configTips.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/mktDataValidation.py` & `azapygui-0.0.2/azapyGUI/mktDataValidation.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/modelParametersValidation.py` & `azapygui-0.0.2/azapyGUI/modelParametersValidation.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/serviceMasterUserConfig.py` & `azapygui-0.0.2/azapyGUI/serviceMasterUserConfig.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI/tkHelper.py` & `azapygui-0.0.2/azapyGUI/tkHelper.py`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/azapyGUI.egg-info/PKG-INFO` & `azapygui-0.0.2/azapyGUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azapyGUI
-Version: 0.0.1
+Version: 0.0.2
 Summary: GUI for azapy library - Financial Portfolio Optimization Algorithms
 Home-page: https://github.com/Mircea-MMXXI/azapyGUI.git
 Author: Mircea Marinescu
 Author-email: mircea.marinescu@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://azapyGUI.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/Mircea-MMXXI/azapyGUI
```

### Comparing `azapyGUI-0.0.1/azapyGUI.egg-info/SOURCES.txt` & `azapygui-0.0.2/azapyGUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azapyGUI-0.0.1/setup.py` & `azapygui-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="azapyGUI",
-    version="0.0.1",
+    version="0.0.2",
     author="Mircea Marinescu",
     author_email="mircea.marinescu@outlook.com",
     description="GUI for azapy library - Financial Portfolio Optimization Algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Mircea-MMXXI/azapyGUI.git",
     project_urls={
```

