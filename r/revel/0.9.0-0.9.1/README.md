# Comparing `tmp/revel-0.9.0.tar.gz` & `tmp/revel-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revel-0.9.0.tar", max compression
+gzip compressed data, was "revel-0.9.1.tar", max compression
```

## Comparing `revel-0.9.0.tar` & `revel-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2332 2023-11-08 19:51:02.358299 revel-0.9.0/README.md
--rw-r--r--   0        0        0      698 2024-04-10 20:53:17.464413 revel-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      409 2024-04-10 19:36:28.949450 revel-0.9.0/revel/__init__.py
--rw-r--r--   0        0        0    19979 2024-04-10 20:42:29.987625 revel-0.9.0/revel/argument_parser.py
--rw-r--r--   0        0        0    12853 2024-04-10 20:49:41.346830 revel-0.9.0/revel/cli_app.py
--rw-r--r--   0        0        0     4912 2024-04-10 19:35:14.694203 revel-0.9.0/revel/common.py
--rw-r--r--   0        0        0     1919 2024-04-10 19:36:28.959449 revel-0.9.0/revel/errors.py
--rw-r--r--   0        0        0    32100 2024-04-10 19:40:05.148617 revel-0.9.0/revel/legacy.py
--rw-r--r--   0        0        0      723 2023-11-08 19:51:03.998300 revel-0.9.0/revel/markup.py
--rw-r--r--   0        0        0     7533 2024-04-10 19:40:50.824400 revel-0.9.0/revel/menu.py
--rw-r--r--   0        0        0       80 2023-11-08 19:51:04.001634 revel-0.9.0/revel/rapidbaby/__init__.py
--rw-r--r--   0        0        0      274 2023-11-08 19:51:04.001634 revel-0.9.0/revel/rapidbaby/common.py
--rw-r--r--   0        0        0     7136 2024-02-04 09:24:39.690123 revel-0.9.0/revel/rapidbaby/parser.py
--rw-r--r--   0        0        0     5836 2024-02-04 09:24:50.466800 revel-0.9.0/revel/rapidbaby/styles.py
--rw-r--r--   0        0        0     2106 2024-02-04 09:24:16.310104 revel-0.9.0/revel/shell_escape.py
--rw-r--r--   0        0        0      815 2023-11-08 19:51:04.001634 revel-0.9.0/revel/style.py
--rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 revel-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2332 2023-11-08 19:51:02.358299 revel-0.9.1/README.md
+-rw-r--r--   0        0        0      698 2024-05-19 13:27:42.943168 revel-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-04-10 19:36:28.949450 revel-0.9.1/revel/__init__.py
+-rw-r--r--   0        0        0    20153 2024-04-15 04:43:41.199800 revel-0.9.1/revel/argument_parser.py
+-rw-r--r--   0        0        0    12853 2024-04-10 20:49:41.346830 revel-0.9.1/revel/cli_app.py
+-rw-r--r--   0        0        0     5014 2024-05-19 13:27:22.556487 revel-0.9.1/revel/common.py
+-rw-r--r--   0        0        0     1919 2024-04-10 19:36:28.959449 revel-0.9.1/revel/errors.py
+-rw-r--r--   0        0        0    32254 2024-04-27 16:45:08.040679 revel-0.9.1/revel/legacy.py
+-rw-r--r--   0        0        0      723 2023-11-08 19:51:03.998300 revel-0.9.1/revel/markup.py
+-rw-r--r--   0        0        0     7533 2024-04-10 19:40:50.824400 revel-0.9.1/revel/menu.py
+-rw-r--r--   0        0        0       80 2023-11-08 19:51:04.001634 revel-0.9.1/revel/rapidbaby/__init__.py
+-rw-r--r--   0        0        0      274 2023-11-08 19:51:04.001634 revel-0.9.1/revel/rapidbaby/common.py
+-rw-r--r--   0        0        0     7136 2024-02-04 09:24:39.690123 revel-0.9.1/revel/rapidbaby/parser.py
+-rw-r--r--   0        0        0     5836 2024-02-04 09:24:50.466800 revel-0.9.1/revel/rapidbaby/styles.py
+-rw-r--r--   0        0        0     2106 2024-02-04 09:24:16.310104 revel-0.9.1/revel/shell_escape.py
+-rw-r--r--   0        0        0      815 2024-04-27 16:42:31.847043 revel-0.9.1/revel/style.py
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 revel-0.9.1/PKG-INFO
```

### Comparing `revel-0.9.0/README.md` & `revel-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/pyproject.toml` & `revel-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "revel"
-version = "0.9.0"
+version = "0.9.1"
 description = "Effortlessly spice up your terminal apps using colors, progressbars & more"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 repository = "https://gitlab.com/Vivern/revel"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `revel-0.9.0/revel/argument_parser.py` & `revel-0.9.1/revel/argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -644,9 +644,12 @@
             options[f"[bold]{pretty_name}[/] - {summary}"] = name
 
     return (
         menu.select(
             prompt="What would you like to do?",
             options=options,
         ),
-        raw_args,
+        # Drop any passed arguments in this case. They cannot be parsed without
+        # knowing the command, and since the command was nonsense they're likely
+        # as well.
+        [],
     )
```

### Comparing `revel-0.9.0/revel/cli_app.py` & `revel-0.9.1/revel/cli_app.py`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/revel/common.py` & `revel-0.9.1/revel/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,24 +76,27 @@
 
     # Expand the options
     expanded_options: list[list[str]] = [
         [option] if isinstance(option, str) else option for option in options
     ]
 
     # Normalize the user input
-    selection = selection.strip().lower()
+    def normalize(value: str) -> str:
+        return value.strip().lower().replace(" ", "-").replace("_", "-")
+
+    selection = normalize(selection)
 
     # Find all choices that match the user's input. If one matches exactly, go
     # with that.
     matching_indices: Set[int] = set()
     matching_values: Set[str] = set()
 
     for ii, choice_set in enumerate(expanded_options):
         for choice in choice_set:
-            choice = choice.strip().lower()
+            choice = normalize(choice)
 
             # Exact match? This is it
             if choice == selection:
                 return ii
 
             # Partial match? Add it to the list of possible matches
             if selection in choice:
```

### Comparing `revel-0.9.0/revel/errors.py` & `revel-0.9.1/revel/errors.py`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/revel/legacy.py` & `revel-0.9.1/revel/legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -960,14 +960,19 @@
         _docked_widget.undock()
         sys.stdout.write("\n")
 
     # Preprocess the prompt
     if markup:
         prompt = markup_module.unescape(prompt)
 
+    if default is not _SENTINEL:
+        prompt += markup_module.unescape(
+            f" [primary][[{markup_module.escape(str(default))}][/]"
+        )
+
     prompt += markup_module.unescape(f"[primary bold]{markup_module.escape(sep)}[/]")
 
     if _chapter is not None:
         prompt = f"   {prompt}"
 
     # Ask for values, until a valid one comes along
     while True:
```

### Comparing `revel-0.9.0/revel/markup.py` & `revel-0.9.1/revel/markup.py`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/revel/menu.py` & `revel-0.9.1/revel/menu.py`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/revel/rapidbaby/parser.py` & `revel-0.9.1/revel/rapidbaby/parser.py`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/revel/rapidbaby/styles.py` & `revel-0.9.1/revel/rapidbaby/styles.py`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/revel/shell_escape.py` & `revel-0.9.1/revel/shell_escape.py`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/revel/style.py` & `revel-0.9.1/revel/style.py`

 * *Files identical despite different names*

### Comparing `revel-0.9.0/PKG-INFO` & `revel-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revel
-Version: 0.9.0
+Version: 0.9.1
 Summary: Effortlessly spice up your terminal apps using colors, progressbars & more
 Home-page: https://gitlab.com/Vivern/revel
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

