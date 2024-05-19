# Comparing `tmp/slidingRP-1.0.0.tar.gz` & `tmp/slidingRP-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slidingRP-1.0.0.tar", last modified: Tue Oct  4 09:59:47 2022, max compression
+gzip compressed data, was "slidingRP-1.1.0.tar", last modified: Sun May 19 10:41:06 2024, max compression
```

## Comparing `slidingRP-1.0.0.tar` & `slidingRP-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 ibladmin  (1001) ibladmin  (1001)        0 2022-10-04 09:59:47.543114 slidingRP-1.0.0/
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)     1977 2022-10-04 09:59:47.543114 slidingRP-1.0.0/PKG-INFO
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)     1084 2022-10-04 08:45:41.000000 slidingRP-1.0.0/README.md
-drwxrwxr-x   0 ibladmin  (1001) ibladmin  (1001)        0 2022-10-04 09:59:47.539114 slidingRP-1.0.0/python/
-drwxrwxr-x   0 ibladmin  (1001) ibladmin  (1001)        0 2022-10-04 09:59:47.543114 slidingRP-1.0.0/python/slidingRP/
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)        0 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/__init__.py
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)     8948 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/computeEstimatedRPs.py
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)     2351 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/exampleScriptIBL.py
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)    19056 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/metrics.py
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)    19175 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/plotEstimatedRPs.py
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)     4115 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/scratch_ampFrACGFit.py
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)     9817 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/scriptTestingSimulations.py
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)     4695 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/script_testSlidingRP.py
--rw-r--r--   0 ibladmin  (1001) ibladmin  (1001)     9131 2022-10-04 08:45:41.000000 slidingRP-1.0.0/python/slidingRP/simulations.py
-drwxrwxr-x   0 ibladmin  (1001) ibladmin  (1001)        0 2022-10-04 09:59:47.543114 slidingRP-1.0.0/python/slidingRP.egg-info/
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)     1977 2022-10-04 09:59:47.000000 slidingRP-1.0.0/python/slidingRP.egg-info/PKG-INFO
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)      546 2022-10-04 09:59:47.000000 slidingRP-1.0.0/python/slidingRP.egg-info/SOURCES.txt
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)        1 2022-10-04 09:59:47.000000 slidingRP-1.0.0/python/slidingRP.egg-info/dependency_links.txt
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)       12 2022-10-04 09:59:47.000000 slidingRP-1.0.0/python/slidingRP.egg-info/requires.txt
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)       10 2022-10-04 09:59:47.000000 slidingRP-1.0.0/python/slidingRP.egg-info/top_level.txt
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)       38 2022-10-04 09:59:47.543114 slidingRP-1.0.0/setup.cfg
--rw-rw-r--   0 ibladmin  (1001) ibladmin  (1001)      999 2022-10-04 09:59:32.000000 slidingRP-1.0.0/setup.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2024-05-19 10:41:06.323487 slidingRP-1.1.0/
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     1786 2024-05-19 10:41:06.323487 slidingRP-1.1.0/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1200 2024-04-12 13:27:04.000000 slidingRP-1.1.0/README.md
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2024-05-19 10:41:06.319486 slidingRP-1.1.0/python/
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2024-05-19 10:41:06.323487 slidingRP-1.1.0/python/slidingRP/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8264 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig2_ACGMetric.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3298 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig3_simulations.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10128 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig4_HillCompConfidence.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8676 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig5_ConfROC.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3619 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig6_drift.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/__init__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    16946 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/loadSaveData.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    31832 2024-05-19 10:40:40.000000 slidingRP-1.1.0/python/slidingRP/metrics.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1885 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/scriptSavePaperFigs.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    67086 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/simulations.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1445 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/spike_sorting_benchmark.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2024-05-19 10:41:06.323487 slidingRP-1.1.0/python/slidingRP.egg-info/
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     1786 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      603 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/SOURCES.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/dependency_links.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       44 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/requires.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       10 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/top_level.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2024-05-19 10:41:06.323487 slidingRP-1.1.0/setup.cfg
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1013 2024-05-19 10:40:40.000000 slidingRP-1.1.0/setup.py
```

### Comparing `slidingRP-1.0.0/README.md` & `slidingRP-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,21 @@
 ```python
 from pathlib import Path
 import numpy as np
 import pandas as pd
 
 from slidingRP import metrics
 
-TEST_DATA_PATH = Path(slidingRP.__file__).parent.parent.joinpath("test-data", "integration")
+# get the small test datasets from the github repository first
+repo_path = "/home/ibladmin/Documents/PYTHON/int-brain-lab/slidingRefractory"
+TEST_DATA_PATH = Path(repo_path).joinpath("test-data", "integration")
 
 params = {'sampleRate': 30000, 'binSizeCorr': 1 / 30000}
 spikes = pd.read_parquet(TEST_DATA_PATH.joinpath('spikes.pqt'))
-table = slidingRP.slidingRP_all(spikes.times, spikes.clusters, **params)
+table = metrics.slidingRP_all(spikes.times, spikes.clusters, **params)
 
 assert np.allclose(pd.read_parquet(TEST_DATA_PATH.joinpath("rp_table.pqt")), pd.DataFrame(table), equal_nan=True)
 ```
 
 ### Contribute
 #### Run unit tests
 ```commandline
```

### Comparing `slidingRP-1.0.0/python/slidingRP.egg-info/SOURCES.txt` & `slidingRP-1.1.0/python/slidingRP.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 README.md
 setup.py
+python/slidingRP/Fig2_ACGMetric.py
+python/slidingRP/Fig3_simulations.py
+python/slidingRP/Fig4_HillCompConfidence.py
+python/slidingRP/Fig5_ConfROC.py
+python/slidingRP/Fig6_drift.py
 python/slidingRP/__init__.py
-python/slidingRP/computeEstimatedRPs.py
-python/slidingRP/exampleScriptIBL.py
+python/slidingRP/loadSaveData.py
 python/slidingRP/metrics.py
-python/slidingRP/plotEstimatedRPs.py
-python/slidingRP/scratch_ampFrACGFit.py
-python/slidingRP/scriptTestingSimulations.py
-python/slidingRP/script_testSlidingRP.py
+python/slidingRP/scriptSavePaperFigs.py
 python/slidingRP/simulations.py
+python/slidingRP/spike_sorting_benchmark.py
 python/slidingRP.egg-info/PKG-INFO
 python/slidingRP.egg-info/SOURCES.txt
 python/slidingRP.egg-info/dependency_links.txt
 python/slidingRP.egg-info/requires.txt
 python/slidingRP.egg-info/top_level.txt
```

### Comparing `slidingRP-1.0.0/setup.py` & `slidingRP-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="slidingRP",
-    version="1.0.0",
+    version="1.1.0",
     author="Noam Roth",
     description="Quality metric from spike trains",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/oliche/viewephys",
+    url="https://github.com/SteinmetzLab/slidingRefractory",
     project_urls={
         "Bug Tracker": "https://github.com/SteinmetzLab/slidingRefractory/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

