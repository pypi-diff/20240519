# Comparing `tmp/mazegroup-0.1.4.0.1.tar.gz` & `tmp/mazegroup-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazegroup-0.1.4.0.1.tar", last modified: Fri Apr 19 14:27:11 2024, max compression
+gzip compressed data, was "mazegroup-0.1.4.1.tar", last modified: Sun May 19 09:42:54 2024, max compression
```

## Comparing `mazegroup-0.1.4.0.1.tar` & `mazegroup-0.1.4.1.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/calc/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/calc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/cd/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/cd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup/echo/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/echo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/help/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/ls/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/ls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/pyeval/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/pyeval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/pyexec/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/pyexec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/pypkg/
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/pypkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/quit/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/quit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/saves/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/saves/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/sc/
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/sc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/sc/out/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/sc/out/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/sc/temp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/sc/temp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/mazegroup/shell/
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/mazegroup/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:27:11.961577 mazegroup-0.1.4.0.1/mazegroup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 14:27:11.000000 mazegroup-0.1.4.0.1/mazegroup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:27:11.965577 mazegroup-0.1.4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-19 14:27:07.000000 mazegroup-0.1.4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.880039 mazegroup-0.1.4.1/mazegroup/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/calc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/cd/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/cd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/echo/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/echo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/ls/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/pyeval/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/pyeval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/pyexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/pyexec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/pypkg/
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/pypkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/quit/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/quit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/rud/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/rud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27363 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/rud/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/saves/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/saves/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/sc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/sc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/sc/out/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/sc/out/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/sc/temp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/sc/temp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/mazegroup/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/mazegroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-19 09:42:54.000000 mazegroup-0.1.4.1/mazegroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-19 09:42:54.000000 mazegroup-0.1.4.1/mazegroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:42:54.000000 mazegroup-0.1.4.1/mazegroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-19 09:42:54.000000 mazegroup-0.1.4.1/mazegroup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 09:42:54.000000 mazegroup-0.1.4.1/mazegroup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 09:42:54.000000 mazegroup-0.1.4.1/mazegroup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 09:42:54.884039 mazegroup-0.1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-19 09:42:48.000000 mazegroup-0.1.4.1/setup.py
```

### Comparing `mazegroup-0.1.4.0.1/PKG-INFO` & `mazegroup-0.1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.4.0.1
+Version: 0.1.4.1
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -51,15 +51,15 @@
 For use a command in your source code (you must do the last step) :
 ```py
 import mazegroup.commands as commands
 import mazegroup.utils as utils  # For error checking
 
 returned = commands.executeCommand("echo", ["Hello,", "world!"])  # Echo "Hello, world!" by example
 
-# If there is a error, shows it (optional) :
+# If there is an error, shows it (optional) :
 if type(returned) != utils.NoError:
 	print("Error :", returned.message)
 ```
 
 ### Arguments
 
 You can evaluate Python expression in using `py:` in the argument (only the actual argument will be evaluate), by example the argument `"py:5 + 5"` will returns 10, we use `"` because we also use spaces on the expression.
@@ -100,8 +100,10 @@
 	- The default output is in the MazeGroup.py Python package directory, on the part of this command, either `mazegroup/sc/out`.
 - `shell <...>`
 	- The MazeGroup.py shell. There are modes available, use their start char for enter on it :
 		- The system shell mode : `§ <...>`
 		- The calc mode : `% <...>`, equivalant of the command `calc` but this mode lock the MazeGroup.py shell for expressions.
 	- Once you enter in a mode, the rest of commands of after will be locked on this mode, for return to the MazeGroup.py shell, you must enter a empty command.
 	- In command arguments (only on the MazeGroup.py shell), the `\s` will provoks a space.
+- `rud <sourcecode> <options>`
+	- RUD interpreter, a minimal stack-based programming language. No documentation available.
```

### Comparing `mazegroup-0.1.4.0.1/README.md` & `mazegroup-0.1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 For use a command in your source code (you must do the last step) :
 ```py
 import mazegroup.commands as commands
 import mazegroup.utils as utils  # For error checking
 
 returned = commands.executeCommand("echo", ["Hello,", "world!"])  # Echo "Hello, world!" by example
 
-# If there is a error, shows it (optional) :
+# If there is an error, shows it (optional) :
 if type(returned) != utils.NoError:
 	print("Error :", returned.message)
 ```
 
 ### Arguments
 
 You can evaluate Python expression in using `py:` in the argument (only the actual argument will be evaluate), by example the argument `"py:5 + 5"` will returns 10, we use `"` because we also use spaces on the expression.
@@ -85,8 +85,10 @@
 	- Usage : `mazegroup sc <compress/decompress> <path> <!* output path> <!* password> <!* increments> <!* tar>`
 	- The default output is in the MazeGroup.py Python package directory, on the part of this command, either `mazegroup/sc/out`.
 - `shell <...>`
 	- The MazeGroup.py shell. There are modes available, use their start char for enter on it :
 		- The system shell mode : `§ <...>`
 		- The calc mode : `% <...>`, equivalant of the command `calc` but this mode lock the MazeGroup.py shell for expressions.
 	- Once you enter in a mode, the rest of commands of after will be locked on this mode, for return to the MazeGroup.py shell, you must enter a empty command.
-	- In command arguments (only on the MazeGroup.py shell), the `\s` will provoks a space.
+	- In command arguments (only on the MazeGroup.py shell), the `\s` will provoks a space.
+- `rud <sourcecode> <options>`
+	- RUD interpreter, a minimal stack-based programming language. No documentation available.
```

### Comparing `mazegroup-0.1.4.0.1/mazegroup/calc/__init__.py` & `mazegroup-0.1.4.1/mazegroup/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/commands.py` & `mazegroup-0.1.4.1/mazegroup/commands.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/help/__init__.py` & `mazegroup-0.1.4.1/mazegroup/help/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/imports.py` & `mazegroup-0.1.4.1/mazegroup/imports.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/ls/__init__.py` & `mazegroup-0.1.4.1/mazegroup/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/pyeval/__init__.py` & `mazegroup-0.1.4.1/mazegroup/pyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/pyexec/__init__.py` & `mazegroup-0.1.4.1/mazegroup/pyexec/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/pypkg/__init__.py` & `mazegroup-0.1.4.1/mazegroup/pypkg/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/sc/__init__.py` & `mazegroup-0.1.4.1/mazegroup/sc/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/shell/__init__.py` & `mazegroup-0.1.4.1/mazegroup/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup/utils.py` & `mazegroup-0.1.4.1/mazegroup/utils.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.4.0.1/mazegroup.egg-info/PKG-INFO` & `mazegroup-0.1.4.1/mazegroup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.4.0.1
+Version: 0.1.4.1
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -51,15 +51,15 @@
 For use a command in your source code (you must do the last step) :
 ```py
 import mazegroup.commands as commands
 import mazegroup.utils as utils  # For error checking
 
 returned = commands.executeCommand("echo", ["Hello,", "world!"])  # Echo "Hello, world!" by example
 
-# If there is a error, shows it (optional) :
+# If there is an error, shows it (optional) :
 if type(returned) != utils.NoError:
 	print("Error :", returned.message)
 ```
 
 ### Arguments
 
 You can evaluate Python expression in using `py:` in the argument (only the actual argument will be evaluate), by example the argument `"py:5 + 5"` will returns 10, we use `"` because we also use spaces on the expression.
@@ -100,8 +100,10 @@
 	- The default output is in the MazeGroup.py Python package directory, on the part of this command, either `mazegroup/sc/out`.
 - `shell <...>`
 	- The MazeGroup.py shell. There are modes available, use their start char for enter on it :
 		- The system shell mode : `§ <...>`
 		- The calc mode : `% <...>`, equivalant of the command `calc` but this mode lock the MazeGroup.py shell for expressions.
 	- Once you enter in a mode, the rest of commands of after will be locked on this mode, for return to the MazeGroup.py shell, you must enter a empty command.
 	- In command arguments (only on the MazeGroup.py shell), the `\s` will provoks a space.
+- `rud <sourcecode> <options>`
+	- RUD interpreter, a minimal stack-based programming language. No documentation available.
```

### Comparing `mazegroup-0.1.4.0.1/mazegroup.egg-info/SOURCES.txt` & `mazegroup-0.1.4.1/mazegroup.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,12 +16,14 @@
 mazegroup/echo/__init__.py
 mazegroup/help/__init__.py
 mazegroup/ls/__init__.py
 mazegroup/pyeval/__init__.py
 mazegroup/pyexec/__init__.py
 mazegroup/pypkg/__init__.py
 mazegroup/quit/__init__.py
+mazegroup/rud/__init__.py
+mazegroup/rud/interpreter.py
 mazegroup/saves/__init__.py
 mazegroup/sc/__init__.py
 mazegroup/sc/out/__init__.py
 mazegroup/sc/temp/__init__.py
 mazegroup/shell/__init__.py
```

### Comparing `mazegroup-0.1.4.0.1/setup.py` & `mazegroup-0.1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mazegroup",
-    version="0.1.4.0.1",
+    version="0.1.4.1",
     description="MazeGroup.py is an general prupose library for Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Genius_um",
     python_requires=">=3.9",
     url="https://github.com/Geniusum/mazegroup.py",
     packages=find_packages(),#["mazegroup", "mazegroup/cli", "mazegroup/echo", "mazegroup/saves"], # find_packages(),
```

