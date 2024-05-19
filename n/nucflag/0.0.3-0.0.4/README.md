# Comparing `tmp/nucflag-0.0.3.tar.gz` & `tmp/nucflag-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucflag-0.0.3.tar", last modified: Sat May  4 04:09:29 2024, max compression
+gzip compressed data, was "nucflag-0.0.4.tar", last modified: Sun May 19 10:23:30 2024, max compression
```

## Comparing `nucflag-0.0.3.tar` & `nucflag-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-04 04:09:29.612541 nucflag-0.0.3/
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     1078 2024-05-04 03:49:09.000000 nucflag-0.0.3/LICENSE
--rw-r--r--   0 koisland  (1000) koisland  (1000)     6429 2024-05-04 04:09:29.612541 nucflag-0.0.3/PKG-INFO
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     5881 2024-05-04 03:50:23.000000 nucflag-0.0.3/README.md
-drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-04 04:09:29.612541 nucflag-0.0.3/nucflag/
--rw-rw-r--   0 koisland  (1000) koisland  (1000)        0 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/__init__.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     9239 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/classifier.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      586 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/config.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      140 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/constants.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     2743 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/io.py
--rwxrwxr-x   0 koisland  (1000) koisland  (1000)     5803 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/main.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      627 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/misassembly.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     2623 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/plot.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     1112 2024-05-04 03:50:23.000000 nucflag-0.0.3/nucflag/region.py
-drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-04 04:09:29.612541 nucflag-0.0.3/nucflag.egg-info/
--rw-r--r--   0 koisland  (1000) koisland  (1000)     6429 2024-05-04 04:09:29.000000 nucflag-0.0.3/nucflag.egg-info/PKG-INFO
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      446 2024-05-04 04:09:29.000000 nucflag-0.0.3/nucflag.egg-info/SOURCES.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)        1 2024-05-04 04:09:29.000000 nucflag-0.0.3/nucflag.egg-info/dependency_links.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)       46 2024-05-04 04:09:29.000000 nucflag-0.0.3/nucflag.egg-info/entry_points.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)       91 2024-05-04 04:09:29.000000 nucflag-0.0.3/nucflag.egg-info/requires.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)        8 2024-05-04 04:09:29.000000 nucflag-0.0.3/nucflag.egg-info/top_level.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      824 2024-05-04 04:09:03.000000 nucflag-0.0.3/pyproject.toml
--rw-rw-r--   0 koisland  (1000) koisland  (1000)       91 2024-05-04 03:49:09.000000 nucflag-0.0.3/requirements.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)       38 2024-05-04 04:09:29.612541 nucflag-0.0.3/setup.cfg
-drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-04 04:09:29.612541 nucflag-0.0.3/test/
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      744 2024-05-04 03:50:23.000000 nucflag-0.0.3/test/test_nucplot.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     1433 2024-05-04 03:50:23.000000 nucflag-0.0.3/test/test_region.py
+drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-19 10:23:30.570388 nucflag-0.0.4/
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)     1078 2024-05-04 03:49:09.000000 nucflag-0.0.4/LICENSE
+-rw-r--r--   0 koisland  (1000) koisland  (1000)     6421 2024-05-19 10:23:30.570388 nucflag-0.0.4/PKG-INFO
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)     5873 2024-05-19 10:08:26.000000 nucflag-0.0.4/README.md
+drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-19 10:23:30.566388 nucflag-0.0.4/nucflag/
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)        0 2024-05-19 10:08:26.000000 nucflag-0.0.4/nucflag/__init__.py
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)     9239 2024-05-19 10:08:26.000000 nucflag-0.0.4/nucflag/classifier.py
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)      586 2024-05-19 10:08:26.000000 nucflag-0.0.4/nucflag/config.py
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)      140 2024-05-19 10:08:26.000000 nucflag-0.0.4/nucflag/constants.py
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)     2743 2024-05-19 10:08:26.000000 nucflag-0.0.4/nucflag/io.py
+-rwxrwxr-x   0 koisland  (1000) koisland  (1000)     5927 2024-05-19 10:23:05.000000 nucflag-0.0.4/nucflag/main.py
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)      627 2024-05-19 10:08:26.000000 nucflag-0.0.4/nucflag/misassembly.py
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)     2623 2024-05-19 10:08:26.000000 nucflag-0.0.4/nucflag/plot.py
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)     1112 2024-05-19 10:08:26.000000 nucflag-0.0.4/nucflag/region.py
+drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-19 10:23:30.570388 nucflag-0.0.4/nucflag.egg-info/
+-rw-r--r--   0 koisland  (1000) koisland  (1000)     6421 2024-05-19 10:23:30.000000 nucflag-0.0.4/nucflag.egg-info/PKG-INFO
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)      446 2024-05-19 10:23:30.000000 nucflag-0.0.4/nucflag.egg-info/SOURCES.txt
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)        1 2024-05-19 10:23:30.000000 nucflag-0.0.4/nucflag.egg-info/dependency_links.txt
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)       46 2024-05-19 10:23:30.000000 nucflag-0.0.4/nucflag.egg-info/entry_points.txt
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)       91 2024-05-19 10:23:30.000000 nucflag-0.0.4/nucflag.egg-info/requires.txt
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)        8 2024-05-19 10:23:30.000000 nucflag-0.0.4/nucflag.egg-info/top_level.txt
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)      824 2024-05-19 10:23:05.000000 nucflag-0.0.4/pyproject.toml
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)       91 2024-05-04 03:49:09.000000 nucflag-0.0.4/requirements.txt
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)       38 2024-05-19 10:23:30.570388 nucflag-0.0.4/setup.cfg
+drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-19 10:23:30.570388 nucflag-0.0.4/test/
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)      744 2024-05-19 10:08:26.000000 nucflag-0.0.4/test/test_nucplot.py
+-rw-rw-r--   0 koisland  (1000) koisland  (1000)     1433 2024-05-19 10:08:26.000000 nucflag-0.0.4/test/test_region.py
```

### Comparing `nucflag-0.0.3/LICENSE` & `nucflag-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.3/PKG-INFO` & `nucflag-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucflag
-Version: 0.0.3
+Version: 0.0.4
 Summary: NucFlag misassembly identifier.
 Author-email: Keith Oshima <oshimak@pennmedicine.upenn.edu>, "Mitchell R. Vollger" <mrvollger@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/logsdon-lab/NucFlag
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,23 +13,23 @@
 Requires-Dist: polars==0.20.16
 Requires-Dist: portion==2.4.2
 Requires-Dist: pysam==0.22.0
 Requires-Dist: scipy==1.12.0
 
 # `NucFlag`
 [![CI](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml/badge.svg)](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml)
+[![PyPI - Version](https://img.shields.io/pypi/v/nucflag)](https://pypi.org/project/nucflag/)
 
 Fork of [`NucFreq`](https://github.com/mrvollger/NucFreq). Script for making nucleotide frequency plots and marking misassemblies.
 
 ![Labeled Misassemblies](docs/imgs/misassemblies.png)
 
 ## Usage
-Install from GitHub.
 ```bash
-pip install git+https://github.com/logsdon-lab/NucFlag.git
+pip install nucflag
 ```
 
 ```
 usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG]
                [--ignore_regions IGNORE_REGIONS]
 
 Use per-base read coverage to classify/plot misassemblies.
@@ -152,10 +152,8 @@
 ## Cite
 - **Vollger MR**, Dishuck PC, Sorensen M, Welch AE, Dang V, Dougherty ML, et al. Long-read sequence and assembly of segmental duplications. Nat Methods. 2019;16: 88–94. doi:10.1038/s41592-018-0236-3
 - **Mc Cartney AM**, Shafin K, Alonge M, Bzikadze AV, Formenti G, Fungtammasan A, et al. Chasing perfection: validation and polishing strategies for telomere-to-telomere genome assemblies. bioRxiv. 2021. p. 2021.07.02.450803. doi:10.1101/2021.07.02.450803
   * Citing `hetDetection.R`
 
 ## TODO
 - Add false duplication detection.
-- Publish on pypi.
-- Refactor so cleaner.
 - Colormap for `Misassembly`
```

### Comparing `nucflag-0.0.3/README.md` & `nucflag-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # `NucFlag`
 [![CI](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml/badge.svg)](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml)
+[![PyPI - Version](https://img.shields.io/pypi/v/nucflag)](https://pypi.org/project/nucflag/)
 
 Fork of [`NucFreq`](https://github.com/mrvollger/NucFreq). Script for making nucleotide frequency plots and marking misassemblies.
 
 ![Labeled Misassemblies](docs/imgs/misassemblies.png)
 
 ## Usage
-Install from GitHub.
 ```bash
-pip install git+https://github.com/logsdon-lab/NucFlag.git
+pip install nucflag
 ```
 
 ```
 usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG]
                [--ignore_regions IGNORE_REGIONS]
 
 Use per-base read coverage to classify/plot misassemblies.
@@ -135,10 +135,8 @@
 ## Cite
 - **Vollger MR**, Dishuck PC, Sorensen M, Welch AE, Dang V, Dougherty ML, et al. Long-read sequence and assembly of segmental duplications. Nat Methods. 2019;16: 88–94. doi:10.1038/s41592-018-0236-3
 - **Mc Cartney AM**, Shafin K, Alonge M, Bzikadze AV, Formenti G, Fungtammasan A, et al. Chasing perfection: validation and polishing strategies for telomere-to-telomere genome assemblies. bioRxiv. 2021. p. 2021.07.02.450803. doi:10.1101/2021.07.02.450803
   * Citing `hetDetection.R`
 
 ## TODO
 - Add false duplication detection.
-- Publish on pypi.
-- Refactor so cleaner.
 - Colormap for `Misassembly`
```

### Comparing `nucflag-0.0.3/nucflag/classifier.py` & `nucflag-0.0.4/nucflag/classifier.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.3/nucflag/config.py` & `nucflag-0.0.4/nucflag/config.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.3/nucflag/io.py` & `nucflag-0.0.4/nucflag/io.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.3/nucflag/main.py` & `nucflag-0.0.4/nucflag/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,19 @@
     for region_info, df_misasm in zip(regions, results):
         if not df_misasm.is_empty():
             region_status.append((*region_info, RegionStatus.MISASSEMBLED))
             dfs_misasm.append(df_misasm)
         else:
             region_status.append((*region_info, RegionStatus.GOOD))
 
-    df_all_misasm: pl.DataFrame = pl.concat(dfs_misasm)
+    try:
+        df_all_misasm: pl.DataFrame = pl.concat(dfs_misasm)
+    except pl.exceptions.NoDataError:
+        df_all_misasm = pl.DataFrame(schema=["contig", "start", "end"])
+
     df_all_misasm.sort(by=["contig", "start"]).write_csv(
         file=args.output_misasm, include_header=False, separator="\t"
     )
 
     if args.output_status:
         df_asm_status = pl.DataFrame(
             region_status, schema=["contig", "start", "end", "status"]
```

### Comparing `nucflag-0.0.3/nucflag/misassembly.py` & `nucflag-0.0.4/nucflag/misassembly.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.3/nucflag/plot.py` & `nucflag-0.0.4/nucflag/plot.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.3/nucflag/region.py` & `nucflag-0.0.4/nucflag/region.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.3/nucflag.egg-info/PKG-INFO` & `nucflag-0.0.4/nucflag.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucflag
-Version: 0.0.3
+Version: 0.0.4
 Summary: NucFlag misassembly identifier.
 Author-email: Keith Oshima <oshimak@pennmedicine.upenn.edu>, "Mitchell R. Vollger" <mrvollger@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/logsdon-lab/NucFlag
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,23 +13,23 @@
 Requires-Dist: polars==0.20.16
 Requires-Dist: portion==2.4.2
 Requires-Dist: pysam==0.22.0
 Requires-Dist: scipy==1.12.0
 
 # `NucFlag`
 [![CI](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml/badge.svg)](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml)
+[![PyPI - Version](https://img.shields.io/pypi/v/nucflag)](https://pypi.org/project/nucflag/)
 
 Fork of [`NucFreq`](https://github.com/mrvollger/NucFreq). Script for making nucleotide frequency plots and marking misassemblies.
 
 ![Labeled Misassemblies](docs/imgs/misassemblies.png)
 
 ## Usage
-Install from GitHub.
 ```bash
-pip install git+https://github.com/logsdon-lab/NucFlag.git
+pip install nucflag
 ```
 
 ```
 usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG]
                [--ignore_regions IGNORE_REGIONS]
 
 Use per-base read coverage to classify/plot misassemblies.
@@ -152,10 +152,8 @@
 ## Cite
 - **Vollger MR**, Dishuck PC, Sorensen M, Welch AE, Dang V, Dougherty ML, et al. Long-read sequence and assembly of segmental duplications. Nat Methods. 2019;16: 88–94. doi:10.1038/s41592-018-0236-3
 - **Mc Cartney AM**, Shafin K, Alonge M, Bzikadze AV, Formenti G, Fungtammasan A, et al. Chasing perfection: validation and polishing strategies for telomere-to-telomere genome assemblies. bioRxiv. 2021. p. 2021.07.02.450803. doi:10.1101/2021.07.02.450803
   * Citing `hetDetection.R`
 
 ## TODO
 - Add false duplication detection.
-- Publish on pypi.
-- Refactor so cleaner.
 - Colormap for `Misassembly`
```

### Comparing `nucflag-0.0.3/pyproject.toml` & `nucflag-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [tool.setuptools.packages.find]
 include = ["nucflag*"]
 exclude = ["docs*", "test*"]
 
 [project]
 name = "nucflag"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name = "Keith Oshima", email = "oshimak@pennmedicine.upenn.edu"},
     {name = "Mitchell R. Vollger", email = "mrvollger@gmail.com"},
 ]
 description = "NucFlag misassembly identifier."
 readme = "README.md"
 requires-python = ">=3.12"
```

### Comparing `nucflag-0.0.3/test/test_nucplot.py` & `nucflag-0.0.4/test/test_nucplot.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.3/test/test_region.py` & `nucflag-0.0.4/test/test_region.py`

 * *Files identical despite different names*

