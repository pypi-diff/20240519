# Comparing `tmp/gpt_pydantic_tools-0.1.tar.gz` & `tmp/gpt_pydantic_tools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_pydantic_tools-0.1.tar", last modified: Wed May  1 08:17:21 2024, max compression
+gzip compressed data, was "gpt_pydantic_tools-0.2.tar", last modified: Sun May 19 17:41:17 2024, max compression
```

## Comparing `gpt_pydantic_tools-0.1.tar` & `gpt_pydantic_tools-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-01 08:17:21.685850 gpt_pydantic_tools-0.1/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1076 2024-05-01 07:44:59.000000 gpt_pydantic_tools-0.1/LICENSE
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2469 2024-05-01 08:17:21.685850 gpt_pydantic_tools-0.1/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1742 2024-05-01 08:12:09.000000 gpt_pydantic_tools-0.1/README.md
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-01 08:17:21.682516 gpt_pydantic_tools-0.1/gpt_pydantic_tools/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     4507 2024-05-01 07:56:31.000000 gpt_pydantic_tools-0.1/gpt_pydantic_tools/__init__.py
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-01 08:17:21.685850 gpt_pydantic_tools-0.1/gpt_pydantic_tools.egg-info/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2469 2024-05-01 08:17:21.000000 gpt_pydantic_tools-0.1/gpt_pydantic_tools.egg-info/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)      272 2024-05-01 08:17:21.000000 gpt_pydantic_tools-0.1/gpt_pydantic_tools.egg-info/SOURCES.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-01 08:17:21.000000 gpt_pydantic_tools-0.1/gpt_pydantic_tools.egg-info/dependency_links.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       69 2024-05-01 08:17:21.000000 gpt_pydantic_tools-0.1/gpt_pydantic_tools.egg-info/requires.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       19 2024-05-01 08:17:21.000000 gpt_pydantic_tools-0.1/gpt_pydantic_tools.egg-info/top_level.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)      890 2024-05-01 08:05:41.000000 gpt_pydantic_tools-0.1/pyproject.toml
--rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-01 08:17:21.685850 gpt_pydantic_tools-0.1/setup.cfg
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-19 17:41:17.295291 gpt_pydantic_tools-0.2/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1076 2024-05-01 07:44:59.000000 gpt_pydantic_tools-0.2/LICENSE
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2670 2024-05-19 17:41:17.295291 gpt_pydantic_tools-0.2/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1943 2024-05-19 17:40:34.000000 gpt_pydantic_tools-0.2/README.md
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-19 17:41:17.291958 gpt_pydantic_tools-0.2/gpt_pydantic_tools/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     5149 2024-05-19 17:36:51.000000 gpt_pydantic_tools-0.2/gpt_pydantic_tools/__init__.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-19 17:41:17.295291 gpt_pydantic_tools-0.2/gpt_pydantic_tools.egg-info/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2670 2024-05-19 17:41:17.000000 gpt_pydantic_tools-0.2/gpt_pydantic_tools.egg-info/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      272 2024-05-19 17:41:17.000000 gpt_pydantic_tools-0.2/gpt_pydantic_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-19 17:41:17.000000 gpt_pydantic_tools-0.2/gpt_pydantic_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       69 2024-05-19 17:41:17.000000 gpt_pydantic_tools-0.2/gpt_pydantic_tools.egg-info/requires.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       19 2024-05-19 17:41:17.000000 gpt_pydantic_tools-0.2/gpt_pydantic_tools.egg-info/top_level.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      890 2024-05-19 17:37:26.000000 gpt_pydantic_tools-0.2/pyproject.toml
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-19 17:41:17.298623 gpt_pydantic_tools-0.2/setup.cfg
```

### Comparing `gpt_pydantic_tools-0.1/LICENSE` & `gpt_pydantic_tools-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_pydantic_tools-0.1/PKG-INFO` & `gpt_pydantic_tools-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_pydantic_tools
-Version: 0.1
+Version: 0.2
 Summary: Define GPT tool schemas using Pydantic.
 Author-email: "Carlos A. Planchón" <carlosandresplanchonprestes@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/carlosplanchon/gpt_pydantic_tools.git
 Keywords: gpt,ai,tool,schemas,pydantic,json
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -52,14 +52,19 @@
 schema_manager = ToolSchemaManager(pydantic_obj=MyModel)
 tool_schema = schema_manager.tools_schema
 
 # Determine tool invocation strategy
 tool_choice = get_tool_choice_dict(ToolChoiceEnum.AUTO, schema_manager)
 ```
 
+If you want to do the Pydantic Schema conversion yourself, and directly provide the JSON instead, you can do:
+```
+schema_manager = ToolSchemaManager(pydantic_obj_json_schema=my_model_json_schema)
+```
+
 ## Contributing
 
 Contributions are welcome! Please feel free to submit pull requests, create issues, and suggest improvements to the repository.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `gpt_pydantic_tools-0.1/README.md` & `gpt_pydantic_tools-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 schema_manager = ToolSchemaManager(pydantic_obj=MyModel)
 tool_schema = schema_manager.tools_schema
 
 # Determine tool invocation strategy
 tool_choice = get_tool_choice_dict(ToolChoiceEnum.AUTO, schema_manager)
 ```
 
+If you want to do the Pydantic Schema conversion yourself, and directly provide the JSON instead, you can do:
+```
+schema_manager = ToolSchemaManager(pydantic_obj_json_schema=my_model_json_schema)
+```
+
 ## Contributing
 
 Contributions are welcome! Please feel free to submit pull requests, create issues, and suggest improvements to the repository.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `gpt_pydantic_tools-0.1/gpt_pydantic_tools/__init__.py` & `gpt_pydantic_tools-0.2/gpt_pydantic_tools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 without it being considered a breaking change.
 """
 from pydantic._internal._model_construction import ModelMetaclass
 
 from enum import StrEnum
 
 from typing import Any
+from typing import Optional
 
 
 def remove_key_from_dict(
     dict_obj: dict[str, Any],
     key_to_remove: str
         ) -> dict[str, Any]:
     """
@@ -52,18 +53,29 @@
 #   --- PYDANTIC OBJ TO TOOL SCHEMA ---   #
 #                                         #
 ###########################################
 ToolsSchemaT = list[dict[str, Any]]
 
 
 def pydantic_obj_to_tool_schema(
-    pydantic_obj: BaseModel,
+    pydantic_obj: BaseModel | None = None,
+    pydantic_obj_json_schema: dict[Any, Any] | None = None,
     description: str = None
         ) -> ToolsSchemaT:
-    json_data = pydantic_obj.schema()
+
+    if pydantic_obj is None and pydantic_obj_json_schema is None:
+        raise ValueError(
+            "You need to provide either pydantic_obj "
+            "or pydantic_obj_json_schema"
+        )
+
+    if pydantic_obj is not None:
+        json_data = pydantic_obj.schema()
+    else:
+        json_data = pydantic_obj_json_schema
 
     func_name: str = json_data["title"]
 
     gpt_function_dict = remove_key_from_dict(
         dict_obj=json_data,
         key_to_remove="title"
     )
@@ -86,15 +98,22 @@
         }
     ]
     return tools_schema
 
 
 @attrs.define()
 class ToolSchemaManager:
-    pydantic_obj: ModelMetaclass = attrs.field(validator=type_validator())
+    pydantic_obj: Optional[ModelMetaclass] = attrs.field(
+        validator=type_validator(),
+        default=None
+    )
+    pydantic_obj_json_schema: Optional[dict[Any, Any]] = attrs.field(
+        validator=type_validator(),
+        default=None
+    )
 
     tools_schema: ToolsSchemaT = attrs.field(
         validator=type_validator(),
         init=False
     )
 
     tool_name: str = attrs.field(
@@ -106,14 +125,15 @@
         validator=type_validator(),
         default=""
     )
 
     def __attrs_post_init__(self):
         self.tools_schema = pydantic_obj_to_tool_schema(
             pydantic_obj=self.pydantic_obj,
+            pydantic_obj_json_schema=self.pydantic_obj_json_schema,
             description=self.description
         )
 
         self.tool_name = self.tools_schema[0]["function"]["name"]
 
     def validate_tool_answer(
         self,
```

### Comparing `gpt_pydantic_tools-0.1/gpt_pydantic_tools.egg-info/PKG-INFO` & `gpt_pydantic_tools-0.2/gpt_pydantic_tools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_pydantic_tools
-Version: 0.1
+Version: 0.2
 Summary: Define GPT tool schemas using Pydantic.
 Author-email: "Carlos A. Planchón" <carlosandresplanchonprestes@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/carlosplanchon/gpt_pydantic_tools.git
 Keywords: gpt,ai,tool,schemas,pydantic,json
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -52,14 +52,19 @@
 schema_manager = ToolSchemaManager(pydantic_obj=MyModel)
 tool_schema = schema_manager.tools_schema
 
 # Determine tool invocation strategy
 tool_choice = get_tool_choice_dict(ToolChoiceEnum.AUTO, schema_manager)
 ```
 
+If you want to do the Pydantic Schema conversion yourself, and directly provide the JSON instead, you can do:
+```
+schema_manager = ToolSchemaManager(pydantic_obj_json_schema=my_model_json_schema)
+```
+
 ## Contributing
 
 Contributions are welcome! Please feel free to submit pull requests, create issues, and suggest improvements to the repository.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `gpt_pydantic_tools-0.1/pyproject.toml` & `gpt_pydantic_tools-0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [options]
 package_dir = "gpt_pydantic_tools"
 packages = ["gpt_pydantic_tools"]
 
 [project]
 name = "gpt_pydantic_tools"
-version = "0.1"
+version = "0.2"
 authors = [
     {name = "Carlos A. Planchón", email = "carlosandresplanchonprestes@gmail.com"}
 ]
 description = "Define GPT tool schemas using Pydantic."
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
```

