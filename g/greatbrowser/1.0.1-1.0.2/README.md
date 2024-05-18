# Comparing `tmp/greatbrowser-1.0.1.tar.gz` & `tmp/greatbrowser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatbrowser-1.0.1.tar", last modified: Sun May 12 23:57:30 2024, max compression
+gzip compressed data, was "greatbrowser-1.0.2.tar", last modified: Sat May 18 22:21:09 2024, max compression
```

## Comparing `greatbrowser-1.0.1.tar` & `greatbrowser-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/greatbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/greatbrowser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/greatbrowser/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/greatbrowser/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/greatbrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:21:09.137856 greatbrowser-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-18 22:20:52.000000 greatbrowser-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-18 22:21:09.137856 greatbrowser-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-18 22:20:52.000000 greatbrowser-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:21:09.137856 greatbrowser-1.0.2/greatbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 22:20:52.000000 greatbrowser-1.0.2/greatbrowser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-18 22:20:52.000000 greatbrowser-1.0.2/greatbrowser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-18 22:20:52.000000 greatbrowser-1.0.2/greatbrowser/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:21:09.137856 greatbrowser-1.0.2/greatbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-18 22:21:09.000000 greatbrowser-1.0.2/greatbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-18 22:21:09.000000 greatbrowser-1.0.2/greatbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:21:09.000000 greatbrowser-1.0.2/greatbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-18 22:21:09.000000 greatbrowser-1.0.2/greatbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 22:21:09.000000 greatbrowser-1.0.2/greatbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:21:09.137856 greatbrowser-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-18 22:20:52.000000 greatbrowser-1.0.2/setup.py
```

### Comparing `greatbrowser-1.0.1/LICENSE` & `greatbrowser-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.1/PKG-INFO` & `greatbrowser-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automate Stanford's GREAT browser
 Author: Sam Anderson
 Author-email: sanderson01@wesleyan.edu
 Project-URL: Source, https://github.com/SamAndTheSun/greatbrowser
 Project-URL: Bug Reports, https://github.com/SamAndTheSun/greatbrowser/issues
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# greatbrowser v1.0.1
+# greatbrowser v1.0.2
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -34,14 +34,15 @@
 
 The user experience is primarily built around a single function, great_analysis(), with the complementary functions great_get_options() and great_global_controls()
 providing context regarding some of the parameters for this function.
 
 The current version supports the ability to find gene associations using probe sets as well the ability to download any GREAT-generated table or plot in dataframe form. 
 UCSC genome browser implementation is also supported. Customizability is controlled through parameter tuning, some of which are specific, 
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
+Because the project uses switch statements, its requires python >= 3.10 to run.
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings, 
 but is not ideal if one desires to perform highly custom visual modifications to specifically the raw barplot or hierarchy plots generated by GREAT. 
 
 This repository is not affiliated with the official GREAT browser and was developed solely for the sake of convenience.
```

### Comparing `greatbrowser-1.0.1/README.md` & `greatbrowser-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# greatbrowser v1.0.1
+# greatbrowser v1.0.2
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -17,14 +17,15 @@
 
 The user experience is primarily built around a single function, great_analysis(), with the complementary functions great_get_options() and great_global_controls()
 providing context regarding some of the parameters for this function.
 
 The current version supports the ability to find gene associations using probe sets as well the ability to download any GREAT-generated table or plot in dataframe form. 
 UCSC genome browser implementation is also supported. Customizability is controlled through parameter tuning, some of which are specific, 
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
+Because the project uses switch statements, its requires python >= 3.10 to run.
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings, 
 but is not ideal if one desires to perform highly custom visual modifications to specifically the raw barplot or hierarchy plots generated by GREAT. 
 
 This repository is not affiliated with the official GREAT browser and was developed solely for the sake of convenience.
```

### Comparing `greatbrowser-1.0.1/greatbrowser/functions.py` & `greatbrowser-1.0.2/greatbrowser/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,27 +51,30 @@
 
     #convert list to np array
     if isinstance(bed_data, list):
         bed_data = np.array(bed_data)
 
     #load file as df
     elif isinstance(bed_data, str):
-        bed_data = pd.read_excel(bed_data)
+        try: bed_data = pd.read_excel(bed_data)
+        except: bed_data = pd.read_csv(bed_data)
 
     #format df
     if isinstance(bed_data, pd.DataFrame) or isinstance(bed_data, pl.DataFrame):
 
         n = 0
         if isinstance(bed_data, pd.DataFrame) or isinstance(bed_data, pl.DataFrame):
             while n < bed_data.shape[1]: #get appropriate columns
-                df_dict[potential_cols[n]] = bed_data.iloc[:, n]
+                try: df_dict[potential_cols[n]] = bed_data[potential_cols[n]]
+                except: pass
                 n+=1
         elif isinstance(bed_data, np.ndarray):
             while n < bed_data.shape[1]: #get appropriate columns
-                df_dict[potential_cols[n]] = bed_data[:, n]
+                try: df_dict[potential_cols[n]] = bed_data[:, n]
+                except: pass
                 n+=1
         if n < 4: #if there's no index, add one:
             df_dict[potential_cols[n]] = [x for x in range(len(df_dict[potential_cols[n-1]]))]
 
         bed_data = pd.DataFrame().from_dict(df_dict)
 
         #mandatory inputs
```

### Comparing `greatbrowser-1.0.1/greatbrowser/main.py` & `greatbrowser-1.0.2/greatbrowser/main.py`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.1/greatbrowser.egg-info/PKG-INFO` & `greatbrowser-1.0.2/greatbrowser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automate Stanford's GREAT browser
 Author: Sam Anderson
 Author-email: sanderson01@wesleyan.edu
 Project-URL: Source, https://github.com/SamAndTheSun/greatbrowser
 Project-URL: Bug Reports, https://github.com/SamAndTheSun/greatbrowser/issues
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# greatbrowser v1.0.1
+# greatbrowser v1.0.2
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -34,14 +34,15 @@
 
 The user experience is primarily built around a single function, great_analysis(), with the complementary functions great_get_options() and great_global_controls()
 providing context regarding some of the parameters for this function.
 
 The current version supports the ability to find gene associations using probe sets as well the ability to download any GREAT-generated table or plot in dataframe form. 
 UCSC genome browser implementation is also supported. Customizability is controlled through parameter tuning, some of which are specific, 
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
+Because the project uses switch statements, its requires python >= 3.10 to run.
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings, 
 but is not ideal if one desires to perform highly custom visual modifications to specifically the raw barplot or hierarchy plots generated by GREAT. 
 
 This repository is not affiliated with the official GREAT browser and was developed solely for the sake of convenience.
```

### Comparing `greatbrowser-1.0.1/setup.py` & `greatbrowser-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = "Automate Stanford's GREAT browser"
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
```

