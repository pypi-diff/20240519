# Comparing `tmp/huracan-0.0a2.tar.gz` & `tmp/huracan-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/huracan-0.0a2.tar", last modified: Tue Sep  7 21:59:48 2021, max compression
+gzip compressed data, was "huracan-0.9.tar", last modified: Sat May 18 22:13:29 2024, max compression
```

## Comparing `huracan-0.0a2.tar` & `huracan-0.9.tar`

### file list

```diff
@@ -1,60 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/
--rw-r--r--   0 runner    (1001) docker     (121)     3437 2021-09-07 21:59:48.000000 huracan-0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2021-09-07 21:59:42.000000 huracan-0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan/components/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8455 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/components/combustion.py
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/components/electrical.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/components/rotary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2815 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/components/static.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    36622 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan/thermo/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10292 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/thermo/fluids.py
--rw-r--r--   0 runner    (1001) docker     (121)     6400 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/thermo/processes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2021-09-07 21:59:42.000000 huracan-0.0a2/huracan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3437 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-07 21:59:48.000000 huracan-0.0a2/huracan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-07 21:59:48.000000 huracan-0.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      915 2021-09-07 21:59:42.000000 huracan-0.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      798 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/tests/verification/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/tests/verification/model_verification/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/tests/verification/model_verification/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19403 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/resources/functions_propulsion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/resources/functions_turbofan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/resources/functions_turbojet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/resources/functions_turboprop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/resources/fundamentals_propulsion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/resources/utils_propulsion.py
--rw-r--r--   0 runner    (1001) docker     (121)     9357 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/turbofan.py
--rw-r--r--   0 runner    (1001) docker     (121)     9929 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/turbofan_ic_r.py
--rw-r--r--   0 runner    (1001) docker     (121)     7742 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/turbojet.py
--rw-r--r--   0 runner    (1001) docker     (121)     9662 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/model_verification/turboprop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/tests/verification/turbofan/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/turbofan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3009 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/turbofan/test_turbofan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/tests/verification/turbojet/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/turbojet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/turbojet/model_v.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/turbojet/test_turbojet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:48.000000 huracan-0.0a2/tests/verification/turboprop/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/turboprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/turboprop/model_v.py
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2021-09-07 21:59:42.000000 huracan-0.0a2/tests/verification/turboprop/test_turboprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.694739 huracan-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 22:13:22.000000 huracan-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-18 22:13:29.694739 huracan-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-18 22:13:22.000000 huracan-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.690739 huracan-0.9/huracan/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-18 22:13:22.000000 huracan-0.9/huracan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.690739 huracan-0.9/huracan/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/heat_exchangers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.690739 huracan-0.9/huracan/components/power/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/power/combustion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/power/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/power/hydrogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/power/sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-18 22:13:22.000000 huracan-0.9/huracan/components/rotary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-18 22:13:22.000000 huracan-0.9/huracan/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40917 2024-05-18 22:13:22.000000 huracan-0.9/huracan/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-18 22:13:22.000000 huracan-0.9/huracan/physical_quantities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.690739 huracan-0.9/huracan/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-18 22:13:22.000000 huracan-0.9/huracan/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-05-18 22:13:22.000000 huracan-0.9/huracan/thermo/fluids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-18 22:13:22.000000 huracan-0.9/huracan/thermo/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-18 22:13:22.000000 huracan-0.9/huracan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.690739 huracan-0.9/huracan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-18 22:13:29.000000 huracan-0.9/huracan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-18 22:13:29.000000 huracan-0.9/huracan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:13:29.000000 huracan-0.9/huracan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-18 22:13:29.000000 huracan-0.9/huracan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 22:13:29.000000 huracan-0.9/huracan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:13:29.694739 huracan-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-18 22:13:22.000000 huracan-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.690739 huracan-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 22:13:22.000000 huracan-0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-18 22:13:22.000000 huracan-0.9/tests/test_compressor_bleed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-18 22:13:22.000000 huracan-0.9/tests/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-18 22:13:22.000000 huracan-0.9/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-18 22:13:22.000000 huracan-0.9/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-18 22:13:22.000000 huracan-0.9/tests/test_turbofan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-18 22:13:22.000000 huracan-0.9/tests/test_turbojet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-18 22:13:22.000000 huracan-0.9/tests/test_turboprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-18 22:13:22.000000 huracan-0.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.694739 huracan-0.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-18 22:13:22.000000 huracan-0.9/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.694739 huracan-0.9/tests/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 22:13:22.000000 huracan-0.9/tests/verification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.694739 huracan-0.9/tests/verification/turbofan/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 22:13:22.000000 huracan-0.9/tests/verification/turbofan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-18 22:13:22.000000 huracan-0.9/tests/verification/turbofan/test_turbofan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.694739 huracan-0.9/tests/verification/turbojet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:22.000000 huracan-0.9/tests/verification/turbojet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-18 22:13:22.000000 huracan-0.9/tests/verification/turbojet/test_turbojet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:13:29.694739 huracan-0.9/tests/verification/turboprop/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 22:13:22.000000 huracan-0.9/tests/verification/turboprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-18 22:13:22.000000 huracan-0.9/tests/verification/turboprop/test_turboprop.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `huracan-0.0a2/README.md` & `huracan-0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,54 +2,53 @@
 
 Huracan is an open source, 0-dimensional, object-oriented airbreathing engine 
 modelling package for preliminary analysis and design of airbreathing engines, 
 divulgation and educational purposes.
 
 At the moment Huracan is capable of modelling engines with an arbitrary number of 
 components connected by an arbitrary number of shafts. It allows for a single 
-combustion chamber per stream and reheating. Multiple-stream systems can be modelled, 
+combustion chamber per stream, reheating, intercooling and the addition of electrical
+system power requirements. Multiple-stream systems can be modelled, 
 as well as splitting (such as the bypass flow of a turbofan) and mixing streams (such 
 as in the nozzle of a mixed exhaust turbofan).
 
 The inspiration for the project lies in traditional thermodynamic plant diagrams, 
 and similar architectures are used in well known proprietary tools such as 
 [GasTurb](https://www.gasturb.de/) and [NLR's GSP](https://www.gspteam.com/index.html).
 
 [The API reference is available here.](https://huracan-docs.github.io/)
 
-`Antonio Lopez Rivera, 2021`
-
 ## Install
 
     pip install huracan
 
 ## Examples
 
-### [Single spool turboprop engine.](https://github.com/alopezrivera/huracan/blob/master/examples/turboprop/turboprop_1s-1s.py)
+### [Single spool turboprop engine.](https://github.com/alopezrivera/huracan/blob/master/examples/engines/turboprop/turboprop_1s-1s.py)
 
-| <p align="left"><img width=625 src="docs/figures/diagram_turbofan.png" /></p> | <p align="right"><img width=250 src="docs/figures/log_turboprop.png" /></p> |
+| <p align="left"><img width=750 src="docs/figures/diagram_turboprop.png" /></p> | <p align="right"><img width=250 src="docs/figures/log_turboprop.png" /></p> |
 | --- | --- |
 
-| ![alt text](docs/figures/Tp_turboprop.png "T-p plot") |
-| --- |
-| ![alt text](docs/figures/pV_turboprop.png "p-V plot") |
+| ![alt text](docs/figures/TS_turboprop.svg "T-S plot") | ![alt text](docs/figures/pV_turboprop.svg "p-V plot") |
+| --- | --- |
+| ![alt text](docs/figures/Hp_turboprop.svg "H-p plot") | ![alt text](docs/figures/Tp_turboprop.svg "T-p plot") |
 
-### [Twin-spool, reheated turbojet engine with an electrical power plant.](https://github.com/alopezrivera/huracan/blob/master/examples/turbojet/turbojet_1s-2s.py)
+### [Twin-spool, reheated turbojet engine with an electrical power plant.](https://github.com/alopezrivera/huracan/blob/master/examples/engines/turbojet/turbojet_1s-2s-ab.py)
 
-| <p align="left"><img width=625 src="docs/figures/diagram_turbofan.png" /></p> | <p align="right"><img width=250 src="docs/figures/log_turbojet.png" /></p> |
+| <p align="left"><img width=750 src="docs/figures/diagram_turbojet.png" /></p> | <p align="right"><img width=250 src="docs/figures/log_turbojet.png" /></p> |
 | --- | --- |
 
-| ![alt text](docs/figures/Tp_turbojet.png "T-p plot") |
-| --- |
-| ![alt text](docs/figures/pV_turbojet.png "p-V plot") |
+| ![alt text](docs/figures/TS_turbojet.svg "T-S plot") | ![alt text](docs/figures/pV_turbojet.svg "p-V plot") |
+| --- | --- |
+| ![alt text](docs/figures/Hp_turbojet.svg "H-p plot") | ![alt text](docs/figures/Tp_turbojet.svg "T-p plot") |
 
-### [Three-spool, separated exhaust turbofan engine.](https://github.com/alopezrivera/huracan/blob/master/examples/turbofan/turbofan_2s-3s.py)
+### [Three-spool, separated exhaust turbofan engine.](https://github.com/alopezrivera/huracan/blob/master/examples/engines/turbofan/turbofan_2s-3s.py)
 
-| <p align="left"><img width=625 src="docs/figures/diagram_turbofan.png" /></p> | <p align="right"><img width=250 src="docs/figures/log_turbofan.png" /></p> |
+| <p align="left"><img width=750 src="docs/figures/diagram_turbofan.png" /></p> | <p align="right"><img width=250 src="docs/figures/log_turbofan.png" /></p> |
 | --- | --- |
 
-| ![alt text](docs/figures/Tp_turbofan.png "T-p plot") |
-| --- |
-| ![alt text](docs/figures/pV_turbofan.png "p-V plot") |
+| ![alt text](docs/figures/TS_turbofan.svg "T-S plot") | ![alt text](docs/figures/pV_turbofan.svg "p-V plot") |
+| --- | --- |
+| ![alt text](docs/figures/Hp_turbofan.svg "H-p plot") | ![alt text](docs/figures/Tp_turbofan.svg "T-p plot") |
 
 ---
 [Back to top](#huracan)
```

### Comparing `huracan-0.0a2/huracan/components/combustion.py` & `huracan-0.9/huracan/components/power/combustion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: GPL-3.0-only
+
+"""
+Combustion power plants
+-----------------------
+"""
+
 from copy import deepcopy
 
 from huracan.engine import component
-from huracan.components import turbine
+from huracan.components.power import plant
 
 
 class combustor(component):
     """
     Combustor
     ---------
 
@@ -58,36 +66,35 @@
         """
 
         assert hasattr(self, 'fmf'), \
             'Component incorporating combustor has no fuel mass flow method implemented.'
 
         self.fmf(gas)
 
-        self.Q = self.fuel.mf*self.eta*self.fuel.LHV      # Heat added to the flow
+        self.Q = self.fuel.mf*self.fuel.LHV      # Heat added to the flow
 
-        approx_process_t = deepcopy(gas).heat_addition(eta=self.eta,
+        approx_process_t = deepcopy(gas).heat_exchange(eta=self.eta,
+                                                       PI=self.PI,
                                                        cp=gas.cp(gas.t0),
-                                                       fuel_mf=self.fuel.mf,
-                                                       fuel_LHV=self.fuel.LHV).t01
-
-        return gas.heat_addition(eta=self.eta,
+                                                       Q_ex=self.Q).t01
+        
+        return gas.heat_exchange(eta=self.eta,
                                  PI=self.PI,
                                  cp=gas.cp(approx_process_t),
-                                 fuel_mf=self.fuel.mf,
-                                 fuel_LHV=self.fuel.LHV)
+                                 Q_ex=self.Q)
 
     def mf_dt(self, dt, gas):
         """
         Fuel mass flow from a required change in total temperature.
         """
         gas_cp = gas.cp(self.t01)       # Heat addition happens at high temperature
         return dt*gas.mf*gas_cp/(self.eta*self.fuel.LHV - dt*gas_cp)
 
 
-class combustion_chamber(combustor):
+class combustion_chamber(plant, combustor):
     """
     Combustion chamber
     ------------------
 
     Constant pressure heat addition.
     """
     def __init__(self,
@@ -159,39 +166,14 @@
 
     def mf_qr(self, qr):
         """
         Fuel mass flow from heat addition required.
         """
         return qr/(self.eta*self.fuel.LHV)
 
-    def Q_min(self, downstream):
-        """
-        Obtain the heat required by all downstream turbines.
-
-        Assumptions:
-        - A single combustion chamber is used to power all
-          downstream turbines, without secondary combustion
-          chambers in any of the affluent streams.
-          If this is the case, the combustion chambers will
-          provide the heat required by each of their common
-          turbines (and so twice the amount needed).
-          For now, it is wise to ensure any secondary combustion
-          chambers do not have shared turbines with the main one.
-
-        :type downstream: list of stream
-
-        :return: Heat required by all downstream turbines.
-        """
-        Qr = []
-        for stream in downstream:
-            for c in stream.components:
-                if isinstance(c, turbine):
-                    Qr.append(c.w_r())
-        return sum(Qr)
-
 
 class afterburner(combustor):
     """
     Afterburner or Reheater
     -----------------------
 
     Constant pressure heat addition.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huracan-0.0a2/huracan/components/electrical.py` & `huracan-0.9/huracan/components/power/sinks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: GPL-3.0-only
+
+"""
+System power sinks
+------------------
+"""
+
 from huracan.engine import component
 
 
-class power_plant(component):
+class electrical_system(component):
     """
-    Aircraft electrical power plant
-    -------------------------------
+    Aircraft electrical system
+    --------------------------
     """
     def __init__(self,
                  w,
                  eta_g=1,
                  eta_c=1):
         """
-        :param w:     [W] Power required by the electrical power plant.
+        :param w:     [W] Power required by the electrical system.
         :param eta_g: [-] Efficiency of the electrical generator attached
                           to the turbine.
         :param eta_c: [-] Efficiency of the electrical power distribution
                           grid of the aircraft.
         """
         self.w_r = w/eta_g/eta_c
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huracan-0.0a2/huracan/components/rotary.py` & `huracan-0.9/huracan/components/rotary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,64 @@
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: GPL-3.0-only
+
+"""
+Rotary components
+-----------------
+"""
+
 from huracan.engine import component
 
 
-class compressor(component):
+class screw(component):
     """
-    Compressor
-    ----------
+    Screw
+    -----
 
-    Adiabatic compression.
+    Mechanical device to turn rotational to axial motion.
     """
     def __init__(self,
                  eta,
                  PI=None,
                  TAU=None):
         """
         :type eta: float
         :type PI:  float
         :type TAU: float
         """
         self.eta = eta
         self.PI  = PI
         self.TAU = TAU
 
+
+class compressor(screw):
+    """
+    Compressor
+    ----------
+
+    Adiabatic compression.
+    """
+    def __init__(self,
+                 eta,
+                 PI=None,
+                 TAU=None):
+        """
+        :type eta: float
+        :type PI:  float
+        :type TAU: float
+        """
+        super().__init__(eta=eta,
+                         PI=PI,
+                         TAU=TAU)
+
     def tf(self, gas):
         return gas.compression(eta=self.eta, PI=self.PI, TAU=self.TAU)
 
 
-class turbine(component):
+class turbine(screw):
     """
     Turbine
     -------
 
     Adiabatic expansion.
     """
     def __init__(self,
@@ -37,17 +66,17 @@
                  PI=None,
                  TAU=None):
         """
         :type eta: float
         :type PI:  float
         :type TAU: float
         """
-        self.eta = eta
-        self.PI  = PI
-        self.TAU = TAU
+        super().__init__(eta=eta,
+                         PI=PI,
+                         TAU=TAU)
 
     def tf(self, gas):
         """
         Before runtime, if no total pressure or temperature
         ratio has been provided, a minimum total temperature
         ratio is calculated.
         This temperature ratio is that required to power the
@@ -60,35 +89,14 @@
 
         return gas.expansion(eta=self.eta, PI=self.PI, TAU=self.TAU)
 
     def w_r(self):
         return self.shaft.w_r()
 
 
-class screw(component):
-    """
-    Screw
-    -----
-
-    Mechanical device to turn rotational to axial motion.
-    """
-    def __init__(self,
-                 eta,
-                 PI=None,
-                 TAU=None):
-        """
-        :type eta: float
-        :type PI:  float
-        :type TAU: float
-        """
-        self.eta = eta
-        self.PI  = PI
-        self.TAU = TAU
-
-
 class fan(screw):
     """
     Fan
     ---
 
     Fundamental differences with a propeller:
     - Disk loading.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huracan-0.0a2/huracan/engine.py` & `huracan-0.9/huracan/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,123 @@
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: GPL-3.0-only
+
+"""
+Huracan engine elements
+-----------------------
+"""
+
+import re
+import types
+import warnings
 import numpy as np
 from copy import deepcopy
 
-from mpl_plotter import figure
-from mpl_plotter.two_d import line, scatter, comparison
-from mpl_plotter.color.schemes import colorscheme_one
-from mpl_plotter.color.functions import delta
-
-from alexandria.shell import print_color, print_result
-from alexandria.data_structs.string import join_set_distance
+import matplotlib.pyplot as plt
 
 from huracan.constants import R
+from huracan import component_codes
+from huracan.physical_quantities import physical_quantities
+from huracan.utils import markers, join_set_distance, delta, colorscheme_one
+
+
+class component_set_constructor(type):
+    """
+    Set metaclass
+    -------------
+
+    Ensure all necessary methods are implemented in child classes.
+    """
+    def __new__(mcs, name, bases, body):
+
+        for method in ['add_component', 'add_set']:
+            if method not in body:
+                raise TypeError(f'set_of_components class build error: {method} method must be implemented in set_of_components child classes.')
+
+        return super().__new__(mcs, name, bases, body)
+
+
+class stream_set_constructor(type):
+    """
+    Superset metaclass
+    ------------------
+
+    Ensure all necessary methods are implemented in child classes.
+    """
+    def __new__(mcs, name, bases, body):
+
+        for method in ['gobble']:
+            if method not in body:
+                raise TypeError(f'set_of_streams class build error: {method} method must be implemented in set_of_streams child classes.')
+
+        return super().__new__(mcs, name, bases, body)
+
+
+class set_of_components:
+    """
+    Component set class
+    """
+    def __sub__(self, other):
+        """
+        Set concatenation operator: <set> - <component/set>
+        """
+        if isinstance(other, component):
+            self.add_component(other)
+            return self
+        if isinstance(other, set_of_components):
+            return self.add_set(other)
+
+    def integrate_in_system(self):
+        """
+        Integrate stream in stream system
+        ---------------------------------
+
+        When a set (a stream) is integrated in a superset
+        (a system), all set methods with a homonimous
+        superset method are renamed as protected
+        instance attributes, and their original names are
+        taken by pointers to the homonimous superset methods.
+        """
+
+        special = r'^__(.*?)\__$'
+
+        def takeover(obj, method):
+            if hasattr(obj.superset, method):
+                return getattr(obj.superset, method)
+            else:
+                return getattr(obj, '_' + method)
+
+        for k in dir(self):
+            v = getattr(self, k)
+            # If the attribute k is:
+            #    - a method
+            #    - which is not special
+            #    - whose name is the name of another method in the stream's system
+            if isinstance(v, types.MethodType) and not re.match(special, k) and k in dir(self.superset):
+                if not hasattr(self, '_' + k):
+                    # Create private method
+                    setattr(self, '_' + k, v)
+                # Replace public method by takeover
+                setattr(self, k, takeover(self, k))
+
+
+class set_of_streams:
+    """
+    Component superset class
+    """
+    def __call__(self, *args):
+        """
+        Superset set addition operator: <superset>(<list of sets>)
+
+        The gobble function must be implemented by the superset
+        child class (system).
+
+        :type args: set
+        """
+        self.gobble(list(args))
 
 
 class component:
     """
     Component
     ---------
     """
@@ -94,15 +198,15 @@
 
         electrical = self.electrical_plants()               # FIXME: ugly
         w_r_e = sum([c.w_r for c in electrical])            # Power required by all electrical plants
 
         return w_r_m + w_r_e
 
 
-class stream:
+class stream(set_of_components, metaclass=component_set_constructor):
     """
     Stream
     ------
     """
     def __init__(self,
                  gas=None,
                  parents=None,
@@ -138,84 +242,83 @@
 
         if not isinstance(gas, type(None)):
             self.gas    = gas
         if not isinstance(parents, type(None)):
             self.parents = parents
 
         # Runtime dictionary
-        self.runtime = {}
+        self.runtime_d = {}
         if not isinstance(fr, type(None)):
-            self.runtime['fr'] = fr
+            self.runtime_d['fr'] = fr
 
     """
     Operators
     """
     def __call__(self, gas):
         self.gas = gas
         return self
 
-    def __sub__(self, other):
+    def __mul__(self, other):
+        """
+        Stream diversion operator: <stream> * n     for n: 0 =< float =< 1
         """
-        Stream concatenation operator: <stream> - <component/stream>
+        return self.divert(other)
+
+    def __getitem__(self, item):
         """
-        if isinstance(other, component):
-            self._add_component(other)
-            return self
-        if isinstance(other, stream):               # TODO: stream merge
-            return self._add_stream(other)
+        Component retrieval operator: <stream>[<component stage name>]
+        """
+        return self.retrieve(item)
 
-    def _add_component(self, c):
+    """
+    Operator functions
+    """
+    def add_component(self, c):
         """
         Component addition
         """
         self.components.append(c)
         c.downstream = self.downstream
-        c.stream = self
+        c.stream = c.set = self
 
-    def _add_stream(self, s):
+    def add_set(self, s):
         """
         Stream addition
         """
         assert hasattr(self, 'gas') and hasattr(s, 'gas'), 'Both streams must have a gas attribute for' \
                                                            'the stream merge operation to be possible.'
 
         n = max(self.stream_id[0], s.stream_id[0])  # Get largest stream_id
         self.stream_id[0] = s.stream_id[0] = n      # Set largest stream_id for both merging streams
 
         merged = stream(parents=[self, s])
         merged.stream_id[0] = n + 1
 
         if hasattr(self, 'system') and hasattr(s, 'system'):
-            self.system = s.system = merged.system = self.system + s.system
+            self.superset = self.system = s.system = merged.system = self.system + s.system
             self.system(merged)
         elif hasattr(self, 'system'):
             self.system(s, merged)
         elif hasattr(s, 'system'):
             s.system(self, merged)
         else:
             system(self, s, merged)
 
         return merged
 
-    def __mul__(self, other):                       # TODO: stream diversion
-        """
-        Stream diversion operator: <stream> * n     for n: 0 =< float =< 1
-        """
-        return self._divert(other)
-
-    def _divert(self, fr, names=None):
+    def divert(self, fr, names=None):
         """
         Stream diversion
         """
 
         assert hasattr(self, 'gas'), 'The stream must have a gas attribute for' \
                                      'the stream diversion operation to be possible.'
 
-        main = stream(self.gas, fr=fr, parents=[self])
-        div  = stream(self.gas, fr=1-fr, parents=[self])
+        main = stream(deepcopy(self.gas), fr=fr, parents=[self])
+        div  = stream(deepcopy(self.gas), fr=1-fr, parents=[self])
 
         # Stream ID
         main.stream_id[0] = self.stream_id[0] + 1
         div.stream_id[0]  = self.stream_id[0] + 1
 
         # Diverted stream IDs
         if not isinstance(names, type(None)):
@@ -234,23 +337,15 @@
             self.system(main, div)
             main.system = div.system = self.system
         else:
             system(self, main, div)
 
         return main, div
 
-    def __getitem__(self, item):
-        """
-        Component retrieval operator: <stream>[<component stage>]
-
-        :type item: str
-        """
-        return self._system_takeover('__getitem__', item)
-
-    def ___getitem__(self, item):
+    def retrieve(self, item):
         """
         Retrieve any stream component by its stage name.
 
         :type item: str
         """
         assert item in self.stages(), 'Specified a non-existent stage.'
 
@@ -264,39 +359,28 @@
     def stages(self):
         """
         Return a list containing the stage name of each
         component in the stream.
         """
         return [c.stage for c in self.components]
 
-    def _stage_name(self, c):
+    def stage_name(self, c):
         """
         Return the stage name of a component in the stream,
         composed of the stream identification number, a code
         representing its parent class, and a numerical index
         if there are more than 1 components of the same class
         in the stream.
         """
-        codes = {'fan':                'fn',
-                 'prop':               'pr',
-                 'propfan':            'pf',
-                 'intake':             'it',
-                 'inlet':              'il',
-                 'compressor':         'cp',
-                 'combustion_chamber': 'cc',
-                 'turbine':            'tb',
-                 'afterburner':        'ab',
-                 'nozzle':             'nz'
-                 }
-
-        code = codes[c.__class__.__name__] + self._n_instances(c)
+        
+        code = component_codes[c.__class__.__name__] + self.n_instances(c)
 
         return f'{".".join([str(c) for c in self.stream_id])}.{code}'
 
-    def _n_instances(self, comp):
+    def n_instances(self, comp):
         """
         Calculate the number of instances of a given component's
         parent class in the stream (n), and its index in the
         stream's components list (i).
 
         The index of the component is returned as follows:
         - If the given component is the only instance of its parent
@@ -315,74 +399,74 @@
             if comp is c:
                 i = n
             if comp.__class__.__name__ == c.__class__.__name__:
                 n += 1
 
         return '' if n == 1 else str(i + 1)
 
-    def _log(self):
+    def log(self):
 
         d = 9
 
         for c in self.components:
             section_name = join_set_distance(c.stage, c.__class__.__name__.capitalize().replace("_", " "), d)
-            print_color(section_name, 'green')
+            print(section_name)
 
             if c.__class__.__name__ == 'nozzle':
                 if c.choked:
-                    print_color(' '*d + 'Choked flow', 'red')
-            print_result(' '*(d+1) + 'T0', c.t0, '[K]')
-            print_result(' '*(d+1) + 'p0', c.p0, '[Pa]')
+                    print(' '*d + 'Choked flow')
+            print(f'{" "*d} T0 {str(c.t0)[:10]} [K]')
+            print(f'{" "*d} p0 {str(c.p0)[:10]} [Pa]')
 
     """
     Stream runtime functions
     """
-    def _run(self, log=True):
+    def run(self, log=True):
         """
         Execute the transfer functions of all components in the stream
         on the instance's gas class instance.
         """
 
-        self._runtime()
+        self.runtime()
 
         assert hasattr(self, 'gas'), 'stream does not have a gas attribute.'
 
         self.choked = False                                 # FIXME: choked flow implementation is ugly
 
         for c in self.components:
-            c(self.gas)                     # Run thermodynamic process on stream gas
-            c.stage = self._stage_name(c)   # Set component stage name
+            c(self.gas)                    # Run thermodynamic process on stream gas
+            c.stage = self.stage_name(c)   # Set component stage name
 
             if hasattr(c, 'choked') and c.choked:           # FIXME: ugly
                 self.choked = c.choked
 
         # Indicate stream has been run.
         self.ran = True
 
         if log:
-            self._log()
+            self.log()
 
-    def _runtime(self):
+    def runtime(self):
         if hasattr(self, 'parents') and len(self.parents) > 1:
-            self._merge()
+            self.merge()
 
-        for k, v in self.runtime.items():
-            f = getattr(self, '_'+k)
+        for k, v in self.runtime_d.items():
+            f = getattr(self, k)
             f(v)
 
-    def _merge(self):
+    def merge(self):
         if hasattr(self, 'gas'):
             for s in self.parents:
                 self.gas += s.gas
         else:
             self.gas = self.parents[0].gas
             for s in self.parents[1:]:
                 self.gas += s.gas
 
-    def _fr(self, fr):
+    def fr(self, fr):
         self.gas, _ = fr * deepcopy(self.gas)
 
     """
     Stream fluid state
     """
     def t0(self):
         """
@@ -412,18 +496,26 @@
         """
         Specific entropy vector.
         """
         assert self.ran, 'The stream must be run to obtain the specific entropy at each stage'
 
         return np.array([c.S for c in self.components])
 
+    def H(self):
+        """
+        Specific enthalpy vector.
+        """
+        assert self.ran, 'The stream must be run to obtain the specific entropy at each stage'
+
+        return np.array([c.H for c in self.components])
+
     """
     Stream outlet flow characteristics
     """
-    def _v_exit(self):
+    def v_exit(self):
         """
         Flow exit velocity
 
         Assumptions:
         - If the flow is not choked:
              The thermal energy lost by the gas as it leaves the nozzle
              is transformed into kinetic energy without losses.
@@ -470,435 +562,364 @@
                                                     'the nozzle tha outside the engine: this happens due to the ' \
                                                     'compressors not providing enough energy to the flow. You must ' \
                                                     'either increase the pressure ratio of the compressors or ' \
                                                     'decrease the power extracted from the flow to solve the ' \
                                                     'inconsistency.'
             return (2*self.gas.cp(t_before_exit)*(t_before_exit - self.gas.t0))**0.5    # Heat -> Kinetic energy
 
-    def _A_exit(self):
+    def A_exit(self):
         """
         Nozzle exit area
         """
-        return self.gas.mf*R*self.gas.t0/(self.gas.p0*self._v_exit())
+        return self.gas.mf*R*self.gas.t0/(self.gas.p0*self.v_exit())
 
     """
-    Stream performance analysis
+    Fuel consumption
     """
-    def _fmf(self):
+    def fmf(self):
         """
         Stream fuel mass flow
         """
         fmf = 0
         for c in self.components:
             if hasattr(c, 'fuel') and hasattr(c.fuel, 'mf'):
                 fmf += c.fuel.mf
         return fmf
 
-    def _flow_thrust(self):
+    """
+    Thrust and specific fuel consumption
+    """
+    def thrust_flow(self):
         """
         Flow thrust
 
         If the flow is choked, the expansion of the gas contributes to the thrust of the flow.
         """
         if self.choked:
-            return self.gas.mf * (self._v_exit() - self.gas.v_0) + self._A_exit() * (
+            return self.gas.mf * (self.v_exit() - self.gas.v_0) + self.A_exit() * (
                         self.gas.p0 - self.gas.p_0)
         else:
-            return self.gas.mf * (self._v_exit() - self.gas.v_0)
+            return self.gas.mf * (self.v_exit() - self.gas.v_0)
 
-    def _prop_thrust(self):
+    def thrust_prop(self):
         """
         Propeller/propfan thrust
         """
         if any([c.__class__.__name__ in ['prop', 'propfan'] for c in self.components]):
             propellers = [c for c in self.components if c.__class__.__name__ in ['prop', 'propfan']]
-            prop_thrust = sum([prop.thrust(self.gas.v_0) for prop in propellers])
+            thrust_prop = sum([prop.thrust(self.gas.v_0) for prop in propellers])
         else:
-            prop_thrust = 0
-        return prop_thrust
+            thrust_prop = 0
+        return thrust_prop
 
-    def _total_thrust(self):
+    def thrust_total(self):
         """
         Flow thrust plus propeller/propfan thrust
         """
-        return self._flow_thrust() + self._prop_thrust()
+        return self.thrust_flow() + self.thrust_prop()
 
-    def _sfc(self):
+    def sfc(self):
         """
         Specific fuel consumption
         """
-        return self.fmf()/self.flow_thrust()
+        if hasattr(self, 'system'):
+            return self._fmf()/self._thrust_flow()
+        else:
+            return self.fmf()/self.thrust_flow()
 
-    def _Q_in(self):               #TODO: verify and implement efficiency calculations
+    """
+    Heat and work
+    """
+    def Q_in(self):                #TODO: verify efficiency calculations
         """
         Heat provided to the flow.
         """
         q_provided = 0
         for c in self.components:
             if c.__class__.__name__ == 'combustion_chamber':
                 q_provided += c.Q
         return q_provided
 
-    def _W_req(self):
+    def W_req(self):
         """
         Work required from the flow.
         """
         w_required = 0
         for c in self.components:
             if c.__class__.__name__ in ['fan',
                                         'prop',
                                         'propfan',
                                         'compressor']:
                 w_required += c.w
         return w_required
 
-    def _E_balance(self):
+    """
+    Power
+    """
+    def power_jet(self):
         """
-        Flow energy balance.
+        Stream jet power.
         """
-        return self._Q_in() - self._W_req()
+        return 1/2*(self.gas.mf*self.v_exit()**2 - (self.gas.mf - self.fmf())*self.gas.v_0**2)
 
-    def _E_prop(self):
+    def power_available(self):
         """
-        Energy added to the flow for propulsion.
+        Stream available power.
         """
-        return self._v_exit()**2/2
+        if hasattr(self, 'system'):
+            return self._efficiency_prop()*self._power_jet()
+        else:
+            return self.efficiency_prop()*self.power_jet()
 
-    def _efficiency(self):
+    """
+    Efficiencies
+    """
+    def efficiency_thermal(self):
         """
-        Engine efficiency
+        Stream thermal efficiency
         """
-        return self._E_balance()/self._Q_in()
+        if hasattr(self, 'system'):
+            return self._power_jet()/self._Q_in()
+        else:
+            return self.power_jet()/self.Q_in()
 
-    def _prop_efficiency(self):
+    def efficiency_prop(self):
         """
         Stream propulsive efficiency.
         """
-        return self._E_prop()/self._Q_in()
+        return 2/(1+self.v_exit()/self.gas.v_0) if self.gas.v_0 > 0 else 0
+
+    def efficiency_total(self):
+        if hasattr(self, 'system'):
+            return self._power_available()/self._Q_in()
+        else:
+            return self.power_available()/self.Q_in()
 
     """
     Plots
     """
-    def _plot_T_p(self,
-                  show=False,
-                  plot_label=None,
-                  color=colorscheme_one()[0],
-                  **kwargs):
+    def plot_T_S(self,
+             show=False,
+             plot_label=None,
+             color=colorscheme_one()[0],
+             **kwargs):
+        warnings.warn('`<stream or system>.plot_T_S(...)` is deprecated in favor of `<stream or system>.plot(x="S", "y=t0", ...)` and will be removed from Huracan in the next major release', DeprecationWarning, stacklevel=2)
         """
-        Plot
-        - Total pressure
-        - Total temperature
+        Temperature-Entropy stream plot.
         """
 
-        figure((9, 5))
+        plt.figure(figsize=(9, 5))
 
-        defaults = {'x_label': 'p$_0$ [kPa]',
-                    'y_label': 'T$_0$ [K]'}
+        defaults = {'label_x': r'$\Delta$S [kJ/K/n]',
+                    'label_y': r'T$_0$ [K]',}
 
         further_custom = {**defaults, **kwargs}
 
-        self.plot_cycle_graph(self.p0()/1000, self.t0(),
+        self.plot_cycle_graph(self.S()/1000, self.t0(),
                               color=color,
                               plot_label=plot_label,
                               show=show,
                               # Further customization
-                              x_tick_ndecimals=2,
+                              tick_label_decimals_y=2,
                               **further_custom)
 
-    def _plot_p_V(self,
-                  show=False,
-                  plot_label=None,
-                  color=colorscheme_one()[0],
-                  **kwargs):
+    def plot_p_V(self,
+                 show=False,
+                 plot_label=None,
+                 color=colorscheme_one()[0],
+                 **kwargs):
+        warnings.warn('`<stream or system>.plot_p_V(...)` is deprecated in favor of `<stream or system>.plot(x="V", "y=p0", ...)` and will be removed from Huracan in the next major release', DeprecationWarning, stacklevel=2)
         """
-        Plot
-        - Total specific volume
-        - Total pressure
+        Pressure-Volume stream plot.
         """
 
-        figure((9, 5))
+        plt.figure(figsize=(9, 5))
 
-        defaults = {'x_label': 'v$_0$ [m$^3$/n]',
-                    'y_label': 'p$_0$ [kPa]'}
+        defaults = {'label_x': 'v$_0$ [m$^3$/n]',
+                    'label_y': 'p$_0$ [kPa]'}
 
         further_custom = {**defaults, **kwargs}
 
         self.plot_cycle_graph(self.V(), self.p0()/1000,
                               color=color,
                               plot_label=plot_label,
                               show=show,
                               # Further customization
-                              y_tick_ndecimals=2,
+                              tick_label_decimals_y=2,
                               **further_custom)
 
-    def _plot_T_S(self,
-                  show=False,
-                  plot_label=None,
-                  color=colorscheme_one()[0],
-                  **kwargs):
+    def plot_H_p(self,
+                 show=False,
+                 plot_label=None,
+                 color=colorscheme_one()[0],
+                 **kwargs):
+        warnings.warn('`<stream or system>.plot_H_p(...)` is deprecated in favor of `<stream or system>.plot(x="p0", y="H", ...)` and will be removed from Huracan in the next major release', DeprecationWarning, stacklevel=2)
         """
-        Plot
-        - Specific entropy
-        - Total temperature
+        Pressure-Enthalpy stream plot.
         """
 
-        figure((9, 5))
+        plt.figure(figsize=(9, 5))
 
-        defaults = {'x_label': 'S [J/K/n]',
-                    'y_label': 'T$_0$ [K]',}
+        defaults = {'label_x': 'p$_0$ [kPa]',
+                    'label_y': 'H$_0$ [kJ]',}
 
         further_custom = {**defaults, **kwargs}
 
-        self.plot_cycle_graph(self.S(), self.t0() / 1000,
+        self.plot_cycle_graph(self.p0()/1000, self.H()/1000,
                               color=color,
                               plot_label=plot_label,
                               show=show,
                               # Further customization
-                              y_tick_ndecimals=2,
+                              tick_label_decimals_y=2,
                               **further_custom)
 
-    def plot_cycle_graph(self,
-                         x, y,
-                         plot_label,
-                         x_label, y_label,
-                         color=colorscheme_one()[0],
-                         show=False,
-                         **kwargs
-                         ):
+    def plot_T_p(self,
+             show=False,
+             plot_label=None,
+             color=colorscheme_one()[0],
+             **kwargs):
+        warnings.warn('`<stream or system>.plot_T_p(...)` is deprecated in favor of `<stream or system>.plot(x="V", "y=p0", ...)` and will be removed from Huracan in the next major release', DeprecationWarning, stacklevel=2)
         """
-        General plot composed of an MPL Plotter line and scatter plot.
-
-        The default arguments plus any valid MPL Plotter line plotting
-        class arguments can be passed to this function.
+        Temperature-Pressure system plot.
         """
-        fig = kwargs.pop('fig', None)
-
-        defaults = {
-            # Specifics
-            'point_size': 30,
-            # Markers
-            'marker': 'x',
-            # Color
-            'color': delta(color, -0.3),
-            # Arrangement
-            'zorder': 2,
-            # Further customization
-            'aspect': 1/2,
-            'x_tick_number': 10,
-            'y_tick_number': 10,
-            'demo_pad_plot': True,
-            'y_label_pad': 5,
-        }
 
-        further_custom = {**defaults, **kwargs}
-
-        # Connecting lines
-        line(   x=x, y=y,
-                # Figure
-                fig=fig,
-                # Specifics
-                line_width=1,
-                # Color
-                color=color, alpha=0.65,
-                # Arrangement
-                zorder=1)
-        # Stages
-        scatter(x=x, y=y,
-                # Figure
-                fig=fig,
-                # Further customization
-                plot_label=plot_label,
-                x_label=x_label,
-                y_label=y_label,
-                show=show,
-                **further_custom)
-
-    """
-    System takeover and API functions
-    ---------------------------------
-    """
-    def _system_takeover(self, method, *args, **kwargs):
-        if hasattr(self, 'system'):
-            return getattr(self.system, method)(*args, **kwargs)
-        else:
-            return getattr(self, '_' + method)(*args, **kwargs)
-
-    def run(self, log=True):
-        args = locals()
-        del args['self']
+        plt.figure(figsize=(9, 5))
 
-        self._system_takeover('run', **args)
+        defaults = {'label_x': 'p$_0$ [kPa]',
+                    'label_y': 'T$_0$ [K]'}
 
-    """
-    Stream outlet flow characteristics
-    """
-    def v_exit(self):
-        """
-        Flow exit velocity
-
-        Assumptions:
-        - If the flow is not choked:
-             The thermal energy lost by the gas as it leaves the nozzle
-             is transformed into kinetic energy without losses.
-        - If the flow is choked:
-             The exit velocity is the velocity of sound before the nozzle
-             exit.
-        """
-        return self._system_takeover('v_exit')
-
-    def A_exit(self):
-        """
-        Nozzle exit area
-        """
-        return self._system_takeover('A_exit')
+        further_custom = {**defaults, **kwargs}
 
-    """
-    Stream performance analysis
-    """
-    def fmf(self):
-        """
-        Stream fuel mass flow
-        """
-        return self._system_takeover('fmf')
+        self.plot_cycle_graph(self.p0()/1000, self.t0(),
+                              color=color,
+                              plot_label=plot_label,
+                              show=show,
+                              # Further customization
+                              tick_label_decimals_x=2,
+                              **further_custom)
 
-    def flow_thrust(self):
+    def plot(self, 
+             x, y,
+             show=False,
+             plot_label=None,
+             color=colorscheme_one()[0],
+             **kwargs):
         """
-        Flow thrust
+        Create a cycle plot of two physical quantities of the stream.
         """
-        return self._system_takeover('flow_thrust')
 
-    def prop_thrust(self):
-        return self._system_takeover('prop_thrust')
+        name_x_default, label_x_default, scale_x_default = physical_quantities[x]
+        name_y_default, label_y_default, scale_y_default = physical_quantities[y]
 
-    def total_thrust(self):
-        return self._system_takeover('total_thrust')
-
-    def sfc(self):
-        """
-        Specific fuel consumption
-        """
-        return self._system_takeover('sfc')
+        scale_x = scale_x_default if isinstance(scale_x, type(None)) else scale_x
+        scale_y = scale_y_default if isinstance(scale_y, type(None)) else scale_y
+        label_x = label_x_default if isinstance(label_x, type(None)) else label_x
+        label_y = label_y_default if isinstance(label_y, type(None)) else label_y
 
-    def Q_in(self):  # TODO: verify and implement efficiency calculations
-        """
-        Heat provided to the flow.
-        """
-        return self._system_takeover('Q_in')
+        x = getattr(self, x) * scale_x
+        y = getattr(self, y) * scale_y
 
-    def W_req(self):
-        """
-        Work required from the flow.
-        """
-        return self._system_takeover('W_req')
+        defaults = {'label_x': label_x,
+                    'label_y': label_y}
 
-    def E_balance(self):
-        """
-        Flow energy balance.
-        """
-        return self._system_takeover('E_balance')
+        further_custom = {**defaults, **kwargs}
 
-    def E_prop(self):
-        """
-        Energy added to the flow for propulsion.
-        """
-        return self._system_takeover('E_prop')
+        self.plot_cycle_graph(
+            x, y,
+            color=color,
+            plot_label=plot_label,
+            show=show,
+            # Further customization
+            tick_label_decimals_x=2,
+            **further_custom)
 
-    def efficiency(self):
-        """
-        Engine efficiency
+    def plot_cycle_graph(self,
+                         x, y,
+                         plot_label,
+                         label_x, label_y,
+                         color=colorscheme_one()[0],
+                         show=False,
+                         **kwargs
+                         ):
         """
-        return self._system_takeover('efficiency')
+        General plot composed of an MPL Plotter line and scatter plot.
 
-    def prop_efficiency(self):
-        """
-        Stream propulsive efficiency.
+        The default arguments plus any valid MPL Plotter line plotting
+        class arguments can be passed to this function.
         """
-        return self._system_takeover('prop_efficiency')
-
-    """
-    Plots
-    """
-    def plot_T_p(self,
-                 show=False,
-                 plot_label=None,
-                 color=colorscheme_one()[0],
-                 **kwargs):
-        args = locals()
-        args.pop('self', None)
-        args.pop('kwargs', None)
 
-        self._system_takeover('plot_T_p', **{**args, **kwargs})
+        fig = kwargs.pop('fig', None)
 
-    def plot_p_V(self,
-                 show=False,
-                 plot_label=None,
-                 color=colorscheme_one()[0],
-                 **kwargs):
-        args = locals()
-        args.pop('self', None)
-        args.pop('kwargs', None)
+        plt.plot(x, y,
+            color=color,
+            marker=kwargs.get('marker', 'x'), markeredgecolor=delta(color, -0.3), markersize=8, markeredgewidth=2, markerfacecolor=kwargs.get('facecolors', color),
+            label=plot_label,
+            zorder=kwargs.get('zorder', 0) + 2.5,
+        )
+        plt.scatter(x, y,
+            marker=kwargs.get('marker', 'x'), s=55,
+            edgecolor=delta(color, -0.3), linewidth=1.5, 
+            facecolor=kwargs.get('facecolors', color),
+            zorder=kwargs.get('zorder', 0) + 1e2,
+        )
+
+        ax = plt.gca()
 
-        self._system_takeover('plot_p_V', **{**args, **kwargs})
-
-    def plot_T_S(self,
-                 show=False,
-                 plot_label=None,
-                 color=colorscheme_one()[0],
-                 **kwargs):
-        args = locals()
-        args.pop('self', None)
-        args.pop('kwargs', None)
-
-        self._system_takeover('plot_T_S', **{**args, **kwargs})
+        if label_x is not None: ax.set_xlabel(label_x)
+        if label_y is not None: ax.set_ylabel(label_y)
 
+        if show:
+            plt.show()
 
-class system:
+class system(set_of_streams, metaclass=stream_set_constructor):
     """
     System
     ------
     """
     def __init__(self, *args):
         """
         Create a system from two objects.
 
         :type args: stream
         """
         self.streams = []
-        self._gobble(list(args))
+        self.gobble(list(args))
 
     """
     Operators
     """
-    def __call__(self, *args):
-        """
-        System stream addition operator: <system>(<list of streams>)
-
-        :type args: stream
-        """
-        self._gobble(list(args))
-
-    def _gobble(self, streams):
-        """
-        :type streams: list of stream
-        """
-        for s in streams:
-            self.streams.append(s)
-            s.system = self
-
     def __add__(self, other):
         """
         System addition operator: <system> + <stream/system>
 
         :type other: system
         """
         streams = list(set(self.streams) & set(other.streams))
         return system(*streams)
 
     def __getitem__(self, item):
         """
+        Component retrieval operator: <system>[<component stage name>]
+        """
+        return self.retrieve(item)
+
+    """
+    Operator functions
+    """
+    def gobble(self, streams):
+        """
+        :type streams: list of stream
+        """
+        for s in streams:
+            self.streams.append(s)
+            s.superset = s.system = self
+            s.integrate_in_system()
+
+    def retrieve(self, item):
+        """
         Retrieve any stream component by its stage name.
 
         :type item: str
         """
         components = []
         for s in self.streams:
             components += s.components
@@ -913,24 +934,24 @@
     System functions
     """
     def run(self, log=True):
         """
         Run stream system.
         """
 
-        self._sort_streams()
+        self.sort_streams()
 
         n = 0
         while not all([s.ran for s in self.streams]):
             for s in self.streams:
                 if s.stream_id[0] == n:
                     s._run(log)
             n += 1
 
-    def _sort_streams(self):
+    def sort_streams(self):
         """
         Sort system streams based on their stream ID
         """
         ids     = [''.join(str(c) for c in stream.stream_id) for stream in self.streams]
         indexes = [float(id.replace('m', '.1').replace('s', '.2')) for id in ids]
         self.streams = [s for _, s in sorted(zip(indexes, self.streams))]
 
@@ -943,103 +964,112 @@
         """
         parents = []
         for s in self.streams:
             parents += s.parents if hasattr(s, 'parents') else []
         return parents
 
     """
-    Stream outlet flow characteristics
+    Fuel consumption
     """
-    def v_exit(self):
-        """
-        Flow exit velocity
-
-        Assumptions:
-        - If the flow is not choked:
-             The thermal energy lost by the gas as it leaves the nozzle
-             is transformed into kinetic energy without losses.
-        - If the flow is choked:
-             The exit velocity is the velocity of sound before the nozzle
-             exit.
-        """
-        v = [s._v_exit() for s in self.streams if s not in self.parents()]
-        return v[0] if len(v) == 1 else v
-
-    def A_exit(self):
+    def fmf(self):
         """
-        Nozzle exit area
+        System fuel mass flow.
         """
-        a = [s._A_exit() for s in self.streams if 'nozzle' in [c.__class__.__name__ for c in s.components]]
-        return a[0] if len(a) == 1 else a
+        return sum([s._fmf() for s in self.streams])
 
     """
-    System performance analysis
+    Thrust and specific fuel consumption
     """
-    def fmf(self):
-        return sum([s._fmf() for s in self.streams])
-
-    def flow_thrust(self):
-        return sum([s._flow_thrust() for s in self.streams if s not in self.parents()])
+    def thrust_flow(self):
+        """
+        System flow thrust.
+        """
+        return sum([s._thrust_flow() for s in self.streams if s not in self.parents()])
 
-    def prop_thrust(self):
-        return sum([s._prop_thrust() for s in self.streams])
+    def thrust_prop(self):
+        """
+        System propeller thrust
+        """
+        return sum([s._thrust_prop() for s in self.streams])
 
-    def total_thrust(self):
-        return self.flow_thrust() + self.prop_thrust()
+    def thrust_total(self):
+        """
+        System total thrust.
+        """
+        return self.thrust_flow() + self.thrust_prop()
 
     def sfc(self):
-        return self.fmf()/self.flow_thrust()
+        """
+        System specific fuel consumption.
+        """
+        return self.fmf()/self.thrust_flow()
 
-    def Q_in(self):  # TODO: verify and implement efficiency calculations
+    """
+    Heat and work
+    """
+    def Q_in(self):                 # TODO: verify efficiency calculations
         """
         Heat provided to the flow.
         """
         return sum([s._Q_in() for s in self.streams])
 
     def W_req(self):
         """
         Work required from the flow.
         """
         return sum([s._W_req() for s in self.streams])
 
-    def E_balance(self):
+    """
+    Power
+    """
+    def power_jet(self):
         """
-        Flow energy balance.
+        Stream jet power.
         """
-        return self.Q_in() - self.W_req()
+        return sum([s._power_jet() for s in self.streams if s not in self.parents()])
 
-    def E_prop(self):
+    def power_available(self):
         """
-        Energy added to the flow for propulsion.
+        Stream available power.
         """
-        return sum([s._E_prop() for s in self.streams])
+        return sum([s._power_available() for s in self.streams if s not in self.parents()])
 
-    def efficiency(self):
+    """
+    Efficiencies
+    """
+    def efficiency_prop(self):
         """
-        System efficiency
+        System propulsive efficiency.
         """
-        return self.E_balance()/self.Q_in()
+        return self.power_available()/self.power_jet()
 
-    def prop_efficiency(self):
+    def efficiency_thermal(self):
         """
-        Stream propulsive efficiency.
+        System thermal efficiency.
         """
-        return self.E_prop()/self.Q_in()
+        return self.power_jet()/self.Q_in()
+
+    def efficiency_total(self):
+        """
+        System total efficiency.
+        """
+        return self.power_available()/self.Q_in()
 
     """
     Plots
     """
-    def _plot(self,
-              x, y,
-              x_scale=None, y_scale=None,
-              x_label=None, y_label=None,
-              show=False,
-              plot_label=None,                  # When called from a _system_takeover the plot_label and color
-              color=colorscheme_one()[0],       # arguments are passed to the function, but disregarded.
-              **kwargs):
+    def plot(self,
+             x, y,
+             scale_x=None, scale_y=None,
+             label_x=None, label_y=None,
+             show=False,
+             plot_label=None,                  # When called from a _system_takeover the plot_label and color
+             color=colorscheme_one()[0],       # arguments are passed to the function, but disregarded.
+             colorblind=False,
+             **kwargs):
         """
         System plot
         -----------
 
         x and y are the stream parameters to be
         plotted for each stream.
 
@@ -1050,127 +1080,174 @@
         3. comparison call
 
         comparison call
             - fig=None, ax=None -> plot_cycle_graph -> fig in **kwargs keys
                 - fig=None, ax=None -> line, scatter
                     - line, scatter plot onto active figure, axis
 
-        :param x_scale: Scaling factor.
-        :param y_scale: Scaling factor.
+        :param scale_x: Scaling factor.
+        :param scale_y: Scaling factor.
 
         :type x:        str
         :type y:        str
-        :type x_scale:  float
-        :type y_scale:  float
+        :type scale_x:  float
+        :type scale_y:  float
         """
+
         plotters   = []
         x_system   = []
         y_system   = []
 
-        scales     = {'t0': 1,
-                      'p0': 1/1000,
-                      'V':  1,
-                      'S':  1,
-                      'H':  1}
-        x_scale    = scales[x] if isinstance(x_scale, type(None)) else x_scale
-        y_scale    = scales[y] if isinstance(y_scale, type(None)) else y_scale
+        defaults   = {'legend': kwargs.pop('legend', True)}
+
+        name_x_default, label_x_default, scale_x_default = physical_quantities[x]
+        name_y_default, label_y_default, scale_y_default = physical_quantities[y]
+
+        scale_x    = scale_x_default if isinstance(scale_x, type(None)) else scale_x
+        scale_y    = scale_y_default if isinstance(scale_y, type(None)) else scale_y
+        label_x    = label_x_default if isinstance(label_x, type(None)) else label_x
+        label_y    = label_y_default if isinstance(label_y, type(None)) else label_y
 
         # 1. Create figure
-        figure((9, 5))
+        plt.figure(figsize=(9, 5))
 
         # 2. Create state variable and plotters vectors
-        for stream in self.streams:
+        for i, stream in enumerate(self.streams):
 
             # Plot defaults
-            defaults = {'plot_label': f'{".".join([str(c) for c in stream.stream_id])}',
-                        'x_label': x_label,
-                        'y_label': y_label,
-                        'color': colorscheme_one()[self.streams.index(stream)],
-                        'zorder': 10-self.streams.index(stream)
-                        }
+            subplot_defaults = {
+                'plot_label': f'{".".join([str(c) for c in stream.stream_id])}',
+                'label_x': label_x,
+                'label_y': label_y,
+                'color': colorscheme_one()[self.streams.index(stream)],
+                'zorder': self.streams.index(stream)
+            }
+
+            if colorblind:
+                m      = markers(hollow=True)
+                marker = m[self.streams.index(stream)]
+                subplot_defaults = {**subplot_defaults, **marker}
 
             def gen_plotter(**defaults):
                 """
                 Returns a plotter using the defaults.
-                Any keyword arguemnts passed to the
+                Any keyword arguments passed to the
                 _plot function overwrite the defaults.
                 """
-                return lambda x, y, **kwargs: stream.plot_cycle_graph(x=x, y=y, **{**kwargs, **defaults})
+                return lambda x, y, **kwargs: stream.plot_cycle_graph(x=x, y=y, **{**defaults, **kwargs})
 
-            x_stream = getattr(stream, x)()*x_scale
-            y_stream = getattr(stream, y)()*y_scale
+            x_stream = getattr(stream, x)()*scale_x
+            y_stream = getattr(stream, y)()*scale_y
 
-            plotters.append(gen_plotter(**defaults))
+            plotters.append(gen_plotter(**subplot_defaults))
             x_system.append(x_stream)
             y_system.append(y_stream)
 
             # 2.1 Parent connectors
             if hasattr(stream, 'parents'):
                 for parent in stream.parents:
-                    x_parent = getattr(parent, x)()*x_scale
-                    y_parent = getattr(parent, y)()*y_scale
+                    x_parent = getattr(parent, x)()*scale_x
+                    y_parent = getattr(parent, y)()*scale_y
                     # If the parent stream has no stages, get parent stream's gas state
-                    p_x = x_parent[-1] if len(x_parent) != 0 else getattr(parent.gas, x)*x_scale
-                    p_y = y_parent[-1] if len(y_parent) != 0 else getattr(parent.gas, y)*y_scale
+                    p_x = x_parent[-1] if len(x_parent) != 0 else getattr(parent.gas, x)*scale_x
+                    p_y = y_parent[-1] if len(y_parent) != 0 else getattr(parent.gas, y)*scale_y
+                    # Connector
                     if len(stream.components) > 0:
                         x_system.append(np.array([p_x, x_stream[0]]))
                         y_system.append(np.array([p_y, y_stream[0]]))
-                        plotters.append(gen_plotter(color=defaults['color'], x_label=None, y_label=None))
+
+                        connector_args = {
+                            'color': subplot_defaults['color'],
+                            'zorder': self.streams.index(stream),
+                            'plot_label': None,
+                            'label_x': None,
+                            'label_y': None,
+                            'marker': '',
+                            'zorder': 0
+                        }
+
+                        if colorblind:
+                            connector_args = {**connector_args}
+
+                        plotters.append(gen_plotter(**connector_args))
 
         # 2.2 Remove streams with no stages
         mask_x = np.array([a.size != 0 for a in x_system])
         mask_y = np.array([a.size != 0 for a in y_system])
         mask = mask_x * mask_y  # Ensure that any x-y array pairs with an empty array are removed
 
         x_system = np.array(x_system, dtype='object')[mask].tolist()
         y_system = np.array(y_system, dtype='object')[mask].tolist()
         plotters = np.array(plotters, dtype='object')[mask].tolist()
 
-        # 4. comparison call
-        #     - fig=None, ax=None -> plot_cycle_graph -> fig in **kwargs keys
-        #         - fig=None, ax=None -> line, scatter
-        #             - line, scatter plot onto active figure, axis
-        comparison(x=x_system, y=y_system, f=plotters,
-                   legend_loc=(0.875, 0.425),
-                   show=show,
-                   **kwargs)
+        # 4. Plot all
+        for i, plotter in enumerate(plotters):
+            plotter(x_system[i], y_system[i], **{**kwargs, **defaults})
+
+        plt.legend()
 
+        plt.show()
+    
     def plot_T_p(self,
                  show=False,
                  plot_label=None,
                  color=colorscheme_one()[0],
+                 colorblind=False,
                  **kwargs
                  ):
+        warnings.warn('`<stream or system>.plot_T_p(...)` is deprecated in favor of `<stream or system>.plot(x="V", "y=p0", ...)` and will be removed from Huracan in the next major release', DeprecationWarning, stacklevel=2)
+        """
+        Temperature-Pressure system plot.
+        """
         args = locals()
         args.pop('self', None)
         args.pop('kwargs', None)
 
-        self._plot(x='p0', x_label='p$_0$ [kPa]',
-                   y='t0', y_label='T$_0$ [K]',
-                   **{**args, **kwargs}
-                   )
+        self.plot(x='p0', y='t0', **{**args, **kwargs})
 
     def plot_p_V(self,
                  show=False,
                  plot_label=None,
                  color=colorscheme_one()[0],
+                 colorblind=False,
                  **kwargs):
+        warnings.warn('`<stream or system>.plot_p_V(...)` is deprecated in favor of `<stream or system>.plot(x="V", "y=p0", ...)` and will be removed from Huracan in the next major release', DeprecationWarning, stacklevel=2)
+        """
+        Pressure-Volume system plot.
+        """
         args = locals()
         args.pop('self', None)
         args.pop('kwargs', None)
 
-        self._plot(x='V',  x_label='v$_0$ [m$^3$/n]',
-                   y='p0', y_label='p$_0$ [kPa]',
-                   **{**args, **kwargs})
+        self.plot(x='V', y='p0', **{**args, **kwargs})
 
     def plot_T_S(self,
                  show=False,
                  plot_label=None,
                  color=colorscheme_one()[0],
+                 colorblind=False,
                  **kwargs):
+        warnings.warn('`<stream or system>.plot_T_S(...)` is deprecated in favor of `<stream or system>.plot(x="S", "y=t0", ...)` and will be removed from Huracan in the next major release', DeprecationWarning, stacklevel=2)
+        """
+        Temperature-Entropy system plot.
+        """
+        args = locals()
+        args.pop('self', None)
+        args.pop('kwargs', None)
+
+        self.plot(x='S', y='t0', **{**args, **kwargs})
+
+    def plot_H_p(self,
+                 show=False,
+                 plot_label=None,
+                 color=colorscheme_one()[0],
+                 colorblind=False,
+                 **kwargs):
+        warnings.warn('`<stream or system>.plot_H_p(...)` is deprecated in favor of `<stream or system>.plot(x="p0", y="H", ...)` and will be removed from Huracan in the next major release', DeprecationWarning, stacklevel=2)
+        """
+        Pressure-Enthalpy system plot.
+        """
         args = locals()
         args.pop('self', None)
         args.pop('kwargs', None)
 
-        self._plot(x='S',  x_label='S [J/K]',
-                   y='t0', y_label='T$_0$ [K]',
-                   **{**args, **kwargs})
+        self.plot(x='p0', y='H', **{**args, **kwargs})
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huracan-0.0a2/huracan/thermo/fluids.py` & `huracan-0.9/huracan/thermo/fluids.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,20 @@
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: GPL-3.0-only
+
+"""
+Huracan fluid models
+--------------------
+"""
+
 from copy import deepcopy
 
 from huracan.constants import R
 from huracan.engine import stream, component
-from huracan.thermo.processes import absolute, diffusion, compression, combustion, expansion
+from huracan.thermo.processes import absolute, diffusion, compression, heat_exchange, expansion
 
 
 class fluid:
     """
     Fluid
     -----
     """
@@ -81,24 +89,27 @@
         self.v_0 = m*(k(t_0)*R*t_0)**0.5
 
         self.t_0 = t_0
         self.p_0 = p_0
 
         self.absolute()
 
+        # Set the gas' initial entropy as 0
+        self.S = 0
+
     def state(self):
         """
         Update gas state variables.
         - V - Specific volume
         - S - Specific entropy
         - H - Specific enthalpy
         """
-        self.V = self.t0*R/self.p0
-        self.S = 1                          #TODO: implement
-        self.H = 1                          #TODO: implement
+        self.V  =  self.t0*R/self.p0
+        self.E  =  self.cp(self.t0)/self.k(self.t0)*self.t0
+        self.H  =  self.E + self.p0*self.V
 
     def __add__(self, other):
         """
         Mixture creation operator: <gas> + <gas>
 
         In the case of adding fuel to a gas, the
         following assumptions are considered:
@@ -295,46 +306,54 @@
         self.t0 = p.t01
         self.p0 = p.p01
 
         self.state()
 
         return p
 
-    def heat_addition(self,
+    def heat_exchange(self,
                       eta,
                       cp,
-                      fuel_mf,
-                      fuel_LHV,
+                      Q_ex,
                       PI=1):
         """
-        Constant pressure heat addition
-        -------------------------------
+        Isobaric heat exchange
+        ----------------------
 
         Assumptions:
         - Perfect heat addition
-        - Constant pressure
 
-        :param eta:      Isentropic efficiency
-        :param cp:       Specific heat of gas during heat addition
-        :param fuel_mf:  Fuel mass flow
-        :param fuel_LHV: Fuel Lower Heating Value (heat of combustion)
-        """
-
-        p = combustion(mf       = self.mf,
-                       cp       = cp,
-                       t00      = self.t0,
-                       p00      = self.p0,
-                       fuel_mf  = fuel_mf,
-                       fuel_LHV = fuel_LHV,
-                       eta      = eta,
-                       PI       = PI)
+        The pressure ratio is assumed to be constant,
+        however a pressure ratio different than 1 can
+        be input to the function in case the process
+        cannot be assumed to be isobaric.
+
+        :param eta:  Isentropic efficiency
+        :param cp:   Specific heat of gas during heat addition
+        :param Q_ex: Heat received by the gas in the heat exchange
+
+        :type eta:   float
+        :type cp:    float
+        :type Q_ex:  float
+        :type PI:    float
+        """
+
+        p = heat_exchange(mf       = self.mf,
+                          cp       = cp,
+                          t00      = self.t0,
+                          p00      = self.p0,
+                          Q_ex     = Q_ex,
+                          eta      = eta,
+                          PI       = PI)
 
         self.t0 = p.t01
         self.p0 = p.p01
 
+        self.S  += Q_ex/self.t0
+
         self.state()
 
         return p
 
 
 class fuel:
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huracan-0.0a2/huracan/thermo/processes.py` & `huracan-0.9/huracan/thermo/processes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: GPL-3.0-only
+
+"""
+Huracan thermodynamic process functions
+---------------------------------------
+"""
+
 from huracan.utils import setattr_namespace
 
 
 class process:
     """
     Process data class
     """
@@ -211,42 +219,77 @@
     w   = cp*dt*mf
 
     setattr_namespace(p, locals())
 
     return p
 
 
-def combustion(mf, cp,
-               t00, p00,
-               fuel_mf, fuel_LHV,
-               eta,
-               PI=1):
+def heat_exchange(mf, cp,
+                  t00, p00,
+                  Q_ex,
+                  eta,
+                  PI=1):
     """
     Constant pressure heat addition.
     - A pressure ratio PI may be specified if required.
 
     :param mf:       [kg/s] Gas mass flow
     :param cp:       [-]    Constant pressure specific heat
     :param t00:      [K]    Initial total temperature
     :param p00:      [Pa]   Initial total pressure
-    :param fuel_mf:  [kg/s] Fuel mass flow
-    :param fuel_LHV: [J/kg] Fuel Lower Heating Value (heat of combustion)
+    :param Q_ex:     [K]    Heat received by the gas in the heat exchange
     :param eta:      [-]    Isentropic efficiency
 
     :type mf:        float
     :type fuel_mf:   float
     :type fuel_LHV:  float
     :type t00:       float
     :type p00:       float
     :type eta:       float
     """
 
     p = process()
 
-    dt = eta*(fuel_mf*fuel_LHV)/(mf*cp)
+    dt = eta*Q_ex/(mf*cp)
 
     t01 = t00 + dt
     p01 = p00*PI
 
     setattr_namespace(p, locals())
 
     return p
+
+
+def combustion(mf, cp,
+               t00, p00,
+               fuel_mf, fuel_LHV,
+               eta,
+               PI=1):
+    """
+    Constant pressure heat addition.
+    - A pressure ratio PI may be specified if required.
+
+    :param mf:       [kg/s] Gas mass flow
+    :param cp:       [-]    Constant pressure specific heat
+    :param t00:      [K]    Initial total temperature
+    :param p00:      [Pa]   Initial total pressure
+    :param fuel_mf:  [kg/s] Fuel mass flow
+    :param fuel_LHV: [J/kg] Fuel Lower Heating Value (heat of combustion)
+    :param eta:      [-]    Isentropic efficiency
+
+    :type mf:        float
+    :type fuel_mf:   float
+    :type fuel_LHV:  float
+    :type t00:       float
+    :type p00:       float
+    :type eta:       float
+    """
+
+    Q_in = (fuel_mf*fuel_LHV)
+
+    return heat_exchange(mf=mf, cp=cp,
+                         t00=t00, p00=p00,
+                         Q_ex=Q_in,
+                         eta=eta,
+                         PI=PI
+                         )
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huracan-0.0a2/setup.py` & `huracan-0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="huracan",
-    version="0.0.a2",
+    version="0.9",
     author="Antonio Lopez Rivera",
     author_email="antonlopezr99@gmail.com",
     description="Open source, 0-dimensional, object-oriented airbreathing engine modelling package for preliminary analysis and design of airbreathing engines, divulgation and educational purposes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alopezrivera/huracan",
     packages=setuptools.find_packages(),
     install_requires=[
-        "Python-Alexandria",
-        "mpl_plotter"
+        "numpy>=1.21.2",
+        "mpl_plotter>=4.0.2"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
 )
```

### Comparing `huracan-0.0a2/tests/utils/__init__.py` & `huracan-0.9/tests/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-from alexandria.shell import print_color
-from alexandria.data_structs.string import join_set_distance
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: MPL-2.0
+
+
+from huracan.utils import join_set_distance
 
 
 def verify(prediction, measurement, error_margin=0.001, log=False, name='Error'):
     """
     Model verification:
     - Error must stay under 0.1% of the measurement.
 
@@ -15,8 +18,8 @@
     :type log:           bool
     """
     assert abs(prediction-measurement) < measurement*error_margin, \
         f'Error = {abs(prediction-measurement)/measurement*100:.2f}% of measurement.'
 
     if log:
         s = join_set_distance(name, '=', 10)
-        print_color(s + f' {abs(prediction-measurement)/measurement*100:.2f}% of measurement.', 'yellow')
+        print(s + f' {abs(prediction-measurement)/measurement*100:.2f}% of measurement.')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huracan-0.0a2/tests/verification/turbofan/test_turbofan.py` & `huracan-0.9/tests/verification/turboprop/test_turboprop.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,80 @@
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: GPL-3.0-only
+
 """
 Huracan
 -------
-Three-spool turbofan engine test.
+Single-spool turboprop engine test.
 """
 
 from huracan.engine import shaft
 from huracan.thermo.fluids import gas, fuel
-from huracan.components import inlet, fan, compressor, combustion_chamber, turbine, afterburner, nozzle, power_plant
+from huracan.components import inlet, prop, compressor, combustion_chamber, turbine, nozzle
 
 from tests.utils import verify
 
-mf = 1440
-M  = 0.4
-t  = 281.65
-p  = 89874
-
-bpr = 9.6
+mf = 35
+M  = 0.5
+t  = 288.15
+p  = 101325.00
 
 fuel = fuel(LHV=43e6)
 
 g = gas(mf=mf,
-        cp=lambda T: 1150 if T > 1000 else 1000,
-        k=lambda T: 1.33 if T > 1000 else 1.4,
+        cp=lambda T: 1150 if T > 600 else 1000,
+        k=lambda T: 1.33 if T > 600 else 1.4,
         m=M, t_0=t, p_0=p)
 
-i  = inlet             (PI=0.98)
-fn = fan               (eta=0.94,  PI=1.54)
-c1 = compressor        (eta=0.991, PI=9.61)
-c2 = compressor        (eta=0.92,  PI=3.38)
-cc = combustion_chamber(fuel=fuel, eta=0.985, PI=0.99, t01=1838)
-t1 = turbine           (eta=0.96)
-t2 = turbine           (eta=0.965)
-t3 = turbine           (eta=0.97)
-nc = nozzle            (eta=0.95)
-nf = nozzle            (eta=0.96)
-
-shaft1 = shaft(fn, t3, eta=0.995)
-shaft2 = shaft(c1, t2, eta=0.995)
-shaft3 = shaft(c2, t1, eta=0.995)
+pr = prop(eta=0.9, w=3.91e6, PI=1)
+i  = inlet(PI=1)
+c  = compressor(eta=0.85, PI=11.5)
+cc = combustion_chamber(fuel=fuel, eta=0.995, t01=1130, PI=0.96)
+t  = turbine(eta=0.89)
+n  = nozzle(eta=0.95)
 
-stream = g-i-fn
+shaft1 = shaft(pr, c, t, eta=0.99)
 
-s1core, s1bypass = stream*(bpr/(bpr+1))
-
-s1core-c1-c2-cc-t1-t2-t3-nc
-s1bypass-nf
+stream = g-pr-i-c-cc-t-n
 
 stream.run()
 
 """
 Verification
 
 - Error must stay below 0.1% of the verification value 
 """
 # Total temperature
-verify(stream['0.il'].t0,    290.7)              # Inlet
-verify(stream['0.fn'].t0,    331.3)              # Fan
-verify(stream['1.m.nz'].t0,  287.2)              # Bypass flow nozzle
-verify(stream['1.s.cp1'].t0, 635.1)              # Compressor 1
-verify(stream['1.s.cp2'].t0, 922.4)              # Compressor 2
+verify(stream['0.il'].t0, 302.56)               # Inlet
+verify(stream['0.cp'].t0, 661.84)               # Compressor
 
 # Total pressure
-verify(stream['0.il'].p0,    98343)              # Inlet
-verify(stream['0.fn'].p0,    151447)             # Fan
-verify(stream['1.m.nz'].p0,  89874)              # Bypass flow nozzle
-verify(stream['1.s.cp1'].p0, 1455410)            # Compressor 1
-verify(stream['1.s.cp2'].p0, 4919286)            # Compressor 2
-
-# Heat and work
-verify(fn.w, 58.46e6)                            # Work: Fan
-verify(c1.w, 41.27e6)                            # Work: Compressor 1
-verify(c2.w, 39.03e6)                            # Work: Compressor 2
+verify(stream['0.il'].p0, 120192.99554985)      # Inlet
+verify(stream['0.cp'].p0, 1382219.44882326)     # Compressor
 
 """
 Exceptions:
 
 The fuel mass flow method differs from
 that used by the verification model. 
 This causes differences in the models'
 results after the main combustion chamber.
 
 - Error must stay below 5% of the verification value 
 """
+
+error = 0.05
+
 # Fuel mass flow
-verify(cc.fuel.mf, 3.377, 0.05)
+verify(cc.fuel.mf, 0.4425,          error, log=True, name='e(fmf)')
 
 # Total temperature
-verify(stream['1.s.tb1'].t0, 1593,    0.05)       # Turbine 1
-verify(stream['1.s.tb2'].t0, 1334,    0.05)       # Turbine 2
-verify(stream['1.s.tb3'].t0, 967,     0.05)       # Turbine 3
+verify(stream['0.tb'].t0, 721.35,   error, log=True, name='e(tb.t0)')     # Turbine
+verify(stream['0.nz'].t0, 645.8,    error, log=True, name='e(nz.t0)')     # Nozzle
 
 # Total pressure
-verify(stream['1.s.tb1'].p0, 2666269, 0.05)       # Turbine 1
-verify(stream['1.s.tb2'].p0, 1267264, 0.05)       # Turbine 2
-verify(stream['1.s.tb3'].p0, 330414,  0.05)       # Turbine 3
-
-# Thrust
-verify(s1core._flow_thrust(), 85703, 0.1,
-       True, 'e(T_core)')                         # Thrust
-
-# Efficiency
-verify(stream.sfc(), 11.36e-6, 0.1,
-       True, 'e(SFC)')                            # Specific fuel consumption
+verify(stream['0.tb'].p0, 162.37e3, error, log=True, name='e(tb.p0)')     # Turbine
+verify(stream['0.nz'].p0, 101325)                                         # Nozzle
+
+# Exit velocity
+verify(stream.v_exit(), 417.2,      error, log=True, name='e(v_exit)')
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huracan-0.0a2/tests/verification/turbojet/test_turbojet.py` & `huracan-0.9/tests/verification/turbojet/test_turbojet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: © 2024 Antonio López Rivera <antonlopezr99@gmail.com>
+# SPDX-License-Identifier: GPL-3.0-only
+
 """
 Huracan
 -------
 Twin-spool, reheated turbojet engine test.
 """
 
 from huracan.engine import shaft
@@ -60,20 +63,23 @@
 The fuel mass flow method differs from
 that used by the verification model. 
 This causes differences in the models'
 results after the main combustion chamber.
 
 - Error must stay below 5% of the verification value 
 """
+
+error = 0.05
+
 # Fuel mass flow
-verify(cc.fuel.mf, 3.1921, 0.05)
+verify(cc.fuel.mf, 3.1921,                  error, log=True, name='e(fmf)')
 
 # Total temperature
-verify(stream['0.tb1'].t0, 1227.1163336,  0.05)    # Turbine 1
-verify(stream['0.tb2'].t0, 1085.31099956, 0.05)    # Turbine 2
+verify(stream['0.tb1'].t0, 1227.1163336,    error, log=True, name='e(tb1.t0)')  # Turbine 1
+verify(stream['0.tb2'].t0, 1085.31099956,   error, log=True, name='e(tb2.t0)')  # Turbine 2
 
 # Total pressure
-verify(stream['0.tb1'].p0, 680119.41922727, 0.05)  # Turbine 1
-verify(stream['0.tb2'].p0, 390882.21425195, 0.05)  # Turbine 2
+verify(stream['0.tb1'].p0, 680119.41922727, error, log=True, name='e(tb1.p0)')  # Turbine 1
+verify(stream['0.tb2'].p0, 390882.21425195, error, log=True, name='e(tb2.p0)')  # Turbine 2
 
 # Exit velocity
-verify(stream.v_exit(), 840.3353)
+verify(stream.v_exit(), 840.3353,           error, log=True, name='e(v_exit)')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

