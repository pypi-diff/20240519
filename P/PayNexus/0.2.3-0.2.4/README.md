# Comparing `tmp/paynexus-0.2.3.tar.gz` & `tmp/paynexus-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paynexus-0.2.3.tar", last modified: Sat May 18 07:11:42 2024, max compression
+gzip compressed data, was "paynexus-0.2.4.tar", last modified: Sat May 18 14:55:24 2024, max compression
```

## Comparing `paynexus-0.2.3.tar` & `paynexus-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 07:11:42.063836 paynexus-0.2.3/
--rw-rw-rw-   0        0        0     1324 2024-05-17 14:22:20.000000 paynexus-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    14507 2024-05-18 07:11:42.062840 paynexus-0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 07:11:42.061843 paynexus-0.2.3/PayNexus.egg-info/
--rw-rw-rw-   0        0        0    14507 2024-05-18 07:11:41.000000 paynexus-0.2.3/PayNexus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-18 07:11:41.000000 paynexus-0.2.3/PayNexus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 07:11:41.000000 paynexus-0.2.3/PayNexus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-18 07:11:41.000000 paynexus-0.2.3/PayNexus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 07:11:41.000000 paynexus-0.2.3/PayNexus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13149 2024-05-18 07:04:36.000000 paynexus-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 07:11:42.060846 paynexus-0.2.3/paynexus/
--rw-rw-rw-   0        0        0    14926 2024-05-17 23:25:22.000000 paynexus-0.2.3/paynexus/Colors.py
--rw-rw-rw-   0        0        0       93 2024-05-18 07:11:39.000000 paynexus-0.2.3/paynexus/__init__.py
--rw-rw-rw-   0        0        0    22191 2024-05-18 07:03:09.000000 paynexus-0.2.3/paynexus/main.py
--rw-rw-rw-   0        0        0       42 2024-05-18 07:11:42.063836 paynexus-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2133 2024-05-18 07:10:48.000000 paynexus-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:55:24.431488 paynexus-0.2.4/
+-rw-rw-rw-   0        0        0     1324 2024-05-17 14:22:20.000000 paynexus-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0    14487 2024-05-18 14:55:24.430491 paynexus-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 14:55:24.430491 paynexus-0.2.4/PayNexus.egg-info/
+-rw-rw-rw-   0        0        0    14487 2024-05-18 14:55:24.000000 paynexus-0.2.4/PayNexus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-18 14:55:24.000000 paynexus-0.2.4/PayNexus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:55:24.000000 paynexus-0.2.4/PayNexus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-18 14:55:24.000000 paynexus-0.2.4/PayNexus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 14:55:24.000000 paynexus-0.2.4/PayNexus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13149 2024-05-18 08:10:43.000000 paynexus-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 14:55:24.429493 paynexus-0.2.4/paynexus/
+-rw-rw-rw-   0        0        0    14926 2024-05-17 23:25:22.000000 paynexus-0.2.4/paynexus/Colors.py
+-rw-rw-rw-   0        0        0       93 2024-05-18 14:55:04.000000 paynexus-0.2.4/paynexus/__init__.py
+-rw-rw-rw-   0        0        0    22191 2024-05-18 07:03:09.000000 paynexus-0.2.4/paynexus/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 14:55:24.431488 paynexus-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2123 2024-05-18 14:54:17.000000 paynexus-0.2.4/setup.py
```

### Comparing `paynexus-0.2.3/LICENSE` & `paynexus-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `paynexus-0.2.3/PKG-INFO` & `paynexus-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: PayNexus
-Version: 0.2.3
+Version: 0.2.4
 Summary: PayNexus: PythonからPayPayを操作できる非公式モジュールです。
 Home-page: https://github.com/harumaki4649/PayNexus
 Download-URL: https://github.com/harumaki4649/PayNexus
-Author: Haruki Kodama
-Author-email: tp-link-z490@outlook.jp
-Maintainer: Haruki Kodama
-Maintainer-email: tp-link-z490@outlook.jp
+Author: tp-link
+Author-email: support@disnana.com
+Maintainer: tp-link
+Maintainer-email: support@disnana.com
 License: BSD 3-Clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `paynexus-0.2.3/PayNexus.egg-info/PKG-INFO` & `paynexus-0.2.4/PayNexus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: PayNexus
-Version: 0.2.3
+Version: 0.2.4
 Summary: PayNexus: PythonからPayPayを操作できる非公式モジュールです。
 Home-page: https://github.com/harumaki4649/PayNexus
 Download-URL: https://github.com/harumaki4649/PayNexus
-Author: Haruki Kodama
-Author-email: tp-link-z490@outlook.jp
-Maintainer: Haruki Kodama
-Maintainer-email: tp-link-z490@outlook.jp
+Author: tp-link
+Author-email: support@disnana.com
+Maintainer: tp-link
+Maintainer-email: support@disnana.com
 License: BSD 3-Clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `paynexus-0.2.3/README.md` & `paynexus-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `paynexus-0.2.3/paynexus/Colors.py` & `paynexus-0.2.4/paynexus/Colors.py`

 * *Files identical despite different names*

### Comparing `paynexus-0.2.3/paynexus/main.py` & `paynexus-0.2.4/paynexus/main.py`

 * *Files identical despite different names*

### Comparing `paynexus-0.2.3/setup.py` & `paynexus-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # License: BSD 3 clause
 
 from setuptools import setup
 import PayNexus
 
 DESCRIPTION = "PayNexus: PythonからPayPayを操作できる非公式モジュールです。"
 NAME = 'PayNexus'
-AUTHOR = 'Haruki Kodama'
-AUTHOR_EMAIL = 'tp-link-z490@outlook.jp'
+AUTHOR = 'tp-link'
+AUTHOR_EMAIL = 'support@disnana.com'
 URL = 'https://github.com/harumaki4649/PayNexus'
 LICENSE = 'BSD 3-Clause'
 DOWNLOAD_URL = 'https://github.com/harumaki4649/PayNexus'
 VERSION = PayNexus.__version__
 PYTHON_REQUIRES = ">=3.9"
 # Readmeのファイルパス指定
 readme_path = r'C:\Users\msi-z\OneDrive\ドキュメント\GitHub\PayNexus\README.md'
```

