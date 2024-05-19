# Comparing `tmp/TaGra-0.1.1.tar.gz` & `tmp/TaGra-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TaGra-0.1.1.tar", last modified: Sat May 18 16:23:49 2024, max compression
+gzip compressed data, was "TaGra-0.1.3.tar", last modified: Sun May 19 00:14:46 2024, max compression
```

## Comparing `TaGra-0.1.1.tar` & `TaGra-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-18 16:23:49.089886 TaGra-0.1.1/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1084 2024-05-18 14:14:07.000000 TaGra-0.1.1/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)     3337 2024-05-18 16:23:49.089886 TaGra-0.1.1/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)     2826 2024-05-18 14:25:52.000000 TaGra-0.1.1/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-18 16:23:49.085886 TaGra-0.1.1/TaGra.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)     3337 2024-05-18 16:23:49.000000 TaGra-0.1.1/TaGra.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      402 2024-05-18 16:23:49.000000 TaGra-0.1.1/TaGra.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-18 16:23:49.000000 TaGra-0.1.1/TaGra.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       39 2024-05-18 16:23:49.000000 TaGra-0.1.1/TaGra.egg-info/entry_points.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       53 2024-05-18 16:23:49.000000 TaGra-0.1.1/TaGra.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       12 2024-05-18 16:23:49.000000 TaGra-0.1.1/TaGra.egg-info/top_level.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       38 2024-05-18 16:23:49.089886 TaGra-0.1.1/setup.cfg
--rw-rw-r--   0 davide    (1000) davide    (1000)      881 2024-05-18 16:23:32.000000 TaGra-0.1.1/setup.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-18 16:23:49.089886 TaGra-0.1.1/tagra/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:06.000000 TaGra-0.1.1/tagra/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    10666 2024-05-18 16:08:18.000000 TaGra-0.1.1/tagra/analysis.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1062 2024-05-18 15:46:39.000000 TaGra-0.1.1/tagra/config.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     3892 2024-05-18 16:04:47.000000 TaGra-0.1.1/tagra/graph.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     7803 2024-05-18 16:00:39.000000 TaGra-0.1.1/tagra/preprocessing.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-18 16:23:49.089886 TaGra-0.1.1/tests/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:49.000000 TaGra-0.1.1/tests/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      951 2024-05-18 14:00:18.000000 TaGra-0.1.1/tests/test_analysis.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1444 2024-05-18 13:20:47.000000 TaGra-0.1.1/tests/test_config.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      977 2024-05-18 14:06:00.000000 TaGra-0.1.1/tests/test_graph.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2803 2024-05-18 13:52:06.000000 TaGra-0.1.1/tests/test_preprocessing.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:14:46.596997 TaGra-0.1.3/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1084 2024-05-18 14:14:07.000000 TaGra-0.1.3/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3336 2024-05-19 00:14:46.596997 TaGra-0.1.3/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2825 2024-05-18 16:28:01.000000 TaGra-0.1.3/README.md
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:14:46.592997 TaGra-0.1.3/TaGra.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3336 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      417 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       39 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/entry_points.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       53 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       12 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       38 2024-05-19 00:14:46.596997 TaGra-0.1.3/setup.cfg
+-rw-rw-r--   0 davide    (1000) davide    (1000)      881 2024-05-19 00:14:10.000000 TaGra-0.1.3/setup.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:14:46.592997 TaGra-0.1.3/tagra/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:06.000000 TaGra-0.1.3/tagra/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2829 2024-05-19 00:09:22.000000 TaGra-0.1.3/tagra/analysis.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1062 2024-05-18 15:46:39.000000 TaGra-0.1.3/tagra/config.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3892 2024-05-18 16:04:47.000000 TaGra-0.1.3/tagra/graph.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7803 2024-05-18 16:00:39.000000 TaGra-0.1.3/tagra/preprocessing.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7373 2024-05-19 00:03:59.000000 TaGra-0.1.3/tagra/utils.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:14:46.596997 TaGra-0.1.3/tests/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:49.000000 TaGra-0.1.3/tests/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2447 2024-05-19 00:12:28.000000 TaGra-0.1.3/tests/test_analysis.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1444 2024-05-18 13:20:47.000000 TaGra-0.1.3/tests/test_config.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      977 2024-05-18 14:06:00.000000 TaGra-0.1.3/tests/test_graph.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2803 2024-05-18 13:52:06.000000 TaGra-0.1.3/tests/test_preprocessing.py
```

### Comparing `TaGra-0.1.1/LICENSE` & `TaGra-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.1/PKG-INFO` & `TaGra-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaGra
-Version: 0.1.1
+Version: 0.1.3
 Summary: TaGra: TAbular data preprocessing to GRAph representation.
 Home-page: https://github.com/davidetorre92/TaGra
 Author: Davide Torre, Davide Chicco
 Author-email: davidetorre92@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 - **Visualization**: Generate insightful visualizations to understand your data and graph structures.
 
 ## Installation
 
 To install TaGra, simply use pip:
 
 ```sh
-pip install ta_gra
+pip install tagra
 ```
 
 # Usage
 ## Data Preprocessing
 
 ```python
 from tagra.preprocessing import preprocess_dataframe
```

### Comparing `TaGra-0.1.1/README.md` & `TaGra-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - **Visualization**: Generate insightful visualizations to understand your data and graph structures.
 
 ## Installation
 
 To install TaGra, simply use pip:
 
 ```sh
-pip install ta_gra
+pip install tagra
 ```
 
 # Usage
 ## Data Preprocessing
 
 ```python
 from tagra.preprocessing import preprocess_dataframe
```

### Comparing `TaGra-0.1.1/TaGra.egg-info/PKG-INFO` & `TaGra-0.1.3/TaGra.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaGra
-Version: 0.1.1
+Version: 0.1.3
 Summary: TaGra: TAbular data preprocessing to GRAph representation.
 Home-page: https://github.com/davidetorre92/TaGra
 Author: Davide Torre, Davide Chicco
 Author-email: davidetorre92@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 - **Visualization**: Generate insightful visualizations to understand your data and graph structures.
 
 ## Installation
 
 To install TaGra, simply use pip:
 
 ```sh
-pip install ta_gra
+pip install tagra
 ```
 
 # Usage
 ## Data Preprocessing
 
 ```python
 from tagra.preprocessing import preprocess_dataframe
```

### Comparing `TaGra-0.1.1/setup.py` & `TaGra-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TaGra',
-    version='0.1.1',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'scikit-learn',
         'matplotlib',
         'networkx',
```

### Comparing `TaGra-0.1.1/tagra/analysis.py` & `TaGra-0.1.3/tagra/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-import pickle
 import datetime
 import networkx as nx
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 import pandas as pd
 import numpy as np
-import plotly.express as px
-from networkx.algorithms import community
-from collections import Counter
 
 def analyze_neighborhood_attributes(graph, attribute_name, return_probs=False):
     """
     Analyzes attributes in the neighborhoods of each node in a graph, optionally returning probabilities.
 
     Parameters:
     - graph (networkx.Graph): The input graph.
     - attribute_name (str): The name of the node attribute to analyze.
     - return_probs (bool): If True, returns the probability of each attribute in the neighborhood.
 
     Returns:
     - pd.DataFrame: A DataFrame with each row representing a node. Columns include the node's attribute,
                     degree, and either the count or probability of each attribute in its neighborhood.
     """
-    # Collect unique attributes
     unique_attributes = set(nx.get_node_attributes(graph, attribute_name).values())
-
-    # Prepare data for DataFrame
     data = []
     for node in graph.nodes:
         neighbors = list(graph.neighbors(node))
         neighbor_attrs = [graph.nodes[n].get(attribute_name, None) for n in neighbors]
 
         attr_counts = {}
         attr_counts[f"node_{attribute_name}"] = graph.nodes[node].get(attribute_name, None)
         attr_counts["node_index"] = node
         attr_counts["degree"] = len(neighbors)
 
         for attr in unique_attributes:
-            if return_probs and attr_counts["degree"] > 0:  # Calculate probabilities
+            if return_probs and attr_counts["degree"] > 0:
                 attr_counts[f"p_{attr}"] = neighbor_attrs.count(attr) / attr_counts["degree"]
-            else:  # Count occurrences
+            else:
                 attr_counts[f"n_{attr}"] = neighbor_attrs.count(attr)
 
         data.append(attr_counts)
 
-    # Create DataFrame
     cols = ["node_index", f"node_{attribute_name}", "degree"] + \
            [f"{'p' if return_probs else 'n'}_{attr}" for attr in unique_attributes]
     df = pd.DataFrame(data, columns=cols)
 
     return df
 
 def print_neighbors_prob(df_neigh, label_col):
-# Calculate the probabilities
     probabilities = {}
     for label_i in df_neigh[f'node_{label_col}'].unique():
         nodes_with_label_i = df_neigh[df_neigh[f'node_{label_col}'] == label_i]
         total_degree_i = nodes_with_label_i['degree'].sum()
         for label_j in df_neigh[f'node_{label_col}'].unique():
             col_name = f'n_{label_j}'
             total_neighbors_with_label_j = nodes_with_label_i[col_name].sum()
@@ -67,20 +58,18 @@
 def heat_map_prob(probabilities, df_neigh, label_col, prob_heatmap_path):
     labels = sorted(df_neigh[f'node_{label_col}'].unique())
     prob_matrix = pd.DataFrame(index=labels, columns=labels, data=0.0)
 
     for (i, j), prob in probabilities.items():
         prob_matrix.loc[i, j] = prob
 
-    # Plotting the heatmap
     fig, ax = plt.subplots(figsize=(8, 6))
     cax = ax.imshow(prob_matrix, cmap='viridis', interpolation='nearest')
     fig.colorbar(cax)
 
-    # Adding annotations
     for i in range(len(labels)):
         for j in range(len(labels)):
             text = ax.text(j, i, f"{prob_matrix.iloc[i, j]:.2f}",
                            ha="center", va="center", color="w")
 
     ax.set_title('Probability Distribution Heatmap')
     ax.set_xticks(range(len(labels)))
@@ -91,20 +80,18 @@
     plt.xlabel('Label j')
     plt.ylabel('Label i')
     if prob_heatmap_path:
         plt.savefig(prob_heatmap_path)
         print(f"{datetime.datetime.now()}: Neighbour probability data saved in {prob_heatmap_path}")
 
 def plot_distribution(data_dict, outpath, bins = None, double_log = True):
-    # Calculate the degree of each node
     data = data_dict['data']
     if bins is None:
         bins = range(0, max(data))
     hist, bin_edges = np.histogram(data, bins = bins)
-    # Plot the degree distribution
     fig, ax = plt.subplots()
     ax.scatter(bin_edges[:-1], hist, alpha=0.75, edgecolor='black')
     ax.set_title(data_dict['title'])
     ax.set_xlim((1,None))
     ax.set_ylim((1,None))
     ax.set_xlabel(data_dict['xlabel'])
     ax.set_ylabel(data_dict['ylabel'])
@@ -114,78 +101,66 @@
     ax.grid()
     fig.show()
     if outpath:
         fig.savefig(outpath)
         print(f"{datetime.datetime.now()}: {data_dict['title']} saved in {outpath}")
 
 def plot_community_composition(G, attribute_name, outpath):
-    # Detect communities
     communities_generator = nx.algorithms.community.girvan_newman(G)
     top_level_communities = next(communities_generator)
     communities = [list(c) for c in sorted(top_level_communities, key=len, reverse=True)]
 
-    # Infer labels from the graph
     if attribute_name is not None:
         labels_per_node = [G.nodes[node][attribute_name] for node in G.nodes()]
         unique_labels = np.unique(labels_per_node)
     else:
         labels_per_node = [0 for node in G.nodes()]
         unique_labels = [0]
 
-    # Prepare data for stacked bar plot
     community_compositions = {}
     if attribute_name is not None:
         for comm_id, community in enumerate(communities):
             labels_community = [G.nodes[node][attribute_name] for node in community]
-            label_count = Counter(labels_community)
-            community_compositions[comm_id] = {label: label_count.get(label, 0) for label in unique_labels}
-
+            unique_labels, counts = np.unique(labels_community, return_counts=True)
+            community_compositions[comm_id] = {label: 0 for label in unique_labels}
+            for label, count in zip(unique_labels, counts):
+                community_compositions[comm_id][label] = count
     else:
         for comm_id, community in enumerate(communities):
             labels_community = [0 for node in community]
-            label_count = Counter(labels_community)
-            community_compositions[comm_id] = {label: label_count.get(label, 0) for label in unique_labels}
+            unique_labels, counts = np.unique(labels_community, return_counts=True)
+            community_compositions[comm_id] = {label: 0 for label in unique_labels}
+            for label, count in zip(unique_labels, counts):
+                community_compositions[comm_id][label] = count
 
-    # Prepare data for plotting
     indices = list(community_compositions.keys())
-    bar_width = 0.35  # Width of the bars
-    print("Community composition:")
-    print(community_compositions)
-    print()
-    # Initialize a figure and axis for the plot
+    bar_width = 0.35
     fig, ax = plt.subplots(figsize = (15,15))
 
-    # Loop through each label to stack the bars
-    bottoms = [0] * len(indices)  # Keeps track of where the next bar starts
+    bottoms = [0] * len(indices)
     for label in unique_labels:
         values = [community_compositions[idx].get(label, 0) for idx in indices]
         ax.bar(indices, values, bar_width, label=label, bottom=bottoms)
-        # Update the bottom positions for the next label
         bottoms = [bottom + value for bottom, value in zip(bottoms, values)]
 
-    # Set the position of the bars on the X-axis
     ax.set_xticks(indices)
     ax.set_xticklabels(indices)
-
-    # Adding labels and title
     ax.set_xlabel('Community ID')
     ax.set_ylabel('Counts')
     ax.set_title('Counts of outcomes by community ID')
     ax.grid()
     ax.legend()
 
-    # Show the plot
     if outpath:
         fig.savefig(outpath)
         print(f"{datetime.datetime.now()}: Community composition saved in {outpath}")
         
 def matplotlib_graph_visualization(G, attribute = None, outpath = None, palette = 'viridis', pos = None):
     palette = 'viridis'
     plt.figure(figsize=(10, 10))
-    # Get node positions using a layout
     if pos is None:
       pos = nx.spring_layout(G, seed=2112)
 
     node_color = []
     if attribute is not None:
         classification_attribute_name = attribute
         y = np.array([G.nodes[node][classification_attribute_name] for node in G.nodes()])
@@ -196,63 +171,7 @@
         color_array = cmap(colors)
         node_color = [color_array[unique_dict[key]] for key in y]
     nx.draw(G, pos, with_labels=True, node_size=50, font_size=8, node_color = node_color)
     plt.title("Graph of Relations Based on Manifold Learning Transformed Data")
     if outpath:
         plt.savefig(outpath)
         print(f'{datetime.datetime.now()}: Graph saved in {outpath}')
-
-
-def analyze_graph(graph_path=None, 
-                  attribute=None, 
-                  clustering_method='hierarchical', 
-                  inconsistency_threshold=0.1, 
-                  verbose=True,
-                  plot_graph=False, 
-                  neigh_prob_path = None,
-                  degree_distribution_outpath = None,
-                  betweenness_distribution_outpath = None,
-                  prob_heatmap_path = None,
-                  community_composition_outpath = None,
-                  graph_visualization_path = None):
-    if isinstance(graph_path, str):
-        G = pickle.load(open(graph_path, 'rb'))
-    elif isinstance(graph_path, nx.Graph):
-        G = graph_path
-    else:
-        raise ValueError("Invalid graph_path. Must be a path to a file or a NetworkX Graph.")
-
-    if neigh_prob_path is None:
-        neigh_prob_path = f"./neighbor_stat_{datetime.datetime.now().strftime('%Y%m%d%H%M')}.dat"
-
-    if verbose:
-        print(f"--------------------------\nGraph analysis options\n--------------------------\n\n"
-              f"\tOptions:\n"
-              f"\tgraph_path: {graph_path}, attribute: {attribute}, \n"
-              f"\tclustering_method: {clustering_method}, inconsistency_threshold: {inconsistency_threshold}, verbose: {verbose}\n\n")
-
-    if attribute is not None:
-        df_neigh = analyze_neighborhood_attributes(G, attribute_name = attribute)
-        probabilities = print_neighbors_prob(df_neigh, attribute)
-        # Display the results
-        for (i, j), prob in probabilities.items():
-            print(f"P({j}|{i}) = {prob}")
-        with open(neigh_prob_path, 'w') as fp:
-            for (i, j), prob in probabilities.items():
-                fp.write(f"P({j}|{i}) = {prob}")   
-
-        heat_map_prob(probabilities, df_neigh, attribute, prob_heatmap_path)
-
-    degree_data = {'data': [degree for _, degree in G.degree()],
-                   'title': 'Degree distribution',
-                   'xlabel': 'Degree',
-                   'ylabel': 'Number of Nodes'}
-    betweenness_data = {'data': [degree for _, degree in G.degree()],
-                   'title': 'Degree distribution',
-                   'xlabel': 'Degree',
-                   'ylabel': 'Number of Nodes'}
-    
-    plot_distribution(degree_data, degree_distribution_outpath)
-    plot_distribution(betweenness_data, betweenness_distribution_outpath)
-    plot_community_composition(G, attribute, community_composition_outpath)
-    if plot_graph:
-        matplotlib_graph_visualization(G, attribute, graph_visualization_path, palette = 'viridis')
```

### Comparing `TaGra-0.1.1/tagra/config.py` & `TaGra-0.1.3/tagra/config.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.1/tagra/graph.py` & `TaGra-0.1.3/tagra/graph.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.1/tagra/preprocessing.py` & `TaGra-0.1.3/tagra/preprocessing.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.1/tests/test_config.py` & `TaGra-0.1.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.1/tests/test_graph.py` & `TaGra-0.1.3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.1/tests/test_preprocessing.py` & `TaGra-0.1.3/tests/test_preprocessing.py`

 * *Files identical despite different names*

