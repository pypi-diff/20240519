# Comparing `tmp/rdfvr-0.3.2.tar.gz` & `tmp/rdfvr-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfvr-0.3.2.tar", last modified: Thu May 16 20:56:58 2024, max compression
+gzip compressed data, was "rdfvr-0.3.3.tar", last modified: Sat May 18 22:25:30 2024, max compression
```

## Comparing `rdfvr-0.3.2.tar` & `rdfvr-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mengli     (501) staff       (20)        0 2024-05-16 20:56:58.270860 rdfvr-0.3.2/
--rw-r--r--   0 mengli     (501) staff       (20)     4537 2024-05-16 20:56:58.270723 rdfvr-0.3.2/PKG-INFO
--rw-r--r--   0 mengli     (501) staff       (20)     4209 2023-12-06 03:15:12.000000 rdfvr-0.3.2/README.md
-drwxr-xr-x   0 mengli     (501) staff       (20)        0 2024-05-16 20:56:58.270549 rdfvr-0.3.2/rdfvr.egg-info/
--rw-r--r--   0 mengli     (501) staff       (20)     4537 2024-05-16 20:56:58.000000 rdfvr-0.3.2/rdfvr.egg-info/PKG-INFO
--rw-r--r--   0 mengli     (501) staff       (20)      203 2024-05-16 20:56:58.000000 rdfvr-0.3.2/rdfvr.egg-info/SOURCES.txt
--rw-r--r--   0 mengli     (501) staff       (20)        1 2024-05-16 20:56:58.000000 rdfvr-0.3.2/rdfvr.egg-info/dependency_links.txt
--rw-r--r--   0 mengli     (501) staff       (20)       37 2024-05-16 20:56:58.000000 rdfvr-0.3.2/rdfvr.egg-info/entry_points.txt
--rw-r--r--   0 mengli     (501) staff       (20)       93 2024-05-16 20:56:58.000000 rdfvr-0.3.2/rdfvr.egg-info/requires.txt
--rw-r--r--   0 mengli     (501) staff       (20)        6 2024-05-16 20:56:58.000000 rdfvr-0.3.2/rdfvr.egg-info/top_level.txt
--rw-r--r--   0 mengli     (501) staff       (20)    10890 2024-05-16 20:44:31.000000 rdfvr-0.3.2/rdfvr.py
--rw-r--r--   0 mengli     (501) staff       (20)       38 2024-05-16 20:56:58.270897 rdfvr-0.3.2/setup.cfg
--rw-r--r--   0 mengli     (501) staff       (20)      767 2024-05-16 20:47:59.000000 rdfvr-0.3.2/setup.py
+drwxr-xr-x   0 mengli     (501) staff       (20)        0 2024-05-18 22:25:30.755913 rdfvr-0.3.3/
+-rw-r--r--   0 mengli     (501) staff       (20)     4489 2024-05-18 22:25:30.755784 rdfvr-0.3.3/PKG-INFO
+-rw-r--r--   0 mengli     (501) staff       (20)     4161 2024-05-18 22:18:47.000000 rdfvr-0.3.3/README.md
+drwxr-xr-x   0 mengli     (501) staff       (20)        0 2024-05-18 22:25:30.755614 rdfvr-0.3.3/rdfvr.egg-info/
+-rw-r--r--   0 mengli     (501) staff       (20)     4489 2024-05-18 22:25:30.000000 rdfvr-0.3.3/rdfvr.egg-info/PKG-INFO
+-rw-r--r--   0 mengli     (501) staff       (20)      203 2024-05-18 22:25:30.000000 rdfvr-0.3.3/rdfvr.egg-info/SOURCES.txt
+-rw-r--r--   0 mengli     (501) staff       (20)        1 2024-05-18 22:25:30.000000 rdfvr-0.3.3/rdfvr.egg-info/dependency_links.txt
+-rw-r--r--   0 mengli     (501) staff       (20)       37 2024-05-18 22:25:30.000000 rdfvr-0.3.3/rdfvr.egg-info/entry_points.txt
+-rw-r--r--   0 mengli     (501) staff       (20)      103 2024-05-18 22:25:30.000000 rdfvr-0.3.3/rdfvr.egg-info/requires.txt
+-rw-r--r--   0 mengli     (501) staff       (20)        6 2024-05-18 22:25:30.000000 rdfvr-0.3.3/rdfvr.egg-info/top_level.txt
+-rw-r--r--   0 mengli     (501) staff       (20)    12236 2024-05-18 22:17:22.000000 rdfvr-0.3.3/rdfvr.py
+-rw-r--r--   0 mengli     (501) staff       (20)       38 2024-05-18 22:25:30.755961 rdfvr-0.3.3/setup.cfg
+-rw-r--r--   0 mengli     (501) staff       (20)      780 2024-05-18 22:25:09.000000 rdfvr-0.3.3/setup.py
```

### Comparing `rdfvr-0.3.2/PKG-INFO` & `rdfvr-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfvr
-Version: 0.3.2
+Version: 0.3.3
 Summary: RDFVR: RDF Validation Report
 Home-page: https://github.com/meng6/rdfvr
 Author: Meng Li
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -54,15 +54,15 @@
   --mappings MAPPINGS, -m MAPPINGS
                         File of the mappings to shorten the report (str): path of the JSON file, where the key is the original text and the value is the shorter text.
   --output OUTPUT, -o OUTPUT
                         Path(s) of the validation report without extension (list[str] | str ). If no value, then output will be a string. Please use comma (no space) to split
                         multiple file paths (e.g. file1,file2,file3).
   --outputformat OUTPUTFORMAT, -of OUTPUTFORMAT
                         File format(s) of the output, validation report (list[str] | str ). Orders should be consistent with the input of --output. Default format is
-                        txt. Each item can only be one of {txt,png,svg,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
+                        txt. Each item can only be one of {txt,html}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
                         output files have the same format, only need to write once.
 
 ```
 
 ## Python Module Use
 You can call the `validation_report` function of the `rdfvr` module as follows:
 
@@ -73,14 +73,14 @@
 
 Where
 - `file_path` is the file path (string) of a RDF graph
 - `file_format` is the format (string) of the RDF graph file
 - `schema` is the file path (string) of the RDF graph's schema
 - `schema_format` is the format (string) of the schema file
 - `output_path` is the file path (string) of the validation report without extension
-- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `svg` or `gv`
+- `output_format` is the format (string) of the validation report, i.e., `txt` or `html`
 - `mappings` is the mappings (dictionary) to shorten the report
 
 The return value is `None`.
 
-The output will be either a `txt` file, a `png` file, a `svg` file, a `gv` file, or a `string` print in Bash.
+The output will be either a `txt` file, a `html` file, or a `string` print in Bash.
```

### Comparing `rdfvr-0.3.2/README.md` & `rdfvr-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   --mappings MAPPINGS, -m MAPPINGS
                         File of the mappings to shorten the report (str): path of the JSON file, where the key is the original text and the value is the shorter text.
   --output OUTPUT, -o OUTPUT
                         Path(s) of the validation report without extension (list[str] | str ). If no value, then output will be a string. Please use comma (no space) to split
                         multiple file paths (e.g. file1,file2,file3).
   --outputformat OUTPUTFORMAT, -of OUTPUTFORMAT
                         File format(s) of the output, validation report (list[str] | str ). Orders should be consistent with the input of --output. Default format is
-                        txt. Each item can only be one of {txt,png,svg,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
+                        txt. Each item can only be one of {txt,html}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
                         output files have the same format, only need to write once.
 
 ```
 
 ## Python Module Use
 You can call the `validation_report` function of the `rdfvr` module as follows:
 
@@ -61,14 +61,14 @@
 
 Where
 - `file_path` is the file path (string) of a RDF graph
 - `file_format` is the format (string) of the RDF graph file
 - `schema` is the file path (string) of the RDF graph's schema
 - `schema_format` is the format (string) of the schema file
 - `output_path` is the file path (string) of the validation report without extension
-- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `svg` or `gv`
+- `output_format` is the format (string) of the validation report, i.e., `txt` or `html`
 - `mappings` is the mappings (dictionary) to shorten the report
 
 The return value is `None`.
 
-The output will be either a `txt` file, a `png` file, a `svg` file, a `gv` file, or a `string` print in Bash.
+The output will be either a `txt` file, a `html` file, or a `string` print in Bash.
```

### Comparing `rdfvr-0.3.2/rdfvr.egg-info/PKG-INFO` & `rdfvr-0.3.3/rdfvr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfvr
-Version: 0.3.2
+Version: 0.3.3
 Summary: RDFVR: RDF Validation Report
 Home-page: https://github.com/meng6/rdfvr
 Author: Meng Li
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -54,15 +54,15 @@
   --mappings MAPPINGS, -m MAPPINGS
                         File of the mappings to shorten the report (str): path of the JSON file, where the key is the original text and the value is the shorter text.
   --output OUTPUT, -o OUTPUT
                         Path(s) of the validation report without extension (list[str] | str ). If no value, then output will be a string. Please use comma (no space) to split
                         multiple file paths (e.g. file1,file2,file3).
   --outputformat OUTPUTFORMAT, -of OUTPUTFORMAT
                         File format(s) of the output, validation report (list[str] | str ). Orders should be consistent with the input of --output. Default format is
-                        txt. Each item can only be one of {txt,png,svg,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
+                        txt. Each item can only be one of {txt,html}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
                         output files have the same format, only need to write once.
 
 ```
 
 ## Python Module Use
 You can call the `validation_report` function of the `rdfvr` module as follows:
 
@@ -73,14 +73,14 @@
 
 Where
 - `file_path` is the file path (string) of a RDF graph
 - `file_format` is the format (string) of the RDF graph file
 - `schema` is the file path (string) of the RDF graph's schema
 - `schema_format` is the format (string) of the schema file
 - `output_path` is the file path (string) of the validation report without extension
-- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `svg` or `gv`
+- `output_format` is the format (string) of the validation report, i.e., `txt` or `html`
 - `mappings` is the mappings (dictionary) to shorten the report
 
 The return value is `None`.
 
-The output will be either a `txt` file, a `png` file, a `svg` file, a `gv` file, or a `string` print in Bash.
+The output will be either a `txt` file, a `html` file, or a `string` print in Bash.
```

### Comparing `rdfvr-0.3.2/rdfvr.py` & `rdfvr-0.3.3/rdfvr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/python3
 
 from pyshacl import validate
 from rdflib import Graph
-import pygraphviz as pgv
+import networkx as nx
+from pyvis.network import Network
 import pandas as pd
 import textwrap, argparse, json, os
 
 def ensure_dir_exists(file_path):
     dir_path = os.path.split(file_path)[0]
     if (dir_path != '') and (not os.path.isdir(dir_path)):
         os.makedirs(dir_path)
@@ -95,29 +96,44 @@
         """
     rows = []
     for r in rdf_graph.query(q):
         rows.append(r)
     rdf_graph_processed = pd.DataFrame(rows, columns=["source", "label", "target"]).replace(mappings, regex=True)
     return rdf_graph_processed
 
-def visualize_graph_as_dot(rdf_graph_processed, errors):
+def visualize_graph(rdf_graph_processed, errors):
+    """
+    This function is to visualize the RDF graph with errors
+    :param rdf_graph_processed: a Pandas data frame with source, label, and target columns
+    :param errors: a Pandas data frame with node, msg, and target columns
+    :return G: a directed graph (a networkx.Graph instance)
+    """
     # Create a directed graph
-    G = pgv.AGraph(directed=True)
-    # Add nodes and edges
-    for _, row in rdf_graph_processed.iterrows():
-        G.add_node(row["source"], shape="box", style="filled, rounded", fillcolor="#b3e2cd")
-        G.add_node(row["target"], shape="box", style="filled, rounded", fillcolor="#b3e2cd")
-        G.add_edge(row["source"], row["target"], label=row["label"])
-    for _, row in errors[["node", "msg"]].drop_duplicates().iterrows():
-        G.add_node(row["node"], shape="box", style="filled, rounded", fillcolor="#fdccac")
-        G.add_node(row["msg"], shape="box", style="filled, rounded, dashed", fillcolor="#fdccac")
-        G.add_edge(row["node"], row["msg"], label="ErrorMsg", style="dashed")
-    # Suggested nodes to be updated
-    for suggested_node in errors["target"].dropna().unique():
-        G.add_node(suggested_node, shape="box", style="filled, rounded", fillcolor="#cbd5e8")
+    G = nx.DiGraph()
+    node_colors = {}
+    # Add edges from the processed RDF graph
+    rdf_graph_processed["edge"] = rdf_graph_processed.apply(lambda row: (row["source"], row["target"], {"title": row["label"]}), axis=1)
+    G.add_edges_from(rdf_graph_processed["edge"].tolist())
+    nodes = set(rdf_graph_processed["source"].tolist())
+    nodes.update(set(rdf_graph_processed["target"].tolist()))
+    for node in nodes:
+        node_colors[node] = "#b3e2cd"
+    # Add edges from the errors
+    errors["edge"] = errors.apply(lambda row: (row["node"], row["msg"], {"title": "ErrorMsg", "color": "#fdccac"}), axis=1)
+    G.add_edges_from(errors["edge"].tolist())
+    for node in set(errors["msg"].tolist()):
+        node_colors[node] = "#fdccac"
+    for node in set(errors["target"].tolist()):
+        node_colors[node] = "#ffcccb"
+    # Update node attributes
+    for node in G.nodes:
+        G.nodes[node]["label"] = str(node)
+        G.nodes[node]["shape"] = "box"
+        G.nodes[node]["shapeProperties"] = {"borderRadius": 5}  # Add borderRadius for rounded corners
+        G.nodes[str(node)]["color"] = node_colors[node]
     return G
 
 def report_graph_as_txt(errors):
     report_text = ""
     errors = errors.groupby(["node", "msg"])["target"].agg(list).reset_index()
     errors["target"] = errors["target"].apply(str)
     for target, group in errors.groupby("target"):
@@ -128,40 +144,61 @@
         for _, row in group.iterrows():
             report_text = report_text + "Node: {node} \nError Message: {msg}\n\n".format(node=row["node"], msg=row["msg"])
     return report_text
 
 def validation_report(file_path, file_format, schema_file, schema_format, output_path, output_format, mappings):
     info = """Path of the RDF graph to be validated: {file_path}
 Path of the SHACL file: {schema_file}
-Datetime: {datetime}
-
-""".format(file_path=file_path, schema_file=schema_file, datetime=pd.Timestamp.now())
+Datetime: {datetime}""".format(file_path=file_path, schema_file=schema_file, datetime=pd.Timestamp.now())
     # Load a file with a given format as a RDF Graph object supported by RDFLib
     rdf_graph = load_file(file_path, graph_format=file_format)
     # Validate the RDF graph
     results_graph = validate_rdf(rdf_graph, schema_file, data_graph_format=file_format, shacl_graph_format=schema_format)
     # Find the most important errors
     errors = extract_errors(results_graph, mappings)
     # Output
-    if output_format not in ["txt", "png", "svg", "gv"]:
-        raise ValueError("The output file format can only be one of {txt, png, svg, gv}, but " + str(output_format) + " was given. Please check --outputformat.")
+    if output_format not in ["txt", "html"]:
+        raise ValueError("The output file format can only be one of {txt, html}, but " + str(output_format) + " was given. Please check --outputformat.")
 
     if output_path:
         output_path = output_path + "." + output_format
         ensure_dir_exists(output_path)
-    if output_format == "png" or output_format == "svg" or output_format == "gv":
+    if output_format == "html":
         print(info)
         rdf_graph_processed = graph(rdf_graph, mappings)
-        G = visualize_graph_as_dot(rdf_graph_processed, errors)
-        if output_format == "png" or output_format == "svg":
-            G.draw(output_path, prog="dot")
-        else: # gv
-            G.write(output_path)
+        G = visualize_graph(rdf_graph_processed.map(str), errors.map(str))
+        # Load the networkx.Graph instance
+        nt = Network(height="100%", width="100%", notebook=False, directed=True, select_menu=True, cdn_resources="remote")
+        nt.from_nx(G)
+        # Update attributes such as edges, layout, etc.
+        nt.set_options("""
+            {
+                "physics": {"barnesHut": {"overlap": 1}},
+                    "interaction": {
+                        "hover": true,
+                        "tooltipDelay": 200,
+                        "hideEdgesOnDrag": true,
+                        "hideNodesOnDrag": false
+                    },
+                    "edges": {
+                    "width": 1,
+                    "selectionWidth": 5,
+                    "hoverWidth": 5
+                },
+                "layout": {
+                    "hierarchical": {
+                        "direction": "LR",
+                        "sortMethod": "directed"
+                    }
+                }
+            }
+        """)
+        nt.save_graph(output_path)
     else: # txt
-        report_text = info + report_graph_as_txt(errors)
+        report_text = info + "\n\n" + report_graph_as_txt(errors)
         if not output_path:
             # If NO --output, print a string
             print(report_text)
         else:
             with open(output_path, mode="w", encoding="utf-8") as fout:
                 fout.write(report_text)
     return
@@ -171,15 +208,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("--file", "-f", help="File(s) of the RDF graph(s) to be validated (list[str] | str ): please use comma (no space) to split multiple file paths (e.g. file1,file2,file3).")
     parser.add_argument("--schema", "-s", help="Schema of the RDF graph, i.e., Shapes Constraint Language (SHACL) graph (str): path of the file.")
     parser.add_argument("--fileformat", "-ff", help="File format(s) of the RDF graph(s) to be validated (list[str] | str ). Orders should be consistent with the input of --file. Default format is json-ld. If all input files have the same format, only need to write once.")
     parser.add_argument("--schemaformat", "-sf", default="ttl", choices=["xml", "n3", "turtle", "nt", "pretty-xml", "trix", "trig", "nquads", "json-ld", "hext"], help="File format of the schema (str). Default format is ttl.")
     parser.add_argument("--mappings", "-m", help="File of the mappings to shorten the report (str): path of the JSON file, where the key is the original text and the value is the shorter text.")
     parser.add_argument("--output", "-o", help="Path(s) of the validation report without extension (list[str] | str ). If no value, then output will be a string. Please use comma (no space) to split multiple file paths (e.g. file1,file2,file3).")
-    parser.add_argument("--outputformat", "-of", help="File format(s) of the output, validation report (list[str] | str ).  Orders should be consistent with the input of --output. Default format is txt. Each item can only be one of {txt,png,svg,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all output files have the same format, only need to write once.")
+    parser.add_argument("--outputformat", "-of", help="File format(s) of the output, validation report (list[str] | str ).  Orders should be consistent with the input of --output. Default format is txt. Each item can only be one of {txt,html}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all output files have the same format, only need to write once.")
     arg_file, arg_schema, arg_fileformat, arg_schemaformat, arg_mappings, arg_outputformat, arg_output = parser.parse_args().file, parser.parse_args().schema, parser.parse_args().fileformat, parser.parse_args().schemaformat, parser.parse_args().mappings, parser.parse_args().outputformat, parser.parse_args().output
 
     if not arg_file:
         parser.error("File(s) of the RDF graph(s) to be validated are missing. Please add: --file.")
     if not arg_schema:
         parser.error("Schema file is missing. Please add: --schema.")
     if arg_mappings:
```

### Comparing `rdfvr-0.3.2/setup.py` & `rdfvr-0.3.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="rdfvr",
-    version="0.3.2",
+    version="0.3.3",
     description="RDFVR: RDF Validation Report",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meng6/rdfvr",
     author="Meng Li",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
-    install_requires=["pandas>=2.0.2", "pyshacl>=0.23.0", "rdflib>=6.3.2", "pygraphviz>=1.11"],
+    install_requires=["pandas>=2.0.2", "pyshacl>=0.23.0", "rdflib>=6.3.2", "pyvis>=0.3.2", "networkx>=3.3"],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires=">=3.10",
     entry_points='''
         [console_scripts]
         rdfvr=rdfvr:main
```

