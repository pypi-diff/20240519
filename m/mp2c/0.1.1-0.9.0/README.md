# Comparing `tmp/mp2c-0.1.1.tar.gz` & `tmp/mp2c-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mp2c-0.1.1.tar", last modified: Wed May 15 12:02:33 2024, max compression
+gzip compressed data, was "mp2c-0.9.0.tar", last modified: Sun May 19 06:28:43 2024, max compression
```

## Comparing `mp2c-0.1.1.tar` & `mp2c-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:02:33.605140 mp2c-0.1.1/
--rw-rw-rw-   0        0        0      138 2024-05-15 12:02:33.604132 mp2c-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-03-30 02:15:52.000000 mp2c-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 12:02:33.593269 mp2c-0.1.1/mp2c/
--rw-rw-rw-   0        0        0      242 2024-05-15 03:43:02.000000 mp2c-0.1.1/mp2c/__init__.py
--rw-rw-rw-   0        0        0     5940 2024-05-15 09:04:47.000000 mp2c-0.1.1/mp2c/context.py
--rw-rw-rw-   0        0        0     1534 2024-05-15 09:19:19.000000 mp2c-0.1.1/mp2c/converter.py
--rw-rw-rw-   0        0        0      144 2024-05-13 03:49:03.000000 mp2c-0.1.1/mp2c/errors.py
--rw-rw-rw-   0        0        0      473 2024-05-15 09:06:52.000000 mp2c-0.1.1/mp2c/result.py
--rw-rw-rw-   0        0        0     9312 2024-05-15 03:05:30.000000 mp2c-0.1.1/mp2c/rules.py
--rw-rw-rw-   0        0        0     5144 2024-05-15 08:50:25.000000 mp2c-0.1.1/mp2c/utils.py
--rw-rw-rw-   0        0        0    36586 2024-05-15 08:10:06.000000 mp2c-0.1.1/mp2c/visitors.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:02:33.597251 mp2c-0.1.1/mp2c.egg-info/
--rw-rw-rw-   0        0        0      138 2024-05-15 12:02:33.000000 mp2c-0.1.1/mp2c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-05-15 12:02:33.000000 mp2c-0.1.1/mp2c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:02:33.000000 mp2c-0.1.1/mp2c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-15 12:02:33.000000 mp2c-0.1.1/mp2c.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-15 12:02:33.000000 mp2c-0.1.1/mp2c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 12:02:33.605140 mp2c-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      379 2024-05-15 12:02:17.000000 mp2c-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:02:33.603126 mp2c-0.1.1/test/
--rw-rw-rw-   0        0        0        0 2024-05-10 01:57:03.000000 mp2c-0.1.1/test/__init__.py
--rw-rw-rw-   0        0        0      528 2024-05-15 03:32:03.000000 mp2c-0.1.1/test/test_array.py
--rw-rw-rw-   0        0        0     1594 2024-05-15 04:07:28.000000 mp2c-0.1.1/test/test_control.py
--rw-rw-rw-   0        0        0      693 2024-05-15 03:37:24.000000 mp2c-0.1.1/test/test_gcd.py
--rw-rw-rw-   0        0        0     2912 2024-05-15 08:11:36.000000 mp2c-0.1.1/test/test_lexical.py
--rw-rw-rw-   0        0        0     1087 2024-05-15 04:07:03.000000 mp2c-0.1.1/test/test_scope.py
--rw-rw-rw-   0        0        0     3228 2024-05-15 03:58:34.000000 mp2c-0.1.1/test/test_visitors.py
+drwxrwxrwx   0 s         (1000) s         (1000)        0 2024-05-19 06:28:43.464130 mp2c-0.9.0/
+-rwxrwxrwx   0 s         (1000) s         (1000)      133 2024-05-19 06:28:43.459669 mp2c-0.9.0/PKG-INFO
+-rwxrwxrwx   0 s         (1000) s         (1000)       14 2024-03-30 02:15:52.000000 mp2c-0.9.0/README.md
+drwxrwxrwx   0 s         (1000) s         (1000)        0 2024-05-19 06:28:43.317934 mp2c-0.9.0/mp2c/
+-rwxrwxrwx   0 s         (1000) s         (1000)      242 2024-05-15 03:43:02.000000 mp2c-0.9.0/mp2c/__init__.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     6514 2024-05-19 02:15:32.000000 mp2c-0.9.0/mp2c/context.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     1505 2024-05-19 02:15:32.000000 mp2c-0.9.0/mp2c/converter.py
+-rwxrwxrwx   0 s         (1000) s         (1000)      144 2024-05-13 03:49:03.000000 mp2c-0.9.0/mp2c/errors.py
+-rwxrwxrwx   0 s         (1000) s         (1000)      473 2024-05-15 09:06:52.000000 mp2c-0.9.0/mp2c/result.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     5319 2024-05-19 06:01:07.000000 mp2c-0.9.0/mp2c/rules.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     5244 2024-05-19 02:59:06.000000 mp2c-0.9.0/mp2c/utils.py
+-rwxrwxrwx   0 s         (1000) s         (1000)    41175 2024-05-19 06:14:51.000000 mp2c-0.9.0/mp2c/visitors.py
+drwxrwxrwx   0 s         (1000) s         (1000)        0 2024-05-19 06:28:43.454049 mp2c-0.9.0/mp2c.egg-info/
+-rwxrwxrwx   0 s         (1000) s         (1000)      133 2024-05-19 06:28:43.000000 mp2c-0.9.0/mp2c.egg-info/PKG-INFO
+-rwxrwxrwx   0 s         (1000) s         (1000)      471 2024-05-19 06:28:43.000000 mp2c-0.9.0/mp2c.egg-info/SOURCES.txt
+-rwxrwxrwx   0 s         (1000) s         (1000)        1 2024-05-19 06:28:43.000000 mp2c-0.9.0/mp2c.egg-info/dependency_links.txt
+-rwxrwxrwx   0 s         (1000) s         (1000)        5 2024-05-19 06:28:43.000000 mp2c-0.9.0/mp2c.egg-info/requires.txt
+-rwxrwxrwx   0 s         (1000) s         (1000)       10 2024-05-19 06:28:43.000000 mp2c-0.9.0/mp2c.egg-info/top_level.txt
+-rwxrwxrwx   0 s         (1000) s         (1000)       38 2024-05-19 06:28:43.464130 mp2c-0.9.0/setup.cfg
+-rwxrwxrwx   0 s         (1000) s         (1000)      391 2024-05-19 06:28:03.000000 mp2c-0.9.0/setup.py
+drwxrwxrwx   0 s         (1000) s         (1000)        0 2024-05-19 06:28:43.443307 mp2c-0.9.0/test/
+-rwxrwxrwx   0 s         (1000) s         (1000)        0 2024-05-10 01:57:03.000000 mp2c-0.9.0/test/__init__.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     1611 2024-05-19 06:23:10.000000 mp2c-0.9.0/test/test_array.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     4217 2024-05-19 02:29:39.000000 mp2c-0.9.0/test/test_comprehensive.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     2100 2024-05-19 06:24:32.000000 mp2c-0.9.0/test/test_control.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     2943 2024-05-19 05:50:31.000000 mp2c-0.9.0/test/test_lexical.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     7476 2024-05-19 05:47:31.000000 mp2c-0.9.0/test/test_math.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     1087 2024-05-15 04:07:03.000000 mp2c-0.9.0/test/test_scope.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     2234 2024-05-19 06:25:56.000000 mp2c-0.9.0/test/test_subprogram.py
+-rwxrwxrwx   0 s         (1000) s         (1000)     6712 2024-05-19 06:19:11.000000 mp2c-0.9.0/test/test_visitors.py
```

### Comparing `mp2c-0.1.1/mp2c/context.py` & `mp2c-0.9.0/mp2c/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,28 +12,28 @@
         self.symbol_table.append({"value": {}, "array": {}, "subprogram": {}})
         self.current_scope_index += 1
 
     def exit_scope(self):
         self.symbol_table.pop()
         self.current_scope_index -= 1
 
-    def register_func(self, name, header, parameter_list):
+    def register_func(self, name, header, parameter_list, var_parameter, tokens = None, is_library = False):
         if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to register function {} in no scope ".format(name))
         functions_in_top_smbltab = self.symbol_table[self.current_scope_index - 1]["subprogram"]
-        functions_in_top_smbltab[name] = FunctionSymbol(name, header, None, parameter_list)
+        functions_in_top_smbltab[name] = FunctionSymbol(name, header, tokens, parameter_list, var_parameter, is_library)
 
     def declare_func(self, name, tokens):
         self.symbol_table[self.current_scope_index - 1]["subprogram"][name].tokens = tokens
 
-    def register_value(self, name, value_type, mutable, value = None):
+    def register_value(self, name, value_type, mutable, value = None, var = False):
         if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to register value {} in no scope ".format(name))
         values_in_top_smbltab = self.symbol_table[self.current_scope_index]["value"]
-        values_in_top_smbltab[name] = ValueSymbol(name, value_type, mutable, value)
+        values_in_top_smbltab[name] = ValueSymbol(name, value_type, mutable, value, var)
 
     def register_array(self, name, array_type, periods):  # periods(start, last) : [[1, 5], [2, 4]]
         if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to register array {} in no scope ".format(name))
         arrays_in_top_smbltab = self.symbol_table[self.current_scope_index]["array"]
         dimensions = []
         for dimension in periods:
@@ -80,46 +80,47 @@
             index -= 1
         return func
 
     def record_error(self, message):
         self.on_error = True
         self.error_messages.append(message)
 
-    # def cname_to_type(self, name):
-    #     res = int
-    #     if name == "float" :
-    #         res = float
-    #     elif name == "char" or name == "char*":
-    #         res = str
-    #     elif name == "bool":
-    #         res = bool
-    #     return res
+    def declare_library_functions(self):
+        single_double_math_function_names = ["acos", "asin", "atan", "cos", "cosh", "sin", "sinh", "tanh", "exp", "log",
+                                             "log10", "sqrt", "ceil", "fabs", "floor"]
+        for function_name in single_double_math_function_names:
+            self.register_func(function_name, ["float", function_name, "(", "float", "x", ")", ";"],
+                               [{'ids': ['x'], 'type': 'float'}], [False], tokens = [], is_library = True)
 
 
 class FunctionSymbol:
-    def __init__(self, name, header, tokens, parameter_list):
+    def __init__(self, name, header, tokens, parameter_list, var_parameter, is_library = False):
         self.name = name
         self.header = header
         self.tokens = tokens
         self.parameter_list = parameter_list
+        self.var_parameter = var_parameter
+        self.is_library = is_library
 
     def __repr__(self) -> str:
-        description = "Function: " + self.name + "\n"
-        description += "Header: " + " ".join(self.header) + "\n"
-        description += "Tokens: " + str(self.tokens) + "\n"
-        description += "Parameters: " + str(self.parameter_list) + "\n"
+        description = "Function: " + self.name + " "
+        description += "Header: " + " ".join(self.header) + " "
+        description += "Tokens: " + str(self.tokens) + " "
+        description += "Parameters: " + str(self.parameter_list) + " "
+        description += "Var Parameter: " + str(self.var_parameter) + " "
         return description
 
 
 class ValueSymbol:
-    def __init__(self, name, value_type, mutable, value):
+    def __init__(self, name, value_type, mutable, value, var = False):
         self.name = name
         self.type = value_type
         self.mutable = mutable
         self.value = value
+        self.var = var
 
     def __repr__(self) -> str:
         description = "Value: " + self.name + "\n"
         description += "Type: " + self.type + "\n"
         description += "Mutable: " + str(self.mutable) + "\n"
         description += "Value: " + str(self.value) + "\n"
         return description
```

### Comparing `mp2c-0.1.1/mp2c/converter.py` & `mp2c-0.9.0/mp2c/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .rules import rules
 from .utils import format_code, preprocess, postprocess
 from .visitors import visit_programstruct
 
 
 class Converter:
     def __init__(self):
-        self.parser = Lark(rules, start = "programstruct", debug = True)
+        self.parser = Lark(rules, start = "programstruct")
 
     def __call__(self, code, debug = False) -> tuple[bool, str]:
         status = True
         parser = self.parser
         code = preprocess(code)
         tree = parser.parse(code)
         context = Context()
@@ -21,15 +21,15 @@
         if context.on_error:
             status = False
         tokens = postprocess(tokens)
         result_string = "\n".join(tokens)
         result_string = format_code(result_string)
         return status, result_string
 
-    def convert(self, code, debug = False) -> Result:
+    def convert(self, code) -> Result:
         status = True
         parser = self.parser
         code = preprocess(code)
         try:
             tree = parser.parse(code)
         except Exception as e:
             return Result("", False, [str(e)])
```

### Comparing `mp2c-0.1.1/mp2c/utils.py` & `mp2c-0.9.0/mp2c/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,87 @@
 import functools
 import re
+import subprocess
+import tempfile
+from enum import Enum
 
 from lark.lark import Tree
 
 from .context import Context
 from .errors import VisitingError
 
-type_map = {"integer": "int", "real": "float", "boolean": "bool", "char": "char"}
-relop_map = {"=": "==", "<>": "!=", "<": "<", "<=": "<=", ">": ">", ">=": ">="}
+type_map = {"integer": "int", "real": "float", "boolean": "bool", "char": "char", "string": "char*"}
+relop_map = {"=": "==", "<>": "!=", "<": "<", "<=": "<=", ">": ">", ">=": ">=", "==": "=="}
 addop_map = {"+": "+", "-": "-", "or": "||"}
 mulop_map = {"*": "*", "/": "/", "div": "/", "mod": "%", "and": "&&"}
 assignop_map = {":=": "="}
 uminus_map = {"-": "-"}
 
 
 def format_code(code: str) -> str:
     # clang-format命令
     command = ["clang-format", "-style=llvm"]
-
     # 启动子进程
     process = subprocess.Popen(
         command,
         stdin = subprocess.PIPE,
         stdout = subprocess.PIPE,
         stderr = subprocess.PIPE,
         text = True,
     )
-
     # 将代码写入stdin并获取格式化后的代码
     formatted_code, _ = process.communicate(code)
-
     return formatted_code
 
 
-def compile_code(code: str, input_ = None, compiler = "clang") -> str:
+def compile_code(code: str, input_ = None, compiler = "gcc") -> str:
     # 创建临时文件来存储代码
     with tempfile.NamedTemporaryFile(suffix = ".c", delete = False) as source_file:
         source_file.write(code.encode())  # 将字符串编码为字节对象
         source_file.flush()
         source_file_path = source_file.name
-
     # 编译代码
     executable_path = source_file_path[:-2]  # 去掉 .c 后缀
-    compile_command = [compiler, source_file_path, "-o", executable_path]
+    compile_command = [compiler, source_file_path, "-o", executable_path, "-lm"]
     compile_process = subprocess.run(
         compile_command,
         stdout = subprocess.PIPE,
         stderr = subprocess.PIPE,
         text = True,
     )
-
     if compile_process.returncode != 0:
         return f"Compilation failed:\n{compile_process.stderr}"
-
     # 运行代码
     run_command = [executable_path]
     run_process = subprocess.Popen(
         run_command,
         stdin = subprocess.PIPE,
         stdout = subprocess.PIPE,
         stderr = subprocess.PIPE,
         text = True,
     )
-
-    # 如果有输入，写入stdin
     if input_:
         stdout, stderr = run_process.communicate(input_)
     else:
         stdout, stderr = run_process.communicate()
-
     if run_process.returncode != 0:
         return f"Runtime error:\n{stderr}"
-
     return stdout
 
 
+class Status(Enum):
+    NORMAL = 0
+    SINGLE_QUOTE = 1
+    DOUBLE_QUOTE = 2
+    COMMENT = 3
+
+
 def preprocess(code: str) -> str:
     # 去除形如 {...} 的注释
     code_without_comments = re.sub(r"\{.*?}", "", code, flags = re.DOTALL)
-
     # 将代码转换成小写
     code_without_comments = code_without_comments.lower()
 
     return code_without_comments
 
 
 def postprocess(tokens: list) -> list:
@@ -140,18 +139,14 @@
         if flag:
             raise TypeError("Tokens must be strings")
         return result
 
     return wrapper
 
 
-import subprocess
-import tempfile
-
-
 def code_analyze(code: str) -> str:
     """
     使用 Clang Static Analyzer 对给定的 C 代码进行静态分析,
     返回分析结果的输出。
     """
     # 创建临时文件存储代码
     with tempfile.NamedTemporaryFile(mode = 'w', suffix = '.c', delete = False) as tmp_file:
```

### Comparing `mp2c-0.1.1/mp2c/visitors.py` & `mp2c-0.9.0/mp2c/visitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from lark.lark import Token
 
+from .context import FunctionSymbol
 from .utils import *
 
 
 def visit_empty(node: Tree, context: Context):
     tokens = []
     return tokens
 
@@ -35,15 +36,15 @@
     periods = []
     current_period = []
     for child in node.children:
         if isinstance(child, Token):
             current_period.append(int(child.value))
         elif child.data == "period":
             current_period = visit_period(child, context)
-            periods.append(current_period)
+            periods.extend(current_period)
             current_period = []
         else:
             raise Exception("Unknown period child data: {}".format(child.data))
     periods.append(current_period)
     return periods
 
 
@@ -98,98 +99,110 @@
         else:
             raise Exception("Unknown value_parameter child data: {}".format(child.data))
     return {"ids": ids, "type": type_}
 
 
 def visit_var_parameter(node: Tree, context: Context):
     value_parameter = visit_value_parameter(node.children[0], context)
-    tokens = construct_parameter_tokens(value_parameter, context)
+    tokens = construct_parameter_tokens(value_parameter, context, var = True)
+
     return tokens, value_parameter
 
 
-def construct_parameter_tokens(value_parameter, context):
+def construct_parameter_tokens(value_parameter, context, var = False):
     tokens = []
     first = True
     for id_ in value_parameter["ids"]:
         if first:
             first = False
         else:
             tokens.append(",")
         id_type = value_parameter["type"]
-        context.register_value(id_, id_type, True)
+        context.register_value(id_, id_type, True, var = var)
         tokens.append(id_type)
+        if var:
+            tokens.append("*")
         tokens.append(id_)
     return tokens
 
 
 def visit_parameter(node: Tree, context: Context):
     tokens = []
     parameter = None
+    var = False
     for child in node.children:
         if child.data == "var_parameter":
             tokens, parameter = visit_var_parameter(child, context)
+            var = True
         elif child.data == "value_parameter":
             parameter = visit_value_parameter(child, context)
             tokens = construct_parameter_tokens(parameter, context)
         else:
             raise Exception("Unknown parameter child data: {}".format(child.data))
-    return tokens, parameter
+    return tokens, parameter, var
 
 
 def visit_parameter_list(node: Tree, context: Context):
     tokens = []
     first = True
     parameter_list = []
+    is_var = []
     for child in node.children:
+        if child.data == "empty":
+            return tokens, parameter_list, is_var
         assert child.data == "parameter"
         if first:
             first = False
         else:
             tokens.append(",")
-        parameter_tokens, parameter = visit_parameter(child, context)
+        parameter_tokens, parameter, var = visit_parameter(child, context)
         tokens.extend(parameter_tokens)
         parameter_list.append(parameter)
-    return tokens, parameter_list
+        is_var.append(var)
+    return tokens, parameter_list, is_var
 
 
 def visit_formal_parameter(node: Tree, context: Context):
     tokens = ["("]
-    parameter_list_tokens, parameter_list = visit_parameter_list(node.children[0], context)
+    parameter_list_tokens, parameter_list, var_list = visit_parameter_list(node.children[0], context)
     tokens.extend(parameter_list_tokens)
     tokens.append(")")
-    return tokens, parameter_list
+    return tokens, parameter_list, var_list
 
 
 def visit_subprogram_head(node: Tree, context: Context):
     tokens = []
     basic_type = None
     id_ = None
     formal_parameter_tokens = None
     parameter_info_list = None
     parameter_list = []
+    var_list = []
     for child in node.children:
         if child.data == "basic_type":
             basic_type = visit_basic_type(child, context)
         elif child.data == "id":
             # subprogram_head中的id不需要考虑func_name修正
             id_ = visit_id(child, context, "")
         elif child.data == "formal_parameter":
-            formal_parameter_tokens, parameter_info_list = visit_formal_parameter(child, context)
+            formal_parameter_tokens, parameter_info_list, var_list = visit_formal_parameter(child, context)
         else:
             raise Exception("Unknown subprogram_head child data: {}".format(child.data))
     if basic_type:
         tokens.append(basic_type)
     else:
         tokens.append("void")
     tokens.append(id_)
     tokens.extend(formal_parameter_tokens)
+    is_reference = []
     for id_group in parameter_info_list:
         for _ in id_group["ids"]:
             parameter_list.append(id_group["type"])
-    context.register_func(id_, tokens, parameter_list)
+            is_reference.append(id_group["var"])
+    context.register_func(id_, tokens, parameter_list, is_reference)
     return tokens
 
 
 def visit_func_id(node):
     tokens = []
     for child in node.children:
         assert child.data == "id"
@@ -219,29 +232,32 @@
             # split expression_list by ','
             count = 0
             for expression_token in expression_list:
                 if expression_token == ",":
                     offset = array_symbol.dimensions[count][1]
                     tokens.extend(['-', str(offset)])
                     count += 1
-                tokens.append(expression_token)
+                    tokens.extend(["]", "["])
+                else:
+                    tokens.append(expression_token)
             offset = array_symbol.dimensions[count][1]
             tokens.extend(['-', str(offset)])
             count += 1
             tokens.append("]")
         else:
             raise Exception("Unknown id_varpart child data: {}".format(child.data))
     return tokens
 
 
 def visit_variable(node: Tree, context: Context, func_name: str):
     tokens = []
     isArray = False
     id_varpart = []
     id_token = None
+    var = False
     for child in node.children:
         if child.data == "id":
             id_token = visit_id(child, context, func_name)
         elif child.data == "id_varpart":
             id_varpart = visit_id_varpart(child, context, func_name, id_token)
             if len(id_varpart) > 0:
                 isArray = True
@@ -256,15 +272,20 @@
         variable_type = array.type
     else:
         value = context.get_value(id_token)
         if value is None:
             # raise Exception("Variable not declared: {}".format(id_token))
             error_message = "Variable not declared: {}".format(id_token)
             context.record_error(error_message)
-        variable_type = value.type
+            variable_type = ""
+        else:
+            variable_type = value.type
+            var = value.var
+    if var:
+        tokens.append("*")
     tokens.append(id_token)
     tokens.extend(id_varpart)
     return tokens, variable_type
 
 
 def visit_variable_list(node: Tree, context: Context, func_name: str):
     tokens = []
@@ -275,49 +296,74 @@
         else:
             tokens.append(",")
         variable_token, variable_type = visit_variable(child, context, func_name)
         tokens.extend(variable_token)
     return tokens
 
 
+def visit_expression_list_for_call(node: Tree, context: Context, func_name: str, function_to_call: FunctionSymbol):
+    tokens = []
+    first = True
+    count = 0
+    parameter_list = []
+    for id_group in function_to_call.parameter_list:
+        for _ in id_group["ids"]:
+            parameter_list.append(id_group["type"])
+    for child in node.children:
+        if first:
+            first = False
+        else:
+            tokens.append(",")
+        if function_to_call.var_parameter[count]:
+            tokens.append("&")
+        expression_tokens, expression_type = visit_expression(child, context, func_name)
+        try:
+            if expression_type != parameter_list[count]:
+                # raise Exception("Parameter types do not match")
+                error_message = "Parameter types do not match: expected {}, got {}".format(
+                    function_to_call.parameter_list[count], expression_type)
+                context.record_error(error_message)
+        except Exception as e:
+            error_message = str(e)
+            context.record_error(error_message)
+        tokens.extend(expression_tokens)
+        count += 1
+    if count != len(function_to_call.var_parameter):
+        # raise Exception("Number of parameters does not match")
+        error_message = "Number of parameters does not match: expected {}, got {}".format(
+            len(function_to_call.var_parameter), count)
+        context.record_error(error_message)
+    return tokens
+
+
 def visit_function_call(node: Tree, context: Context, func_name: str):
     tokens = []
     function_type = None
     function = None
     function_name = None
     for child in node.children:
         if child.data == "func_id":
             function_token = visit_func_id(child)
             function_name = function_token[0]
             function = context.get_func(function_name)
             if function is None:
-                # raise Exception("Function not declared: {}".format(function_name))
                 error_message = "Function not declared: {}".format(function_name)
                 context.record_error(error_message)
-            function_type = function.header[0]
+                function_type = ""
+            else:
+                function_type = function.header[0]
             tokens.extend(function_token)
-        elif child.data == "expression_list":
             tokens.append("(")
-            expression_list_tokens, expression_types = visit_expression_list(child, context, func_name)
-            # check if the number of parameters is correct
-            if len(expression_types) != len(function.parameter_list):
-                # raise Exception("Number of parameters does not match")
-                error_message = "Number of parameters while calling function {} does not match:".format(function_name)
-                error_message += " expected {}, got {}".format(len(function.parameter_list), len(expression_types))
-                context.record_error(error_message)
-            if expression_types != function.parameter_list:
-                # raise Exception("Parameter types do not match")
-                error_message = "Parameter types while calling function {} do not match:".format(function_name)
-                error_message += " expected {}, got {}".format(function.parameter_list, expression_types)
-                context.record_error(error_message)
+        elif child.data == "expression_list":
+            expression_list_tokens = visit_expression_list_for_call(child, context, func_name,
+                                                                    function)
             tokens.extend(expression_list_tokens)
-            tokens.append(")")
         else:
             raise Exception("Unknown procedure_call child data: {}".format(child.data))
-
+    tokens.append(")")
     return tokens, function_type
 
 
 def visit_factor(node: Tree, context: Context, func_name: str):
     tokens = []
     factor_type = None
     for child in node.children:
@@ -350,26 +396,32 @@
             raise Exception("Unknown factor child data: {}".format(child.data))
     return tokens, factor_type
 
 
 def visit_term(node: Tree, context: Context, func_name: str):
     term_type = None
     tokens = []
+    operator = None
     for child in node.children:
         if isinstance(child, Token):
             tokens.append(mulop_map[child.value])
+            operator = child.value
+            if operator == "/":
+                tokens[:0] = ["(", "float", ")"]
         elif child.data == "factor":
             factor_token, factor_type = visit_factor(child, context, func_name)
             tokens.extend(factor_token)
             term_type = factor_type
         elif child.data == "term":
             term_token, term_type = visit_term(child, context, func_name)
             tokens.extend(term_token)
         else:
             raise Exception("Unknown term child data: {}".format(child.data))
+        if operator == "/":
+            term_type = "float"
     return tokens, term_type
 
 
 def visit_simple_expression(node: Tree, context: Context, func_name: str):
     tokens = []
     simple_expression_type = None
     for child in node.children:
@@ -396,24 +448,30 @@
     for child in node.children:
         if isinstance(child, Token):
             tokens.append(relop_map[child.value])
             isBool = True
         elif child.data == "simple_expression":
             simple_expression_token, simple_expression_type = visit_simple_expression(child, context, func_name)
             tokens.extend(simple_expression_token)
+        elif child.data == "char_literal":
+            tokens.append(child.children[0].value)
+            simple_expression_type = "char"
+        elif child.data == "string_literal":
+            tokens.append(child.children[0].value)
+            simple_expression_type = "char*"
         else:
             raise Exception("Unknown expression child data: {}".format(child.data))
     if isBool:
         expression_type = "bool"
     else:
         expression_type = simple_expression_type
     return tokens, expression_type
 
 
-def visit_expression_list(node: Tree, context: Context, func_name: str):
+def visit_expression_list(node: Tree, context: Context, func_name: str, is_call = False):
     tokens = []
     first = True
     expression_types = []
     for child in node.children:
         if first:
             first = False
         else:
@@ -440,19 +498,19 @@
             variable_tokens, variable_type = visit_variable(child, context, func_name)
             tokens.extend(variable_tokens)
         else:
             raise Exception(
                 "Unknown assignment_statement child data: {}".format(child.data)
             )
     if variable_type != expression_type:
-        raise Exception("Type mismatch in assignment: {},{} != {}, {}".
-                        format("".join(variable_tokens),
-                               variable_type,
-                               "".join(expression_tokens),
-                               expression_type))
+        error_message = "Type mismatch in assignment: {},{} != {}, {}".format(
+            "".join(variable_tokens), variable_type, "".join(expression_tokens), expression_type
+        )
+        context.record_error(error_message)
+
     return tokens
 
 
 def visit_if_else_statement(node: Tree, context: Context, func_name: str):
     tokens = []
     for child in node.children:
         if child.data == "expression":
@@ -490,46 +548,46 @@
         else:
             raise Exception("Unknown else_part child data: {}".format(child.data))
     return tokens
 
 
 def construct_read_params(node: Tree, context: Context, func_name: str):
     tokens = []
-    ids = []
     types = []
+    expressions = []
     for child in node.children:
         if child.data == "expression":
             expression_tokens, expression_type = visit_expression(child, context, func_name)
-            assert len(expression_tokens) == 1
-            id_ = expression_tokens[0]
-            ids.append(id_)
-            value = context.get_value(id_)
-            if value is None:
-                raise Exception("Variable not declared: {}".format(id_))
-            types.append(value.type)
+            expressions.append(expression_tokens)
+            types.append(expression_type)
         else:
             raise Exception("Unknown read_params child data: {}".format(child.data))
-    format_ = types_to_format(types)
+    format_ = types_to_format(types, context)
     tokens.append(format_)
-    for id_ in ids:
+    for expression in expressions:
         tokens.append(",")
         tokens.append("&")
-        tokens.append(id_)
+        tokens.extend(expression)
     return tokens
 
 
-def types_to_format(types, line = False):
+def types_to_format(types, context, line = False):
     format_ = '"'
     for id_type in types:
         if id_type == "int":
             format_ += r"%d"
         elif id_type == "float":
             format_ += r"%f"
         elif id_type == "char":
             format_ += r"%c"
+        elif id_type == "":
+            error_message = "Variable not declared"
+            context.record_error(error_message)
+        elif id_type == "char*":
+            format_ += r"%s"
         else:
             raise Exception("Unknown type: {}".format(id_type))
     if line:
         format_ += r"\n"
     format_ += '"'
     return format_
 
@@ -541,20 +599,21 @@
     for child in node.children:
         if child.data == "expression":
             expression_token, expression_type = visit_expression(child, context, func_name)
             expressions.append(expression_token)
             types.append(expression_type)
         else:
             raise Exception("Unknown write_params child data: {}".format(child.data))
-    format_ = types_to_format(types, line)
+    format_ = types_to_format(types, context, line)
     tokens.append(format_)
     for expression in expressions:
         tokens.append(",")
         tokens.extend(expression)
-
+    if len(tokens) == 0:
+        tokens.append('""')
     return tokens
 
 
 def visit_procedure_call(node: Tree, context: Context, func_name: str):
     tokens = []
     isRead = False
     isWrite = False
@@ -588,40 +647,43 @@
                     child, context, func_name
                 )
             elif isWriteLn:
                 expression_list_tokens = construct_write_params(
                     child, context, func_name, True
                 )
             else:
-                expression_list_tokens, expression_types = visit_expression_list(
-                    child, context, func_name
+                expression_list_tokens = visit_expression_list_for_call(
+                    child, context, func_name, context.get_func(procedure_name)
                 )
-                function = context.get_func(procedure_name)
-                if function is None:
-                    raise Exception("Procedure not declared: {}".format(procedure_name))
-                if len(expression_types) != len(function.parameter_list):
-                    raise Exception("Number of parameters does not match")
-                if expression_types != function.parameter_list:
-                    raise Exception("Parameter types do not match")
+
             tokens.extend(expression_list_tokens)
             tokens.append(")")
         else:
             raise Exception("Unknown procedure_call child data: {}".format(child.data))
     if not flag:
-        tokens.extend(["(", ")"])
+        tokens.append("(")
+        if isWriteLn:
+            tokens.append(r'"\n"')
+        elif isWrite:
+            tokens.append('""')
+        tokens.append(")")
     return tokens
 
 
 def visit_statement_list(node: Tree, context: Context, func_name: str):
     tokens = []
     for child in node.children:
-        assert child.data == "statement"
-        statement_tokens = visit_statement(child, context, func_name)
-        tokens.extend(statement_tokens)
-        tokens.append(";")
+        if child.data == "statement":
+            statement_tokens = visit_statement(child, context, func_name)
+            tokens.extend(statement_tokens)
+        elif child.data == "statement_list":
+            statement_list_tokens = visit_statement_list(child, context, func_name)
+            tokens.extend(statement_list_tokens)
+        else:
+            raise Exception("Unknown statement_list child data: {}".format(child.data))
     return tokens
 
 
 def visit_compound_statement(node: Tree, context: Context, func_name: str):
     tokens = []
     assert node.children[0].data == "statement_list"
     statement_list_tokens = visit_statement_list(node.children[0], context, func_name)
@@ -631,18 +693,21 @@
 
 def visit_for_statement(node: Tree, context: Context, func_name: str):
     tokens = []
     id_token = []
     from_tokens = []
     to_tokens = []
     statement_tokens = []
+    down_to = False
     first = True
     for child in node.children:
         if isinstance(child, Token):
-            if child.type != "ASSIGNOP":
+            if child.type == "DOWN":
+                down_to = True
+            elif child.type != "ASSIGNOP":
                 raise Exception("Unknown for_statement child type: {}".format(child.type))
         elif child.data == "id":
             context.enter_scope()
             id_token = visit_id(child, context, func_name)
             context.register_value(id_token, "int", True)
         elif child.data == "expression":
             if first:
@@ -660,15 +725,19 @@
     tokens.extend(from_tokens)
     tokens.append(";")
     tokens.extend(id_token)
     tokens.append("<=")
     tokens.extend(to_tokens)
     tokens.append(";")
     tokens.extend(id_token)
-    tokens.extend(["++", ")"])
+    if down_to:
+        tokens.append("--")
+    else:
+        tokens.append("++")
+    tokens.append(")")
     tokens.append("{")
     tokens.extend(statement_tokens)
     tokens.append("}")
     context.exit_scope()
     return tokens
 
 
@@ -767,15 +836,14 @@
             )  # [123.456, "float"] 或 ["test", "char*"] ...
             tokens.append(res[1])
             tokens.append(const_id)
             tokens.append("=")
             tokens.extend(res[0])
             tokens.append(";")
             # 符号表注册
-            # type = context.cname_to_type(res[1])
             context.register_value(const_id, res[1], False, res[0])
         elif child.data == "const_declaration":
             tokens.extend(visit_const_declaration(child, context))
         else:
             raise Exception(
                 "Unknown const_declaration child data: {}".format(child.data)
             )
@@ -801,24 +869,26 @@
     id_lists = []
     id_types = []
     for child in node.children:
         if child.data == "idlist":
             id_lists.append(visit_idlist(child, context))
         elif child.data == "type":
             id_types.append(visit_type(child, context))
+        elif child.data == "var_declaration":
+            tokens.extend(visit_var_declaration(child, context))
         else:
             raise Exception("Unknown var_declaration child data: {}".format(child.data))
     for id_list, id_type in zip(id_lists, id_types):
         for id_ in id_list:
             tokens.append(id_type["basic_type"])
             tokens.append(id_)
             if id_type["is_array"]:
                 for period in id_type["period"]:
                     tokens.append("[")
-                    tokens.append(str(period[0]))
+                    tokens.append(str(period[1] - period[0] + 1))
                     tokens.append("]")
                 context.register_array(id_, id_type["basic_type"], id_type["period"])
             else:
                 context.register_value(id_, id_type["basic_type"], True)
             tokens.append(";")
 
     return tokens
@@ -835,34 +905,19 @@
             raise Exception(
                 "Unknown var_declarations child data: {}".format(child.data)
             )
     return tokens
 
 
 def visit_program_head(node: Tree, context: Context):
-    # tokens = []
-    # for child in node.children:
-    #     if child.data == "id":
-    #         id_tokens = visit_id(child,context)
-    #         tokens.extend(id_tokens)
-    #         tokens.append(";\n")
-    #     elif child.data == "idlist":
-    #         tokens.append("int ")
-    #         idlist_tokens = visit_idlist(child,context)
-
-    #         tokens.append(";")
-    #     else:
-    #         raise Exception("Unknown program_head child data: {}".format(child.data))
-    tokens = ['#include "stdio.h"']
+    tokens = ['#include <stdio.h>', '#include <math.h>']
     return tokens
 
 
-def visit_subprogram_body(node: Tree, context: Context, subprogram_head_tokens: list[str]):
-    func_name = subprogram_head_tokens[1]
-    ret_type = subprogram_head_tokens[0]
+def visit_subprogram_body(node: Tree, context: Context, func_name: str, ret_type: str):
     if ret_type != "void":
         context.register_value("_" + func_name, ret_type, True)
     tokens = []
     for child in node.children:
         if child.data == "const_declarations":
             tokens.extend(visit_const_declarations(child, context))
         elif child.data == "var_declarations":
@@ -871,50 +926,112 @@
             # compound_statement中如果遇到对func_name符号的引用且并非函数递归调用，则前面加一个_
             tokens.extend(visit_compound_statement(child, context, func_name))
         else:
             raise Exception("Unknown subprogram_body child data: {}".format(child.data))
     return tokens
 
 
+def visit_function_declaration(child, context):
+    # "function" id formal_parameter ":" basic_type  subprogram_body
+    head_tokens = []
+    function_name = ""
+    formal_parameter_tokens = []
+    parameter_info_list = []
+    var_list = []
+    basic_type = None
+    body_tokens = ["{"]
+    subprogram_body_tokens = []
+    for child in child.children:
+        if child.data == "id":
+            function_name = visit_id(child, context, "")
+        elif child.data == "formal_parameter":
+            formal_parameter_tokens, parameter_info_list, is_vars = visit_formal_parameter(child, context)
+            for id_group, var in zip(parameter_info_list, is_vars):
+                for _ in id_group["ids"]:
+                    var_list.append(var)
+        elif child.data == "basic_type":
+            basic_type = visit_basic_type(child, context)
+        elif child.data == "subprogram_body":
+            head_tokens.append(basic_type)
+            head_tokens.append(function_name)
+            head_tokens.extend(formal_parameter_tokens)
+            context.register_func(function_name, head_tokens, parameter_info_list, var_list, body_tokens)
+            context.enter_scope()
+            subprogram_body_tokens = visit_subprogram_body(child, context, function_name, basic_type)
+            context.exit_scope()
+        else:
+            raise Exception("Unknown function_declaration child data: {}".format(child.data))
+    body_tokens.append(basic_type)
+    body_tokens.append("_" + function_name)
+    body_tokens.append(";")
+    body_tokens.extend(subprogram_body_tokens)
+    body_tokens.append("return")
+    body_tokens.append("_" + function_name)
+    body_tokens.append(";")
+    body_tokens.append("}")
+    context.register_func(function_name, head_tokens, parameter_info_list, var_list, body_tokens)
+    return head_tokens
+
+
+def visit_procedure_declaration(child, context):
+    head_tokens = []
+    procedure_name = ""
+    formal_parameter_tokens = []
+    parameter_info_list = []
+    body_tokens = ["{"]
+    subprogram_body_tokens = []
+    var_list = []
+    for child in child.children:
+        if child.data == "id":
+            procedure_name = visit_id(child, context, "")
+        elif child.data == "formal_parameter":
+            formal_parameter_tokens, parameter_info_list, var_list = visit_formal_parameter(child, context)
+            for id_group, var in zip(parameter_info_list, var_list):
+                for _ in id_group["ids"]:
+                    var_list.append(var)
+        elif child.data == "subprogram_body":
+            head_tokens.append("void")
+            head_tokens.append(procedure_name)
+            head_tokens.extend(formal_parameter_tokens)
+            context.register_func(procedure_name, head_tokens, parameter_info_list, var_list, body_tokens)
+            context.enter_scope()
+            subprogram_body_tokens = visit_subprogram_body(child, context, procedure_name, "void")
+            context.exit_scope()
+        else:
+            raise Exception("Unknown procedure_declaration child data: {}".format(child.data))
+    body_tokens.extend(subprogram_body_tokens)
+    body_tokens.append("}")
+    context.register_func(procedure_name, head_tokens, parameter_info_list, var_list, body_tokens)
+    return head_tokens
+
+
 def visit_subprogram(node: Tree, context: Context):
-    context.enter_scope()
     tokens = []
-    subprogram_head_tokens = []
-    subprogram_body_tokens = []
     for child in node.children:
-        if child.data == "subprogram_head":
-            subprogram_head_tokens = visit_subprogram_head(child, context)
-        elif child.data == "subprogram_body":
-            subprogram_body_tokens = visit_subprogram_body(
-                child, context, subprogram_head_tokens
-            )
+        if child.data == "function_declaration":
+            function_declaration_tokens = visit_function_declaration(child, context)
+            tokens.extend(function_declaration_tokens)
+        elif child.data == "procedure_declaration":
+            procedure_declaration_tokens = visit_procedure_declaration(child, context)
+            tokens.extend(procedure_declaration_tokens)
         else:
             raise Exception("Unknown subprogram child data: {}".format(child.data))
-    ret_type = subprogram_head_tokens[0]
-    function_name = subprogram_head_tokens[1]
-    function_header = subprogram_head_tokens
-    function_tokens = ["{"]
-    if ret_type != "void":
-        function_tokens.extend([ret_type, "_" + function_name, ";"])
-    function_tokens.extend(subprogram_body_tokens)
-    if ret_type != "void":
-        function_tokens.append("return")
-        function_tokens.append("_" + function_name)
-        function_tokens.append(";")
-    function_tokens.append("}")
-    context.declare_func(function_name, function_tokens)
-    context.exit_scope()
-    return tokens
+    tokens.append(";")
+    return []
 
 
 def visit_subprogram_declarations(node: Tree, context: Context):
     tokens = []
     for child in node.children:
         if child.data == "subprogram":
             tokens.extend(visit_subprogram(child, context))
+        elif child.data == "empty":
+            return tokens
+        elif child.data == "subprogram_declarations":
+            tokens.extend(visit_subprogram_declarations(child, context))
         else:
             raise Exception(
                 "Unknown subprogram_declarations child data: {}".format(child.data)
             )
     return tokens
 
 
@@ -934,31 +1051,35 @@
             tokens.append("}")
         else:
             raise Exception("Unknown program_body child data: {}".format(child.data))
     return tokens
 
 
 def visit_programstruct(node: Tree, context: Context):
-    # 进入全局作用域
     context.enter_scope()
     tokens = []
     program_head_tokens = []
     program_body_tokens = []
+    context.declare_library_functions()
     for child in node.children:
         if child.data == "program_head":
             program_head_tokens = visit_program_head(child, context)
         elif child.data == "program_body":
             program_body_tokens = visit_program_body(child, context)
         else:
             raise Exception("Unknown programstruct child data: {}".format(child.data))
     tokens.extend(program_head_tokens)
     functions = context.get_funcs()
     for function in functions:
+        if functions[function].is_library:
+            continue
         tokens.extend(functions[function].header)
         tokens.append(";")
     tokens.extend(program_body_tokens)
     for function in functions:
+        if functions[function].is_library:
+            continue
         tokens.extend(functions[function].header)
         tokens.extend(functions[function].tokens)
     context.exit_scope()
 
     return tokens
```

### Comparing `mp2c-0.1.1/test/test_control.py` & `mp2c-0.9.0/test/test_lexical.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,111 @@
+import pytest
+
 from mp2c import Converter, compile_code
 
 
-class TestControl:
-    def test_if_else_simple(self):
-        control_test_code = r"""
-        program IfElseTest;
+class TestLexical:
+    def test_lexical_identifier(self):
+        identifier_test_code = r"""
+        program IdentifierTest(input, output);
         var
-            a, b: INTEGER;
+          a, b2, _temp, MyVariable: integer;
         begin
-            a := 10;
-            b := 20;
-            if a > b then
-                write(a)
-            else
-                write(b);
+          { 测试合法和非法标识符 }
         end.
         """
         converter = Converter()
-        success, result = converter(control_test_code, debug = True)
+        success, result = converter(identifier_test_code, debug = True)
         output = compile_code(result)
-        assert output == "20"
+        assert output == ""
 
-    def test_if_else_nested(self):
-        control_test_code = r"""
-        program IfElseNested;
+    def test_lexical_keyword(self):
+        keyword_test_code = r"""
+        program KeywordTest;
+        const
+          Pi = 3.14;
+          p = 'p';
+          z = 'z';
         var
-            a, b: integer;
+          x: real;
+
         begin
-            a := 10;
-            b := 20;
-            if a > b then
-                write(a)
-            else
-                if a < b then
-                    write(b)
-                else
-                    write(0);
+          x := Pi;
+          if x > 0 then
+            write(p)
+          else
+            write(z);
         end.
         """
         converter = Converter()
-        success, result = converter(control_test_code, debug = True)
+        success, result = converter(keyword_test_code, debug = True)
         output = compile_code(result)
-        assert output == "20"
+        assert output == "p"
 
-    def test_for_loop(self):
-        control_test_code = r"""
-        program ForLoopTest;
+    def test_lexical_number(self):
+        number_test_code = r"""
+        program NumberTest;
+        const
+          A = 123;
+          B = -456;
+          C = 3.14;
+          D = -0.618;
+        begin
+          write(A, B, C, D);
+        end.
+        """
+        converter = Converter()
+        success, result = converter(number_test_code, debug = True)
+        output = compile_code(result)
+        assert output == "123-4563.140000-0.618000"
+
+    def test_lexical_char(self):
+        char_test_code = r"""
+        program CharTest;
+        const
+            c1 = 'a';
+            c2 = '''';
+        begin
+          write(c1, c2);
+        end.
+        """
+        converter = Converter()
+        with pytest.raises(Exception):
+            success, result = converter(char_test_code, debug = True)
+
+    def test_lexical_operator(self):
+        operator_test_code = r"""
+        program OperatorTest;
         var
-            i: integer;
+          a, b: integer;
         begin
-            for i := 1 to 10 do
-                write(i);
+          a := 10;
+          b := 3;
+          writeln(a + b);
+          writeln(a - b);
+          writeln(a * b);
+          writeln(a / b);
+          writeln(a div b);
+          writeln(a mod b);
         end.
         """
         converter = Converter()
-        success, result = converter(control_test_code, debug = True)
-        print(result)
+        success, result = converter(operator_test_code, debug = True)
         output = compile_code(result)
+        assert output == "13\n7\n30\n3.333333\n3\n1\n"
+
+    def test_lexical_comment(self):
+        comment_test_code = r"""
+        program CommentTest;
+        { 这是一个程序注释 }
+
+        var
+          x: integer; { 这是一个变量注释 }
 
-        assert output == "12345678910"
+        begin
+          x := 42; { 计算 }
+        end.
+        """
+        converter = Converter()
+        success, result = converter(comment_test_code, debug = True)
+        output = compile_code(result)
+        assert output == ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mp2c-0.1.1/test/test_gcd.py` & `mp2c-0.9.0/test/test_scope.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,56 @@
 from mp2c import Converter, compile_code
 
 
-class TestGCD:
-    def test_gcd(self):
-        gcd_test_code = r"""
-        program example(input, output);
-
-        var
-          x, y: integer;
-        
-        function gcd(a, b: integer): integer;
-        begin
-          if b = 0 then
-            gcd := a
-          else
-            gcd := gcd(b, a mod b);
-        end;
-        
-        begin
-          read(x, y);
-          writeln(gcd(x, y));
-        end.
-        """
-        converter = Converter()
-        success, result = converter(gcd_test_code, debug = True)
-        print(result)
-        output = compile_code(result, "6 9\n")
-        assert output == "3\n"
+def test_scope_success():
+    scope_test_code2 = r"""
+    program ScopeDemo;
+
+    var
+      A: integer;
+
+    procedure ScopeInner;
+    var
+      A: integer;
+    begin
+      A := 10;
+      write(A);
+    end;
+
+    begin
+      A := 20;
+      write(A);
+      ScopeInner;
+      write(A);
+    end.
+    """
+    converter = Converter()
+    success, result = converter(scope_test_code2, debug = True)
+    output = compile_code(result)
+    assert output == "201020"
+
+
+def test_scope_failure():
+    scope_test_code = r"""
+    program VariableScope;
+
+    var
+      globalVar: integer;
+
+    procedure LocalScope;
+    var
+      localVar: integer;
+    begin
+      globalVar := 10;
+      localVar := 20;
+    end;
+
+    begin
+      globalVar := 5;
+      LocalScope;
+      write(globalVar);  { Output: 10 }
+      write(localVar);   { Compilation error: localVar not defined in this scope }
+    end.
+    """
+    converter = Converter()
+    success, result = converter(scope_test_code)
+    assert not success
```

