# Comparing `tmp/binary_to_text-0.0.2.tar.gz` & `tmp/binary_to_text-0.0.3.tar.gz`

## Comparing `binary_to_text-0.0.2.tar` & `binary_to_text-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/btt.iml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/src/binary_to_text/__init__.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/src/binary_to_text/main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/LICENSE
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/README.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/.idea/btt.iml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/src/binary_to_text/__init__.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/src/binary_to_text/main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/LICENSE
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/README.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 binary_to_text-0.0.3/PKG-INFO
```

### Comparing `binary_to_text-0.0.2/.idea/workspace.xml` & `binary_to_text-0.0.3/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `binary_to_text-0.0.2/src/binary_to_text/main.py` & `binary_to_text-0.0.3/src/binary_to_text/main.py`

 * *Files identical despite different names*

### Comparing `binary_to_text-0.0.2/LICENSE` & `binary_to_text-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `binary_to_text-0.0.2/README.md` & `binary_to_text-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,36 @@
-
-Hello this is my first library this library converts binary code into text and vice versa
-----------
-
-Converts a string of binary code to text
-----------
-    translator.binary_to_text(binary_code)
-
-Converts a string of text to binary code
-----------
-    translator.text_to_binary(text)
-Usage example
-----------
-Binary code to text
-
-    binary_code = '01001000 01100101 01101100 01101100 01101111'
-    text = translator.binary_to_text(binary_code)
-    print(f"Translation of binary code '{binary_code}' to text: '{text}'")
-
-Text to binary code
-
-    text = 'Hello'
-    binary_code = translator.text_to_binary(text)
+Metadata-Version: 2.3
+Name: binary_to_text
+Version: 0.0.3
+Summary: Binary to text and Text to binary
+Author: Muka
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+
+
+Hello this is my first library this library converts binary code into text and vice versa
+----------
+
+Converts a string of binary code to text
+----------
+    binary_to_text(binary_code)
+
+Converts a string of text to binary code
+----------
+    text_to_binary(text)
+Usage example
+----------
+Binary code to text
+
+    binary_code = '01001000 01100101 01101100 01101100 01101111'
+    text = binary_to_text(binary_code)
+    print(f"Translation of binary code '{binary_code}' to text: '{text}'")
+
+Text to binary code
+
+    text = 'Hello'
+    binary_code = text_to_binary(text)
     print(f"Translation of text '{text}' to binary code: '{binary_code}'")
```

### Comparing `binary_to_text-0.0.2/PKG-INFO` & `binary_to_text-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,24 @@
-Metadata-Version: 2.3
-Name: binary_to_text
-Version: 0.0.2
-Summary: Binary to text
-Author: Muka
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-
-
-Hello this is my first library this library converts binary code into text and vice versa
-----------
-
-Converts a string of binary code to text
-----------
-    translator.binary_to_text(binary_code)
-
-Converts a string of text to binary code
-----------
-    translator.text_to_binary(text)
-Usage example
-----------
-Binary code to text
-
-    binary_code = '01001000 01100101 01101100 01101100 01101111'
-    text = translator.binary_to_text(binary_code)
-    print(f"Translation of binary code '{binary_code}' to text: '{text}'")
-
-Text to binary code
-
-    text = 'Hello'
-    binary_code = translator.text_to_binary(text)
+
+Hello this is my first library this library converts binary code into text and vice versa
+----------
+
+Converts a string of binary code to text
+----------
+    binary_to_text(binary_code)
+
+Converts a string of text to binary code
+----------
+    text_to_binary(text)
+Usage example
+----------
+Binary code to text
+
+    binary_code = '01001000 01100101 01101100 01101100 01101111'
+    text = binary_to_text(binary_code)
+    print(f"Translation of binary code '{binary_code}' to text: '{text}'")
+
+Text to binary code
+
+    text = 'Hello'
+    binary_code = text_to_binary(text)
     print(f"Translation of text '{text}' to binary code: '{binary_code}'")
```

