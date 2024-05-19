# Comparing `tmp/wizlib-3.0.0.tar.gz` & `tmp/wizlib-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-3.0.0.tar", max compression
+gzip compressed data, was "wizlib-3.0.1.tar", max compression
```

## Comparing `wizlib-3.0.0.tar` & `wizlib-3.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1094 2024-05-13 05:49:36.321921 wizlib-3.0.0/README.md
--rw-r--r--   0        0        0      698 2024-05-13 05:49:48.180954 wizlib-3.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 05:49:36.413921 wizlib-3.0.0/wizlib/__init__.py
--rw-r--r--   0        0        0     3263 2024-05-13 05:49:36.360921 wizlib-3.0.0/wizlib/app.py
--rw-r--r--   0        0        0     4506 2024-05-13 05:49:36.360921 wizlib-3.0.0/wizlib/class_family.py
--rw-r--r--   0        0        0     1686 2024-05-13 05:49:36.360921 wizlib-3.0.0/wizlib/command.py
--rw-r--r--   0        0        0     2588 2024-05-13 05:49:36.360921 wizlib-3.0.0/wizlib/config_handler.py
--rw-r--r--   0        0        0       46 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/error.py
--rw-r--r--   0        0        0      446 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/handler.py
--rw-r--r--   0        0        0     1505 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/parser.py
--rw-r--r--   0        0        0     1754 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/rlinput.py
--rw-r--r--   0        0        0      663 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/stream_handler.py
--rw-r--r--   0        0        0      272 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/super_wrapper.py
--rw-r--r--   0        0        0     4249 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui/__init__.py
--rw-r--r--   0        0        0      943 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui/shell/__init__.py
--rw-r--r--   0        0        0     7419 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui/shell/line_editor.py
--rw-r--r--   0        0        0     2030 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui/shell_ui.py
--rw-r--r--   0        0        0      634 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/ui_handler.py
--rw-r--r--   0        0        0      156 2024-05-13 05:49:36.361921 wizlib-3.0.0/wizlib/util.py
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 wizlib-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-19 00:07:31.324488 wizlib-3.0.1/README.md
+-rw-r--r--   0        0        0      698 2024-05-19 00:07:42.820476 wizlib-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 00:07:31.411488 wizlib-3.0.1/wizlib/__init__.py
+-rw-r--r--   0        0        0     3263 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/app.py
+-rw-r--r--   0        0        0     4506 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/class_family.py
+-rw-r--r--   0        0        0     1747 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/command.py
+-rw-r--r--   0        0        0     2588 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/config_handler.py
+-rw-r--r--   0        0        0       46 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/error.py
+-rw-r--r--   0        0        0      446 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/handler.py
+-rw-r--r--   0        0        0     1505 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/parser.py
+-rw-r--r--   0        0        0     1754 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/rlinput.py
+-rw-r--r--   0        0        0      663 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/stream_handler.py
+-rw-r--r--   0        0        0      272 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/super_wrapper.py
+-rw-r--r--   0        0        0     4241 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/ui/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/ui/shell/__init__.py
+-rw-r--r--   0        0        0     7419 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/ui/shell/line_editor.py
+-rw-r--r--   0        0        0     2064 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/ui/shell_ui.py
+-rw-r--r--   0        0        0      634 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/ui_handler.py
+-rw-r--r--   0        0        0      156 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/util.py
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 wizlib-3.0.1/PKG-INFO
```

### Comparing `wizlib-3.0.0/README.md` & `wizlib-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/pyproject.toml` & `wizlib-3.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wizlib"
-version = "3.0.0"
+version = "3.0.1"
 description = "Framework for flexible and powerful command-line applications"
 authors = ["Steampunk Wizard <wizlib@steampunkwizard.ca>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `wizlib-3.0.0/wizlib/app.py` & `wizlib-3.0.1/wizlib/app.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/wizlib/class_family.py` & `wizlib-3.0.1/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/wizlib/command.py` & `wizlib-3.0.1/wizlib/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Note that commands once used dataclass, but no longer.
+
 from argparse import ArgumentParser
 from pathlib import Path
 
 from wizlib.class_family import ClassFamily
 from wizlib.config_handler import ConfigHandler
 from wizlib.stream_handler import StreamHandler
 from wizlib.super_wrapper import SuperWrapper
@@ -12,16 +14,15 @@
     pass
 
 
 class WizCommand(ClassFamily, SuperWrapper):
     """Define all the args you want, but stdin always works."""
 
     status = ''
-    handlers = []
-    ui: UI = None
+    handlers = []  # TODO: Move to app
 
     @classmethod
     def add_args(self, parser):
         """Add arguments to the command's parser - override this.
         Add global arguments in the base class. Not wrapped."""
         pass
```

### Comparing `wizlib-3.0.0/wizlib/config_handler.py` & `wizlib-3.0.1/wizlib/config_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/wizlib/parser.py` & `wizlib-3.0.1/wizlib/parser.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/wizlib/rlinput.py` & `wizlib-3.0.1/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/wizlib/stream_handler.py` & `wizlib-3.0.1/wizlib/stream_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/wizlib/ui/__init__.py` & `wizlib-3.0.1/wizlib/ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,20 +123,20 @@
             self.choices = []
 
     def add_choice(self, *args, **kwargs):
         choice = Choice(*args, **kwargs)
         self.choices.append(choice)
 
     def choice_by_key(self, key):
-        if key == '\n':
-            choice = self.default
+        if key == '\n' and self.default:
+            choice = self.choices[0].value
         else:
             choice = next(
                 (o.value for o in self.choices if key in o.keys), None)
-        return choice() if callable(choice) else choice
+        return choice
 
     def choices_by_text(self, text):
         return [o.value for o in self.choices if o.hit_text(text)]
 
 
 @dataclass
 class UI(ClassFamily):
```

### Comparing `wizlib-3.0.0/wizlib/ui/shell/__init__.py` & `wizlib-3.0.1/wizlib/ui/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/wizlib/ui/shell/line_editor.py` & `wizlib-3.0.1/wizlib/ui/shell/line_editor.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/wizlib/ui/shell_ui.py` & `wizlib-3.0.1/wizlib/ui/shell_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 key if key.isprintable() else ''
             choice = chooser.choice_by_key(key)
             emphasis = Emphasis.ERROR if (
                 choice is None) else Emphasis.PRINCIPAL
             self.send(out, emphasis=emphasis)
             if choice is not None:
                 break
-        return choice
+        return choice() if callable(choice) else choice
 
     def get_text(self, prompt='', choices=[], default=''):
         """Allow the user to input an arbitrary line of text, with possible tab
         completion"""
         self.ask(prompt)
         if INTERACTIVE:
             value = ShellLineEditor(choices, default).edit()
```

### Comparing `wizlib-3.0.0/wizlib/ui_handler.py` & `wizlib-3.0.1/wizlib/ui_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.0/PKG-INFO` & `wizlib-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 3.0.0
+Version: 3.0.1
 Summary: Framework for flexible and powerful command-line applications
 License: MIT
 Author: Steampunk Wizard
 Author-email: wizlib@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

