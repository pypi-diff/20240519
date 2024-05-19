# Comparing `tmp/meltdown-0.0.3.tar.gz` & `tmp/meltdown-0.0.4.tar.gz`

## Comparing `meltdown-0.0.3.tar` & `meltdown-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 meltdown-0.0.3/requirements.txt
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 meltdown-0.0.3/src/meltdown/HtmlProducer.py
--rw-r--r--   0        0        0    13528 2020-02-02 00:00:00.000000 meltdown-0.0.3/src/meltdown/MarkdownParser.py
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 meltdown-0.0.3/src/meltdown/Nodes.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 meltdown-0.0.3/src/meltdown/__init__.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 meltdown-0.0.3/tests/test_complex_html.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 meltdown-0.0.3/tests/test_simple_html.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 meltdown-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 meltdown-0.0.3/LICENSE
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 meltdown-0.0.3/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 meltdown-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 meltdown-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 meltdown-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 meltdown-0.0.4/src/meltdown/HtmlProducer.py
+-rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 meltdown-0.0.4/src/meltdown/MarkdownParser.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 meltdown-0.0.4/src/meltdown/Nodes.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 meltdown-0.0.4/src/meltdown/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 meltdown-0.0.4/tests/test_complex_html.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 meltdown-0.0.4/tests/test_simple_html.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 meltdown-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 meltdown-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 meltdown-0.0.4/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 meltdown-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 meltdown-0.0.4/PKG-INFO
```

### Comparing `meltdown-0.0.3/requirements.txt` & `meltdown-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `meltdown-0.0.3/src/meltdown/HtmlProducer.py` & `meltdown-0.0.4/src/meltdown/HtmlProducer.py`

 * *Files identical despite different names*

### Comparing `meltdown-0.0.3/src/meltdown/MarkdownParser.py` & `meltdown-0.0.4/src/meltdown/MarkdownParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         while not self._match("---") and not self._is_eof():
             line = self._consume_till(["\n", "\0"])
             self._consume_while(["\n", " "])
             if line.strip() == "":
                 continue
 
-            parts = line.split(":")
+            parts = line.split(":", 1)
             if len(parts) != 2:
                 # Malformed frontmatter, rewind and parse as paragraph
                 self._index = start_index
                 return {}
 
             metadata[parts[0].strip()] = parts[1].strip()
 
@@ -364,15 +364,14 @@
             # resetting the parsing position
             self._index -= len(url)
             return [TextNode("![")] + alt + [TextNode("](")]
 
         return [ImageNode(url, alt)]
 
     def _parse_comment(self: Self) -> Node:
-        print("comment")
         start_index = self._index
         comment = ""
         while not self._match("-->"):
             if self._is_eof():
                 # Rewind
                 self._index = start_index
                 return TextNode("<!--")
```

### Comparing `meltdown-0.0.3/src/meltdown/Nodes.py` & `meltdown-0.0.4/src/meltdown/Nodes.py`

 * *Files identical despite different names*

### Comparing `meltdown-0.0.3/tests/test_complex_html.py` & `meltdown-0.0.4/tests/test_complex_html.py`

 * *Files identical despite different names*

### Comparing `meltdown-0.0.3/tests/test_simple_html.py` & `meltdown-0.0.4/tests/test_simple_html.py`

 * *Files identical despite different names*

### Comparing `meltdown-0.0.3/.gitignore` & `meltdown-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `meltdown-0.0.3/LICENSE` & `meltdown-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meltdown-0.0.3/README.md` & `meltdown-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `meltdown-0.0.3/pyproject.toml` & `meltdown-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "meltdown"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "flofriday", email = "flohacksfriday@gmail.com" }]
 description = "A markdown parser"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `meltdown-0.0.3/PKG-INFO` & `meltdown-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: meltdown
-Version: 0.0.3
+Version: 0.0.4
 Summary: A markdown parser
 Project-URL: Homepage, https://github.com/flofriday/meltdown
 Project-URL: Issues, https://github.com/flofriday/meltdown/issues
 Author-email: flofriday <flohacksfriday@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

