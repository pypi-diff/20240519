# Comparing `tmp/model_explorer_onnx-0.1.7.tar.gz` & `tmp/model_explorer_onnx-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.1.7.tar", last modified: Sat May 18 16:41:25 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.1.8.tar", last modified: Sat May 18 18:16:55 2024, max compression
```

## Comparing `model_explorer_onnx-0.1.7.tar` & `model_explorer_onnx-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:41:25.833750 model_explorer_onnx-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 16:41:22.000000 model_explorer_onnx-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 16:41:25.829749 model_explorer_onnx-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-18 16:41:22.000000 model_explorer_onnx-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 16:41:22.000000 model_explorer_onnx-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:41:25.833750 model_explorer_onnx-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:41:25.829749 model_explorer_onnx-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:41:25.829749 model_explorer_onnx-0.1.7/src/model_explorer_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-05-18 16:41:22.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:41:25.829749 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 16:41:25.000000 model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:16:55.835657 model_explorer_onnx-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 18:16:52.000000 model_explorer_onnx-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 18:16:55.835657 model_explorer_onnx-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-18 18:16:52.000000 model_explorer_onnx-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 18:16:52.000000 model_explorer_onnx-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 18:16:55.835657 model_explorer_onnx-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:16:55.831657 model_explorer_onnx-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:16:55.831657 model_explorer_onnx-0.1.8/src/model_explorer_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)    19020 2024-05-18 18:16:52.000000 model_explorer_onnx-0.1.8/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:16:55.835657 model_explorer_onnx-0.1.8/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 18:16:55.000000 model_explorer_onnx-0.1.8/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-18 18:16:55.000000 model_explorer_onnx-0.1.8/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 18:16:55.000000 model_explorer_onnx-0.1.8/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 18:16:55.000000 model_explorer_onnx-0.1.8/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 18:16:55.000000 model_explorer_onnx-0.1.8/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.1.7/LICENSE` & `model_explorer_onnx-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.7/PKG-INFO` & `model_explorer_onnx-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.7
+Version: 0.1.8
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `model_explorer_onnx-0.1.7/README.md` & `model_explorer_onnx-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.1.7/pyproject.toml` & `model_explorer_onnx-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.1.7"
+version = "0.1.8"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `model_explorer_onnx-0.1.7/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.1.8/src/model_explorer_onnx/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import logging
-import os
 from typing import Any, Literal, Sequence
 
 import ml_dtypes
 import model_explorer
 import numpy as np
 import onnx
 from model_explorer import graph_builder
@@ -16,31 +15,31 @@
 _TENSOR_DISPLAY_LIMIT = 1024
 _DEFAULT_OPSET_VERSION = 18
 
 
 def display_tensor(tensor: ir.TensorProtocol | None) -> str:
     if tensor is None:
         return "Data not available"
-    if tensor.size < _TENSOR_DISPLAY_LIMIT:
-        try:
-            array = tensor.numpy()
-            if tensor.dtype == ir.DataType.BFLOAT16:
-                array = array.view(ml_dtypes.bfloat16)
-            elif tensor.dtype == ir.DataType.FLOAT8E4M3FN:
-                array = array.view(ml_dtypes.float8_e4m3fn)
-            elif tensor.dtype == ir.DataType.FLOAT8E4M3FNUZ:
-                array = array.view(ml_dtypes.float8_e4m3fnuz)
-            elif tensor.dtype == ir.DataType.FLOAT8E5M2:
-                array = array.view(ml_dtypes.float8_e5m2)
-            elif tensor.dtype == ir.DataType.FLOAT8E5M2FNUZ:
-                array = array.view(ml_dtypes.float8_e5m2fnuz)
-            return np.array2string(array, separator=",")
-        except Exception as e:
-            logger.warning("Failed to display tensor: %s", e)
-            return str(tensor)
+    if tensor.size > _TENSOR_DISPLAY_LIMIT or isinstance(tensor, ir.ExternalTensor):
+        return str(tensor)
+    try:
+        array = tensor.numpy()
+        if tensor.dtype == ir.DataType.BFLOAT16:
+            array = array.view(ml_dtypes.bfloat16)
+        elif tensor.dtype == ir.DataType.FLOAT8E4M3FN:
+            array = array.view(ml_dtypes.float8_e4m3fn)
+        elif tensor.dtype == ir.DataType.FLOAT8E4M3FNUZ:
+            array = array.view(ml_dtypes.float8_e4m3fnuz)
+        elif tensor.dtype == ir.DataType.FLOAT8E5M2:
+            array = array.view(ml_dtypes.float8_e5m2)
+        elif tensor.dtype == ir.DataType.FLOAT8E5M2FNUZ:
+            array = array.view(ml_dtypes.float8_e5m2fnuz)
+        return np.array2string(array, separator=",")
+    except Exception as e:
+        logger.warning("Failed to display tensor: %s", e)
     return str(tensor)
 
 
 def format_shape(shape: ir.ShapeProtocol | None) -> str:
     return str(shape) if shape is not None else "[?]"
 
 
@@ -258,17 +257,21 @@
         graph_inputs: The set of graph inputs.
         namespace: The namespace of the node.
         all_function_ids: The set of all function identifiers.
         opset_version: The current ONNX opset version.
     """
     assert onnx_node.name, "Bug: Node name is required"
 
-    embedded_namespace = parse_namespace(onnx_node.name)
-    if embedded_namespace:
-        namespace = namespace + "/" + "/".join(embedded_namespace)
+    if onnx_node.op_type == "Constant":
+        # Move the constant closer to the user node's namespace
+        namespace = get_constant_namespace(onnx_node.outputs[0], namespace)
+    else:
+        embedded_namespace = parse_namespace(onnx_node.name)
+        if embedded_namespace:
+            namespace = namespace + "/" + "/".join(embedded_namespace)
     node = graph_builder.GraphNode(
         id=onnx_node.name,
         label=create_op_label(onnx_node.domain, onnx_node.op_type),
         namespace=namespace,
     )
     add_incoming_edges(onnx_node, node, graph_inputs)
     add_node_attrs(onnx_node, node)
@@ -308,25 +311,26 @@
         set_attr(node, "name", value.name or "")
         set_attr(node, "index", str(i))
         graph.nodes.append(node)
         # Record nodes for quick lookup
         all_nodes[node.id] = node
 
 
-def get_initializer_namespace(initializer: ir.Value, root_namespace: str) -> str:
-    # If the initializer is used by a single node, move it to the same namespace as the node
+def get_constant_namespace(initializer: ir.Value, root_namespace: str) -> str:
+    """Move the constant/initializer closer to the user's namespace."""
     initializer_namespace = root_namespace
     # A single node can have multiple uses of the same value.
     # Here we only count the unique nodes that use the initializer to push the
     # initializer to the same namespace as much as possible.
     user_nodes = tuple(set(node for node, _ in initializer.uses()))
     if not user_nodes:
         # The initializer is not used by any node. Keep it in the root namespace.
         return initializer_namespace
     if len(user_nodes) == 1:
+        # If the initializer is used by a single node, move it to the same namespace as the node
         user_node = user_nodes[0]
         assert (
             user_node.name
         ), "Bug: Node name is required and should have been assigned"
         user_node_namespace = parse_namespace(user_node.name)
         if user_node_namespace:
             initializer_namespace = (
@@ -372,15 +376,15 @@
             node = all_nodes[initializer_node_name]
             metadata = node.outputsMetadata[0]
             set_attr(metadata, "value", display_tensor(initializer.const_value))
             continue
         node = graph_builder.GraphNode(
             id=initializer_node_name,
             label="Initializer",
-            namespace=get_initializer_namespace(initializer, namespace),
+            namespace=get_constant_namespace(initializer, namespace),
         )
         # Add metadata for the output tensor
         if initializer.const_value is None:
             logger.warning(
                 "Initializer %s does not have a const value. Skipping.", initializer
             )
             graph.nodes.append(node)
@@ -454,32 +458,33 @@
     )
 
     def convert(
         self, model_path: str, settings: dict[str, Any]
     ) -> model_explorer.ModelExplorerGraphs:
         del settings  # Unused
 
+        # Do not load external data because the model file is copied to a temporary location
+        # and the external data paths are not valid anymore.
         onnx_model = onnx.load(model_path, load_external_data=False)
         try:
-            onnx_model = onnx.shape_inference.infer_shapes(onnx_model)
+            onnx_model = onnx.shape_inference.infer_shapes(onnx_model, data_prop=True)
         except Exception as e:
             logger.warning(
                 "Failed to infer shapes. Continue with the original model. Error: %s", e
             )
 
-        # Load external data after shape inference
-        model_filepath = os.path.abspath(model_path)
-        base_dir = os.path.dirname(model_filepath)
-        onnx.load_external_data_for_model(onnx_model, base_dir)
-
         # Convert to ONNX IR
         model = ir.serde.deserialize_model(onnx_model)
         all_function_ids = set(model.functions)
         graphs = []
-        opset_version = model.opset_imports.get("", _DEFAULT_OPSET_VERSION)
+        opset_version = model.opset_imports.get("")
+        if opset_version is None:
+            opset_version = model.opset_imports.get("ai.onnx")
+        if opset_version is None:
+            opset_version = _DEFAULT_OPSET_VERSION
         # TODO: Better support subgraphs in nodes
         main_graph = create_graph(
             model.graph, all_function_ids, opset_version=opset_version
         )
         assert main_graph is not None
         graphs.append(main_graph)
```

### Comparing `model_explorer_onnx-0.1.7/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.1.8/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.1.7
+Version: 0.1.8
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

