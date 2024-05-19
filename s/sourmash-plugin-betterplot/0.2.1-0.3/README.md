# Comparing `tmp/sourmash_plugin_betterplot-0.2.1.tar.gz` & `tmp/sourmash_plugin_betterplot-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_betterplot-0.2.1.tar", last modified: Sat May 18 15:06:17 2024, max compression
+gzip compressed data, was "sourmash_plugin_betterplot-0.3.tar", last modified: Sun May 19 15:10:36 2024, max compression
```

## Comparing `sourmash_plugin_betterplot-0.2.1.tar` & `sourmash_plugin_betterplot-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 15:06:17.812973 sourmash_plugin_betterplot-0.2.1/
--rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.2.1/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     4638 2024-05-18 15:06:17.812783 sourmash_plugin_betterplot-0.2.1/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     4275 2024-05-18 14:55:28.000000 sourmash_plugin_betterplot-0.2.1/README.md
--rw-r--r--   0 t          (502) staff       (20)      514 2024-05-18 15:06:08.000000 sourmash_plugin_betterplot-0.2.1/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2024-05-18 15:06:17.813007 sourmash_plugin_betterplot-0.2.1/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 15:06:17.811006 sourmash_plugin_betterplot-0.2.1/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 15:06:17.812575 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     4638 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      422 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)      132 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       55 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       27 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)    13099 2024-05-18 14:41:09.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 15:06:17.812269 sourmash_plugin_betterplot-0.2.1/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.2.1/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 15:10:36.845518 sourmash_plugin_betterplot-0.3/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     6202 2024-05-19 15:10:36.845306 sourmash_plugin_betterplot-0.3/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     5841 2024-05-19 15:10:31.000000 sourmash_plugin_betterplot-0.3/README.md
+-rw-r--r--   0 t          (502) staff       (20)      654 2024-05-19 15:10:31.000000 sourmash_plugin_betterplot-0.3/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2024-05-19 15:10:36.845556 sourmash_plugin_betterplot-0.3/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 15:10:36.843729 sourmash_plugin_betterplot-0.3/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 15:10:36.845090 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     6202 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      422 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      270 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       55 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       27 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)    17963 2024-05-19 15:10:31.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 15:10:36.844707 sourmash_plugin_betterplot-0.3/tests/
+-rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_betterplot-0.2.1/LICENSE` & `sourmash_plugin_betterplot-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_betterplot-0.2.1/PKG-INFO` & `sourmash_plugin_betterplot-0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_betterplot
-Version: 0.2.1
+Version: 0.3
 Summary: sourmash plugin for improved plotting/viz and cluster examination.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sourmash<5,>=4.8.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
@@ -15,29 +15,29 @@
 
 [sourmash](https://sourmash.readthedocs.io/) is a tool for biological
 sequence analysis and comparisons.
 
 `betterplot` is a sourmash plugin that provides improved plotting/viz
 and cluster examination for sourmash-based sketch comparisons.
 
-## Why are we using the 
+## Why does this plugin exist?
 
 [`sourmash compare`](https://sourmash.readthedocs.io/en/latest/command-line.html#sourmash-compare-compare-many-signatures)
 and
 [`sourmash plot`](https://sourmash.readthedocs.io/en/latest/command-line.html#sourmash-plot-cluster-and-visualize-comparisons-of-many-signatures)
 produce basic distance matrix plots that are useful for comparing and
 visualizing the relationships between dozens to hundreds of
 genomes. And this is one of the most popular use cases for sourmash!
 
-But! The visualization can be improved a lot beyond the basic viz
-that `sourmash plot` produces, and there are a lot of only slightly
-more complicated use cases for comparing, clustering, and visualizing
-many genomes!
+However, the visualization can be improved a lot beyond the basic viz
+that `sourmash plot` produces. There are a lot of only slightly more
+complicated use cases for comparing, clustering, and visualizing many
+genomes!
 
-This plugin will explore some of these use cases!
+And this plugin exists to explore some of these use cases!
 
 Specific goals:
 
 * provide a variety of plotting and exploration commands that can be used
   with sourmash tools;
 * provide both command-line functionality _and_ functions that can be
   imported and used in Jupyter notebooks;
@@ -131,14 +131,62 @@
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS](examples/mds.10sketches.cmp.png)
 
+### Multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
+
+Use MDS to display a sparse comparison created using the
+[branchwater plugin's](https://github.com/sourmash-bio/sourmash_plugin_branchwater)
+`pairwise` command. The output of `pairwise` is distinct from the
+`sourmash compare` output: `pairwise` produces a sparse CSV file that
+contains just the matches above threshold, while `sourmash compare`
+produces a dense numpy matrix.
+
+These commands:
+```
+sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.sig.zip
+sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
+
+sourmash scripts mds 10sketches.cmp \
+    -o mds.10sketches.cmp.png \
+    -C 10sketches-categories.csv
+```
+
+produces this plot:
+![10-sketches plotted using MDS2](examples/mds2.10sketches.cmp.png)
+
+### Convert `pairwise` output to `sourmash compare` output and plot
+
+These commands:
+```
+# build pairwise
+sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.sig.zip
+sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
+
+# convert pairwise
+sourmash scripts pairwise_to_compare 10sketches.pairwise.csv \
+    -o 10sketches.pairwise.cmp --write-all \
+    --labels-to 10sketches.pairwise.cmp.labels_to.csv
+    
+# plot!
+sourmash scripts plot2 10sketches.pairwise.cmp \
+    10sketches.pairwise.cmp.labels_to.csv \
+    -o plot2.pairwise.10sketches.cmp.png
+```
+
+produce this plot:
+
+![10-sketches plotted from pairwise](examples/plot2.pairwise.10sketches.cmp.png)
+
+
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
 
 `betterplot` is developed at
```

### Comparing `sourmash_plugin_betterplot-0.2.1/README.md` & `sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,43 @@
+Metadata-Version: 2.1
+Name: sourmash_plugin_betterplot
+Version: 0.3
+Summary: sourmash plugin for improved plotting/viz and cluster examination.
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sourmash<5,>=4.8.8
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+
 # sourmash_plugin_betterplot
 
 [sourmash](https://sourmash.readthedocs.io/) is a tool for biological
 sequence analysis and comparisons.
 
 `betterplot` is a sourmash plugin that provides improved plotting/viz
 and cluster examination for sourmash-based sketch comparisons.
 
-## Why are we using the 
+## Why does this plugin exist?
 
 [`sourmash compare`](https://sourmash.readthedocs.io/en/latest/command-line.html#sourmash-compare-compare-many-signatures)
 and
 [`sourmash plot`](https://sourmash.readthedocs.io/en/latest/command-line.html#sourmash-plot-cluster-and-visualize-comparisons-of-many-signatures)
 produce basic distance matrix plots that are useful for comparing and
 visualizing the relationships between dozens to hundreds of
 genomes. And this is one of the most popular use cases for sourmash!
 
-But! The visualization can be improved a lot beyond the basic viz
-that `sourmash plot` produces, and there are a lot of only slightly
-more complicated use cases for comparing, clustering, and visualizing
-many genomes!
+However, the visualization can be improved a lot beyond the basic viz
+that `sourmash plot` produces. There are a lot of only slightly more
+complicated use cases for comparing, clustering, and visualizing many
+genomes!
 
-This plugin will explore some of these use cases!
+And this plugin exists to explore some of these use cases!
 
 Specific goals:
 
 * provide a variety of plotting and exploration commands that can be used
   with sourmash tools;
 * provide both command-line functionality _and_ functions that can be
   imported and used in Jupyter notebooks;
@@ -118,14 +131,62 @@
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS](examples/mds.10sketches.cmp.png)
 
+### Multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
+
+Use MDS to display a sparse comparison created using the
+[branchwater plugin's](https://github.com/sourmash-bio/sourmash_plugin_branchwater)
+`pairwise` command. The output of `pairwise` is distinct from the
+`sourmash compare` output: `pairwise` produces a sparse CSV file that
+contains just the matches above threshold, while `sourmash compare`
+produces a dense numpy matrix.
+
+These commands:
+```
+sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.sig.zip
+sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
+
+sourmash scripts mds 10sketches.cmp \
+    -o mds.10sketches.cmp.png \
+    -C 10sketches-categories.csv
+```
+
+produces this plot:
+![10-sketches plotted using MDS2](examples/mds2.10sketches.cmp.png)
+
+### Convert `pairwise` output to `sourmash compare` output and plot
+
+These commands:
+```
+# build pairwise
+sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.sig.zip
+sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
+
+# convert pairwise
+sourmash scripts pairwise_to_compare 10sketches.pairwise.csv \
+    -o 10sketches.pairwise.cmp --write-all \
+    --labels-to 10sketches.pairwise.cmp.labels_to.csv
+    
+# plot!
+sourmash scripts plot2 10sketches.pairwise.cmp \
+    10sketches.pairwise.cmp.labels_to.csv \
+    -o plot2.pairwise.10sketches.cmp.png
+```
+
+produce this plot:
+
+![10-sketches plotted from pairwise](examples/plot2.pairwise.10sketches.cmp.png)
+
+
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
 
 `betterplot` is developed at
```

### Comparing `sourmash_plugin_betterplot-0.2.1/pyproject.toml` & `sourmash_plugin_betterplot-0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [project]
 name = "sourmash_plugin_betterplot"
 description = "sourmash plugin for improved plotting/viz and cluster examination."
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.2.1"
+version = "0.3"
 
 dependencies = ["sourmash>=4.8.8,<5",
                 "matplotlib", "numpy", "scipy", "scikit-learn"]
 
 [metadata]
 license = { text = "BSD 3-Clause License" }
 
 [project.entry-points."sourmash.cli_script"]
 plot2_command = "sourmash_plugin_betterplot:Command_Plot2"
 mds_command = "sourmash_plugin_betterplot:Command_MDS"
+mds2_command = "sourmash_plugin_betterplot:Command_MDS2"
+pairwise_to_compare_command = "sourmash_plugin_betterplot:Command_PairwiseToCompare"
```

### Comparing `sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/PKG-INFO` & `sourmash_plugin_betterplot-0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,30 @@
-Metadata-Version: 2.1
-Name: sourmash_plugin_betterplot
-Version: 0.2.1
-Summary: sourmash plugin for improved plotting/viz and cluster examination.
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: sourmash<5,>=4.8.8
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-
 # sourmash_plugin_betterplot
 
 [sourmash](https://sourmash.readthedocs.io/) is a tool for biological
 sequence analysis and comparisons.
 
 `betterplot` is a sourmash plugin that provides improved plotting/viz
 and cluster examination for sourmash-based sketch comparisons.
 
-## Why are we using the 
+## Why does this plugin exist?
 
 [`sourmash compare`](https://sourmash.readthedocs.io/en/latest/command-line.html#sourmash-compare-compare-many-signatures)
 and
 [`sourmash plot`](https://sourmash.readthedocs.io/en/latest/command-line.html#sourmash-plot-cluster-and-visualize-comparisons-of-many-signatures)
 produce basic distance matrix plots that are useful for comparing and
 visualizing the relationships between dozens to hundreds of
 genomes. And this is one of the most popular use cases for sourmash!
 
-But! The visualization can be improved a lot beyond the basic viz
-that `sourmash plot` produces, and there are a lot of only slightly
-more complicated use cases for comparing, clustering, and visualizing
-many genomes!
+However, the visualization can be improved a lot beyond the basic viz
+that `sourmash plot` produces. There are a lot of only slightly more
+complicated use cases for comparing, clustering, and visualizing many
+genomes!
 
-This plugin will explore some of these use cases!
+And this plugin exists to explore some of these use cases!
 
 Specific goals:
 
 * provide a variety of plotting and exploration commands that can be used
   with sourmash tools;
 * provide both command-line functionality _and_ functions that can be
   imported and used in Jupyter notebooks;
@@ -131,14 +118,62 @@
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS](examples/mds.10sketches.cmp.png)
 
+### Multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
+
+Use MDS to display a sparse comparison created using the
+[branchwater plugin's](https://github.com/sourmash-bio/sourmash_plugin_branchwater)
+`pairwise` command. The output of `pairwise` is distinct from the
+`sourmash compare` output: `pairwise` produces a sparse CSV file that
+contains just the matches above threshold, while `sourmash compare`
+produces a dense numpy matrix.
+
+These commands:
+```
+sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.sig.zip
+sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
+
+sourmash scripts mds 10sketches.cmp \
+    -o mds.10sketches.cmp.png \
+    -C 10sketches-categories.csv
+```
+
+produces this plot:
+![10-sketches plotted using MDS2](examples/mds2.10sketches.cmp.png)
+
+### Convert `pairwise` output to `sourmash compare` output and plot
+
+These commands:
+```
+# build pairwise
+sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.sig.zip
+sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
+
+# convert pairwise
+sourmash scripts pairwise_to_compare 10sketches.pairwise.csv \
+    -o 10sketches.pairwise.cmp --write-all \
+    --labels-to 10sketches.pairwise.cmp.labels_to.csv
+    
+# plot!
+sourmash scripts plot2 10sketches.pairwise.cmp \
+    10sketches.pairwise.cmp.labels_to.csv \
+    -o plot2.pairwise.10sketches.cmp.png
+```
+
+produce this plot:
+
+![10-sketches plotted from pairwise](examples/plot2.pairwise.10sketches.cmp.png)
+
+
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
 
 `betterplot` is developed at
```

### Comparing `sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.py` & `sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """betterplot plugin implementation"""
 
-usage="""
-   sourmash scripts plot2 <@CTB>
-"""
-
-epilog="""
+epilog = """
 
 Need help? Have questions? Ask at http://github.com/sourmash-bio/sourmash/issues!
 """
 
 import argparse
 import sourmash
 from sourmash import sourmash_args
@@ -32,81 +28,115 @@
 ###
 
 
 def load_labelinfo_csv(filename):
     with sourmash_args.FileInputCSV(filename) as r:
         labelinfo = list(r)
 
-    labelinfo.sort(key=lambda row: int(row['sort_order']))
+    labelinfo.sort(key=lambda row: int(row["sort_order"]))
     return labelinfo
 
 
 def load_categories_csv(filename, labelinfo):
     with sourmash_args.FileInputCSV(filename) as r:
         categories = list(r)
 
     category_map = {}
     colors = None
     if categories:
         assert labelinfo
         keys = set(categories[0].keys())
-        keys -= { "category" }
+        keys -= {"category"}
 
         key = None
         for k in keys:
             if k in labelinfo[0].keys():
                 notify(f"found category key: {k}")
                 key = k
                 break
 
         if key:
-            category_values = list(set([ row["category"] for row in categories ]))
+            category_values = list(set([row["category"] for row in categories]))
+            category_values.sort()
+
             cat_colors = list(map(plt.cm.tab10, range(len(category_values))))
             category_map = {}
             for v, color in zip(category_values, cat_colors):
                 category_map[v] = color
 
             category_map2 = {}
             for row in categories:
-                category_map2[row[key]] = category_map[row['category']]
-
-#            from pprint import pprint
-#            pprint(category_map2)
+                category_map2[row[key]] = category_map[row["category"]]
 
             colors = []
             for row in labelinfo:
                 value = row[key]
                 color = category_map2[value]
                 colors.append(color)
 
         else:
             notify(f"no valid key column found in categories file '{filename}'.")
     else:
         notify(f"nothing in categories file '{filename}'?!")
-        
+
+    return category_map, colors
+
+
+def load_categories_csv_for_labels(filename, queries):
+    "Load a categories CSV that must use label name."
+    with sourmash_args.FileInputCSV(filename) as r:
+        categories = list(r)
+
+    category_map = {}
+    colors = None
+    if categories:
+        key = "label"
+
+        category_values = list(set([row["category"] for row in categories]))
+        category_values.sort()
+
+        cat_colors = list(map(plt.cm.tab10, range(len(category_values))))
+        category_map = {}
+        for v, color in zip(category_values, cat_colors):
+            category_map[v] = color
+
+        category_map2 = {}
+        for row in categories:
+            label = row[key]
+            cat = row["category"]
+            category_map2[label] = category_map[cat]
+
+        colors = []
+        for label, idx in queries:
+            color = category_map2[label]
+            colors.append(color)
+    else:
+        notify(f"nothing in categories file '{filename}'?!")
+
     return category_map, colors
 
 
 #
 # CLI plugin - supports 'sourmash scripts plot2'
 #
 
+
 class Command_Plot2(CommandLinePlugin):
-    command = 'plot2'             # 'scripts <command>'
-    description = "@CTB"       # output with -h
-    usage = "@CTB"               # output with no args/bad args as well as -h
-    epilog = epilog             # output with -h
-    formatter_class = argparse.RawTextHelpFormatter # do not reformat multiline
+    command = "plot2"  # 'scripts <command>'
+    description = "plot a distance matrix produced by 'sourmash compare'"  # output with -h
+    usage = "sourmash scripts plot <matrix> <labels_csv> -o <output.png>"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
 
     def __init__(self, subparser):
         super().__init__(subparser)
-        subparser.add_argument("distances",
-                               help='output from "sourmash compare"')
-        subparser.add_argument("labels_from",
-                               help='output from "sourmash compare --labels-to"')
+        subparser.add_argument("distances", help='output from "sourmash compare"')
+        subparser.add_argument(
+            "labels_from", help='output from "sourmash compare --labels-to"'
+        )
         subparser.add_argument(
             "--vmin",
             default=0.0,
             type=float,
             help="lower limit of heatmap scale; default=%(default)f",
         )
         subparser.add_argument(
@@ -127,46 +157,58 @@
             "--subsample-seed",
             type=int,
             default=1,
             metavar="S",
             help="random seed for --subsample; default=1",
         )
         subparser.add_argument(
-            "-f", "--force", action="store_true", help="forcibly plot non-distance matrices"
+            "-f",
+            "--force",
+            action="store_true",
+            help="forcibly plot non-distance matrices",
         )
         subparser.add_argument(
-            "-o", "--output-figure", help="output figure to this file",
-            required=True
+            "-o", "--output-figure", help="output figure to this file", required=True
         )
         subparser.add_argument(
-            "--cut-point", type=float,
-            help="cut point for dendrogram, to produce clusters"
+            "--cut-point",
+            type=float,
+            help="cut point for dendrogram, to produce clusters",
         )
         subparser.add_argument(
-            "--cluster-out", action='store_true',
-            help="output clusters"
+            "--cluster-out", action="store_true", help="output clusters"
         )
         subparser.add_argument(
-            "--cluster-prefix", default=None,
-            help="prefix to prepend to cluster names; default is cmp file"
+            "--cluster-prefix",
+            default=None,
+            help="prefix to prepend to cluster names; default is cmp file",
         )
         subparser.add_argument(
-            "--dendrogram-only", "--no-matrix", action='store_true',
-            help="plot only the dendrogram"
+            "--dendrogram-only",
+            "--no-matrix",
+            action="store_true",
+            help="plot only the dendrogram",
         )
 
     def main(self, args):
-        # code that we actually run.
         super().main(args)
         plot2(args)
 
 
 def plot_composite_matrix(
-    D, labelinfo, show_labels=True, vmax=1.0, vmin=0.0, force=False,
-        cut_point=None, figsize_x=11, figsize_y=8, dendrogram_only=False,
+    D,
+    labelinfo,
+    show_labels=True,
+    vmax=1.0,
+    vmin=0.0,
+    force=False,
+    cut_point=None,
+    figsize_x=11,
+    figsize_y=8,
+    dendrogram_only=False,
 ):
     """Build a composite plot showing dendrogram + distance matrix/heatmap.
 
     Returns a matplotlib figure.
 
     If show_labels is True, display labels. Otherwise, no labels are
     shown on the plot.
@@ -190,27 +232,27 @@
     # plot dendrogram
     Y = sch.linkage(D, method="single")  # centroid
 
     dend_kwargs = {}
     if cut_point is not None:
         cut_point = float(cut_point)
         dend_kwargs = dict(color_threshold=float(cut_point))
-        
-    labeltext = [ row['label'] for row in labelinfo ]
+
+    labeltext = [row["label"] for row in labelinfo]
     Z1 = sch.dendrogram(
         Y,
         orientation="left",
         labels=labeltext,
         no_labels=not show_labels,
         get_leaves=True,
     )
-    #ax1.set_xticks([])
+    # ax1.set_xticks([])
 
     if cut_point is not None:
-        ax1.axvline(x=cut_point, c='red', linestyle='dashed')
+        ax1.axvline(x=cut_point, c="red", linestyle="dashed")
 
     xstart = 0.45
     width = 0.45
     if not show_labels:
         xstart = 0.315
     scale_xstart = xstart + width + 0.01
 
@@ -221,16 +263,15 @@
         D = D[idx1, :]
         D = D[:, idx1]
 
         # show matrix
         axmatrix = fig.add_axes([xstart, 0.1, width, 0.6])
 
         im = axmatrix.matshow(
-            D, aspect="auto", origin="lower", cmap=pylab.cm.YlGnBu,
-            vmin=vmin, vmax=vmax
+            D, aspect="auto", origin="lower", cmap=pylab.cm.YlGnBu, vmin=vmin, vmax=vmax
         )
         axmatrix.set_xticks([])
         axmatrix.set_yticks([])
 
         # Plot colorbar.
         axcolor = fig.add_axes([scale_xstart, 0.1, 0.02, 0.6])
         pylab.colorbar(im, cax=axcolor)
@@ -285,125 +326,244 @@
         vmax=args.vmax,
         force=args.force,
         cut_point=args.cut_point,
         figsize_x=args.figsize_x,
         figsize_y=args.figsize_y,
         dendrogram_only=args.dendrogram_only,
     )
-    fig.savefig(args.output_figure, bbox_inches='tight')
+    fig.savefig(args.output_figure, bbox_inches="tight")
     notify(f"wrote numpy distance matrix to: {args.output_figure}")
 
     # re-order labels along rows, top to bottom
-    #reordered_labels = [labelinfo[i] for i in idx1]
+    # reordered_labels = [labelinfo[i] for i in idx1]
 
     # output reordered labels with their clusters?
     if args.cut_point is not None and args.cluster_out:
         cut_point = float(args.cut_point)
         prefix = args.cluster_prefix or os.path.basename(D_filename)
         notify(f"outputting clusters with prefix '{prefix}'")
 
         # generate clusters using 'fcluster'
         # @CTB 'distance'...? does this conflict with 'linkage'?
-        assignments = sch.fcluster(linkage_Z, cut_point, 'distance')
-
-        #print(assignments)
+        assignments = sch.fcluster(linkage_Z, cut_point, "distance")
 
         # reorganize labelinfo by cluster
         cluster_d = defaultdict(list)
         for cluster_n, label_row in zip(assignments, labelinfo):
             cluster_d[cluster_n].append(label_row)
 
         # output labelinfo rows.
         notify(f"writing {len(cluster_d)} clusters.")
         for k, v in cluster_d.items():
-            #print(f"cluster {k}")
-            #for row in v:
-            #    print(f"\t{row['label']}")
-
             filename = f"{prefix}.{k}.csv"
             with sourmash_args.FileOutputCSV(filename) as fp:
                 w = csv.DictWriter(fp, fieldnames=labelinfo[0].keys())
                 w.writeheader()
                 for row in v:
                     w.writerow(row)
 
 
 class Command_MDS(CommandLinePlugin):
-    command = 'mds'             # 'scripts <command>'
-    description = "@CTB"       # output with -h
-    usage = "@CTB"               # output with no args/bad args as well as -h
-    epilog = epilog             # output with -h
-    formatter_class = argparse.RawTextHelpFormatter # do not reformat multiline
+    command = "mds"  # 'scripts <command>'
+    description = "plot a 2-D multidimensional scaling plot from 'sourmash compare' output"  # output with -h
+    usage = "sourmash scripts mds <matrix> <labels_csv> -o <figure.png>"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
 
     def __init__(self, subparser):
         super().__init__(subparser)
 
-        subparser.add_argument('comparison_matrix',
-                               help="output from 'sourmash compare'")
-        subparser.add_argument('labels_from',
-                               help="output from 'sourmash compare --labels-to'")
-        subparser.add_argument('-C', '--categories-csv',
-                               help="CSV mapping label columns to categories")
-        subparser.add_argument('-o', '--output-figure', required=True)
+        subparser.add_argument(
+            "comparison_matrix", help="output from 'sourmash compare'"
+        )
+        subparser.add_argument(
+            "labels_from", help="output from 'sourmash compare --labels-to'"
+        )
+        subparser.add_argument(
+            "-C", "--categories-csv", help="CSV mapping label columns to categories"
+        )
+        subparser.add_argument("-o", "--output-figure", required=True)
 
     def main(self, args):
-        # code that we actually run.
         super().main(args)
 
-        with open(args.comparison_matrix, 'rb') as f:
+        with open(args.comparison_matrix, "rb") as f:
             mat = numpy.load(f)
 
         labelinfo = load_labelinfo_csv(args.labels_from)
 
         # load categories?
         category_map = None
         colors = None
         if args.categories_csv:
-            category_map, colors = load_categories_csv(args.categories_csv,
-                                                       labelinfo)
+            category_map, colors = load_categories_csv(args.categories_csv, labelinfo)
 
-        # Example usage
-        # Assume object indices instead of names for simplicity
-        #similarity_tuples = [(0, 1, 0.7), (0, 2, 0.4), (1, 2, 0.5)]
-        #num_objects = 3  # You should know the total number of objects
-        #sparse_matrix = create_sparse_similarity_matrix(similarity_tuples, num_objects)
-        plot_mds_sparse(mat, labelinfo, colors=colors,
-                        category_map=category_map)
+        dissim = 1 - mat
+        plot_mds(dissim, colors=colors, category_map=category_map)
 
         plt.savefig(args.output_figure)
 
 
-# @CTB unused for now
-def create_sparse_similarity_matrix(tuples, num_objects):
+class Command_PairwiseToCompare(CommandLinePlugin):
+    command = "pairwise_to_compare"  # 'scripts <command>'
+    description = "convert pairwise CSV output to a 'compare' matrix"  # output with -h
+    usage = "sourmash scripts pairwise_to_compare <pairwise_csv> -o <matrix_cmp>"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
+
+    def __init__(self, subparser):
+        super().__init__(subparser)
+
+        subparser.add_argument(
+            "pairwise_csv", help="output from 'sourmash scripts pairwise'"
+        )
+        subparser.add_argument('-o', '--output-matrix', required=True)
+        subparser.add_argument('--labels-to')
+
+    def main(self, args):
+        super().main(args)
+
+        with sourmash_args.FileInputCSV(args.pairwise_csv) as r:
+            rows = list(r)
+
+        # pick out all the distinct queries/matches.
+        print(f"loaded {len(rows)} rows from '{args.pairwise_csv}'")
+        queries = set( [ row['query_name'] for row in rows ] )
+        queries.update(set( [ row['match_name'] for row in rows ] ))
+        print(f"loaded {len(queries)} total elements")
+
+        queries = list(sorted(queries))
+
+        sample_d = {}
+        for n, sample_name in enumerate(queries):
+            sample_d[sample_name] = n
+
+        assert n == len(queries) - 1
+
+        mat = numpy.zeros((len(queries), len(queries)))
+
+        pairs = []
+        for row in rows:
+            # get unique indices for each query/match pair.
+            q = row['query_name']
+            qi = sample_d[q]
+            m = row['match_name']
+            mi = sample_d[m]
+            jaccard = float(row['jaccard'])
+
+            mat[qi, mi] = jaccard
+            mat[mi, qi] = jaccard
+
+        numpy.fill_diagonal(mat, 1)
+
+        with open(args.output_matrix, 'wb') as fp:
+            numpy.save(fp, mat)
+
+        with open(args.output_matrix + '.labels.txt', 'wt') as fp:
+            for label, n in sample_d.items():
+                fp.write(label + "\n")
+
+        if args.labels_to:
+            with open(args.labels_to, 'w', newline="") as fp:
+                w = csv.writer(fp)
+                w.writerow(['sort_order', 'label'])
+                for label, n in sample_d.items():
+                    w.writerow([n, label])
+
+
+class Command_MDS2(CommandLinePlugin):
+    command = "mds2"  # 'scripts <command>'
+    description = "plot a 2-D multidimensional scaling plot from branchwater plugin's 'pairwise' output"  # output with -h
+    usage = "sourmash scripts mds2 <matrix> -o <figure.png>"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
+
+    def __init__(self, subparser):
+        super().__init__(subparser)
+
+        subparser.add_argument(
+            "pairwise_csv", help="output from 'sourmash scripts pairwise'"
+        )
+        subparser.add_argument(
+            "-C", "--categories-csv", help="CSV mapping label columns to categories"
+        )
+        subparser.add_argument("-o", "--output-figure", required=True)
+
+    def main(self, args):
+        super().main(args)
+
+        with sourmash_args.FileInputCSV(args.pairwise_csv) as r:
+            rows = list(r)
+
+        # pick out all the distinct queries/matches.
+        print(f"loaded {len(rows)} rows from '{args.pairwise_csv}'")
+        queries = set( [ row['query_name'] for row in rows ] )
+        queries.update(set( [ row['match_name'] for row in rows ] ))
+        print(f"loaded {len(queries)} total elements")
+
+        queries = list(sorted(queries))
+
+        sample_d = {}
+        for n, sample_name in enumerate(queries):
+            sample_d[sample_name] = n
+
+        assert n == len(queries) - 1
+
+        mat = numpy.zeros((len(queries), len(queries)))
+
+        pairs = []
+        for row in rows:
+            # get unique indices for each query/match pair.
+            q = row['query_name']
+            qi = sample_d[q]
+            m = row['match_name']
+            mi = sample_d[m]
+            jaccard = float(row['jaccard'])
+
+            mat[qi, mi] = jaccard
+            mat[mi, qi] = jaccard
+
+        numpy.fill_diagonal(mat, 1)
+
+        # load categories?
+        category_map = None
+        colors = None
+        if args.categories_csv:
+            category_map, colors = load_categories_csv_for_labels(args.categories_csv, sample_d.items())
+
+        dissim = 1 - mat
+        plot_mds(dissim, colors=colors, category_map=category_map)
+
+        plt.savefig(args.output_figure)
+
+
+#@CTB unused again...
+def create_sparse_dissimilarity_matrix(tuples, num_objects):
     # Initialize matrix in LIL format for efficient setup
     similarity_matrix = lil_matrix((num_objects, num_objects))
 
     for obj1, obj2, similarity in tuples:
-        similarity_matrix[obj1, obj2] = similarity
+        similarity_matrix[obj1, obj2] = 1 - similarity
         if obj1 != obj2:
-            similarity_matrix[obj2, obj1] = similarity
+            similarity_matrix[obj2, obj1] = 1 - similarity
 
     # Ensure diagonal elements are 1
     similarity_matrix.setdiag(1)
 
-    # Convert to CSR format for efficient operations later
-    return similarity_matrix.tocsr()
-
+    # Convert to array format
+    # @CTB use tocsr or tocoo instead??
+    return similarity_matrix.toarray()
 
-def plot_mds_sparse(matrix, labelinfo, *, colors=None, category_map=None):
-    # Convert sparse similarity to dense dissimilarity matrix
-    #dissimilarities = 1 - matrix.toarray()
-    dissimilarities = 1 - matrix
 
-    mds = MDS(n_components=2, dissimilarity='precomputed', random_state=42)
-    mds_coords = mds.fit_transform(dissimilarities)
+def plot_mds(matrix, *, colors=None, category_map=None):
+    mds = MDS(n_components=2, dissimilarity="precomputed", random_state=42)
+    mds_coords = mds.fit_transform(matrix)
     plt.scatter(mds_coords[:, 0], mds_coords[:, 1], color=colors)
-    plt.xlabel('Dimension 1')
-    plt.ylabel('Dimension 2')
+    plt.xlabel("Dimension 1")
+    plt.ylabel("Dimension 2")
 
     if colors and category_map:
         # create a custom legend of just the categories
         legend_elements = []
         for k, v in category_map.items():
-            legend_elements.append(Line2D([0], [0], color=v, label=k,
-                                          marker='o', lw=0))
+            legend_elements.append(Line2D([0], [0], color=v, label=k, marker="o", lw=0))
         plt.legend(handles=legend_elements)
```

