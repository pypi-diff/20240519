# Comparing `tmp/scorev-0.0.4.tar.gz` & `tmp/scorev-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorev-0.0.4.tar", last modified: Sun Mar 27 09:45:19 2022, max compression
+gzip compressed data, was "scorev-0.0.5.tar", last modified: Sun May 19 01:13:26 2024, max compression
```

## Comparing `scorev-0.0.4.tar` & `scorev-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-03-27 09:45:19.818698 scorev-0.0.4/
--rw-r--r--   0 yt        (1000) yt        (1000)     1521 2022-03-27 09:45:19.818698 scorev-0.0.4/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      986 2022-03-27 09:44:19.000000 scorev-0.0.4/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2022-03-27 09:45:19.818698 scorev-0.0.4/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      949 2022-03-27 09:44:46.000000 scorev-0.0.4/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-03-27 09:45:19.802946 scorev-0.0.4/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-03-27 09:45:19.818698 scorev-0.0.4/src/scorev.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1521 2022-03-27 09:45:19.000000 scorev-0.0.4/src/scorev.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      205 2022-03-27 09:45:19.000000 scorev-0.0.4/src/scorev.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2022-03-27 09:45:19.000000 scorev-0.0.4/src/scorev.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       40 2022-03-27 09:45:19.000000 scorev-0.0.4/src/scorev.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        7 2022-03-27 09:45:19.000000 scorev-0.0.4/src/scorev.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     7232 2022-03-27 09:43:23.000000 scorev-0.0.4/src/scorev.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-19 01:13:26.598336 scorev-0.0.5/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1855 2024-05-19 01:13:26.598336 scorev-0.0.5/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1318 2024-05-19 01:12:35.000000 scorev-0.0.5/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-05-19 01:13:26.598336 scorev-0.0.5/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      951 2024-05-19 01:13:04.000000 scorev-0.0.5/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-19 01:13:26.598336 scorev-0.0.5/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-19 01:13:26.598336 scorev-0.0.5/src/scorev.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1855 2024-05-19 01:13:26.000000 scorev-0.0.5/src/scorev.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      205 2024-05-19 01:13:26.000000 scorev-0.0.5/src/scorev.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-05-19 01:13:26.000000 scorev-0.0.5/src/scorev.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       40 2024-05-19 01:13:26.000000 scorev-0.0.5/src/scorev.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        7 2024-05-19 01:13:26.000000 scorev-0.0.5/src/scorev.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     7232 2022-03-27 09:43:23.000000 scorev-0.0.5/src/scorev.py
```

### Comparing `scorev-0.0.4/PKG-INFO` & `scorev-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 Metadata-Version: 2.1
 Name: scorev
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for scoring policies of covid-19 with vaccine rates
-Home-page: https://github.com/ytakefuji/scorev
+Home-page: https://github.com/y-takefuji/scorev
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/scorev
+Project-URL: Bug Tracker, https://github.com/y-takefuji/scorev
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # scorev
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/1f1cb392-a56c-41da-a18d-ca8853a398e7/tree)
+
+Cite:
+takefuji (2022) scorev for scoring COVID-19 policies with vaccine rates [Source Code]. https://doi.org/10.24433/CO.4373206.v1
+
+
 scorev is a PyPI tool for scoring COVID-19 policies in a filename 'oecd.csv' with vaccine rates 
 such as at least 1 dose, fully vaccinated, and booster given.
 
 scorev subsumes PyPI scorecovid application.
 
-The score is calculated by dividing the number of deaths due to COVID-19.
+The score is calculated by dividing the number of deaths due to COVID-19 by the population in millions.
 Generated result.csv has the following determinants:
 deaths, population, score, 1dose (rate: at least 1 dose), full (rate: fully vaccinated), booster (rate: booster given).
 
 Vaccine rates such as 1dose, full, and booster are unreliable 
 since some countries do not often update.
 
 The current program checks the last 8 days in the dataset.
@@ -35,13 +41,13 @@
 
 # How to install scorev
 $ pip install scorev
 
 # How to run scorev
 $ scorerev
 
-<img src='https://github.com/ytakefuji/scorev/raw/main/result.png' width=800 height=1300 >
+<img src='https://github.com/y-takefuji/scorev/raw/main/result.png' width=800 height=1300 >
 
 # How to modify country names
 Modify oecd.csv file for adding and deleting countries.
```

### Comparing `scorev-0.0.4/README.md` & `scorev-0.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # scorev
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/1f1cb392-a56c-41da-a18d-ca8853a398e7/tree)
+
+Cite:
+takefuji (2022) scorev for scoring COVID-19 policies with vaccine rates [Source Code]. https://doi.org/10.24433/CO.4373206.v1
+
+
 scorev is a PyPI tool for scoring COVID-19 policies in a filename 'oecd.csv' with vaccine rates 
 such as at least 1 dose, fully vaccinated, and booster given.
 
 scorev subsumes PyPI scorecovid application.
 
-The score is calculated by dividing the number of deaths due to COVID-19.
+The score is calculated by dividing the number of deaths due to COVID-19 by the population in millions.
 Generated result.csv has the following determinants:
 deaths, population, score, 1dose (rate: at least 1 dose), full (rate: fully vaccinated), booster (rate: booster given).
 
 Vaccine rates such as 1dose, full, and booster are unreliable 
 since some countries do not often update.
 
 The current program checks the last 8 days in the dataset.
@@ -19,11 +25,11 @@
 
 # How to install scorev
 $ pip install scorev
 
 # How to run scorev
 $ scorerev
 
-<img src='https://github.com/ytakefuji/scorev/raw/main/result.png' width=800 height=1300 >
+<img src='https://github.com/y-takefuji/scorev/raw/main/result.png' width=800 height=1300 >
 
 # How to modify country names
 Modify oecd.csv file for adding and deleting countries.
```

### Comparing `scorev-0.0.4/setup.py` & `scorev-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scorev",
-    version="0.0.4",
+    version="0.0.5",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for scoring policies of covid-19 with vaccine rates",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/scorev",
+    url="https://github.com/y-takefuji/scorev",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/scorev",
+        "Bug Tracker": "https://github.com/y-takefuji/scorev",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['scorev'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'scorev = scorev:main'
         ]
     },
 )
```

### Comparing `scorev-0.0.4/src/scorev.egg-info/PKG-INFO` & `scorev-0.0.5/src/scorev.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 Metadata-Version: 2.1
 Name: scorev
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for scoring policies of covid-19 with vaccine rates
-Home-page: https://github.com/ytakefuji/scorev
+Home-page: https://github.com/y-takefuji/scorev
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/scorev
+Project-URL: Bug Tracker, https://github.com/y-takefuji/scorev
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # scorev
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/1f1cb392-a56c-41da-a18d-ca8853a398e7/tree)
+
+Cite:
+takefuji (2022) scorev for scoring COVID-19 policies with vaccine rates [Source Code]. https://doi.org/10.24433/CO.4373206.v1
+
+
 scorev is a PyPI tool for scoring COVID-19 policies in a filename 'oecd.csv' with vaccine rates 
 such as at least 1 dose, fully vaccinated, and booster given.
 
 scorev subsumes PyPI scorecovid application.
 
-The score is calculated by dividing the number of deaths due to COVID-19.
+The score is calculated by dividing the number of deaths due to COVID-19 by the population in millions.
 Generated result.csv has the following determinants:
 deaths, population, score, 1dose (rate: at least 1 dose), full (rate: fully vaccinated), booster (rate: booster given).
 
 Vaccine rates such as 1dose, full, and booster are unreliable 
 since some countries do not often update.
 
 The current program checks the last 8 days in the dataset.
@@ -35,13 +41,13 @@
 
 # How to install scorev
 $ pip install scorev
 
 # How to run scorev
 $ scorerev
 
-<img src='https://github.com/ytakefuji/scorev/raw/main/result.png' width=800 height=1300 >
+<img src='https://github.com/y-takefuji/scorev/raw/main/result.png' width=800 height=1300 >
 
 # How to modify country names
 Modify oecd.csv file for adding and deleting countries.
```

### Comparing `scorev-0.0.4/src/scorev.py` & `scorev-0.0.5/src/scorev.py`

 * *Files identical despite different names*

