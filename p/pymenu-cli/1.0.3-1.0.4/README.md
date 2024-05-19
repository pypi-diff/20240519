# Comparing `tmp/pymenu_cli-1.0.3.tar.gz` & `tmp/pymenu_cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymenu_cli-1.0.3.tar", last modified: Fri May 17 19:25:59 2024, max compression
+gzip compressed data, was "pymenu_cli-1.0.4.tar", last modified: Sun May 19 18:07:16 2024, max compression
```

## Comparing `pymenu_cli-1.0.3.tar` & `pymenu_cli-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:25:59.132922 pymenu_cli-1.0.3/
--rw-r--r--   0 moraneus   (501) staff       (20)     2857 2024-05-17 19:25:59.132721 pymenu_cli-1.0.3/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)     2587 2024-05-17 18:53:28.000000 pymenu_cli-1.0.3/README.md
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:25:59.131586 pymenu_cli-1.0.3/pymenu_cli/
--rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.3/pymenu_cli/__init__.py
--rw-r--r--   0 moraneus   (501) staff       (20)     5117 2024-05-17 18:51:29.000000 pymenu_cli-1.0.3/pymenu_cli/menu.py
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:25:59.132547 pymenu_cli-1.0.3/pymenu_cli.egg-info/
--rw-r--r--   0 moraneus   (501) staff       (20)     2857 2024-05-17 19:25:59.000000 pymenu_cli-1.0.3/pymenu_cli.egg-info/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)      233 2024-05-17 19:25:59.000000 pymenu_cli-1.0.3/pymenu_cli.egg-info/SOURCES.txt
--rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-17 19:25:59.000000 pymenu_cli-1.0.3/pymenu_cli.egg-info/dependency_links.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       52 2024-05-17 19:25:59.000000 pymenu_cli-1.0.3/pymenu_cli.egg-info/entry_points.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-17 19:25:59.000000 pymenu_cli-1.0.3/pymenu_cli.egg-info/top_level.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-17 19:25:59.132958 pymenu_cli-1.0.3/setup.cfg
--rw-r--r--   0 moraneus   (501) staff       (20)      644 2024-05-17 19:25:57.000000 pymenu_cli-1.0.3/setup.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:07:16.011323 pymenu_cli-1.0.4/
+-rw-r--r--   0 moraneus   (501) staff       (20)     3023 2024-05-19 18:07:16.011036 pymenu_cli-1.0.4/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)     2753 2024-05-19 18:06:42.000000 pymenu_cli-1.0.4/README.md
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:07:16.008799 pymenu_cli-1.0.4/pymenu_cli/
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.4/pymenu_cli/__init__.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     5117 2024-05-17 18:51:29.000000 pymenu_cli-1.0.4/pymenu_cli/menu.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:07:16.010025 pymenu_cli-1.0.4/pymenu_cli.egg-info/
+-rw-r--r--   0 moraneus   (501) staff       (20)     3023 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)      233 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       52 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/entry_points.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/top_level.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-19 18:07:16.011372 pymenu_cli-1.0.4/setup.cfg
+-rw-r--r--   0 moraneus   (501) staff       (20)      644 2024-05-19 18:01:22.000000 pymenu_cli-1.0.4/setup.py
```

### Comparing `pymenu_cli-1.0.3/PKG-INFO` & `pymenu_cli-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pymenu-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for creating interactive CLI menus
 Home-page: https://github.com/moraneus/pymenu-cli
 Author: Moraneus
 Author-email: moraneus@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # pymenu-cli
 
-[![PyPI version](https://badge.fury.io/py/pymenu-cli.svg)](https://badge.fury.io/py/pymenu-cli)
+![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pymenu-cli)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 pymenu-cli is a Python library that simplifies the creation of interactive command-line interface (CLI) menus. It provides a convenient way to define hierarchical menu structures and associate actions with menu items.
 
 ## Features
 
 - Define menus and submenus using a simple JSON file format
@@ -94,12 +95,19 @@
     print("Executing action 2")
 
 def action_function_3():
     print("Executing action 3")
 ```
 
 ### Examples
-Check out the examples directory for sample menu configurations and action implementations.
-### Contributing
-Contributions are welcome! Please read the contribution guidelines for more information.
+Explore the examples directory for sample menu configurations and action implementations. 
+To run an example, follow these steps:
+
+1. Clone the project repository.
+2. Open your command line and navigate to the examples directory.
+3. Execute the example by running the following command:
+```python
+python3 menu_example.py
+```
+
 ### License
 This project is licensed under the MIT License.
```

### Comparing `pymenu_cli-1.0.3/README.md` & `pymenu_cli-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pymenu-cli
 
-[![PyPI version](https://badge.fury.io/py/pymenu-cli.svg)](https://badge.fury.io/py/pymenu-cli)
+![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pymenu-cli)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 pymenu-cli is a Python library that simplifies the creation of interactive command-line interface (CLI) menus. It provides a convenient way to define hierarchical menu structures and associate actions with menu items.
 
 ## Features
 
 - Define menus and submenus using a simple JSON file format
@@ -84,12 +85,19 @@
     print("Executing action 2")
 
 def action_function_3():
     print("Executing action 3")
 ```
 
 ### Examples
-Check out the examples directory for sample menu configurations and action implementations.
-### Contributing
-Contributions are welcome! Please read the contribution guidelines for more information.
+Explore the examples directory for sample menu configurations and action implementations. 
+To run an example, follow these steps:
+
+1. Clone the project repository.
+2. Open your command line and navigate to the examples directory.
+3. Execute the example by running the following command:
+```python
+python3 menu_example.py
+```
+
 ### License
 This project is licensed under the MIT License.
```

### Comparing `pymenu_cli-1.0.3/pymenu_cli/menu.py` & `pymenu_cli-1.0.4/pymenu_cli/menu.py`

 * *Files identical despite different names*

### Comparing `pymenu_cli-1.0.3/pymenu_cli.egg-info/PKG-INFO` & `pymenu_cli-1.0.4/pymenu_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pymenu-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for creating interactive CLI menus
 Home-page: https://github.com/moraneus/pymenu-cli
 Author: Moraneus
 Author-email: moraneus@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # pymenu-cli
 
-[![PyPI version](https://badge.fury.io/py/pymenu-cli.svg)](https://badge.fury.io/py/pymenu-cli)
+![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pymenu-cli)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 pymenu-cli is a Python library that simplifies the creation of interactive command-line interface (CLI) menus. It provides a convenient way to define hierarchical menu structures and associate actions with menu items.
 
 ## Features
 
 - Define menus and submenus using a simple JSON file format
@@ -94,12 +95,19 @@
     print("Executing action 2")
 
 def action_function_3():
     print("Executing action 3")
 ```
 
 ### Examples
-Check out the examples directory for sample menu configurations and action implementations.
-### Contributing
-Contributions are welcome! Please read the contribution guidelines for more information.
+Explore the examples directory for sample menu configurations and action implementations. 
+To run an example, follow these steps:
+
+1. Clone the project repository.
+2. Open your command line and navigate to the examples directory.
+3. Execute the example by running the following command:
+```python
+python3 menu_example.py
+```
+
 ### License
 This project is licensed under the MIT License.
```

### Comparing `pymenu_cli-1.0.3/setup.py` & `pymenu_cli-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pymenu-cli',
-    version='1.0.3',
+    version='1.0.4',
     description='A Python library for creating interactive CLI menus',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Moraneus',
     author_email='moraneus@gmail.com',
     url='https://github.com/moraneus/pymenu-cli',
     packages=find_packages(),
```

