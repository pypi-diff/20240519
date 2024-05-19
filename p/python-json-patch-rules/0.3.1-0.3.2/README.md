# Comparing `tmp/python_json_patch_rules-0.3.1.tar.gz` & `tmp/python_json_patch_rules-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_json_patch_rules-0.3.1.tar", last modified: Mon May  6 07:49:39 2024, max compression
+gzip compressed data, was "python_json_patch_rules-0.3.2.tar", last modified: Sun May 19 08:53:54 2024, max compression
```

## Comparing `python_json_patch_rules-0.3.1.tar` & `python_json_patch_rules-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-06 07:49:39.920216 python_json_patch_rules-0.3.1/
--rw-r--r--   0 bagutoli   (503) staff       (20)     1069 2024-05-02 14:21:33.000000 python_json_patch_rules-0.3.1/LICENSE
--rw-r--r--   0 bagutoli   (503) staff       (20)     8898 2024-05-06 07:49:39.919442 python_json_patch_rules-0.3.1/PKG-INFO
--rw-r--r--   0 bagutoli   (503) staff       (20)     8369 2024-05-05 12:18:46.000000 python_json_patch_rules-0.3.1/README.md
-drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-06 07:49:39.898943 python_json_patch_rules-0.3.1/json_patch_rules/
--rw-r--r--   0 bagutoli   (503) staff       (20)     6626 2024-05-06 07:44:22.000000 python_json_patch_rules-0.3.1/json_patch_rules/__init__.py
--rw-r--r--   0 bagutoli   (503) staff       (20)      482 2024-05-05 12:18:46.000000 python_json_patch_rules-0.3.1/json_patch_rules/__symbols__.py
--rw-r--r--   0 bagutoli   (503) staff       (20)      519 2024-05-03 15:38:44.000000 python_json_patch_rules-0.3.1/json_patch_rules/paths.py
--rw-r--r--   0 bagutoli   (503) staff       (20)      382 2024-05-02 14:27:47.000000 python_json_patch_rules-0.3.1/pyproject.toml
-drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-06 07:49:39.918753 python_json_patch_rules-0.3.1/python_json_patch_rules.egg-info/
--rw-r--r--   0 bagutoli   (503) staff       (20)     8898 2024-05-06 07:49:39.000000 python_json_patch_rules-0.3.1/python_json_patch_rules.egg-info/PKG-INFO
--rw-r--r--   0 bagutoli   (503) staff       (20)      442 2024-05-06 07:49:39.000000 python_json_patch_rules-0.3.1/python_json_patch_rules.egg-info/SOURCES.txt
--rw-r--r--   0 bagutoli   (503) staff       (20)        1 2024-05-06 07:49:39.000000 python_json_patch_rules-0.3.1/python_json_patch_rules.egg-info/dependency_links.txt
--rw-r--r--   0 bagutoli   (503) staff       (20)        7 2024-05-06 07:49:39.000000 python_json_patch_rules-0.3.1/python_json_patch_rules.egg-info/requires.txt
--rw-r--r--   0 bagutoli   (503) staff       (20)       23 2024-05-06 07:49:39.000000 python_json_patch_rules-0.3.1/python_json_patch_rules.egg-info/top_level.txt
--rw-r--r--   0 bagutoli   (503) staff       (20)      553 2024-05-06 07:49:39.920984 python_json_patch_rules-0.3.1/setup.cfg
--rw-r--r--   0 bagutoli   (503) staff       (20)     1281 2024-05-06 07:44:28.000000 python_json_patch_rules-0.3.1/setup.py
-drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-06 07:49:39.917276 python_json_patch_rules-0.3.1/tests/
--rw-r--r--   0 bagutoli   (503) staff       (20)        0 2024-05-02 12:17:58.000000 python_json_patch_rules-0.3.1/tests/__init__.py
--rw-r--r--   0 bagutoli   (503) staff       (20)    11566 2024-05-06 07:49:14.000000 python_json_patch_rules-0.3.1/tests/test_module.py
+drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-19 08:53:54.228636 python_json_patch_rules-0.3.2/
+-rw-r--r--   0 bagutoli   (503) staff       (20)     1069 2024-05-02 14:21:33.000000 python_json_patch_rules-0.3.2/LICENSE
+-rw-r--r--   0 bagutoli   (503) staff       (20)     8898 2024-05-19 08:53:54.227262 python_json_patch_rules-0.3.2/PKG-INFO
+-rw-r--r--   0 bagutoli   (503) staff       (20)     8369 2024-05-05 12:18:46.000000 python_json_patch_rules-0.3.2/README.md
+drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-19 08:53:54.210191 python_json_patch_rules-0.3.2/json_patch_rules/
+-rw-r--r--   0 bagutoli   (503) staff       (20)     6625 2024-05-06 13:18:29.000000 python_json_patch_rules-0.3.2/json_patch_rules/__init__.py
+-rw-r--r--   0 bagutoli   (503) staff       (20)      482 2024-05-05 12:18:46.000000 python_json_patch_rules-0.3.2/json_patch_rules/__symbols__.py
+-rw-r--r--   0 bagutoli   (503) staff       (20)      519 2024-05-03 15:38:44.000000 python_json_patch_rules-0.3.2/json_patch_rules/paths.py
+-rw-r--r--   0 bagutoli   (503) staff       (20)      382 2024-05-02 14:27:47.000000 python_json_patch_rules-0.3.2/pyproject.toml
+drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-19 08:53:54.226212 python_json_patch_rules-0.3.2/python_json_patch_rules.egg-info/
+-rw-r--r--   0 bagutoli   (503) staff       (20)     8898 2024-05-19 08:53:53.000000 python_json_patch_rules-0.3.2/python_json_patch_rules.egg-info/PKG-INFO
+-rw-r--r--   0 bagutoli   (503) staff       (20)      442 2024-05-19 08:53:54.000000 python_json_patch_rules-0.3.2/python_json_patch_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 bagutoli   (503) staff       (20)        1 2024-05-19 08:53:53.000000 python_json_patch_rules-0.3.2/python_json_patch_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 bagutoli   (503) staff       (20)        7 2024-05-19 08:53:53.000000 python_json_patch_rules-0.3.2/python_json_patch_rules.egg-info/requires.txt
+-rw-r--r--   0 bagutoli   (503) staff       (20)       23 2024-05-19 08:53:53.000000 python_json_patch_rules-0.3.2/python_json_patch_rules.egg-info/top_level.txt
+-rw-r--r--   0 bagutoli   (503) staff       (20)      553 2024-05-19 08:53:54.230022 python_json_patch_rules-0.3.2/setup.cfg
+-rw-r--r--   0 bagutoli   (503) staff       (20)     1281 2024-05-19 08:53:47.000000 python_json_patch_rules-0.3.2/setup.py
+drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-19 08:53:54.222323 python_json_patch_rules-0.3.2/tests/
+-rw-r--r--   0 bagutoli   (503) staff       (20)        0 2024-05-02 12:17:58.000000 python_json_patch_rules-0.3.2/tests/__init__.py
+-rw-r--r--   0 bagutoli   (503) staff       (20)    12916 2024-05-06 13:01:38.000000 python_json_patch_rules-0.3.2/tests/test_module.py
```

### Comparing `python_json_patch_rules-0.3.1/LICENSE` & `python_json_patch_rules-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_json_patch_rules-0.3.1/PKG-INFO` & `python_json_patch_rules-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-json-patch-rules
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library to apply JSON patches with rule-based access control.
 Home-page: https://github.com/agutoli/python-json-patch-rules
 Author: Bruno Agutoli
 Author-email: bruno.agutoli@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python_json_patch_rules-0.3.1/README.md` & `python_json_patch_rules-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `python_json_patch_rules-0.3.1/json_patch_rules/__init__.py` & `python_json_patch_rules-0.3.2/json_patch_rules/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,21 +111,20 @@
 
         actions_data = {"unique": []}
         value_obj_paths = list(self.get_paths(new_data))
         
         if len(value_obj_paths) == 0:
             value_obj_paths = [EMPTY_ARRAY_SYMBOL]
 
-        replace_data = pydash.clone_deep(new_data)
+        replace_data = pydash.clone_deep(old_data)
         for path in value_obj_paths:
             is_allowed, rule_item, data_path = self.verify_permission(path, new_data)
             if is_allowed:
                 should_replace = 'replace' in rule_item.actions
                 should_be_unique = 'unique' in rule_item.actions
-
                 result.successed_paths.append(path)
                 if should_replace and data_path is None:
                     result.data = new_data
                 elif should_replace and data_path:
                     pydash.set_(replace_data, data_path, pydash.get(new_data, data_path))
                     result.data = replace_data
                 elif should_be_unique:
```

### Comparing `python_json_patch_rules-0.3.1/json_patch_rules/paths.py` & `python_json_patch_rules-0.3.2/json_patch_rules/paths.py`

 * *Files identical despite different names*

### Comparing `python_json_patch_rules-0.3.1/python_json_patch_rules.egg-info/PKG-INFO` & `python_json_patch_rules-0.3.2/python_json_patch_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-json-patch-rules
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library to apply JSON patches with rule-based access control.
 Home-page: https://github.com/agutoli/python-json-patch-rules
 Author: Bruno Agutoli
 Author-email: bruno.agutoli@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python_json_patch_rules-0.3.1/setup.cfg` & `python_json_patch_rules-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `python_json_patch_rules-0.3.1/setup.py` & `python_json_patch_rules-0.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-json-patch-rules",
-    version="0.3.1",
+    version="0.3.2",
     author="Bruno Agutoli",
     author_email="bruno.agutoli@gmail.com",
     description="A library to apply JSON patches with rule-based access control.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/agutoli/python-json-patch-rules",
     # Correct the package_dir to point to 'json_patch_rules' since your actual package code is there
```

### Comparing `python_json_patch_rules-0.3.1/tests/test_module.py` & `python_json_patch_rules-0.3.2/tests/test_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -279,8 +279,54 @@
         "[*].tags|replace"
     ]
     patch = patch_rules(rules)
     old_data = [{"tags": ["a", "b", "c"]}]
     new_data = [{"tags": ["overwrite"]}]
 
     result = patch.apply(old_data, new_data)
-    assert result.data[0]["tags"] == ['overwrite'], "Should replace array"
+    assert result.data[0]["tags"] == ['overwrite'], "Should replace array"
+
+
+def test_replace_nested_attribute_within_array():
+    rules = [
+        # "{*}.id",
+        # "{*}.title",
+        "{*}.tags|replace",
+        # "{*}.tier",
+        # "{*}.categories|replace",
+        # "{*}.validTo",
+        # "{*}.validFrom",
+        # "{*}.duration"
+    ]
+    patch = patch_rules(rules)
+
+    old_data = {
+        "key_a": {
+            "tags": [
+                "rz"
+            ],
+            "tier": 1,
+            "video": {
+                "src": {
+                    "model:app_label": "app_media_content",
+                    "model:object_id": "8a400a98-29aa-42bb-bc29-fcd895a6416b",
+                    "model:model_name": "file",
+                    "model:values_mapping": {
+                        "ext": "png",
+                        "name": "env_Angelway.png",
+                        "mimetype": "image/png",
+                        "local_object_path": "media_content/png/8a400a98-29aa-42bb-bc29-fcd895a6416b.png",
+                        "published_object_path": "prod/media-content/2024-05-02/8a400a98-29aa-42bb-bc29-fcd895a6416b.png"
+                    }
+                }
+            }
+        }
+    }
+
+    new_data = {
+        "key_a": {
+            "tags": ["overwrite"]
+        }
+    }
+
+    result = patch.apply(old_data, new_data)
+    assert result.data["key_a"] == 'overwrite', "Should replace array"
```

