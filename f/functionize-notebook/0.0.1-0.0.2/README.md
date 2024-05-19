# Comparing `tmp/functionize-notebook-0.0.1.tar.gz` & `tmp/functionize-notebook-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functionize-notebook-0.0.1.tar", last modified: Fri May 17 07:55:17 2024, max compression
+gzip compressed data, was "functionize-notebook-0.0.2.tar", last modified: Sun May 19 13:07:22 2024, max compression
```

## Comparing `functionize-notebook-0.0.1.tar` & `functionize-notebook-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-17 07:55:17.557743 functionize-notebook-0.0.1/
--rw-rw-r--   0 tu        (1001) tu        (1001)       29 2024-05-17 06:36:21.000000 functionize-notebook-0.0.1/AUTHORS.md
--rw-rw-r--   0 tu        (1001) tu        (1001)       50 2024-05-17 06:36:58.000000 functionize-notebook-0.0.1/CHANGES.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)     1053 2024-05-17 02:14:10.000000 functionize-notebook-0.0.1/LICENSE.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)       27 2024-05-17 07:16:02.000000 functionize-notebook-0.0.1/MANIFEST.in
--rw-rw-r--   0 tu        (1001) tu        (1001)     2204 2024-05-17 07:55:17.557743 functionize-notebook-0.0.1/PKG-INFO
--rw-rw-r--   0 tu        (1001) tu        (1001)     1746 2024-05-17 07:43:18.000000 functionize-notebook-0.0.1/README.md
--rw-rw-r--   0 tu        (1001) tu        (1001)     1836 2024-05-17 07:53:31.000000 functionize-notebook-0.0.1/README.rst
-drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-17 07:55:17.557743 functionize-notebook-0.0.1/functionize_notebook.egg-info/
--rw-rw-r--   0 tu        (1001) tu        (1001)     2204 2024-05-17 07:55:17.000000 functionize-notebook-0.0.1/functionize_notebook.egg-info/PKG-INFO
--rw-rw-r--   0 tu        (1001) tu        (1001)      324 2024-05-17 07:55:17.000000 functionize-notebook-0.0.1/functionize_notebook.egg-info/SOURCES.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)        1 2024-05-17 07:55:17.000000 functionize-notebook-0.0.1/functionize_notebook.egg-info/dependency_links.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)       19 2024-05-17 07:55:17.000000 functionize-notebook-0.0.1/functionize_notebook.egg-info/requires.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)       17 2024-05-17 07:55:17.000000 functionize-notebook-0.0.1/functionize_notebook.egg-info/top_level.txt
-drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-17 07:55:17.557743 functionize-notebook-0.0.1/notebook_wrapper/
--rw-rw-r--   0 tu        (1001) tu        (1001)     4416 2024-05-17 07:10:12.000000 functionize-notebook-0.0.1/notebook_wrapper/__init__.py
--rw-rw-r--   0 tu        (1001) tu        (1001)       38 2024-05-17 07:55:17.557743 functionize-notebook-0.0.1/setup.cfg
--rw-rw-r--   0 tu        (1001) tu        (1001)      602 2024-05-17 07:52:54.000000 functionize-notebook-0.0.1/setup.py
+drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/
+-rw-rw-r--   0 tu        (1001) tu        (1001)       29 2024-05-17 06:36:21.000000 functionize-notebook-0.0.2/AUTHORS.md
+-rw-rw-r--   0 tu        (1001) tu        (1001)       92 2024-05-19 13:06:57.000000 functionize-notebook-0.0.2/CHANGES.txt
+-rw-rw-r--   0 tu        (1001) tu        (1001)     1053 2024-05-17 02:14:10.000000 functionize-notebook-0.0.2/LICENSE.txt
+-rw-rw-r--   0 tu        (1001) tu        (1001)       27 2024-05-17 07:16:02.000000 functionize-notebook-0.0.2/MANIFEST.in
+-rw-rw-r--   0 tu        (1001) tu        (1001)     2204 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/PKG-INFO
+-rw-rw-r--   0 tu        (1001) tu        (1001)     1746 2024-05-17 07:43:18.000000 functionize-notebook-0.0.2/README.md
+-rw-rw-r--   0 tu        (1001) tu        (1001)     1836 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/README.rst
+drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/functionize_notebook.egg-info/
+-rw-rw-r--   0 tu        (1001) tu        (1001)     2204 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/PKG-INFO
+-rw-rw-r--   0 tu        (1001) tu        (1001)      324 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/SOURCES.txt
+-rw-rw-r--   0 tu        (1001) tu        (1001)        1 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/dependency_links.txt
+-rw-rw-r--   0 tu        (1001) tu        (1001)       19 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/requires.txt
+-rw-rw-r--   0 tu        (1001) tu        (1001)       17 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/top_level.txt
+drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/notebook_wrapper/
+-rw-rw-r--   0 tu        (1001) tu        (1001)     4274 2024-05-19 13:05:06.000000 functionize-notebook-0.0.2/notebook_wrapper/__init__.py
+-rw-rw-r--   0 tu        (1001) tu        (1001)       38 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/setup.cfg
+-rw-rw-r--   0 tu        (1001) tu        (1001)      602 2024-05-19 13:07:17.000000 functionize-notebook-0.0.2/setup.py
```

### Comparing `functionize-notebook-0.0.1/LICENSE.txt` & `functionize-notebook-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `functionize-notebook-0.0.1/PKG-INFO` & `functionize-notebook-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.1
+Version: 0.0.2
 Summary: run notebook like a function
 Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `functionize-notebook-0.0.1/README.md` & `functionize-notebook-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `functionize-notebook-0.0.1/README.rst` & `functionize-notebook-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `functionize-notebook-0.0.1/functionize_notebook.egg-info/PKG-INFO` & `functionize-notebook-0.0.2/functionize_notebook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.1
+Version: 0.0.2
 Summary: run notebook like a function
 Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `functionize-notebook-0.0.1/notebook_wrapper/__init__.py` & `functionize-notebook-0.0.2/notebook_wrapper/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         pass
 
     def __call__(self, *args, **kwargs):
         return self.run(args, kwargs)
 
     def run(self, *args, **kwargs) -> Any | List[Any]:
         # map input
-        variableMapping = dict(zip(self.inputVariable, args))
+        variableMapping = dict(zip(self.inputVariable, list(args)))
         variableMapping.update(**kwargs)
 
         nb = nbformat.read(self.notebook, as_version=nbformat.NO_CONVERT)
 
         if len(variableMapping) > 0:
             # add saving path for input
             inputPath = Path(
@@ -50,15 +50,15 @@
                 self.notebook.stem,
                 "input",
                 datetime.now().__str__() + ".pkl",
             )
             inputPath.parent.mkdir(parents=True, exist_ok=True)
 
             # add input values
-            pickle.dump(variableMapping, inputPath.open("wb+"))
+            inputPath.write_bytes(pickle.dumps(variableMapping))
             # wait for nb input file
             for _ in range(50):
                 if inputPath.exists():
                     break
                 else:
                     sleep(0.2)
             else:
@@ -74,19 +74,17 @@
 
             # add input cell to nb
             newCell = nbbase.new_code_cell(
                 source="""
                 from pathlib import Path
                 import pickle
                 
-                with Path("%s").open("rb") as inputFile:
-                    inputVariables = pickle.load(inputFile)
-                    for key, value in inputVariables.items():
-                        globals()[key] = value
-                        pass
+                inputVariables = pickle.loads(Path("%s").read_bytes())
+                for key, value in inputVariables.items():
+                    globals()[key] = value
                     pass
             """
                 % inputPath
             )
 
             nb.cells.insert(inputIndex + 1, newCell)
 
@@ -109,17 +107,15 @@
 
             newCell = nbbase.new_code_cell(
                 source="""
                 from pathlib import Path
                 import pickle
                 
                 outputVariable = %s
-                with Path("%s").open("wb+") as inputPath:
-                    pickle.dump(outputVariable, inputPath)
-                pass
+                Path("%s").write_bytes(pickle.dumps(outputVariable))
             """
                 % (requestVars, outputPath)
             )
 
             nb.cells.append(newCell)
             pass
 
@@ -132,12 +128,12 @@
                 if outputPath.exists():
                     break
                 else:
                     sleep(0.2)
             else:
                 raise IOError(outputPath.__str__() + " took too much time to write.")
 
-            res = pickle.load(outputPath.open("rb"))
+            res = pickle.loads(outputPath.read_bytes())
 
             return res
         else:
             return None
```

### Comparing `functionize-notebook-0.0.1/setup.py` & `functionize-notebook-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name="functionize-notebook",
-    version="0.0.1",
+    version="0.0.2",
     author="Bui Hoang Tu",
     author_email="bhtu.work@gmail.com",
     url="https://github.com/BuiHoangTu/functionize-notebook/tree/release",
     license="MIT",
     packages=find_packages(),
     package_dir={"notebook_wrapper": "notebook_wrapper"},
     description="run notebook like a function",
```

