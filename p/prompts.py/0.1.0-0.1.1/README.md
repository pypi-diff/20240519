# Comparing `tmp/prompts_py-0.1.0.tar.gz` & `tmp/prompts_py-0.1.1.tar.gz`

## Comparing `prompts_py-0.1.0.tar` & `prompts_py-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,33 @@
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 prompts_py-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 prompts_py-0.1.0/netlify.toml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 prompts_py-0.1.0/requirements.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 prompts_py-0.1.0/runtime.txt
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 prompts_py-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 prompts_py-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0   137162 2020-02-02 00:00:00.000000 prompts_py-0.1.0/assets/example.gif
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 prompts_py-0.1.0/docs/asking.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 prompts_py-0.1.0/docs/click.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 prompts_py-0.1.0/docs/index.md
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 prompts_py-0.1.0/docs/radios.md
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 prompts_py-0.1.0/docs/reference.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/_getch.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/_styles.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/input.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/integration.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/prompt.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/question.py
--rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 prompts_py-0.1.0/src/prompts/radio.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 prompts_py-0.1.0/tests/test_prompts.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 prompts_py-0.1.0/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 prompts_py-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 prompts_py-0.1.0/README.md
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 prompts_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 prompts_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 prompts_py-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 prompts_py-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 prompts_py-0.1.1/netlify.toml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 prompts_py-0.1.1/requirements.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 prompts_py-0.1.1/runtime.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 prompts_py-0.1.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 prompts_py-0.1.1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 prompts_py-0.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 prompts_py-0.1.1/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 prompts_py-0.1.1/.github/ISSUE_TEMPLATE/improvement.yml
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 prompts_py-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 prompts_py-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0   137162 2020-02-02 00:00:00.000000 prompts_py-0.1.1/assets/example.gif
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 prompts_py-0.1.1/docs/asking.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 prompts_py-0.1.1/docs/click.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 prompts_py-0.1.1/docs/index.md
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 prompts_py-0.1.1/docs/radios.md
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 prompts_py-0.1.1/docs/reference.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/_getch.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/_styles.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/input.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/integration.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/prompt.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/question.py
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 prompts_py-0.1.1/src/prompts/radio.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 prompts_py-0.1.1/tests/test_prompts.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 prompts_py-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 prompts_py-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 prompts_py-0.1.1/README.md
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 prompts_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 prompts_py-0.1.1/PKG-INFO
```

### Comparing `prompts_py-0.1.0/mkdocs.yml` & `prompts_py-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/.github/workflows/build.yml` & `prompts_py-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/.github/workflows/tests.yml` & `prompts_py-0.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/assets/example.gif` & `prompts_py-0.1.1/assets/example.gif`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/docs/asking.md` & `prompts_py-0.1.1/docs/asking.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,11 +61,11 @@
 !!! warning
 
     Some wacky behavior can occur if you add extra newlines between prompt API calls!
 
 ```py
 from prompts import Prompt
 
-with Prompt("Always look on the bright side of life...") as prompt:
-    prompt.answer = "*whistling*"
+with Prompt("My prompt...") as prompt:
+    prompt.answer = "My answer..."
     prompt.done()  # Mark the prompt as a success!
 ```
```

### Comparing `prompts_py-0.1.0/docs/click.md` & `prompts_py-0.1.1/docs/click.md`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/docs/index.md` & `prompts_py-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/docs/radios.md` & `prompts_py-0.1.1/docs/radios.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,18 +36,23 @@
 In some cases (such as with using the low level `Prompt` API), you might want to erase the radio display after a selection has been made. This can be done by passing `transient=True` to either `radio` or `ask_radio`. For example:
 
 ```py
 from prompts import radio
 
 print("What is your favorite color?", end=" ", flush=True)
 items = ["Blue", "No, yellow!"]
-index = radio(items)
+index = radio(items, transient=True)
 chosen_item = items[index]
+print(chosen_item)
 ```
 
+!!! note
+
+    The radio selection in `ask_radio` is always transient.
+
 ## Confirmations
 
 If you want a simple Y/N value from the user, you can use `confirm` or `ask_confirm`, which will display a radio containing a `Yes` and a `No`.
 
 ```py
 from prompts import ask_confirm
```

### Comparing `prompts_py-0.1.0/src/prompts/_getch.py` & `prompts_py-0.1.1/src/prompts/_getch.py`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/src/prompts/_styles.py` & `prompts_py-0.1.1/src/prompts/_styles.py`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/src/prompts/input.py` & `prompts_py-0.1.1/src/prompts/input.py`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/src/prompts/integration.py` & `prompts_py-0.1.1/src/prompts/integration.py`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/src/prompts/prompt.py` & `prompts_py-0.1.1/src/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/src/prompts/question.py` & `prompts_py-0.1.1/src/prompts/question.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,16 @@
             error: str | bool | None = None
             for validator in validators:
                 failed_message = validator(text)
 
                 if failed_message is not True:
                     if failed_message is False:
                         error = default_invalid
-
-                    error = failed_message
+                    else:
+                        error = failed_message
 
             prompt.answer = text
             if error:
                 prompt.error(error)
                 initial = text
             else:
                 prompt.done()
```

### Comparing `prompts_py-0.1.0/src/prompts/radio.py` & `prompts_py-0.1.1/src/prompts/radio.py`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/tests/test_prompts.py` & `prompts_py-0.1.1/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/LICENSE.txt` & `prompts_py-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/README.md` & `prompts_py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prompts_py-0.1.0/pyproject.toml` & `prompts_py-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 ]
 dependencies = ["colorama", "typing_extensions"]
 
 [project.optional-dependencies]
 click = ["click"]
 
 [project.urls]
-Documentation = "https://github.com/ZeroIntensity/prompts#readme"
-Issues = "https://github.com/ZeroIntensity/prompts/issues"
-Source = "https://github.com/ZeroIntensity/prompts"
+Documentation = "https://github.com/ZeroIntensity/prompts.py#readme"
+Issues = "https://github.com/ZeroIntensity/prompts.py/issues"
+Source = "https://github.com/ZeroIntensity/prompts.py"
 
 [tool.hatch.version]
 path = "src/prompts/__about__.py"
 
 [tool.hatch.envs.types]
 extra-dependencies = [
   "mypy>=1.0.0",
```

### Comparing `prompts_py-0.1.0/PKG-INFO` & `prompts_py-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: prompts.py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Beautiful prompts for Python.
-Project-URL: Documentation, https://github.com/ZeroIntensity/prompts#readme
-Project-URL: Issues, https://github.com/ZeroIntensity/prompts/issues
-Project-URL: Source, https://github.com/ZeroIntensity/prompts
+Project-URL: Documentation, https://github.com/ZeroIntensity/prompts.py#readme
+Project-URL: Issues, https://github.com/ZeroIntensity/prompts.py/issues
+Project-URL: Source, https://github.com/ZeroIntensity/prompts.py
 Author-email: ZeroIntensity <zintensitydev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

