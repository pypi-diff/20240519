# Comparing `tmp/pyflagoras-0.2.0.tar.gz` & `tmp/pyflagoras-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflagoras-0.2.0.tar", last modified: Sun May 19 03:29:51 2024, max compression
+gzip compressed data, was "pyflagoras-0.2.1.tar", last modified: Sun May 19 04:18:49 2024, max compression
```

## Comparing `pyflagoras-0.2.0.tar` & `pyflagoras-0.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.954154 pyflagoras-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-19 03:29:51.950153 pyflagoras-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 03:29:51.954154 pyflagoras-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.938154 pyflagoras-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.942154 pyflagoras-0.2.0/src/pyflagoras/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flag_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.950153 pyflagoras-0.2.0/src/pyflagoras/flags/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/agender_2014.json
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/aroace_2018.json
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/aromantic_2014.json
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/asexual_2010.json
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/bear_1995.json
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/bigender_2014.json
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/bisexual_1998.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/gay_men_2019.json
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/genderfluid_2012.json
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/genderqueer_2011.json
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/intersexInclusive_2021.json
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/intersex_2013.json
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/labrysLesbian_1999.json
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2010.json
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2018.json
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2019.json
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/lipstick_lesbian_2010.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/nonbinary_2014.json
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/omnisexual_2015.json
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pangender_2015.json
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pansexual_2010.json
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/philadelphiaPride_2017.json
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pinkUnionJack_2009.json
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/polysexual_2012.json
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pride_1978_eightStripes.json
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pride_1978_sevenStripes.json
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pride_1979.json
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/progressPride_2018.json
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/sapphic_2015.json
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/southAfricaPride_2010.json
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/transgender_1999.json
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/twink_2009.json
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/image_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/pyflagoras.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/similarity_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.950153 pyflagoras-0.2.0/src/pyflagoras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:18:49.589040 pyflagoras-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-19 04:18:49.589040 pyflagoras-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:18:49.589040 pyflagoras-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:18:49.577040 pyflagoras-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:18:49.581040 pyflagoras-0.2.1/src/pyflagoras/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flag_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:18:49.585040 pyflagoras-0.2.1/src/pyflagoras/flags/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/agender_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/aroace_2018.json
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/aromantic_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/asexual_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/bear_1995.json
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/bigender_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/bisexual_1998.json
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/gay_men_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/genderfluid_2012.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/genderqueer_2011.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/intersexInclusive_2021.json
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/intersex_2013.json
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/labrysLesbian_1999.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/lesbian_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/lesbian_2018.json
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/lesbian_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/lipstick_lesbian_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/nonbinary_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/omnisexual_2015.json
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/pangender_2015.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/pansexual_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/philadelphiaPride_2017.json
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/pinkUnionJack_2009.json
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/polysexual_2012.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/pride_1978_eightStripes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/pride_1978_sevenStripes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/pride_1979.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/progressPride_2018.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/sapphic_2015.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/southAfricaPride_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/transgender_1999.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/flags/twink_2009.json
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/image_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/pyflagoras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/similarity_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 04:18:40.000000 pyflagoras-0.2.1/src/pyflagoras/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:18:49.585040 pyflagoras-0.2.1/src/pyflagoras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-19 04:18:49.000000 pyflagoras-0.2.1/src/pyflagoras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-19 04:18:49.000000 pyflagoras-0.2.1/src/pyflagoras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:18:49.000000 pyflagoras-0.2.1/src/pyflagoras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 04:18:49.000000 pyflagoras-0.2.1/src/pyflagoras.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 04:18:49.000000 pyflagoras-0.2.1/src/pyflagoras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 04:18:49.000000 pyflagoras-0.2.1/src/pyflagoras.egg-info/top_level.txt
```

### Comparing `pyflagoras-0.2.0/LICENSE` & `pyflagoras-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/PKG-INFO` & `pyflagoras-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflagoras
-Version: 0.2.0
+Version: 0.2.1
 Summary: A command line interface tool to generate pride flags from images.
 Author-email: Annabel Quach <annabelquach13@gmail.com>
 Project-URL: Homepage, https://github.com/phthallo/pyflagoras
 Project-URL: Bug Tracker, https://github.com/phthallo/pyflagoras/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyflagoras-0.2.0/README.md` & `pyflagoras-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/pyproject.toml` & `pyflagoras-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 
 build-backend = "setuptools.build_meta"
 [project.scripts]
 pyflagoras = "pyflagoras:__main__.main"
 [project]
 name = "pyflagoras"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
 "pillow>=10.3.0"
 ]
 authors = [
   { name="Annabel Quach", email="annabelquach13@gmail.com" },
 ]
 description = "A command line interface tool to generate pride flags from images."
```

### Comparing `pyflagoras-0.2.0/src/pyflagoras/__main__.py` & `pyflagoras-0.2.1/src/pyflagoras/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,13 +53,13 @@
                     version=__version__, help="show the program's version number and exit")
 
 def main() -> None:
     args = parser.parse_args()
     pyflag = Pyflagoras(
         image=args.image,
         flag=args.flag,
-        output=args.output
+        name=args.name
     )
     pyflag.run()
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flag_info.py` & `pyflagoras-0.2.1/src/pyflagoras/flag_info.py`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/agender_2014.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/agender_2014.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/aroace_2018.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/aroace_2018.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/aromantic_2014.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/aromantic_2014.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/asexual_2010.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/asexual_2010.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/bear_1995.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/bear_1995.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/bigender_2014.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/bigender_2014.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/bisexual_1998.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/bisexual_1998.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/gay_men_2019.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/gay_men_2019.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/genderfluid_2012.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/genderfluid_2012.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/intersexInclusive_2021.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/intersexInclusive_2021.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/labrysLesbian_1999.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/labrysLesbian_1999.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2010.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/lesbian_2010.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2018.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/lesbian_2018.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2019.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/lesbian_2019.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/lipstick_lesbian_2010.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/lipstick_lesbian_2010.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/nonbinary_2014.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/nonbinary_2014.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/omnisexual_2015.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/omnisexual_2015.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/pangender_2015.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/pangender_2015.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/philadelphiaPride_2017.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/philadelphiaPride_2017.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/pinkUnionJack_2009.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/pinkUnionJack_2009.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/pride_1978_eightStripes.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/pride_1978_eightStripes.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/pride_1978_sevenStripes.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/pride_1978_sevenStripes.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/pride_1979.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/pride_1979.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/progressPride_2018.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/progressPride_2018.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/sapphic_2015.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/sapphic_2015.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/southAfricaPride_2010.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/southAfricaPride_2010.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/transgender_1999.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/transgender_1999.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/flags/twink_2009.json` & `pyflagoras-0.2.1/src/pyflagoras/flags/twink_2009.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/pyflagoras.py` & `pyflagoras-0.2.1/src/pyflagoras/pyflagoras.py`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras/similarity_algorithms.py` & `pyflagoras-0.2.1/src/pyflagoras/similarity_algorithms.py`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.2.0/src/pyflagoras.egg-info/PKG-INFO` & `pyflagoras-0.2.1/src/pyflagoras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflagoras
-Version: 0.2.0
+Version: 0.2.1
 Summary: A command line interface tool to generate pride flags from images.
 Author-email: Annabel Quach <annabelquach13@gmail.com>
 Project-URL: Homepage, https://github.com/phthallo/pyflagoras
 Project-URL: Bug Tracker, https://github.com/phthallo/pyflagoras/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyflagoras-0.2.0/src/pyflagoras.egg-info/SOURCES.txt` & `pyflagoras-0.2.1/src/pyflagoras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

