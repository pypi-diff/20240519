# Comparing `tmp/gridlooper-0.0.1.tar.gz` & `tmp/gridlooper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridlooper-0.0.1.tar", last modified: Fri Apr 12 21:44:38 2024, max compression
+gzip compressed data, was "gridlooper-0.0.2.tar", last modified: Sun May 19 00:16:03 2024, max compression
```

## Comparing `gridlooper-0.0.1.tar` & `gridlooper-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:44:38.284627 gridlooper-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-12 21:41:36.000000 gridlooper-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-12 21:44:38.284627 gridlooper-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-12 21:41:36.000000 gridlooper-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:44:38.284627 gridlooper-0.0.1/gridlooper/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 21:44:36.000000 gridlooper-0.0.1/gridlooper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-12 21:44:36.000000 gridlooper-0.0.1/gridlooper/gridlooper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-12 21:44:37.000000 gridlooper-0.0.1/gridlooper/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:44:38.284627 gridlooper-0.0.1/gridlooper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-12 21:44:38.000000 gridlooper-0.0.1/gridlooper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-12 21:44:38.000000 gridlooper-0.0.1/gridlooper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:44:38.000000 gridlooper-0.0.1/gridlooper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 21:44:38.000000 gridlooper-0.0.1/gridlooper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 21:44:38.000000 gridlooper-0.0.1/gridlooper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:44:38.284627 gridlooper-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:16:03.969398 gridlooper-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-19 00:13:01.000000 gridlooper-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-19 00:16:03.969398 gridlooper-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-19 00:13:01.000000 gridlooper-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:16:03.969398 gridlooper-0.0.2/gridlooper/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 00:15:54.000000 gridlooper-0.0.2/gridlooper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-05-19 00:15:54.000000 gridlooper-0.0.2/gridlooper/gridlooper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-19 00:16:03.000000 gridlooper-0.0.2/gridlooper/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:16:03.969398 gridlooper-0.0.2/gridlooper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-19 00:16:03.000000 gridlooper-0.0.2/gridlooper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-19 00:16:03.000000 gridlooper-0.0.2/gridlooper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 00:16:03.000000 gridlooper-0.0.2/gridlooper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 00:16:03.000000 gridlooper-0.0.2/gridlooper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 00:16:03.000000 gridlooper-0.0.2/gridlooper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 00:16:03.969398 gridlooper-0.0.2/setup.cfg
```

### Comparing `gridlooper-0.0.1/LICENSE` & `gridlooper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridlooper-0.0.1/PKG-INFO` & `gridlooper-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridlooper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to run experiments based on defined grid and function with single iteration.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -99,50 +99,50 @@
 
 gl.experiment_configs
 ```
 
 
 
 
-    [{'c': 100,
-      'runner_params': {'a': '1', 'b': 2},
-      'config_id': '8562104a0147be32e0a7611eb5229773906d12c2614826c5fc16b05b76466aba'},
-     {'c': 100,
-      'runner_params': {'a': '2', 'b': 2},
-      'config_id': 'a6148a8d9c48e610c40e5fdde002c1601a0c0344b7df4dcd458dbe7e6fe27772'},
-     {'c': 100,
-      'runner_params': {'a': '4', 'b': 2},
-      'config_id': '53bc174470bf27ac5b821773d691f6290dd546a703461cde818e1b18eb5224c8'},
-     {'c': 100,
-      'runner_params': {'a': '4', 'b': 6},
-      'config_id': 'c341935f88d73f9c0919bdfb061a6d6548ceb83a24e88ce2bda409e489e57e11'},
-     {'c': 100,
-      'runner_params': {'a': '4', 'b': 10},
-      'config_id': 'd5643e3314c572d7c65c86cf5f36686891b306473f5958f7d019ecaad768a6d8'},
-     {'c': 100,
-      'runner_params': {'a': '4', 'b': 100},
-      'config_id': '4500841c83a8731c56f661b570a7f2a754e2808c41de44a5dd7097accdb437ce'},
-     {'c': 500,
-      'runner_params': {'a': '1', 'b': 2},
-      'config_id': '3757452851f2829021b4cf33d08f0fe8049ca4617e6dead2f78aa45db48eeeb4'},
-     {'c': 500,
-      'runner_params': {'a': '2', 'b': 2},
-      'config_id': '598e1072c1d2953abffc9cb2518b09daec7fc78d261920a328a9396820cd3edd'},
-     {'c': 500,
-      'runner_params': {'a': '4', 'b': 2},
-      'config_id': '052e617f5141d37da96e804759603c6d0e8df10dfb5489cf383ed2813b8f87b8'},
-     {'c': 500,
-      'runner_params': {'a': '4', 'b': 6},
-      'config_id': '5c862e5bfeab31aa17483a39a92b455401e49679b1fa3f191beaebec74b396d7'},
-     {'c': 500,
-      'runner_params': {'a': '4', 'b': 10},
-      'config_id': 'aded884015788f0e9152cbb286604945e7a2f109309a8059efbe35a801ff8b54'},
-     {'c': 500,
-      'runner_params': {'a': '4', 'b': 100},
-      'config_id': 'c2900743d454591bcce89c767591edf9044c2c77baae1e271f19a3570f2b0c8f'}]
+    [{'runner_params': {'a': '1', 'b': 2},
+      'c': 100,
+      'config_id': '54eac3ee5ce6ae6d126502ee87dbbafce54111b346b895e1d5e29c50097fa800'},
+     {'runner_params': {'a': '1', 'b': 2},
+      'c': 500,
+      'config_id': 'b2ef1c49a36375e88203f9ff1f01db69457fc9eb6435333aaafee68bb871d9da'},
+     {'runner_params': {'a': '2', 'b': 2},
+      'c': 100,
+      'config_id': '4b1a723841dbf9f6e2a415159d0deb938373ba21506285289e46cafdcf455f05'},
+     {'runner_params': {'a': '2', 'b': 2},
+      'c': 500,
+      'config_id': '44a22efdfe7e385b4fbaeb84976ac0d10703a98902ce134cddd1000e09ba156a'},
+     {'runner_params': {'a': '4', 'b': 2},
+      'c': 100,
+      'config_id': '6dc5a94f832532513b1d739fdad694029b6b9d97cec9fa869ce3d75b822c23ce'},
+     {'runner_params': {'a': '4', 'b': 2},
+      'c': 500,
+      'config_id': '9e7ec3d2e9d7d5ccf4b8c05b9a7a145fc443f77cd7031dcdaf139a77f88d5944'},
+     {'runner_params': {'a': '4', 'b': 6},
+      'c': 100,
+      'config_id': 'dcd7c1aeb1b3c41ab924ece9ed471d682cef319304a9675dfd1f7d27f6e29c7c'},
+     {'runner_params': {'a': '4', 'b': 6},
+      'c': 500,
+      'config_id': 'ad38629f25dd962d157ee8b36b1fc34a54079f8b08d0d4e79fd45cecfa167d49'},
+     {'runner_params': {'a': '4', 'b': 10},
+      'c': 100,
+      'config_id': '6cd8cc53587798f4fc2583a122a7cad6e79cb7b6c10639e6a9714d12fa2c3092'},
+     {'runner_params': {'a': '4', 'b': 10},
+      'c': 500,
+      'config_id': '495efcc2399e24fed5a5dee4b3909f27688b7723eb62b28be6ff6eb74c4e8574'},
+     {'runner_params': {'a': '4', 'b': 100},
+      'c': 100,
+      'config_id': '2dcdd7a719ce8fa4731c8d9adefd131d809fd29e014aa9acd3be8a6538cc8765'},
+     {'runner_params': {'a': '4', 'b': 100},
+      'c': 500,
+      'config_id': '64f83d857c2c3a0030bd187330da30dc6d4aaf2ae1418f150b9902a269a4f3d8'}]
 
 
 
 ### 3. Running experiments
 
 `executing_experimets` function will run `runner_function` for each set of parameters from defined `experiment_configs` for a select loop strategy.
 
@@ -156,36 +156,36 @@
     loop_type= 'brute',
     save_path = 'example_run.dill'
 )
 ```
 
     Looping:   0%|          | 0/12 [00:00<?, ?item/s]
 
-    Looping: 100%|██████████| 12/12 [00:00<00:00, 136400.13item/s]
+    Looping: 100%|██████████| 12/12 [00:00<00:00, 156796.41item/s]
 
     
 
 
 ### 4. Analysing results
 
 
 ```python
 gl.experiment_results['results']
 ```
 
 
 
 
-    {'8562104a0147be32e0a7611eb5229773906d12c2614826c5fc16b05b76466aba': 103,
-     'a6148a8d9c48e610c40e5fdde002c1601a0c0344b7df4dcd458dbe7e6fe27772': 104,
-     '53bc174470bf27ac5b821773d691f6290dd546a703461cde818e1b18eb5224c8': 106,
-     'c341935f88d73f9c0919bdfb061a6d6548ceb83a24e88ce2bda409e489e57e11': 110,
-     'd5643e3314c572d7c65c86cf5f36686891b306473f5958f7d019ecaad768a6d8': 114,
-     '4500841c83a8731c56f661b570a7f2a754e2808c41de44a5dd7097accdb437ce': 204,
-     '3757452851f2829021b4cf33d08f0fe8049ca4617e6dead2f78aa45db48eeeb4': 503,
-     '598e1072c1d2953abffc9cb2518b09daec7fc78d261920a328a9396820cd3edd': 504,
-     '052e617f5141d37da96e804759603c6d0e8df10dfb5489cf383ed2813b8f87b8': 506,
-     '5c862e5bfeab31aa17483a39a92b455401e49679b1fa3f191beaebec74b396d7': 510,
-     'aded884015788f0e9152cbb286604945e7a2f109309a8059efbe35a801ff8b54': 514,
-     'c2900743d454591bcce89c767591edf9044c2c77baae1e271f19a3570f2b0c8f': 604}
+    {'54eac3ee5ce6ae6d126502ee87dbbafce54111b346b895e1d5e29c50097fa800': 103,
+     'b2ef1c49a36375e88203f9ff1f01db69457fc9eb6435333aaafee68bb871d9da': 503,
+     '4b1a723841dbf9f6e2a415159d0deb938373ba21506285289e46cafdcf455f05': 104,
+     '44a22efdfe7e385b4fbaeb84976ac0d10703a98902ce134cddd1000e09ba156a': 504,
+     '6dc5a94f832532513b1d739fdad694029b6b9d97cec9fa869ce3d75b822c23ce': 106,
+     '9e7ec3d2e9d7d5ccf4b8c05b9a7a145fc443f77cd7031dcdaf139a77f88d5944': 506,
+     'dcd7c1aeb1b3c41ab924ece9ed471d682cef319304a9675dfd1f7d27f6e29c7c': 110,
+     'ad38629f25dd962d157ee8b36b1fc34a54079f8b08d0d4e79fd45cecfa167d49': 510,
+     '6cd8cc53587798f4fc2583a122a7cad6e79cb7b6c10639e6a9714d12fa2c3092': 114,
+     '495efcc2399e24fed5a5dee4b3909f27688b7723eb62b28be6ff6eb74c4e8574': 514,
+     '2dcdd7a719ce8fa4731c8d9adefd131d809fd29e014aa9acd3be8a6538cc8765': 204,
+     '64f83d857c2c3a0030bd187330da30dc6d4aaf2ae1418f150b9902a269a4f3d8': 604}
```

### Comparing `gridlooper-0.0.1/README.md` & `gridlooper-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -19,52 +19,57 @@
 ## Content:
  
 [module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
 
 This module provides a set of functions for interacting with the Google Drive API.
 It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
 
+[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [release notes](release_notes/package_auto_assembler.md) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
+
+This tool is meant to streamline creation of single module packages.
+Its purpose is to automate as many aspects of python package creation as possible,
+to shorten a development cycle of reusable components, maintain certain standard of quality
+for reusable code. It provides tool to simplify the process of package creatrion
+to a point that it can be triggered automatically within ci/cd pipelines,
+with minimal preparations and requirements for new modules.
+
+[module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [release notes](release_notes/parameterframe.md) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameterframe
+
+The module provides an interface for managing solution parameters.
+It allows for the structured storage and retrieval of parameter sets from a database.
+
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
 Designed to automate and streamline the process of comparing textual data, particularly focusing on various metrics
 such as character and word count, punctuation usage, and semantic similarity.
 It's particularly useful for scenarios where consistent text analysis is required,
 such as evaluating the performance of natural language processing models, monitoring content quality,
 or tracking changes in textual data over time using manual evaluation.
 
+[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
+
+This class uses the logging module to create and manage a logger for displaying formatted messages.
+It provides a method to output various types of lines and headers, with customizable message and line lengths.
+The purpose is to be integrated into other classes that also use logger.
+
+[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [release notes](release_notes/gridlooper.md) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
+
+A tool to run experiments based on defined grid and function with single iteration.
+
 [module](python_modules/mocker_db.py) | [usage](docs/mocker_db.md) | [drawio: -flow](docs/mocker_db-flow.png) | [release notes](release_notes/mocker_db.md) | [![PyPiVersion](https://img.shields.io/pypi/v/mocker-db)](https://pypi.org/project/mocker-db/) - MockerDB
 
 A python module that contains mock vector database like solution built around
 dictionary data type. It contains methods necessary to interact with this 'database',
 embed, search and persist.
 
-[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) - Grid Looper
-
-A tool to run experiments based on defined grid and function with single iteration.
-
 [module](python_modules/search_based_extractor.py) | [usage](docs/search_based_extractor.md) - Search Based Extractor
 
 Utility to simplify webscraping by taking advantave of search and assumptions about html structure.
 Extractor allows to find parent html element that contains searched term, record path to it in a file
 and reuse that to scrape data with same html structure.
 
 [module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
 
 A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
 The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
 with a use of more expensive, slower or simply no-existant method.
 
-[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
-
-This tool is meant to streamline creation of single module packages.
-Its purpose is to automate as many aspects of python package creation as possible,
-to shorten a development cycle of reusable components, maintain certain standard of quality
-for reusable code. It provides tool to simplify the process of package creatrion
-to a point that it can be triggered automatically within ci/cd pipelines,
-with minimal preparations and requirements for new modules.
-
-[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
-
-This class uses the logging module to create and manage a logger for displaying formatted messages.
-It provides a method to output various types of lines and headers, with customizable message and line lengths.
-The purpose is to be integrated into other classes that also use logger.
-
```

### Comparing `gridlooper-0.0.1/gridlooper/gridlooper.py` & `gridlooper-0.0.2/gridlooper/gridlooper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Grid Looper
 
 A tool to run experiments based on defined grid and function with single iteration.
 """
 
-import logging
-import attr #>=22.2.0
-from itertools import product
-import dill #==0.3.7
 ## for making keys
 import hashlib
 import json
-## to track time
+
+import logging
+
 from datetime import datetime
+from itertools import product
 from tqdm import tqdm
 
+import attr #>=22.2.0
+import dill #==0.3.7
+
 
 __design_choices__ = {
 }
 
 # Metadata for package creation
 __package_metadata__ = {
     "author": "Kyrylo Mordan",
@@ -26,28 +28,34 @@
     "description": "A tool to run experiments based on defined grid and function with single iteration.",
     # Add other metadata as needed
 }
 
 @attr.s
 class GridLooper:
 
+    """
+    A tool to run experiments based on defined grid and function with single iteration.
+    """
+
     # for defining grid
     experiments_settings = attr.ib(default=None)
     exclusion_keys = attr.ib(default=None)
     exclusion_combos = attr.ib(default=None)
 
     # for runnning experiment
     runner_function = attr.ib(default=None)
     loop_type = attr.ib(default='brute')
     data = attr.ib(default=None)
 
     # for saving
     save_path = attr.ib(default='./experiments.dill')
 
     # outputs
+    runner_results = attr.ib(default=None,init=None)
+    runner_time = attr.ib(default=None,init=None)
     experiment_configs = attr.ib(default=None,init=None)
     experiment_results = attr.ib(default=None,init=None)
     experiment_config_ids = attr.ib(default=None,init=None)
 
     logger = attr.ib(default=None)
     logger_name = attr.ib(default='Similarity search')
     loggerLvl = attr.ib(default=logging.INFO)
@@ -87,15 +95,16 @@
         Generate all combinations for keys in a dictionary, handling both
         dictionary and non-dictionary values.
         """
         combinations = []
         for key, values in settings_dict.items():
             if isinstance(values, dict):
                 # Generate combinations for nested dictionaries
-                nested_combinations = list(product(*[[(nested_key, value) for value in nested_values] for nested_key, nested_values in values.items()]))
+                nested_combinations = list(product(*[[(nested_key, value) for value in nested_values] \
+                    for nested_key, nested_values in values.items()]))
                 combinations.extend([(key, dict(combo)) for combo in nested_combinations])
             else:
                 # Directly use values for non-dictionary types
                 combinations.extend([(key, value) for value in values])
         return combinations
 
     def _generate_experiment_configurations(self,
@@ -107,15 +116,16 @@
         # Extract keys for combination generation, excluding excepted keys
         if excepted_keys is not None:
             keys_to_combine = set(experiments_settings.keys()) - excepted_keys
         else:
             keys_to_combine = set(experiments_settings.keys())
 
         # Generate combinations for each key
-        all_combinations = [self._expand_dict_combinations({key: experiments_settings[key]}) for key in keys_to_combine if key in experiments_settings]
+        all_combinations = [self._expand_dict_combinations({key: experiments_settings[key]}) \
+            for key in keys_to_combine if key in experiments_settings]
 
         # Compute the cartesian product of all combinations
         product_combinations = list(product(*all_combinations))
 
         # Convert combinations into dictionary format
         experiment_configs = []
         for combination in product_combinations:
@@ -278,9 +288,7 @@
                               'exlusions' : self.exclusion_combos,
                               'results' : self.runner_results,
                               'time' : self.runner_time}
 
 
         with open(save_path, 'wb') as file:
             dill.dump(self.experiment_results, file)
-
-
```

### Comparing `gridlooper-0.0.1/gridlooper/setup.py` & `gridlooper-0.0.2/gridlooper/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="gridlooper",
     packages=["gridlooper"],
-    install_requires=['### gridlooper.py', 'dill==0.3.7', 'attrs>=22.2.0', 'tqdm'],
+    install_requires=['### gridlooper.py', 'dill==0.3.7', 'tqdm', 'attrs>=22.2.0'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to run experiments based on defined grid and function with single iteration.", version="0.0.1"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to run experiments based on defined grid and function with single iteration.", version="0.0.2"
 )
```

### Comparing `gridlooper-0.0.1/gridlooper.egg-info/PKG-INFO` & `gridlooper-0.0.2/gridlooper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridlooper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to run experiments based on defined grid and function with single iteration.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -99,50 +99,50 @@
 
 gl.experiment_configs
 ```
 
 
 
 
-    [{'c': 100,
-      'runner_params': {'a': '1', 'b': 2},
-      'config_id': '8562104a0147be32e0a7611eb5229773906d12c2614826c5fc16b05b76466aba'},
-     {'c': 100,
-      'runner_params': {'a': '2', 'b': 2},
-      'config_id': 'a6148a8d9c48e610c40e5fdde002c1601a0c0344b7df4dcd458dbe7e6fe27772'},
-     {'c': 100,
-      'runner_params': {'a': '4', 'b': 2},
-      'config_id': '53bc174470bf27ac5b821773d691f6290dd546a703461cde818e1b18eb5224c8'},
-     {'c': 100,
-      'runner_params': {'a': '4', 'b': 6},
-      'config_id': 'c341935f88d73f9c0919bdfb061a6d6548ceb83a24e88ce2bda409e489e57e11'},
-     {'c': 100,
-      'runner_params': {'a': '4', 'b': 10},
-      'config_id': 'd5643e3314c572d7c65c86cf5f36686891b306473f5958f7d019ecaad768a6d8'},
-     {'c': 100,
-      'runner_params': {'a': '4', 'b': 100},
-      'config_id': '4500841c83a8731c56f661b570a7f2a754e2808c41de44a5dd7097accdb437ce'},
-     {'c': 500,
-      'runner_params': {'a': '1', 'b': 2},
-      'config_id': '3757452851f2829021b4cf33d08f0fe8049ca4617e6dead2f78aa45db48eeeb4'},
-     {'c': 500,
-      'runner_params': {'a': '2', 'b': 2},
-      'config_id': '598e1072c1d2953abffc9cb2518b09daec7fc78d261920a328a9396820cd3edd'},
-     {'c': 500,
-      'runner_params': {'a': '4', 'b': 2},
-      'config_id': '052e617f5141d37da96e804759603c6d0e8df10dfb5489cf383ed2813b8f87b8'},
-     {'c': 500,
-      'runner_params': {'a': '4', 'b': 6},
-      'config_id': '5c862e5bfeab31aa17483a39a92b455401e49679b1fa3f191beaebec74b396d7'},
-     {'c': 500,
-      'runner_params': {'a': '4', 'b': 10},
-      'config_id': 'aded884015788f0e9152cbb286604945e7a2f109309a8059efbe35a801ff8b54'},
-     {'c': 500,
-      'runner_params': {'a': '4', 'b': 100},
-      'config_id': 'c2900743d454591bcce89c767591edf9044c2c77baae1e271f19a3570f2b0c8f'}]
+    [{'runner_params': {'a': '1', 'b': 2},
+      'c': 100,
+      'config_id': '54eac3ee5ce6ae6d126502ee87dbbafce54111b346b895e1d5e29c50097fa800'},
+     {'runner_params': {'a': '1', 'b': 2},
+      'c': 500,
+      'config_id': 'b2ef1c49a36375e88203f9ff1f01db69457fc9eb6435333aaafee68bb871d9da'},
+     {'runner_params': {'a': '2', 'b': 2},
+      'c': 100,
+      'config_id': '4b1a723841dbf9f6e2a415159d0deb938373ba21506285289e46cafdcf455f05'},
+     {'runner_params': {'a': '2', 'b': 2},
+      'c': 500,
+      'config_id': '44a22efdfe7e385b4fbaeb84976ac0d10703a98902ce134cddd1000e09ba156a'},
+     {'runner_params': {'a': '4', 'b': 2},
+      'c': 100,
+      'config_id': '6dc5a94f832532513b1d739fdad694029b6b9d97cec9fa869ce3d75b822c23ce'},
+     {'runner_params': {'a': '4', 'b': 2},
+      'c': 500,
+      'config_id': '9e7ec3d2e9d7d5ccf4b8c05b9a7a145fc443f77cd7031dcdaf139a77f88d5944'},
+     {'runner_params': {'a': '4', 'b': 6},
+      'c': 100,
+      'config_id': 'dcd7c1aeb1b3c41ab924ece9ed471d682cef319304a9675dfd1f7d27f6e29c7c'},
+     {'runner_params': {'a': '4', 'b': 6},
+      'c': 500,
+      'config_id': 'ad38629f25dd962d157ee8b36b1fc34a54079f8b08d0d4e79fd45cecfa167d49'},
+     {'runner_params': {'a': '4', 'b': 10},
+      'c': 100,
+      'config_id': '6cd8cc53587798f4fc2583a122a7cad6e79cb7b6c10639e6a9714d12fa2c3092'},
+     {'runner_params': {'a': '4', 'b': 10},
+      'c': 500,
+      'config_id': '495efcc2399e24fed5a5dee4b3909f27688b7723eb62b28be6ff6eb74c4e8574'},
+     {'runner_params': {'a': '4', 'b': 100},
+      'c': 100,
+      'config_id': '2dcdd7a719ce8fa4731c8d9adefd131d809fd29e014aa9acd3be8a6538cc8765'},
+     {'runner_params': {'a': '4', 'b': 100},
+      'c': 500,
+      'config_id': '64f83d857c2c3a0030bd187330da30dc6d4aaf2ae1418f150b9902a269a4f3d8'}]
 
 
 
 ### 3. Running experiments
 
 `executing_experimets` function will run `runner_function` for each set of parameters from defined `experiment_configs` for a select loop strategy.
 
@@ -156,36 +156,36 @@
     loop_type= 'brute',
     save_path = 'example_run.dill'
 )
 ```
 
     Looping:   0%|          | 0/12 [00:00<?, ?item/s]
 
-    Looping: 100%|██████████| 12/12 [00:00<00:00, 136400.13item/s]
+    Looping: 100%|██████████| 12/12 [00:00<00:00, 156796.41item/s]
 
     
 
 
 ### 4. Analysing results
 
 
 ```python
 gl.experiment_results['results']
 ```
 
 
 
 
-    {'8562104a0147be32e0a7611eb5229773906d12c2614826c5fc16b05b76466aba': 103,
-     'a6148a8d9c48e610c40e5fdde002c1601a0c0344b7df4dcd458dbe7e6fe27772': 104,
-     '53bc174470bf27ac5b821773d691f6290dd546a703461cde818e1b18eb5224c8': 106,
-     'c341935f88d73f9c0919bdfb061a6d6548ceb83a24e88ce2bda409e489e57e11': 110,
-     'd5643e3314c572d7c65c86cf5f36686891b306473f5958f7d019ecaad768a6d8': 114,
-     '4500841c83a8731c56f661b570a7f2a754e2808c41de44a5dd7097accdb437ce': 204,
-     '3757452851f2829021b4cf33d08f0fe8049ca4617e6dead2f78aa45db48eeeb4': 503,
-     '598e1072c1d2953abffc9cb2518b09daec7fc78d261920a328a9396820cd3edd': 504,
-     '052e617f5141d37da96e804759603c6d0e8df10dfb5489cf383ed2813b8f87b8': 506,
-     '5c862e5bfeab31aa17483a39a92b455401e49679b1fa3f191beaebec74b396d7': 510,
-     'aded884015788f0e9152cbb286604945e7a2f109309a8059efbe35a801ff8b54': 514,
-     'c2900743d454591bcce89c767591edf9044c2c77baae1e271f19a3570f2b0c8f': 604}
+    {'54eac3ee5ce6ae6d126502ee87dbbafce54111b346b895e1d5e29c50097fa800': 103,
+     'b2ef1c49a36375e88203f9ff1f01db69457fc9eb6435333aaafee68bb871d9da': 503,
+     '4b1a723841dbf9f6e2a415159d0deb938373ba21506285289e46cafdcf455f05': 104,
+     '44a22efdfe7e385b4fbaeb84976ac0d10703a98902ce134cddd1000e09ba156a': 504,
+     '6dc5a94f832532513b1d739fdad694029b6b9d97cec9fa869ce3d75b822c23ce': 106,
+     '9e7ec3d2e9d7d5ccf4b8c05b9a7a145fc443f77cd7031dcdaf139a77f88d5944': 506,
+     'dcd7c1aeb1b3c41ab924ece9ed471d682cef319304a9675dfd1f7d27f6e29c7c': 110,
+     'ad38629f25dd962d157ee8b36b1fc34a54079f8b08d0d4e79fd45cecfa167d49': 510,
+     '6cd8cc53587798f4fc2583a122a7cad6e79cb7b6c10639e6a9714d12fa2c3092': 114,
+     '495efcc2399e24fed5a5dee4b3909f27688b7723eb62b28be6ff6eb74c4e8574': 514,
+     '2dcdd7a719ce8fa4731c8d9adefd131d809fd29e014aa9acd3be8a6538cc8765': 204,
+     '64f83d857c2c3a0030bd187330da30dc6d4aaf2ae1418f150b9902a269a4f3d8': 604}
```

