# Comparing `tmp/beancount_multitool-0.1.0.tar.gz` & `tmp/beancount_multitool-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_multitool-0.1.0.tar", max compression
+gzip compressed data, was "beancount_multitool-0.2.0.tar", max compression
```

## Comparing `beancount_multitool-0.1.0.tar` & `beancount_multitool-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.1.0/LICENSE
--rw-r--r--   0        0        0     2377 2024-05-19 13:43:09.435510 beancount_multitool-0.1.0/README.md
--rw-r--r--   0        0        0     1183 2024-05-19 14:02:10.674561 beancount_multitool-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      152 2024-05-18 06:24:03.000000 beancount_multitool-0.1.0/src/beancount_multitool/Institution.py
--rw-r--r--   0        0        0     4777 2024-05-18 12:42:08.000000 beancount_multitool-0.1.0/src/beancount_multitool/JABank.py
--rw-r--r--   0        0        0     4022 2024-05-18 06:34:16.000000 beancount_multitool-0.1.0/src/beancount_multitool/RakutenBank.py
--rw-r--r--   0        0        0     3853 2024-05-18 08:40:03.000000 beancount_multitool-0.1.0/src/beancount_multitool/RakutenCard.py
--rw-r--r--   0        0        0     4683 2024-05-18 08:33:38.000000 beancount_multitool-0.1.0/src/beancount_multitool/ShinseiBank.py
--rw-r--r--   0        0        0      454 2024-05-19 11:28:08.465883 beancount_multitool-0.1.0/src/beancount_multitool/__init__.py
--rw-r--r--   0        0        0       89 2024-05-18 12:52:29.000000 beancount_multitool-0.1.0/src/beancount_multitool/__main__.py
--rw-r--r--   0        0        0       22 2024-05-19 11:26:32.765522 beancount_multitool-0.1.0/src/beancount_multitool/__version__.py
--rw-r--r--   0        0        0     1219 2024-05-17 14:23:38.000000 beancount_multitool-0.1.0/src/beancount_multitool/as_transaction.py
--rw-r--r--   0        0        0     1563 2024-05-19 12:37:59.542282 beancount_multitool-0.1.0/src/beancount_multitool/cli.py
--rw-r--r--   0        0        0      588 2024-05-18 08:03:00.000000 beancount_multitool-0.1.0/src/beancount_multitool/read_config.py
--rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 beancount_multitool-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2498 2024-05-19 14:48:29.553748 beancount_multitool-0.2.0/README.md
+-rw-r--r--   0        0        0     1183 2024-05-19 14:44:09.227258 beancount_multitool-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-05-18 06:24:03.000000 beancount_multitool-0.2.0/src/beancount_multitool/Institution.py
+-rw-r--r--   0        0        0     4777 2024-05-18 12:42:08.000000 beancount_multitool-0.2.0/src/beancount_multitool/JABank.py
+-rw-r--r--   0        0        0     4022 2024-05-18 06:34:16.000000 beancount_multitool-0.2.0/src/beancount_multitool/RakutenBank.py
+-rw-r--r--   0        0        0     3853 2024-05-18 08:40:03.000000 beancount_multitool-0.2.0/src/beancount_multitool/RakutenCard.py
+-rw-r--r--   0        0        0     4683 2024-05-18 08:33:38.000000 beancount_multitool-0.2.0/src/beancount_multitool/ShinseiBank.py
+-rw-r--r--   0        0        0      454 2024-05-19 14:27:19.202196 beancount_multitool-0.2.0/src/beancount_multitool/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-18 12:52:29.000000 beancount_multitool-0.2.0/src/beancount_multitool/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-19 14:44:02.886647 beancount_multitool-0.2.0/src/beancount_multitool/__version__.py
+-rw-r--r--   0        0        0     1219 2024-05-17 14:23:38.000000 beancount_multitool-0.2.0/src/beancount_multitool/as_transaction.py
+-rw-r--r--   0        0        0     1576 2024-05-19 14:38:01.059850 beancount_multitool-0.2.0/src/beancount_multitool/cli.py
+-rw-r--r--   0        0        0      588 2024-05-18 08:03:00.000000 beancount_multitool-0.2.0/src/beancount_multitool/read_config.py
+-rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 beancount_multitool-0.2.0/PKG-INFO
```

### Comparing `beancount_multitool-0.1.0/LICENSE` & `beancount_multitool-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.1.0/README.md` & `beancount_multitool-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Beancount Multitool
 
 ![Tests badge](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml/badge.svg)
-![python version required](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Frlan%2Fbeancount-multitool%2Fmain%2Fpyproject.toml)
+![pypi version](https://img.shields.io/pypi/v/beancount-multitool
+)
+![python version required](https://img.shields.io/pypi/pyversions/beancount-multitool
+)
 ![static coverage badge](https://img.shields.io/badge/Coverage-97%25-blue)
 
 Beancount Multitool is a command-line-interface (CLI) tool that converts financial data from financial institutions to Beancount files.
 
 The following institutions are supported:
 
 * Japan
@@ -21,32 +24,45 @@
   * Debit: `Expenses:JP:Unknown:NameOfInstitution`
   * Credit: `Income:JP:Unknown:NameOfInstitution`
 
 What these scripts __can not__ (yet) do:
 
 * Label transactions with different sub-accounts, e.g., `Expenses:JP:Food:Grocery` or `Expenses:JP:Food:Restaurant`.
 
+Installation:
+
+```sh
+pip install beancount-multitool
+```
+
 Usage:
 
+```sh
+bean-mt --help
+```
+
 ```txt
-$ bean-mt --help
 Usage: bean-mt [OPTIONS] NAME CONFIG DATA
 
   Read financial data and output a Beancount file.
 
-  NAME is the name of the financial institution, e.g. RakutenBank.
+  NAME is the name of the financial institution. See Note below for a list of
+  supported names.
 
   CONFIG is a .toml file with run-time configurations, e.g. config.toml.
 
   DATA is the raw financial data downloaded from NAME, e.g. input.csv.
 
 Options:
   --output PATH  Resulting Beancount file
   --version      Show the version and exit.
   --help         Show this message and exit.
+
+  Note: supported names of financial institutions: ['ja_bank', 'rakuten_bank',
+  'rakuten_card', 'shinsei_bank']
 ```
 
 Example:
 
 ```sh
 bean-mt rakuten_bank config.toml 2024-01.csv --output 2024-01.bean
 ```
@@ -58,20 +74,14 @@
 3. Include the `output.bean` file in my ledger.
 4. Manually edit that Beancount file to my needs.
 
 config.toml:
 
 There is a default config.toml per financial institutions. Examples are in the test [data folder](./tests/data/).
 
-## Installation
-
-```sh
-pip install beancount-multitool
-```
-
 ## Requirements
 
 * Python 3.9 or higher.
 
 ## More
 
 * [Todo](./todo.md)
```

### Comparing `beancount_multitool-0.1.0/pyproject.toml` & `beancount_multitool-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-multitool"
-version = "0.1.0"
+version = "0.2.0"
 description = "A CLI tool that converts financial data to Beancount files"
 authors = ["Rick Lan <rlan@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rlan/beancount-multitool"
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `beancount_multitool-0.1.0/src/beancount_multitool/JABank.py` & `beancount_multitool-0.2.0/src/beancount_multitool/JABank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.1.0/src/beancount_multitool/RakutenBank.py` & `beancount_multitool-0.2.0/src/beancount_multitool/RakutenBank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.1.0/src/beancount_multitool/RakutenCard.py` & `beancount_multitool-0.2.0/src/beancount_multitool/RakutenCard.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.1.0/src/beancount_multitool/ShinseiBank.py` & `beancount_multitool-0.2.0/src/beancount_multitool/ShinseiBank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.1.0/src/beancount_multitool/as_transaction.py` & `beancount_multitool-0.2.0/src/beancount_multitool/as_transaction.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.1.0/src/beancount_multitool/cli.py` & `beancount_multitool-0.2.0/src/beancount_multitool/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,33 +13,29 @@
     """Check given name is one of supported financial institutions.
     """
     if value in __INSTITUTIONS__:
         return value
     else:
         raise click.BadParameter(f"Name must be one of: {__INSTITUTIONS__}")
 
-@click.command()
+@click.command(epilog=f"Note: supported names of financial institutions: {__INSTITUTIONS__}")
 @click.argument('name', type=str, callback=validate_name)
 @click.argument('config', type=click.Path(exists=True))
 @click.argument('data', type=click.Path(exists=True))
 @click.option('--output', default="output.bean", type=click.Path(), help="Resulting Beancount file")
 @click.version_option()
 def main(name: str, config, data, output):
     """Read financial data and output a Beancount file.
 
-    NAME is the name of the financial institution, e.g. RakutenBank.
+    NAME is the name of the financial institution. See Note below for a list of supported names.
 
     CONFIG is a .toml file with run-time configurations, e.g. config.toml.
 
     DATA is the raw financial data downloaded from NAME, e.g. input.csv.
     """
-    #click.echo(name)
-    #click.echo(data)
-    #click.echo(config)
-    #click.echo(output)
     if name == JABank.NAME:
         tool = JABank(config)
     elif name == RakutenBank.NAME:
         tool = RakutenBank(config)
     elif name == RakutenCard.NAME:
         tool = RakutenCard(config)
     elif name == ShinseiBank.NAME:
```

### Comparing `beancount_multitool-0.1.0/src/beancount_multitool/read_config.py` & `beancount_multitool-0.2.0/src/beancount_multitool/read_config.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.1.0/PKG-INFO` & `beancount_multitool-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-multitool
-Version: 0.1.0
+Version: 0.2.0
 Summary: A CLI tool that converts financial data to Beancount files
 Home-page: https://github.com/rlan/beancount-multitool
 License: MIT
 Author: Rick Lan
 Author-email: rlan@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -28,15 +28,18 @@
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/rlan/beancount-multitool
 Description-Content-Type: text/markdown
 
 # Beancount Multitool
 
 ![Tests badge](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml/badge.svg)
-![python version required](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Frlan%2Fbeancount-multitool%2Fmain%2Fpyproject.toml)
+![pypi version](https://img.shields.io/pypi/v/beancount-multitool
+)
+![python version required](https://img.shields.io/pypi/pyversions/beancount-multitool
+)
 ![static coverage badge](https://img.shields.io/badge/Coverage-97%25-blue)
 
 Beancount Multitool is a command-line-interface (CLI) tool that converts financial data from financial institutions to Beancount files.
 
 The following institutions are supported:
 
 * Japan
@@ -52,32 +55,45 @@
   * Debit: `Expenses:JP:Unknown:NameOfInstitution`
   * Credit: `Income:JP:Unknown:NameOfInstitution`
 
 What these scripts __can not__ (yet) do:
 
 * Label transactions with different sub-accounts, e.g., `Expenses:JP:Food:Grocery` or `Expenses:JP:Food:Restaurant`.
 
+Installation:
+
+```sh
+pip install beancount-multitool
+```
+
 Usage:
 
+```sh
+bean-mt --help
+```
+
 ```txt
-$ bean-mt --help
 Usage: bean-mt [OPTIONS] NAME CONFIG DATA
 
   Read financial data and output a Beancount file.
 
-  NAME is the name of the financial institution, e.g. RakutenBank.
+  NAME is the name of the financial institution. See Note below for a list of
+  supported names.
 
   CONFIG is a .toml file with run-time configurations, e.g. config.toml.
 
   DATA is the raw financial data downloaded from NAME, e.g. input.csv.
 
 Options:
   --output PATH  Resulting Beancount file
   --version      Show the version and exit.
   --help         Show this message and exit.
+
+  Note: supported names of financial institutions: ['ja_bank', 'rakuten_bank',
+  'rakuten_card', 'shinsei_bank']
 ```
 
 Example:
 
 ```sh
 bean-mt rakuten_bank config.toml 2024-01.csv --output 2024-01.bean
 ```
@@ -89,20 +105,14 @@
 3. Include the `output.bean` file in my ledger.
 4. Manually edit that Beancount file to my needs.
 
 config.toml:
 
 There is a default config.toml per financial institutions. Examples are in the test [data folder](./tests/data/).
 
-## Installation
-
-```sh
-pip install beancount-multitool
-```
-
 ## Requirements
 
 * Python 3.9 or higher.
 
 ## More
 
 * [Todo](./todo.md)
```

