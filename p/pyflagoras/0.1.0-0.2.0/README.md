# Comparing `tmp/pyflagoras-0.1.0.tar.gz` & `tmp/pyflagoras-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflagoras-0.1.0.tar", last modified: Sat May 18 12:04:24 2024, max compression
+gzip compressed data, was "pyflagoras-0.2.0.tar", last modified: Sun May 19 03:29:51 2024, max compression
```

## Comparing `pyflagoras-0.1.0.tar` & `pyflagoras-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 12:04:24.863814 pyflagoras-0.1.0/
--rw-rw-rw-   0        0        0     1085 2024-05-17 13:55:21.000000 pyflagoras-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-18 06:08:59.000000 pyflagoras-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1576 2024-05-18 12:04:24.861750 pyflagoras-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      915 2024-05-18 04:19:42.000000 pyflagoras-0.1.0/README.md
--rw-rw-rw-   0        0        0      778 2024-05-18 12:03:41.000000 pyflagoras-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 12:04:24.863814 pyflagoras-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-18 12:04:24.590549 pyflagoras-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-18 12:04:24.651619 pyflagoras-0.1.0/src/pyflagoras/
--rw-rw-rw-   0        0        0       34 2024-05-18 05:52:11.000000 pyflagoras-0.1.0/src/pyflagoras/__init__.py
--rw-rw-rw-   0        0        0      674 2024-05-18 11:10:41.000000 pyflagoras-0.1.0/src/pyflagoras/__main__.py
--rw-rw-rw-   0        0        0      798 2024-05-18 10:45:46.000000 pyflagoras-0.1.0/src/pyflagoras/flag_info.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:04:24.833982 pyflagoras-0.1.0/src/pyflagoras/flags/
--rw-rw-rw-   0        0        0      515 2024-05-16 07:11:17.000000 pyflagoras-0.1.0/src/pyflagoras/flags/agender_2014.json
--rw-rw-rw-   0        0        0      719 2024-05-16 07:11:18.000000 pyflagoras-0.1.0/src/pyflagoras/flags/aroace_2018.json
--rw-rw-rw-   0        0        0      639 2024-05-16 07:11:20.000000 pyflagoras-0.1.0/src/pyflagoras/flags/aromantic_2014.json
--rw-rw-rw-   0        0        0      571 2024-05-16 07:11:21.000000 pyflagoras-0.1.0/src/pyflagoras/flags/asexual_2010.json
--rw-rw-rw-   0        0        0     1579 2024-05-16 07:11:23.000000 pyflagoras-0.1.0/src/pyflagoras/flags/bear_1995.json
--rw-rw-rw-   0        0        0      835 2024-05-16 07:11:24.000000 pyflagoras-0.1.0/src/pyflagoras/flags/bigender_2014.json
--rw-rw-rw-   0        0        0      533 2024-05-16 07:11:26.000000 pyflagoras-0.1.0/src/pyflagoras/flags/bisexual_1998.json
--rw-rw-rw-   0        0        0      929 2024-05-16 07:11:27.000000 pyflagoras-0.1.0/src/pyflagoras/flags/gay_men_2019.json
--rw-rw-rw-   0        0        0      631 2024-05-16 07:11:29.000000 pyflagoras-0.1.0/src/pyflagoras/flags/genderfluid_2012.json
--rw-rw-rw-   0        0        0      484 2024-05-16 07:11:30.000000 pyflagoras-0.1.0/src/pyflagoras/flags/genderqueer_2011.json
--rw-rw-rw-   0        0        0     1750 2024-05-16 07:11:34.000000 pyflagoras-0.1.0/src/pyflagoras/flags/intersexInclusive_2021.json
--rw-rw-rw-   0        0        0      420 2024-05-16 07:11:32.000000 pyflagoras-0.1.0/src/pyflagoras/flags/intersex_2013.json
--rw-rw-rw-   0        0        0      773 2024-05-16 07:11:35.000000 pyflagoras-0.1.0/src/pyflagoras/flags/labrysLesbian_1999.json
--rw-rw-rw-   0        0        0      930 2024-05-16 07:11:37.000000 pyflagoras-0.1.0/src/pyflagoras/flags/lesbian_2010.json
--rw-rw-rw-   0        0        0     1026 2024-05-16 07:11:39.000000 pyflagoras-0.1.0/src/pyflagoras/flags/lesbian_2018.json
--rw-rw-rw-   0        0        0      704 2024-05-16 07:39:08.000000 pyflagoras-0.1.0/src/pyflagoras/flags/lesbian_2019.json
--rw-rw-rw-   0        0        0     4536 2024-05-16 07:11:42.000000 pyflagoras-0.1.0/src/pyflagoras/flags/lipstick_lesbian_2010.json
--rw-rw-rw-   0        0        0      643 2024-05-16 07:11:43.000000 pyflagoras-0.1.0/src/pyflagoras/flags/nonbinary_2014.json
--rw-rw-rw-   0        0        0      728 2024-05-16 07:11:44.000000 pyflagoras-0.1.0/src/pyflagoras/flags/omnisexual_2015.json
--rw-rw-rw-   0        0        0      656 2024-05-16 07:11:46.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pangender_2015.json
--rw-rw-rw-   0        0        0      485 2024-05-16 07:11:48.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pansexual_2010.json
--rw-rw-rw-   0        0        0     1024 2024-05-16 07:11:49.000000 pyflagoras-0.1.0/src/pyflagoras/flags/philadelphiaPride_2017.json
--rw-rw-rw-   0        0        0      817 2024-05-16 07:11:50.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pinkUnionJack_2009.json
--rw-rw-rw-   0        0        0      483 2024-05-16 07:11:52.000000 pyflagoras-0.1.0/src/pyflagoras/flags/polysexual_2012.json
--rw-rw-rw-   0        0        0     1036 2024-05-16 07:11:53.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pride_1978_eightStripes.json
--rw-rw-rw-   0        0        0      920 2024-05-16 07:11:55.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pride_1978_sevenStripes.json
--rw-rw-rw-   0        0        0      833 2024-05-16 07:11:56.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pride_1979.json
--rw-rw-rw-   0        0        0     1568 2024-05-16 07:11:58.000000 pyflagoras-0.1.0/src/pyflagoras/flags/progressPride_2018.json
-drwxrwxrwx   0        0        0        0 2024-05-18 12:04:24.855527 pyflagoras-0.1.0/src/pyflagoras/flags/pyflagoras.egg-info/
--rw-rw-rw-   0        0        0     1576 2024-05-18 05:52:35.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pyflagoras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2024-05-18 05:52:35.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pyflagoras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 05:52:35.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pyflagoras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-18 05:52:35.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pyflagoras.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-05-18 05:52:35.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pyflagoras.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 05:52:35.000000 pyflagoras-0.1.0/src/pyflagoras/flags/pyflagoras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2544 2024-05-16 07:11:59.000000 pyflagoras-0.1.0/src/pyflagoras/flags/sapphic_2015.json
--rw-rw-rw-   0        0        0     1135 2024-05-16 07:12:01.000000 pyflagoras-0.1.0/src/pyflagoras/flags/southAfricaPride_2010.json
--rw-rw-rw-   0        0        0      517 2024-05-16 07:12:02.000000 pyflagoras-0.1.0/src/pyflagoras/flags/transgender_1999.json
--rw-rw-rw-   0        0        0     1591 2024-05-16 07:12:04.000000 pyflagoras-0.1.0/src/pyflagoras/flags/twink_2009.json
--rw-rw-rw-   0        0        0      464 2024-05-18 05:16:25.000000 pyflagoras-0.1.0/src/pyflagoras/image_processor.py
--rw-rw-rw-   0        0        0     3426 2024-05-18 11:56:33.000000 pyflagoras-0.1.0/src/pyflagoras/pyflagoras.py
--rw-rw-rw-   0        0        0     1365 2024-05-18 02:23:43.000000 pyflagoras-0.1.0/src/pyflagoras/similarity_algorithms.py
--rw-rw-rw-   0        0        0      145 2024-05-18 03:31:44.000000 pyflagoras-0.1.0/src/pyflagoras/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:04:24.859228 pyflagoras-0.1.0/src/pyflagoras.egg-info/
--rw-rw-rw-   0        0        0     1576 2024-05-18 12:04:24.000000 pyflagoras-0.1.0/src/pyflagoras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2162 2024-05-18 12:04:24.000000 pyflagoras-0.1.0/src/pyflagoras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 12:04:24.000000 pyflagoras-0.1.0/src/pyflagoras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-18 12:04:24.000000 pyflagoras-0.1.0/src/pyflagoras.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-05-18 12:04:24.000000 pyflagoras-0.1.0/src/pyflagoras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 12:04:24.000000 pyflagoras-0.1.0/src/pyflagoras.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.954154 pyflagoras-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-19 03:29:51.950153 pyflagoras-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 03:29:51.954154 pyflagoras-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.938154 pyflagoras-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.942154 pyflagoras-0.2.0/src/pyflagoras/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flag_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.950153 pyflagoras-0.2.0/src/pyflagoras/flags/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/agender_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/aroace_2018.json
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/aromantic_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/asexual_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/bear_1995.json
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/bigender_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/bisexual_1998.json
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/gay_men_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/genderfluid_2012.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/genderqueer_2011.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/intersexInclusive_2021.json
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/intersex_2013.json
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/labrysLesbian_1999.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2018.json
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/lipstick_lesbian_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/nonbinary_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/omnisexual_2015.json
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pangender_2015.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pansexual_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/philadelphiaPride_2017.json
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pinkUnionJack_2009.json
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/polysexual_2012.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pride_1978_eightStripes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pride_1978_sevenStripes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/pride_1979.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/progressPride_2018.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/sapphic_2015.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/southAfricaPride_2010.json
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/transgender_1999.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/flags/twink_2009.json
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/image_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/pyflagoras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/similarity_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 03:29:44.000000 pyflagoras-0.2.0/src/pyflagoras/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:29:51.950153 pyflagoras-0.2.0/src/pyflagoras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 03:29:51.000000 pyflagoras-0.2.0/src/pyflagoras.egg-info/top_level.txt
```

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flag_info.py` & `pyflagoras-0.2.0/src/pyflagoras/flag_info.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import json
-import os 
-from importlib.resources import files
-
-def flag_attr(flag_name: str) -> str:
-    if not (os.path.exists(os.path.join(os.path.dirname(__file__), "flags", flag_name+".json"))):
-        raise Exception(f"{flag_name} is an invalid flag name.")
-    location = files("pyflagoras.flags").joinpath(flag_name+".json").read_text(encoding="utf-8")
-    data = json.loads(location)
-    return data
-
-def format_rgb(flag_colours: list[dict]) -> list[tuple]:
-    """
-    Formats the colours of the provided flag as a list of tuples.
-
-    Arguments:
-    flag_colours (list[dict]): The "colours" metadata (including name, hex, RGB codes etc) from a standard flag.json file.
-    """
-    return [ 
-        (i["r"], i["g"], i["b"]) for i in flag_colours
-        ] 
-        
+import json
+import os 
+from importlib.resources import files
+
+def flag_attr(flag_name: str) -> str:
+    if not (os.path.exists(os.path.join(os.path.dirname(__file__), "flags", flag_name+".json"))):
+        raise Exception(f"{flag_name} is an invalid flag name.")
+    location = files("pyflagoras.flags").joinpath(flag_name+".json").read_text(encoding="utf-8")
+    data = json.loads(location)
+    return data
+
+def format_rgb(flag_colours: list[dict]) -> list[tuple]:
+    """
+    Formats the colours of the provided flag as a list of tuples.
+
+    Arguments:
+    flag_colours (list[dict]): The "colours" metadata (including name, hex, RGB codes etc) from a standard flag.json file.
+    """
+    return [ 
+        (i["r"], i["g"], i["b"]) for i in flag_colours
+        ] 
+
```

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/agender_2014.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/agender_2014.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/aroace_2018.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/aroace_2018.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/aromantic_2014.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/aromantic_2014.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/asexual_2010.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/asexual_2010.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/bear_1995.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/bear_1995.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/bigender_2014.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/bigender_2014.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/bisexual_1998.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/bisexual_1998.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/gay_men_2019.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/gay_men_2019.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/genderfluid_2012.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/genderfluid_2012.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/intersexInclusive_2021.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/intersexInclusive_2021.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/labrysLesbian_1999.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/labrysLesbian_1999.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/lesbian_2010.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2010.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/lesbian_2018.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2018.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/lesbian_2019.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/lesbian_2019.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/lipstick_lesbian_2010.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/lipstick_lesbian_2010.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/nonbinary_2014.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/nonbinary_2014.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/omnisexual_2015.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/omnisexual_2015.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/pangender_2015.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/pangender_2015.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/philadelphiaPride_2017.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/philadelphiaPride_2017.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/pinkUnionJack_2009.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/pinkUnionJack_2009.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/pride_1978_eightStripes.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/pride_1978_eightStripes.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/pride_1978_sevenStripes.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/pride_1978_sevenStripes.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/pride_1979.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/pride_1979.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/progressPride_2018.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/progressPride_2018.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/sapphic_2015.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/sapphic_2015.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/southAfricaPride_2010.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/southAfricaPride_2010.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/transgender_1999.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/transgender_1999.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/flags/twink_2009.json` & `pyflagoras-0.2.0/src/pyflagoras/flags/twink_2009.json`

 * *Files identical despite different names*

### Comparing `pyflagoras-0.1.0/src/pyflagoras/similarity_algorithms.py` & `pyflagoras-0.2.0/src/pyflagoras/similarity_algorithms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-import math
-def _low_cost(rgb1: tuple[int], rgb2: tuple[int]) -> list[tuple]:
-    """
-    Calculates the similarity of two colours in RGB format using the low-cost approximation here: https://www.compuphase.com/cmetric.htm
-    See the note at the top of the linked page describing about how the human eye interprets colours makes this somewhat difficult.
-    A lower distance value means a more similar colour; a higher distance value means a more dissimilar colour.
-
-    Arguments:
-    rgb1 (tuple[int]): The first RGB value.
-    rgb2 (tuple[int]): The second RGB value.
-    """
-    mean_red = (rgb1[0]+rgb2[0])/2
-    range_red = rgb1[0]-rgb2[0]
-    range_green = rgb1[1]-rgb2[1]
-    range_blue = rgb1[2]-rgb2[2]
-    return (rgb1, 
-            rgb2,
-            ((2+ mean_red/256) * (range_red)**2 + 4 * (range_green)**2 + (2 + (255-mean_red)/256) * (range_blue)**2)
-    )
-def _pythagoras(rgb1: tuple[int], rgb2: tuple[int]) -> list[tuple]:
-    """Calculates the similarity of two colours in RGB format by positioning them as points on a 3D vector plane, then finding the Euclidian distance."""
-    d=((rgb2[0]-rgb1[0])**2+(rgb2[1]-rgb1[1])**2+(rgb2[2]-rgb1[2])**2)
-    return (rgb1, rgb2, d)
-
-def _weighted(rgb1: tuple[int], rgb2: tuple[int]) -> list[tuple]: 
-    """Calculates the similarity of two colours in RGB format by """
+import math
+def _low_cost(rgb1: tuple[int], rgb2: tuple[int]) -> tuple:
+    """
+    Calculates the similarity of two colours in RGB format using the low-cost approximation here: https://www.compuphase.com/cmetric.htm
+    See the note at the top of the linked page describing about how the human eye interprets colours makes this somewhat difficult.
+    A lower distance value means a more similar colour; a higher distance value means a more dissimilar colour.
+
+    Arguments:
+    rgb1 (tuple[int]): The first RGB value.
+    rgb2 (tuple[int]): The second RGB value.
+    """
+    mean_red = (rgb1[0]+rgb2[0])/2
+    range_red = rgb1[0]-rgb2[0]
+    range_green = rgb1[1]-rgb2[1]
+    range_blue = rgb1[2]-rgb2[2]
+    return (rgb1, 
+            rgb2,
+            math.sqrt((2+ mean_red/256) * (range_red)**2 + 4 * (range_green)**2 + (2 + (255-mean_red)/256) * (range_blue)**2)
+    )
+
+
+def _pythagoras(rgb1: tuple[int], rgb2: tuple[int]) -> tuple:
+    """Calculates the similarity of two colours in RGB format by positioning them as points on a 3D vector plane, then finding the Euclidian distance.
+    
+    Arguments:
+    rgb1 (tuple[int]): The first RGB value.
+    rgb2 (tuple[int]): The second RGB value.
+    """
+    return (rgb1, 
+            rgb2, 
+            math.sqrt((rgb2[0]-rgb1[0])**2+(rgb2[1]-rgb1[1])**2+(rgb2[2]-rgb1[2])**2))
+
+def _weighted(rgb1: tuple[int], rgb2: tuple[int]) -> list[tuple]: 
+    """Calculates the similarity of two colours in RGB format by """
     pass
```

### Comparing `pyflagoras-0.1.0/src/pyflagoras.egg-info/SOURCES.txt` & `pyflagoras-0.2.0/src/pyflagoras.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,8 @@
 src/pyflagoras/flags/pride_1978_eightStripes.json
 src/pyflagoras/flags/pride_1978_sevenStripes.json
 src/pyflagoras/flags/pride_1979.json
 src/pyflagoras/flags/progressPride_2018.json
 src/pyflagoras/flags/sapphic_2015.json
 src/pyflagoras/flags/southAfricaPride_2010.json
 src/pyflagoras/flags/transgender_1999.json
-src/pyflagoras/flags/twink_2009.json
-src/pyflagoras/flags/pyflagoras.egg-info/PKG-INFO
-src/pyflagoras/flags/pyflagoras.egg-info/SOURCES.txt
-src/pyflagoras/flags/pyflagoras.egg-info/dependency_links.txt
-src/pyflagoras/flags/pyflagoras.egg-info/entry_points.txt
-src/pyflagoras/flags/pyflagoras.egg-info/requires.txt
-src/pyflagoras/flags/pyflagoras.egg-info/top_level.txt
+src/pyflagoras/flags/twink_2009.json
```

