# Comparing `tmp/seleniumuser-1.1.2.tar.gz` & `tmp/seleniumuser-1.1.3.tar.gz`

## Comparing `seleniumuser-1.1.2.tar` & `seleniumuser-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,8 @@
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/CHANGELOG.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/docs/index.html
--rw-r--r--   0        0        0    55839 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/docs/search.js
--rw-r--r--   0        0        0    34088 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/docs/seleniumuser.html
--rw-r--r--   0        0        0   543628 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/docs/seleniumuser/seleniumuser.html
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/src/seleniumuser/__init__.py
--rw-r--r--   0        0        0    27160 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/src/seleniumuser/seleniumuser.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/README.md
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 seleniumuser-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 seleniumuser-1.1.3/src/seleniumuser/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seleniumuser-1.1.3/src/seleniumuser/py.typed
+-rw-r--r--   0        0        0    27160 2020-02-02 00:00:00.000000 seleniumuser-1.1.3/src/seleniumuser/seleniumuser.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 seleniumuser-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 seleniumuser-1.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 seleniumuser-1.1.3/README.md
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 seleniumuser-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 seleniumuser-1.1.3/PKG-INFO
```

### Comparing `seleniumuser-1.1.2/src/seleniumuser/seleniumuser.py` & `seleniumuser-1.1.3/src/seleniumuser/seleniumuser.py`

 * *Files identical despite different names*

### Comparing `seleniumuser-1.1.2/LICENSE.txt` & `seleniumuser-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seleniumuser-1.1.2/README.md` & `seleniumuser-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `seleniumuser-1.1.2/pyproject.toml` & `seleniumuser-1.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,32 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
 [project]
 name = "seleniumuser"
-authors = [{name="Matt Manes"}]
 description = "Selenium wrapper to streamline usage."
-version = "1.1.2"
-requires-python = ">=3.10"
-dependencies = ["bs4", "selenium", "noiftimer", "voxscribe", "whosyouragent", "pytest"]
-keywords = [
-    "selenium",
-    "automation",
-    "webscraping"
-]
+version = "1.1.3"
+dependencies = ["bs4", "selenium==4.5.0", "noiftimer", "voxscribe", "whosyouragent", "beautifulsoup4"]
 readme = "README.md"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
+keywords = ["selenium", "automation", "webscraping"]
+classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
+requires-python = ">=3.10"
+
+[[project.authors]]
+name = "Matt Manes"
+email = ""
 
 [project.urls]
-"Homepage" = "https://github.com/matt-manes/seleniumuser"
-"Documentation" = "https://github.com/matt-manes/seleniumuser/tree/main/docs"
+Homepage = "https://github.com/matt-manes/seleniumuser"
+Documentation = "https://github.com/matt-manes/seleniumuser/tree/main/docs"
 "Source code" = "https://github.com/matt-manes/seleniumuser/tree/main/src/seleniumuser"
 
+[project.scripts]
+
+[tool]
 [tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
+addopts = ["--import-mode=importlib"]
 pythonpath = "src"
 
 [tool.hatch.build.targets.sdist]
-exclude = [
-    ".coverage",
-    ".pytest_cache",
-    ".vscode",
-    "tests"
-]
+exclude = [".coverage", ".pytest_cache", ".vscode", "tests", "htmlcov", "docs", "*log*", "*.md"]
+
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

### Comparing `seleniumuser-1.1.2/PKG-INFO` & `seleniumuser-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: seleniumuser
-Version: 1.1.2
+Version: 1.1.3
 Summary: Selenium wrapper to streamline usage.
 Project-URL: Homepage, https://github.com/matt-manes/seleniumuser
 Project-URL: Documentation, https://github.com/matt-manes/seleniumuser/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/seleniumuser/tree/main/src/seleniumuser
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: automation,selenium,webscraping
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: beautifulsoup4
 Requires-Dist: bs4
 Requires-Dist: noiftimer
-Requires-Dist: pytest
-Requires-Dist: selenium
+Requires-Dist: selenium==4.5.0
 Requires-Dist: voxscribe
 Requires-Dist: whosyouragent
 Description-Content-Type: text/markdown
 
 # Seleniumuser
 A module that sits ontop of Selenium to streamline scraping and automation workflows.<br>
 Install with:
```

