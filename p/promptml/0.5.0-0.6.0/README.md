# Comparing `tmp/promptml-0.5.0.tar.gz` & `tmp/promptml-0.6.0.tar.gz`

## Comparing `promptml-0.5.0.tar` & `promptml-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 promptml-0.5.0/BUILD.md
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 promptml-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0   158793 2020-02-02 00:00:00.000000 promptml-0.5.0/prompt-github.png
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 promptml-0.5.0/prompt.pml
--rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 promptml-0.5.0/promptml.jpeg
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 promptml-0.5.0/requirements.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 promptml-0.5.0/requirements_dev.txt
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 promptml-0.5.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 promptml-0.5.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 promptml-0.5.0/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 promptml-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/basic-calculator/README.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/basic-calculator/calculator.jinja2
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/basic-calculator/calculator.pml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/basic-calculator/main.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/basic-calculator/requirements.txt
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/poem-writer/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/poem-writer/main.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/poem-writer/poem.jinja2
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/poem-writer/poem.pml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/poem-writer/requirements.txt
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/recommend-challenges/main.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/recommend-challenges/recommend.jinja2
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/recommend-challenges/recommend.pml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.5.0/examples/recommend-challenges/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 promptml-0.5.0/src/promptml/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 promptml-0.5.0/src/promptml/__init__.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 promptml-0.5.0/src/promptml/grammar.lark
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 promptml-0.5.0/src/promptml/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 promptml-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 promptml-0.5.0/tests/test_parser.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 promptml-0.5.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 promptml-0.5.0/LICENSE
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 promptml-0.5.0/README.md
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 promptml-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 promptml-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 promptml-0.6.0/BUILD.md
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 promptml-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    20850 2020-02-02 00:00:00.000000 promptml-0.6.0/logo.png
+-rw-r--r--   0        0        0   158793 2020-02-02 00:00:00.000000 promptml-0.6.0/prompt-github.png
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 promptml-0.6.0/prompt.pml
+-rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 promptml-0.6.0/promptml.jpeg
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 promptml-0.6.0/requirements.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 promptml-0.6.0/requirements_dev.txt
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 promptml-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 promptml-0.6.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 promptml-0.6.0/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 promptml-0.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/README.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/calculator.jinja2
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/calculator.pml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/main.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/basic-calculator/requirements.txt
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/main.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/poem.jinja2
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/poem.pml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/poem-writer/requirements.txt
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/recommend-challenges/main.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/recommend-challenges/recommend.jinja2
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/recommend-challenges/recommend.pml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 promptml-0.6.0/examples/recommend-challenges/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/__init__.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/grammar.lark
+-rw-r--r--   0        0        0     7452 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/parser.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 promptml-0.6.0/src/promptml/serializer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 promptml-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 promptml-0.6.0/tests/test_parser.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 promptml-0.6.0/tests/test_serializer.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 promptml-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 promptml-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 promptml-0.6.0/README.md
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 promptml-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 promptml-0.6.0/PKG-INFO
```

### Comparing `promptml-0.5.0/BUILD.md` & `promptml-0.6.0/BUILD.md`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/CODE_OF_CONDUCT.md` & `promptml-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/prompt-github.png` & `promptml-0.6.0/prompt-github.png`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/prompt.pml` & `promptml-0.6.0/prompt.pml`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/promptml.jpeg` & `promptml-0.6.0/promptml.jpeg`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/.github/workflows/build.yml` & `promptml-0.6.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/.github/workflows/pylint.yml` & `promptml-0.6.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/.github/workflows/unittest.yml` & `promptml-0.6.0/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/examples/basic-calculator/README.md` & `promptml-0.6.0/examples/basic-calculator/README.md`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/examples/basic-calculator/calculator.pml` & `promptml-0.6.0/examples/basic-calculator/calculator.pml`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/examples/basic-calculator/main.py` & `promptml-0.6.0/examples/basic-calculator/main.py`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/examples/poem-writer/README.md` & `promptml-0.6.0/examples/poem-writer/README.md`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/examples/poem-writer/main.py` & `promptml-0.6.0/examples/poem-writer/main.py`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/examples/poem-writer/poem.jinja2` & `promptml-0.6.0/examples/poem-writer/poem.jinja2`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/examples/poem-writer/poem.pml` & `promptml-0.6.0/examples/poem-writer/poem.pml`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/examples/recommend-challenges/main.py` & `promptml-0.6.0/examples/recommend-challenges/main.py`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/src/promptml/grammar.lark` & `promptml-0.6.0/src/promptml/grammar.lark`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/src/promptml/parser.py` & `promptml-0.6.0/src/promptml/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,17 @@
         ...
     '''
 
     parser = PromptParser(dsl_code)
     prompt = parser.parse()
 """
 
-import json
 import os
-import re
-
 from lark import Lark, Transformer
+from .serializer import SerializerFactory
 
 class PromptMLTransformer(Transformer):
     """
     A class for transforming the parsed PromptML tree into a Python dictionary.
     """
 
     def start(self, items):
@@ -178,14 +176,17 @@
         dir_path = os.path.abspath(os.path.dirname(__file__))
         with open(f'{dir_path}/grammar.lark', 'r', encoding="utf-8") as f:
             promptml_grammar = f.read()
 
         self.code = code
         self.prompt = {}
         self.parser = Lark(promptml_grammar)
+        self.xml_serializer = SerializerFactory.create_serializer("xml")
+        self.json_serializer = SerializerFactory.create_serializer("json")
+        self.yaml_serializer = SerializerFactory.create_serializer("yaml")
 
     def parse(self):
         """
         Parse the DSL code and extract the prompt information.
 
         Returns:
             dict: A dictionary containing the prompt information.
@@ -197,24 +198,28 @@
         """
         Parse the prompt section of the DSL code and extract the prompt content.
         """
         tree = self.parser.parse(self.code)
         self.prompt = PromptParser.transformer.transform(tree)
         return self.prompt
 
-    def serialize_json(self, indent=None):
+    def to_json(self, indent=None):
         """ Serialize the prompt data to JSON.
         """
-        return json.dumps(self.prompt, indent=indent)
+        return self.json_serializer.serialize(self.prompt, indent=indent)
 
-    def deserialize_json(self, serialized_data):
-        """ Deserialize the prompt data from JSON.
+    def to_yaml(self):
+        """ Serialize the prompt data to YAML.
         """
-        self.prompt = json.loads(serialized_data)
+        return self.yaml_serializer.serialize(self.prompt)
 
+    def to_xml(self):
+        """ Serialize the prompt data to XML.
+        """
+        return self.xml_serializer.serialize(self.prompt)
 
 class PromptParserFromFile(PromptParser):
     """
     A subclass of PromptParser that reads DSL code from a file.
     """
     def __init__(self, file_path: str):
         """
```

### Comparing `promptml-0.5.0/tests/test_parser.py` & `promptml-0.6.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/.gitignore` & `promptml-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/LICENSE` & `promptml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/README.md` & `promptml-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # PromptML (Prompt Markup Language)
 
-![](./promptml.jpeg)
+![logo](./logo.png)
 
 <i>A simple, yet elegant markup language for defining AI Prompts as Code (APaC). Built to be used by AI agents to automatically prompt for other AI systems.</i>
 
-The architecture is shown as below. A `PromptML` prompt can be version controlled like any other code file. Using promptml parser package, one can easily generate a natural language prompt, and execute it against a LLM. See examples for using promptml library package: [open examples](./examples/)
-
-![prompt-ml architecture](./prompt-github.png)
 
 ## Why PromptML ?
 
 PromptML is built to provide a way for prompt engineers to define the AI prompts in a deterministic way. This is a Domain Specific Language (DSL) which defines characteristics of a prompt including context, objective, instructions and it's metadata.
 A regular prompt is an amalgamation of all these aspects into one entity. PromptML splits it into multiple sections and makes the information explicit.
 
 The language grammar can be found here: [grammar.lark](./src/promptml/grammar.lark)
@@ -180,12 +177,10 @@
 @end
 ```
 
 ## TODO
 
 We are currently working on:
 
-1. Supporting more annotations (Ex: temperature, top_p)
-2. `VSCode` syntax highlighting support
-3. Publishing `promptml` package to PyPi
-4. Add more unit tests
-5. Add support for `XML` & `YAML` serialization
+1. `VSCode` syntax highlighting support
+2. Add more unit tests
+3. Add support for `XML` & `YAML` serialization
```

### Comparing `promptml-0.5.0/pyproject.toml` & `promptml-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `promptml-0.5.0/PKG-INFO` & `promptml-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: promptml
-Version: 0.5.0
+Version: 0.6.0
 Summary: A simple, yet elegant markup language for defining AI Prompts as Code (APaC). Built to be used by AI agents to automatically prompt for other AI systems
 Project-URL: Documentation, https://github.com/narenaryan/promptml/blob/main/README.md
 Project-URL: Issues, https://github.com/narenaryan/promptml/issues
 Project-URL: Source, https://github.com/narenaryan/promptml/
 Author-email: "Vidura Labs Inc." <contact@vidura.ai>, Naren Yellavula <naren.yellavula@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -19,21 +19,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # PromptML (Prompt Markup Language)
 
-![](./promptml.jpeg)
+![logo](./logo.png)
 
 <i>A simple, yet elegant markup language for defining AI Prompts as Code (APaC). Built to be used by AI agents to automatically prompt for other AI systems.</i>
 
-The architecture is shown as below. A `PromptML` prompt can be version controlled like any other code file. Using promptml parser package, one can easily generate a natural language prompt, and execute it against a LLM. See examples for using promptml library package: [open examples](./examples/)
-
-![prompt-ml architecture](./prompt-github.png)
 
 ## Why PromptML ?
 
 PromptML is built to provide a way for prompt engineers to define the AI prompts in a deterministic way. This is a Domain Specific Language (DSL) which defines characteristics of a prompt including context, objective, instructions and it's metadata.
 A regular prompt is an amalgamation of all these aspects into one entity. PromptML splits it into multiple sections and makes the information explicit.
 
 The language grammar can be found here: [grammar.lark](./src/promptml/grammar.lark)
@@ -203,12 +200,10 @@
 @end
 ```
 
 ## TODO
 
 We are currently working on:
 
-1. Supporting more annotations (Ex: temperature, top_p)
-2. `VSCode` syntax highlighting support
-3. Publishing `promptml` package to PyPi
-4. Add more unit tests
-5. Add support for `XML` & `YAML` serialization
+1. `VSCode` syntax highlighting support
+2. Add more unit tests
+3. Add support for `XML` & `YAML` serialization
```

