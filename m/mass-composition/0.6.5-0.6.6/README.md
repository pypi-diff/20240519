# Comparing `tmp/mass_composition-0.6.5.tar.gz` & `tmp/mass_composition-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.6.5.tar", max compression
+gzip compressed data, was "mass_composition-0.6.6.tar", max compression
```

## Comparing `mass_composition-0.6.5.tar` & `mass_composition-0.6.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0     1069 2024-05-17 00:46:01.317905 mass_composition-0.6.5/LICENSE
--rw-r--r--   0        0        0     3491 2024-05-17 00:46:01.317905 mass_composition-0.6.5/README.md
--rw-r--r--   0        0        0      360 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9816 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0    13884 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/dag.py
--rw-r--r--   0        0        0       59 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     6604 2024-05-17 00:46:01.721910 mass_composition-0.6.5/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0    41619 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/flowsheet.py
--rw-r--r--   0        0        0     2080 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    56291 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      908 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19483 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0     5752 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0     6623 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/stream.py
--rw-r--r--   0        0        0       42 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     4867 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0      842 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/parallel.py
--rw-r--r--   0        0        0     1033 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0     2164 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1717 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8865 2024-05-17 00:46:01.725910 mass_composition-0.6.5/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     2040 2024-05-17 00:46:01.729910 mass_composition-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 mass_composition-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-18 15:48:39.096999 mass_composition-0.6.6/LICENSE
+-rw-r--r--   0        0        0     3491 2024-05-18 15:48:39.096999 mass_composition-0.6.6/README.md
+-rw-r--r--   0        0        0      360 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9816 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0    13885 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     7275 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0    41619 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/flowsheet.py
+-rw-r--r--   0        0        0     2080 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    62872 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      908 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19483 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0     5752 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0     7737 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/stream.py
+-rw-r--r--   0        0        0       42 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     4867 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0      842 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/parallel.py
+-rw-r--r--   0        0        0     1033 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     4838 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/sklearn.py
+-rw-r--r--   0        0        0     1717 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8865 2024-05-18 15:48:39.513001 mass_composition-0.6.6/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     2123 2024-05-18 15:48:39.517001 mass_composition-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 mass_composition-0.6.6/PKG-INFO
```

### Comparing `mass_composition-0.6.5/LICENSE` & `mass_composition-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/README.md` & `mass_composition-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/balance.py` & `mass_composition-0.6.6/elphick/mass_composition/balance.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/config/config_read.py` & `mass_composition-0.6.6/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.6.6/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/dag.py` & `mass_composition-0.6.6/elphick/mass_composition/dag.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
                     self.graph.edges[edge]['mc'] = strm
                 if progress_bar:
                     # update the progress bar by one step
                     pbar.set_postfix_str(f"Processed node: {node}")
                     pbar.update()
         if progress_bar:
             pbar.close()  # Close the progress bar
-        logger.info(f"DAG execution complete for the nodes: {executed_nodes}")
+        logger.debug(f"DAG execution complete for the nodes: {executed_nodes}")
 
     def execute_node(self, node: str, strms: dict):
         """
         Executes a node in the DAG.
 
         This method takes a node and a dictionary of Stream objects. It executes the operation associated with the
         node using the Stream objects as inputs. If the node has successors and is defined, the result of the node
```

### Comparing `mass_composition-0.6.5/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.6.6/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.6.6/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.6.6/elphick/mass_composition/datasets/register.csv`

 * *Files 8% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 1,A072391_collars,..\..\datasets\A072391_collars\A072391_collars.csv,765470,True,True,True,597f5fe444270fe4409814b002b6e5cd,..\..\datasets\A072391_collars\A072391_collars.zip,A072391_collars.zip,9c01345766dc39462327c26604bddbd02db38f76118fe092bc90407e15bb5d09
 2,A072391_geo,..\..\datasets\A072391_geo\A072391_geo.csv,23544608,True,True,True,cdd8aed2841c73f3c203b995e099b590,..\..\datasets\A072391_geo\A072391_geo.zip,A072391_geo.zip,cf687584cc891fa084a45432e82747b7ef581eb21fe54f885f0b4c4f342c1641
 3,A072391_met,..\..\datasets\A072391_met\A072391_met.csv,412184,True,True,True,d2ac41f41ab7ba56f8239d63dba8a906,..\..\datasets\A072391_met\A072391_met.zip,A072391_met.zip,f4f84eeb4826755410d9979771a7e4f96afa2333586be85b775f179ece9c7bdf
 4,A072391_wireline,..\..\datasets\A072391_wireline\A072391_wireline.csv,4904606,True,True,True,6c810d264e83fe9c25576a53ebe8ff07,..\..\datasets\A072391_wireline\A072391_wireline.zip,A072391_wireline.zip,d3a566ec8806277a6c4e7a594d8e39f9e71c634947f9001766a03d32683e4baf
 5,demo_data,..\..\datasets\demo_data\demo_data.csv,284,True,True,True,746da032cebd545d165bdc5f3c9fb625,..\..\datasets\demo_data\demo_data.zip,demo_data.zip,0e294393e3980da04ba18f56a3a0a8f9fac2fa8f066f773846e23a6a9de89d8e
 6,iron_ore_sample_A072391,..\..\datasets\iron_ore_sample_A072391\iron_ore_sample_A072391.csv,10923,True,True,True,8403fb2acbc37e98738486ba5f49fa7d,..\..\datasets\iron_ore_sample_A072391\iron_ore_sample_A072391.zip,iron_ore_sample_A072391.zip,698b6ae7dacded385fcddf39070d8dfead0b769cc0127363ad9fec03f38d61b0
 7,iron_ore_sample_xyz_A072391,..\..\datasets\iron_ore_sample_xyz_A072391\iron_ore_sample_xyz_A072391.csv,14496,True,True,True,4ea605c41b073a304514a8c5e1d9cca3,..\..\datasets\iron_ore_sample_xyz_A072391\iron_ore_sample_xyz_A072391.zip,iron_ore_sample_xyz_A072391.zip,37dd3872d4da12b0a145f7f52b43c2541da44b1ef21826757dc3616aa372766d
-8,nordic_iron_ore_sink_float,..\..\datasets\nordic_iron_ore_sink_float\nordic_iron_ore_sink_float.csv,698,True,True,True,9ff12a4195620133a93ddc34c026745e,..\..\datasets\nordic_iron_ore_sink_float\nordic_iron_ore_sink_float.zip,nordic_iron_ore_sink_float.zip,13feeaa99a285f6451c4c2c8ef1f8b9737cd806b68139c6e53bb4499e1abbd40
+8,nordic_iron_ore_sink_float,..\..\datasets\nordic_iron_ore_sink_float\nordic_iron_ore_sink_float.csv,698,True,True,True,9ff12a4195620133a93ddc34c026745e,..\..\datasets\nordic_iron_ore_sink_float\nordic_iron_ore_sink_float.zip,nordic_iron_ore_sink_float.zip,f796f2b07b55466e2392cfe4b10d50f12de8ed9c39e231f216773a41d925faa1
 9,size_by_assay,..\..\datasets\size_by_assay\size_by_assay.csv,249,True,True,True,3ea813789ad8efb1b9d4cbb7d47f00a4,..\..\datasets\size_by_assay\size_by_assay.zip,size_by_assay.zip,28010532f3da6d76fa32aa2ae8c4521c83f9864f8f0972949c931a49ad982d7c
 10,size_distribution,..\..\datasets\size_distribution\size_distribution.csv,565,True,True,True,bd183c8240cceda4c9690746a69ce729,..\..\datasets\size_distribution\size_distribution.zip,size_distribution.zip,cd996c940010e859a16dbf508a9928fdbd04c9278c5eb1131873444db7382766
```

### Comparing `mass_composition-0.6.5/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.6.6/elphick/mass_composition/datasets/sample_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,25 +146,41 @@
     df_met: pd.DataFrame = load_a072391_met()
     df_met.dropna(subset=['Dry Weight Lump (kg)'], inplace=True)
     df_met['Dry Weight Lump (kg)'] = df_met['Dry Weight Lump (kg)'].apply(lambda x: x.replace('..', '.')).astype(
         'float64')
     df_met['Fe'] = df_met['Fe'].replace('MISSING', np.nan).astype('float64')
     df_met.dropna(subset=['Fe', 'Bulk_Hole_No', 'Dry Weight Fines (kg)'], inplace=True)
     df_met.columns = [col.replace('LOITotal', 'LOI') for col in df_met.columns]
+    df_met.columns = [
+        col.strip().lower().replace(' ', '_').replace('(', '').replace(')', '').replace('%', 'pct').replace('__', '_')
+        for
+        col in df_met.columns]
+    df_met = df_met.pipe(_move_suffix_to_prefix, '_head')
+    df_met = df_met.pipe(_move_suffix_to_prefix, '_lump')
     return df_met
 
 
 def demo_size_network() -> Flowsheet:
     mc_size: MassComposition = MassComposition(size_by_assay(), name='size sample')
     partition = partial(perfect, d50=0.150, dim='size')
     mc_coarse, mc_fine = mc_size.split_by_partition(partition_definition=partition)
     mc_coarse.name = 'coarse'
     mc_fine.name = 'fine'
     fs: Flowsheet = Flowsheet().from_streams([mc_size, mc_coarse, mc_fine])
     return fs
 
 
+def _move_suffix_to_prefix(df, suffix):
+    suffix_length = len(suffix)
+    for col in df.columns:
+        if col.endswith(suffix):
+            new_col = suffix[1:] + '_' + col[:-suffix_length]  # Remove the suffix and prepend it to the start
+            df.rename(columns={col: new_col}, inplace=True)
+    return df
+
+
 if __name__ == '__main__':
     df1: pd.DataFrame = size_by_assay()
     df2: pd.DataFrame = size_by_assay_2()
     df3: pd.DataFrame = size_by_assay_3()
+    df4: pd.DataFrame = iron_ore_met_sample_data()
     print('done')
```

### Comparing `mass_composition-0.6.5/elphick/mass_composition/flowsheet.py` & `mass_composition-0.6.6/elphick/mass_composition/flowsheet.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/layout.py` & `mass_composition-0.6.6/elphick/mass_composition/layout.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/mass_composition.py` & `mass_composition-0.6.6/elphick/mass_composition/mass_composition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import logging
+import os
 from copy import deepcopy
 from pathlib import Path
 from typing import Dict, List, Optional, Union, Tuple, Iterable, Callable, Set, Literal, Any
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 import xarray as xr
+from sklearn.base import BaseEstimator, RegressorMixin
 
 from elphick.mass_composition.config import read_yaml
 from elphick.mass_composition.mc_status import Status
 from elphick.mass_composition.plot import parallel_plot, comparison_plot
 from elphick.mass_composition.utils import solve_mass_moisture
 from elphick.mass_composition.utils.amenability import amenability_index
 from elphick.mass_composition.utils.interp import mass_preserving_interp
 from elphick.mass_composition.utils.pd_utils import weight_average, calculate_recovery, calculate_partition
 from elphick.mass_composition.utils.sampling import random_int
+from elphick.mass_composition.utils.sklearn import extract_feature_names, PandasPipeline
 
 from elphick.mass_composition.variables import Variables, VariableGroups
 
 
 class MassComposition:
 
     def __init__(self,
                  data: Optional[pd.DataFrame] = None,
-                 name: Optional[str] = 'unnamed',
+                 name: Optional[str] = None,
                  mass_wet_var: Optional[str] = None,
                  mass_dry_var: Optional[str] = None,
                  moisture_var: Optional[str] = None,
                  chem_vars: Optional[List[str]] = None,
                  mass_units: Optional[str] = None,
                  composition_units: Optional[str] = None,
                  constraints: Optional[Dict[str, List]] = None,
@@ -70,31 +73,43 @@
         self.variables: Optional[Variables] = None
         self.constraints: Optional[Dict[str, List]] = None
         self.status: Optional[Status] = None
 
         if data is not None:
             self.set_data(data, constraints=constraints)
 
+    @staticmethod
+    def _strip_common_prefix(df: pd.DataFrame) -> Tuple[pd.DataFrame, str]:
+        common_prefix = os.path.commonprefix(df.columns.to_list())
+        stripped_df = df.copy()
+        stripped_df.columns = [col.replace(common_prefix, '') for col in df.columns]
+        return stripped_df, common_prefix
+
     def set_data(self, data: Union[pd.DataFrame, xr.Dataset],
                  constraints: Optional[Dict[str, List]] = None):
         if isinstance(data, xr.Dataset):
             # we assume it is a compliant mc-xarray
             self._data = data
             self.variables = Variables(config=self.config['vars'],
                                        supplied=[str(v) for v in data.variables if v not in data.dims],
                                        specified_map=self._specified_columns)
         elif isinstance(data, pd.DataFrame):
+
             if sum(data.index.duplicated()) > 0:
                 raise KeyError('The data has duplicate indexes.')
             if isinstance(data.index, pd.MultiIndex) and data.index.nlevels >= 3:
                 self._logger.warning('The data has more than 2 levels in the index, which can consume excessive '
                                      'memory for large datasets.  Is this is what you intend?  Depending on your'
                                      'requirements you may be able to process ths dataset with a single index.')
 
-            data: pd.DataFrame = data.copy()
+            # seek a prefix to self assign the name
+            data, common_prefix = self._strip_common_prefix(data)
+            if common_prefix:
+                self._specified_columns = {k: v.replace(common_prefix, '') for k, v in self._specified_columns.items()
+                                           if v is not None}
 
             self.variables = Variables(config=self.config['vars'],
                                        supplied=list(data.columns),
                                        specified_map=self._specified_columns)
 
             # if interval pairs are passed as indexes then create the proper interval index
             data = self._create_interval_indexes(data=data)
@@ -105,14 +120,19 @@
             # solve or validate the moisture balance
             data = self._solve_mass_moisture(data)
 
             xr_ds = self._dataframe_to_mc_dataset(data)
 
             self._data = xr_ds
 
+            if not self._name:
+                self.rename('unnamed') if not common_prefix else self.rename(common_prefix.strip('_'))
+            else:
+                self.rename(self._name)
+
         # explicitly define the constraints
         self.constraints: Dict = self.get_constraint_bounds(constraints=constraints)
         self.status = Status(self._check_constraints())
 
     def rename(self, new_name: str) -> 'MassComposition':
         self.name = new_name
         return self
@@ -573,45 +593,140 @@
         comp: MassComposition = self.sub(other=out, name=name_2)
 
         self._post_process_split(out, comp, name_1, name_2)
 
         return out, comp
 
     def split_by_estimator(self,
-                           estimator: 'sklearn.base.BaseEstimator',
+                           estimator: PandasPipeline,
                            name_1: Optional[str] = None,
-                           name_2: Optional[str] = None) -> Tuple['MassComposition', 'MassComposition']:
+                           name_2: Optional[str] = None,
+                           extra_features: Optional[pd.DataFrame] = None,
+                           allow_prefix_mismatch: bool = False,
+                           mass_recovery_column: Optional[str] = None,
+                           mass_recovery_max: float = 1.0) -> Tuple['MassComposition', 'MassComposition']:
         """Split an object using a sklearn estimator.
 
         This method applies the function to self, resulting in two new objects. The object returned with name_1
         is the result of the estimator.predict() method.  The object returned with name_2 is the complement.
 
         See also: split, split_by_function, split_by_partition
 
         Args:
             estimator: Any sklearn estimator that transforms the dataframe from a MassComposition object into a new
              dataframe with values representing a new (output) stream using the predict method.  The returned
              dataframe structure must be identical to the input dataframe.
             name_1: The name of the stream created by the estimator.
             name_2: The name of the complement stream created by the split, which is calculated automatically.
+            extra_features: Optional additional features to pass to the estimator as features.
+            allow_prefix_mismatch: If True, allow feature names to be different and log an info message. If False,
+             raise an error when feature names are different.
+            mass_recovery_column: If provided, this indicates that the model has estimated mass recovery, not mass
+             explicitly.  This will execute a transformation of the predicted `dry` mass recovery to dry mass.
+            mass_recovery_max: The maximum mass recovery value, used to scale the mass recovery to mass.  Only
+             applicable if mass_recovery_column is provided.  Should be either 1.0 or 100.0.
+
+        Returns:
+            tuple of two MassComposition objects, the first the output of the estimator, the other the complement
+        """
+        # Extract feature names from the estimator, and get the actual features
+        feature_names: list[str] = list(extract_feature_names(estimator))
+        features: pd.DataFrame = self._get_features(feature_names, extra_features, allow_prefix_mismatch)
+
+        # Apply the estimator
+        estimates: pd.DataFrame = estimator.predict(X=features)
+        if isinstance(estimates, np.ndarray):
+            raise NotImplementedError("The estimator must return a DataFrame")
+
+        # Detect a possible prefix from the estimate columns
+        features_prefix: str = os.path.commonprefix(features.columns.to_list())
+        estimates_prefix: str = os.path.commonprefix(estimates.columns.to_list())
+
+        # If there is a prefix, check that it matches name_1, subject to allow_prefix_mismatch
+        if estimates_prefix.strip(
+                '_') and not allow_prefix_mismatch and name_1 and not name_1 == estimates_prefix.strip('_'):
+            raise ValueError(f"Common prefix mismatch: {features_prefix} and name_1: {name_1}")
+
+        # assign the output names, based on specified names, allow for prefix mismatch
+        name_1 = name_1 if name_1 else estimates_prefix.strip('_')
+
+        if mass_recovery_column:
+            # Transform the mass recovery to mass by applying the mass recovery to the dry mass of the input stream
+            if mass_recovery_max not in [1.0, 100.0]:
+                raise ValueError(f"mass_recovery_max must be either 1.0 or 100.0, not {mass_recovery_max}")
+            if mass_recovery_column not in estimates.columns:
+                raise KeyError(f"mass_recovery_column: {mass_recovery_column} not found in the estimates.")
+
+            dry_mass_var: str = self.data.mass_dry.name
+            estimates[mass_recovery_column] = estimates[mass_recovery_column] * self.data[
+                dry_mass_var].values / mass_recovery_max
+            estimates.rename(columns={mass_recovery_column: dry_mass_var}, inplace=True)
 
-        Returns:
-            tuple of two datasets, the first with the mass fraction specified, the other the complement
-        """
-        out_data: Union[pd.DataFrame, np.ndarray] = estimator.predict(self.data.to_dataframe())
-        if isinstance(out_data, np.ndarray):
-            out_data = pd.DataFrame(out_data, index=self.data.to_dataframe().index,
-                                    columns=self.data.to_dataframe().columns)
-        out: MassComposition = MassComposition(name=name_1, constraints=self.constraints, data=out_data)
+        estimates.columns = [f.replace(estimates_prefix, "") for f in estimates.columns]
+
+        out: MassComposition = MassComposition(name=name_1, constraints=self.constraints, data=estimates)
         comp: MassComposition = self.sub(other=out, name=name_2)
 
         self._post_process_split(out, comp, name_1, name_2)
 
         return out, comp
 
+    def _get_features(self, feature_names: List[str], allow_prefix_mismatch: bool,
+                      extra_features: Optional[pd.DataFrame] = None,) -> pd.DataFrame:
+        """
+        This method checks if the feature names required by an estimator are present in the data. If not, it tries to
+        match the feature names by considering a common prefix. If a match is found, the columns in the data are renamed
+        accordingly. If a match is not found and `allow_prefix_mismatch` is False, an error is raised. If
+        `allow_prefix_mismatch` is True, the method proceeds with the mismatched feature names.
+
+        If `extra_features` is provided, these features are added to the data.
+
+        Args:
+            feature_names (List[str]): A list of feature names required by the estimator.
+            allow_prefix_mismatch (bool): If True, allows the feature names in the data and the estimator to be different.
+            extra_features (Optional[pd.DataFrame]): Additional features to be added to the data.
+
+        Returns:
+            pd.DataFrame: The data with the correct feature names.
+
+        Raises:
+            ValueError: If `allow_prefix_mismatch` is False and the feature names in the data and the estimator do not match.
+        """
+
+        # Create a mapping of lower-case feature names to original feature names
+        feature_name_map = {name.lower(): name for name in feature_names}
+
+        df_features: pd.DataFrame = self.data.to_dataframe()
+        if extra_features:
+            df_features = pd.concat([df_features, extra_features], axis=1)
+
+        missing_features = set(f.lower() for f in feature_names) - set(c.lower() for c in df_features.columns)
+
+        if missing_features:
+            prefix: str = f"{self.name}_"
+            common_prefix: str = os.path.commonprefix(feature_names)
+            if common_prefix and common_prefix != prefix and allow_prefix_mismatch:
+                prefix = common_prefix
+
+            # create a map to support renaming the columns
+            prefixed_feature_map: dict[str, str] = {f: feature_name_map.get(f"{prefix}{f.lower()}") for f in
+                                                    df_features.columns if
+                                                    feature_name_map.get(f"{prefix}{f.lower()}") is not None}
+            df_features.rename(columns=prefixed_feature_map, inplace=True)
+            missing_features = set(f.lower() for f in feature_names) - set(c.lower() for c in df_features.columns)
+
+            if missing_features:
+                raise ValueError(f"Missing features: {missing_features}, with mc.name: {self.name}, prefix: {prefix}"
+                                 f" and allow_prefix_mismatch set to {allow_prefix_mismatch}.")
+
+        # Return the dataframe with the selected features
+        df_features: pd.DataFrame = df_features[feature_names]
+
+        return df_features
+
     def calculate_partition(self, ref: 'MassComposition') -> pd.DataFrame:
         """Calculate the partition of the ref stream relative to self"""
         self._check_one_dim_interval()
         return calculate_partition(df_feed=self.data.to_dataframe(), df_ref=ref.data.to_dataframe(),
                                    col_mass_dry='mass_dry')
 
     # def resample(self, dim: str, num_intervals: int = 50, edge_precision: int = 8) -> 'MassComposition':
```

### Comparing `mass_composition-0.6.5/elphick/mass_composition/mc_node.py` & `mass_composition-0.6.6/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/mc_status.py` & `mass_composition-0.6.6/elphick/mass_composition/mc_status.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.6.6/elphick/mass_composition/mc_xarray.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/plot.py` & `mass_composition-0.6.6/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.6.6/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.6.6/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.6.6/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/components.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/interp.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/loader.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/loader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/parallel.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/partition.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/size.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/size.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/utils/viz.py` & `mass_composition-0.6.6/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/elphick/mass_composition/variables.py` & `mass_composition-0.6.6/elphick/mass_composition/variables.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.5/pyproject.toml` & `mass_composition-0.6.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.6.5"
+version = "0.6.6"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
 
@@ -43,18 +43,21 @@
 jsonpickle = ">=3.0.1"
 
 kaleido = { version = "0.2.1", optional = true }
 statsmodels = { version = ">=0.14.0", optional = true }
 networkx = { version = ">2.0,<4.0", optional = true }
 joblib = {version = "^1.4.0", optional = true}
 tqdm = {version = "^4.66.2", optional = true}
+scikit-learn = {version = ">=1.0", optional = true}
+
 
 [tool.poetry.extras]
 viz = ["kaleido", "statsmodels"]
 network = ["networkx", "joblib", "tqdm"]
+estimation = ["scikit-learn"]
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.0.5"
 notebook = "^6.5.2"
 pytest = "^7.2.0"
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `mass_composition-0.6.5/PKG-INFO` & `mass_composition-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.6.5
+Version: 0.6.6
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: estimation
 Provides-Extra: network
 Provides-Extra: viz
 Requires-Dist: joblib (>=1.4.0,<2.0.0) ; extra == "network"
 Requires-Dist: jsonpickle (>=3.0.1)
 Requires-Dist: kaleido (==0.2.1) ; extra == "viz"
 Requires-Dist: matplotlib (>=3.3,<4.0)
 Requires-Dist: networkx (>2.0,<4.0) ; extra == "network"
 Requires-Dist: periodictable (>=1.6.1,<2.0.0)
 Requires-Dist: plotly (>=5.3,<6.0)
 Requires-Dist: pooch (>=1.7.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: scikit-learn (>=1.0) ; extra == "estimation"
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: seaborn (>0.11)
 Requires-Dist: statsmodels (>=0.14.0) ; extra == "viz"
 Requires-Dist: tqdm (>=4.66.2,<5.0.0) ; extra == "network"
 Requires-Dist: xarray (>=2022.6.0)
 Project-URL: Documentation, https://elphick.github.io/mass-composition
 Project-URL: Repository, https://github.com/elphick/mass-composition
```

