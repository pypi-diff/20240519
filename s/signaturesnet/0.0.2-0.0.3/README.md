# Comparing `tmp/signaturesnet-0.0.2.tar.gz` & `tmp/signaturesnet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signaturesnet-0.0.2.tar", last modified: Wed May 15 18:07:11 2024, max compression
+gzip compressed data, was "signaturesnet-0.0.3.tar", last modified: Sun May 19 17:10:04 2024, max compression
```

## Comparing `signaturesnet-0.0.2.tar` & `signaturesnet-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-15 18:07:11.702499 signaturesnet-0.0.2/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1064 2024-05-08 20:34:21.000000 signaturesnet-0.0.2/LICENSE
--rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6689 2024-05-15 18:07:11.702499 signaturesnet-0.0.2/PKG-INFO
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     6080 2024-05-15 17:47:46.000000 signaturesnet-0.0.2/README.md
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       38 2024-05-15 18:07:11.702499 signaturesnet-0.0.2/setup.cfg
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      927 2024-05-15 18:05:52.000000 signaturesnet-0.0.2/setup.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-15 18:07:11.698499 signaturesnet-0.0.2/signaturesnet/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      197 2024-05-08 20:34:21.000000 signaturesnet-0.0.2/signaturesnet/__init__.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-15 18:07:11.698499 signaturesnet-0.0.2/signaturesnet/loggers/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      189 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/loggers/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1036 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/loggers/classifier_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      668 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/loggers/errorfinder_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1689 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/loggers/finetuner_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4566 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/loggers/generator_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      600 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/loggers/nummut_logger.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-15 18:07:11.702499 signaturesnet-0.0.2/signaturesnet/models/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      229 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/models/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3269 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/models/baseline.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2102 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/models/classifier.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4185 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/models/errorfinder.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     8037 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/models/finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5396 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/models/generator.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1963 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/models/nummut.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-15 18:07:11.702499 signaturesnet-0.0.2/signaturesnet/modules/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      118 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/modules/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5444 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/modules/classified_tunning_error.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3164 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/modules/combined_finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9604 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/modules/signet_module.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1936 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/train_classifier.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3421 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/train_errorfinder.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2559 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/train_finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3030 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/train_generator.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1673 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/train_nummutnet.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-15 18:07:11.702499 signaturesnet-0.0.2/signaturesnet/trainers/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      315 2024-05-08 20:34:22.000000 signaturesnet-0.0.2/signaturesnet/trainers/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5607 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/trainers/classifier_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13270 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/trainers/error_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5319 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/trainers/finetuner_crossvalidation.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9103 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/trainers/finetuner_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9620 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/trainers/generator_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5714 2024-05-15 17:24:40.000000 signaturesnet-0.0.2/signaturesnet/trainers/nummut_trainer.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-15 18:07:11.702499 signaturesnet-0.0.2/signaturesnet.egg-info/
--rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6689 2024-05-15 18:07:11.000000 signaturesnet-0.0.2/signaturesnet.egg-info/PKG-INFO
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1352 2024-05-15 18:07:11.000000 signaturesnet-0.0.2/signaturesnet.egg-info/SOURCES.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        1 2024-05-15 18:07:11.000000 signaturesnet-0.0.2/signaturesnet.egg-info/dependency_links.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      178 2024-05-15 18:07:11.000000 signaturesnet-0.0.2/signaturesnet.egg-info/requires.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       14 2024-05-15 18:07:11.000000 signaturesnet-0.0.2/signaturesnet.egg-info/top_level.txt
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1064 2024-05-08 20:34:21.000000 signaturesnet-0.0.3/LICENSE
+-rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6876 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/PKG-INFO
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     6323 2024-05-17 07:24:47.000000 signaturesnet-0.0.3/README.md
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       38 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/setup.cfg
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      863 2024-05-19 17:06:27.000000 signaturesnet-0.0.3/setup.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.863119 signaturesnet-0.0.3/signaturesnet/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      197 2024-05-08 20:34:21.000000 signaturesnet-0.0.3/signaturesnet/__init__.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.867118 signaturesnet-0.0.3/signaturesnet/loggers/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      189 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/loggers/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1036 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/loggers/classifier_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      668 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/loggers/errorfinder_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1689 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/loggers/finetuner_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4566 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/loggers/generator_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      600 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/loggers/nummut_logger.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.867118 signaturesnet-0.0.3/signaturesnet/models/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      229 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/models/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3269 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/models/baseline.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2102 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/models/classifier.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4185 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/models/errorfinder.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     8037 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/models/finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5396 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/models/generator.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1963 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/models/nummut.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/signaturesnet/modules/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      118 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/modules/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5444 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/modules/classified_tunning_error.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3164 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/modules/combined_finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9604 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/modules/signet_module.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1936 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_classifier.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3421 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_errorfinder.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2559 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3030 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_generator.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1673 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_nummutnet.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/signaturesnet/trainers/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      315 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/trainers/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5607 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/classifier_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13270 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/error_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5319 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/finetuner_crossvalidation.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9103 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/finetuner_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9620 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/generator_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5714 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/nummut_trainer.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/signaturesnet.egg-info/
+-rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6876 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/PKG-INFO
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1352 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        1 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      122 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/requires.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       14 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/top_level.txt
```

### Comparing `signaturesnet-0.0.2/LICENSE` & `signaturesnet-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/PKG-INFO` & `signaturesnet-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: signaturesnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to manipulate mutational processes.
 Home-page: https://github.com/weghornlab/SigNet
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch==1.11
+Requires-Dist: torch
 Requires-Dist: scipy
-Requires-Dist: numpy==1.23.3
-Requires-Dist: matplotlib==3.3.4
+Requires-Dist: numpy
+Requires-Dist: matplotlib
 Requires-Dist: pandas
-Requires-Dist: seaborn==0.11.1
-Requires-Dist: scikit_optimize==0.8.1
-Requires-Dist: tqdm==4.59.0
-Requires-Dist: pyparsing==2.4.7
-Requires-Dist: PyYAML==6.0
+Requires-Dist: seaborn
+Requires-Dist: scikit_optimize
+Requires-Dist: tqdm
+Requires-Dist: pyparsing
+Requires-Dist: PyYAML
 Requires-Dist: scikit_learn
 Requires-Dist: openpyxl
 Requires-Dist: tensorboard
 Requires-Dist: wandb
 
 # SigNet
 
@@ -27,14 +27,17 @@
 As of now, it contains 3 solutions:
 
 - **[SigNet Refitter](documentation/signet_refitter.md)**: Tool for signature decomposition.
 - **[SigNet Generator](documentation/signet_generator.md)**: Tool for realistic mutational data generation.
 - **[SigNet Detector](documentation/signet_detector.md)**: Tool for mutational vector out-of-distribution detection.
 
 
+This is the official code implementation of the paper: [Mutational signature decomposition with deep neural networks reveals origins of clock-like processes and hypoxia dependencies](https://www.biorxiv.org/content/10.1101/2023.12.06.570467v1).
+By [Claudia Serrano](https://www.linkedin.com/in/claudia-serrano-colome-440aa9182/), [Oleguer Canal](https://github.com/OleguerCanal), et all.
+
 ## Readme contents
 
 You can use SigNet in 3 different ways depending on your workflow:
 
 1. **[Python Package](#python-package)**
    1. Python Package Installation
    2. Python Package Usage
@@ -49,15 +52,14 @@
 ## Python Package
 Recommended if you want to integrate SigNet as part of your python workflow, or intending to re-train models on custom data with limited ANN architectural changes.
 You can install the python package running:
 
 ```BASH
 pip install signaturesnet
 ```
-**NOTE:** *The package hasn't yet been published to [pypi](https://pypi.org/). Please refer to [Source Code](#source-code)* to use it for now.*
 
 Once installed, you can run Signet Refitter like so:
 
 ```python
 import pandas as pd
 import signaturesnet
 
@@ -161,13 +163,13 @@
 Recommended if you want to play around with the code, re-train custom models or [do contributions](documentation/).
 
 ### Downloading Source Code
 
 Clone the repo and install it as an editable pip package like so:
 
 ```BASH
-git clone git@github.com:OleguerCanal/SigNet.git
+git clone git@github.com:weghornlab/SigNet.git
 cd SigNet
 pip install -e .
 ```
 
 Refer [here](documentation/code_structure.md) for the project code organization.
```

### Comparing `signaturesnet-0.0.2/README.md` & `signaturesnet-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 As of now, it contains 3 solutions:
 
 - **[SigNet Refitter](documentation/signet_refitter.md)**: Tool for signature decomposition.
 - **[SigNet Generator](documentation/signet_generator.md)**: Tool for realistic mutational data generation.
 - **[SigNet Detector](documentation/signet_detector.md)**: Tool for mutational vector out-of-distribution detection.
 
 
+This is the official code implementation of the paper: [Mutational signature decomposition with deep neural networks reveals origins of clock-like processes and hypoxia dependencies](https://www.biorxiv.org/content/10.1101/2023.12.06.570467v1).
+By [Claudia Serrano](https://www.linkedin.com/in/claudia-serrano-colome-440aa9182/), [Oleguer Canal](https://github.com/OleguerCanal), et all.
+
 ## Readme contents
 
 You can use SigNet in 3 different ways depending on your workflow:
 
 1. **[Python Package](#python-package)**
    1. Python Package Installation
    2. Python Package Usage
@@ -27,15 +30,14 @@
 ## Python Package
 Recommended if you want to integrate SigNet as part of your python workflow, or intending to re-train models on custom data with limited ANN architectural changes.
 You can install the python package running:
 
 ```BASH
 pip install signaturesnet
 ```
-**NOTE:** *The package hasn't yet been published to [pypi](https://pypi.org/). Please refer to [Source Code](#source-code)* to use it for now.*
 
 Once installed, you can run Signet Refitter like so:
 
 ```python
 import pandas as pd
 import signaturesnet
 
@@ -139,13 +141,13 @@
 Recommended if you want to play around with the code, re-train custom models or [do contributions](documentation/).
 
 ### Downloading Source Code
 
 Clone the repo and install it as an editable pip package like so:
 
 ```BASH
-git clone git@github.com:OleguerCanal/SigNet.git
+git clone git@github.com:weghornlab/SigNet.git
 cd SigNet
 pip install -e .
 ```
 
 Refer [here](documentation/code_structure.md) for the project code organization.
```

### Comparing `signaturesnet-0.0.2/setup.py` & `signaturesnet-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='signaturesnet',
-      version='0.0.2',
+      version='0.0.3',
       description="Package to manipulate mutational processes.",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/weghornlab/SigNet',
       packages=find_packages(),
       install_requires=[
-            'torch==1.11',
+            'torch',
             'scipy',
-            'numpy==1.23.3',
-            'matplotlib==3.3.4',
+            'numpy',
+            'matplotlib',
             'pandas',
-            'seaborn==0.11.1',
-            'scikit_optimize==0.8.1',
-            'tqdm==4.59.0',
-            'pyparsing==2.4.7',
-            # 'gaussian_process==0.0.14',
-            'PyYAML==6.0',
+            'seaborn',
+            'scikit_optimize',
+            'tqdm',
+            'pyparsing',
+            # 'gaussian_process',
+            'PyYAML',
             'scikit_learn',
             'openpyxl',
             'tensorboard',
             'wandb',
       ])
```

### Comparing `signaturesnet-0.0.2/signaturesnet/loggers/classifier_logger.py` & `signaturesnet-0.0.3/signaturesnet/loggers/classifier_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/loggers/errorfinder_logger.py` & `signaturesnet-0.0.3/signaturesnet/loggers/errorfinder_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/loggers/finetuner_logger.py` & `signaturesnet-0.0.3/signaturesnet/loggers/finetuner_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/loggers/generator_logger.py` & `signaturesnet-0.0.3/signaturesnet/loggers/generator_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/loggers/nummut_logger.py` & `signaturesnet-0.0.3/signaturesnet/loggers/nummut_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/models/baseline.py` & `signaturesnet-0.0.3/signaturesnet/models/baseline.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/models/classifier.py` & `signaturesnet-0.0.3/signaturesnet/models/classifier.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/models/errorfinder.py` & `signaturesnet-0.0.3/signaturesnet/models/errorfinder.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/models/finetuner.py` & `signaturesnet-0.0.3/signaturesnet/models/finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/models/generator.py` & `signaturesnet-0.0.3/signaturesnet/models/generator.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/models/nummut.py` & `signaturesnet-0.0.3/signaturesnet/models/nummut.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/modules/classified_tunning_error.py` & `signaturesnet-0.0.3/signaturesnet/modules/classified_tunning_error.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/modules/combined_finetuner.py` & `signaturesnet-0.0.3/signaturesnet/modules/combined_finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/modules/signet_module.py` & `signaturesnet-0.0.3/signaturesnet/modules/signet_module.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/train_classifier.py` & `signaturesnet-0.0.3/signaturesnet/train_classifier.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/train_errorfinder.py` & `signaturesnet-0.0.3/signaturesnet/train_errorfinder.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/train_finetuner.py` & `signaturesnet-0.0.3/signaturesnet/train_finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/train_generator.py` & `signaturesnet-0.0.3/signaturesnet/train_generator.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/train_nummutnet.py` & `signaturesnet-0.0.3/signaturesnet/train_nummutnet.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/trainers/classifier_trainer.py` & `signaturesnet-0.0.3/signaturesnet/trainers/classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/trainers/error_trainer.py` & `signaturesnet-0.0.3/signaturesnet/trainers/error_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/trainers/finetuner_crossvalidation.py` & `signaturesnet-0.0.3/signaturesnet/trainers/finetuner_crossvalidation.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/trainers/finetuner_trainer.py` & `signaturesnet-0.0.3/signaturesnet/trainers/finetuner_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/trainers/generator_trainer.py` & `signaturesnet-0.0.3/signaturesnet/trainers/generator_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet/trainers/nummut_trainer.py` & `signaturesnet-0.0.3/signaturesnet/trainers/nummut_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.2/signaturesnet.egg-info/PKG-INFO` & `signaturesnet-0.0.3/signaturesnet.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: signaturesnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to manipulate mutational processes.
 Home-page: https://github.com/weghornlab/SigNet
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch==1.11
+Requires-Dist: torch
 Requires-Dist: scipy
-Requires-Dist: numpy==1.23.3
-Requires-Dist: matplotlib==3.3.4
+Requires-Dist: numpy
+Requires-Dist: matplotlib
 Requires-Dist: pandas
-Requires-Dist: seaborn==0.11.1
-Requires-Dist: scikit_optimize==0.8.1
-Requires-Dist: tqdm==4.59.0
-Requires-Dist: pyparsing==2.4.7
-Requires-Dist: PyYAML==6.0
+Requires-Dist: seaborn
+Requires-Dist: scikit_optimize
+Requires-Dist: tqdm
+Requires-Dist: pyparsing
+Requires-Dist: PyYAML
 Requires-Dist: scikit_learn
 Requires-Dist: openpyxl
 Requires-Dist: tensorboard
 Requires-Dist: wandb
 
 # SigNet
 
@@ -27,14 +27,17 @@
 As of now, it contains 3 solutions:
 
 - **[SigNet Refitter](documentation/signet_refitter.md)**: Tool for signature decomposition.
 - **[SigNet Generator](documentation/signet_generator.md)**: Tool for realistic mutational data generation.
 - **[SigNet Detector](documentation/signet_detector.md)**: Tool for mutational vector out-of-distribution detection.
 
 
+This is the official code implementation of the paper: [Mutational signature decomposition with deep neural networks reveals origins of clock-like processes and hypoxia dependencies](https://www.biorxiv.org/content/10.1101/2023.12.06.570467v1).
+By [Claudia Serrano](https://www.linkedin.com/in/claudia-serrano-colome-440aa9182/), [Oleguer Canal](https://github.com/OleguerCanal), et all.
+
 ## Readme contents
 
 You can use SigNet in 3 different ways depending on your workflow:
 
 1. **[Python Package](#python-package)**
    1. Python Package Installation
    2. Python Package Usage
@@ -49,15 +52,14 @@
 ## Python Package
 Recommended if you want to integrate SigNet as part of your python workflow, or intending to re-train models on custom data with limited ANN architectural changes.
 You can install the python package running:
 
 ```BASH
 pip install signaturesnet
 ```
-**NOTE:** *The package hasn't yet been published to [pypi](https://pypi.org/). Please refer to [Source Code](#source-code)* to use it for now.*
 
 Once installed, you can run Signet Refitter like so:
 
 ```python
 import pandas as pd
 import signaturesnet
 
@@ -161,13 +163,13 @@
 Recommended if you want to play around with the code, re-train custom models or [do contributions](documentation/).
 
 ### Downloading Source Code
 
 Clone the repo and install it as an editable pip package like so:
 
 ```BASH
-git clone git@github.com:OleguerCanal/SigNet.git
+git clone git@github.com:weghornlab/SigNet.git
 cd SigNet
 pip install -e .
 ```
 
 Refer [here](documentation/code_structure.md) for the project code organization.
```

### Comparing `signaturesnet-0.0.2/signaturesnet.egg-info/SOURCES.txt` & `signaturesnet-0.0.3/signaturesnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

