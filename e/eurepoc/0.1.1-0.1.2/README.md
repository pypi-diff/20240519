# Comparing `tmp/eurepoc-0.1.1.tar.gz` & `tmp/eurepoc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurepoc-0.1.1.tar", last modified: Sat May 18 13:24:08 2024, max compression
+gzip compressed data, was "eurepoc-0.1.2.tar", last modified: Sat May 18 13:34:04 2024, max compression
```

## Comparing `eurepoc-0.1.1.tar` & `eurepoc-0.1.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.784630 eurepoc-0.1.1/
--rw-r--r--   0 camille    (501) staff       (20)     1068 2024-05-18 11:49:09.000000 eurepoc-0.1.1/LICENSE
--rw-r--r--   0 camille    (501) staff       (20)      310 2024-05-18 11:42:32.000000 eurepoc-0.1.1/MANIFEST.in
--rw-r--r--   0 camille    (501) staff       (20)     1798 2024-05-18 13:24:08.779723 eurepoc-0.1.1/PKG-INFO
--rw-r--r--   0 camille    (501) staff       (20)     1158 2024-05-18 12:57:33.000000 eurepoc-0.1.1/README.md
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.328928 eurepoc-0.1.1/docs/
--rw-r--r--   0 camille    (501) staff       (20)      638 2024-05-17 13:41:39.000000 eurepoc-0.1.1/docs/Makefile
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.367973 eurepoc-0.1.1/docs/build/
--rw-r--r--   0 camille    (501) staff       (20)      230 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/.buildinfo
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.421360 eurepoc-0.1.1/docs/build/.doctrees/
--rw-r--r--   0 camille    (501) staff       (20)    37350 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/DatabaseQuery.doctree
--rw-r--r--   0 camille    (501) staff       (20)    48029 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/IncidentDataFrames.doctree
--rw-r--r--   0 camille    (501) staff       (20)     4978 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/date_type.doctree
--rw-r--r--   0 camille    (501) staff       (20)   370061 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/environment.pickle
--rw-r--r--   0 camille    (501) staff       (20)     2438 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/flag_type.doctree
--rw-r--r--   0 camille    (501) staff       (20)     8255 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/index.doctree
--rw-r--r--   0 camille    (501) staff       (20)    52464 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/initiator_country.doctree
--rw-r--r--   0 camille    (501) staff       (20)     9106 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/read_token.doctree
--rw-r--r--   0 camille    (501) staff       (20)     6564 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/receiver_category.doctree
--rw-r--r--   0 camille    (501) staff       (20)    52411 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/receiver_country.doctree
--rw-r--r--   0 camille    (501) staff       (20)    13421 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/.doctrees/receiver_region.doctree
--rw-r--r--   0 camille    (501) staff       (20)    21104 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/DatabaseQuery.html
--rw-r--r--   0 camille    (501) staff       (20)    38404 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/IncidentDataFrames.html
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.443165 eurepoc-0.1.1/docs/build/_modules/
--rw-r--r--   0 camille    (501) staff       (20)    19320 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/_modules/database_query.html
--rw-r--r--   0 camille    (501) staff       (20)    46603 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/_modules/incident_dataframes.html
--rw-r--r--   0 camille    (501) staff       (20)     9178 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/_modules/index.html
--rw-r--r--   0 camille    (501) staff       (20)    12071 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/_modules/read_token.html
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.591304 eurepoc-0.1.1/docs/build/_sources/
--rw-r--r--   0 camille    (501) staff       (20)      506 2024-05-18 11:23:56.000000 eurepoc-0.1.1/docs/build/_sources/DatabaseQuery.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      129 2024-05-17 15:35:02.000000 eurepoc-0.1.1/docs/build/_sources/IncidentDataFrames.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      580 2024-05-18 11:23:56.000000 eurepoc-0.1.1/docs/build/_sources/date_type.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)       19 2024-05-18 10:46:49.000000 eurepoc-0.1.1/docs/build/_sources/flag_type.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)     1714 2024-05-18 10:48:12.000000 eurepoc-0.1.1/docs/build/_sources/index.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)     4085 2024-05-18 11:09:52.000000 eurepoc-0.1.1/docs/build/_sources/initiator_country.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      104 2024-05-18 10:18:35.000000 eurepoc-0.1.1/docs/build/_sources/read_token.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      708 2024-05-18 11:23:56.000000 eurepoc-0.1.1/docs/build/_sources/receiver_category.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)     4059 2024-05-18 11:09:52.000000 eurepoc-0.1.1/docs/build/_sources/receiver_country.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      980 2024-05-18 11:23:56.000000 eurepoc-0.1.1/docs/build/_sources/receiver_region.rst.txt
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.684505 eurepoc-0.1.1/docs/build/_static/
--rw-r--r--   0 camille    (501) staff       (20)    15094 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/_static/basic.css
--rw-r--r--   0 camille    (501) staff       (20)     4913 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/_static/classic.css
--rw-r--r--   0 camille    (501) staff       (20)     3508 2024-05-17 15:45:22.000000 eurepoc-0.1.1/docs/build/_static/copybutton.js
--rw-r--r--   0 camille    (501) staff       (20)       28 2024-05-17 13:40:31.000000 eurepoc-0.1.1/docs/build/_static/default.css
--rw-r--r--   0 camille    (501) staff       (20)     4472 2024-05-17 13:40:31.000000 eurepoc-0.1.1/docs/build/_static/doctools.js
--rw-r--r--   0 camille    (501) staff       (20)      328 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/_static/documentation_options.js
--rw-r--r--   0 camille    (501) staff       (20)      286 2024-05-17 13:40:31.000000 eurepoc-0.1.1/docs/build/_static/file.png
--rw-r--r--   0 camille    (501) staff       (20)     4758 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/_static/language_data.js
--rw-r--r--   0 camille    (501) staff       (20)     2137 2024-05-17 15:45:22.000000 eurepoc-0.1.1/docs/build/_static/menu.js
--rw-r--r--   0 camille    (501) staff       (20)       90 2024-05-17 13:40:31.000000 eurepoc-0.1.1/docs/build/_static/minus.png
--rw-r--r--   0 camille    (501) staff       (20)       90 2024-05-17 13:40:31.000000 eurepoc-0.1.1/docs/build/_static/plus.png
--rw-r--r--   0 camille    (501) staff       (20)      695 2024-05-17 15:45:22.000000 eurepoc-0.1.1/docs/build/_static/py.png
--rw-r--r--   0 camille    (501) staff       (20)     2041 2024-05-17 15:45:22.000000 eurepoc-0.1.1/docs/build/_static/py.svg
--rw-r--r--   0 camille    (501) staff       (20)    13101 2024-05-17 15:45:22.000000 eurepoc-0.1.1/docs/build/_static/pydoctheme.css
--rw-r--r--   0 camille    (501) staff       (20)     2371 2024-05-17 15:45:22.000000 eurepoc-0.1.1/docs/build/_static/pydoctheme_dark.css
--rw-r--r--   0 camille    (501) staff       (20)     4902 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/_static/pygments.css
--rw-r--r--   0 camille    (501) staff       (20)     5055 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/_static/pygments_dark.css
--rw-r--r--   0 camille    (501) staff       (20)      559 2024-05-17 15:45:22.000000 eurepoc-0.1.1/docs/build/_static/search-focus.js
--rw-r--r--   0 camille    (501) staff       (20)    20731 2024-05-17 13:40:31.000000 eurepoc-0.1.1/docs/build/_static/searchtools.js
--rw-r--r--   0 camille    (501) staff       (20)     2617 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/_static/sidebar.js
--rw-r--r--   0 camille    (501) staff       (20)     5123 2024-05-17 13:40:31.000000 eurepoc-0.1.1/docs/build/_static/sphinx_highlight.js
--rw-r--r--   0 camille    (501) staff       (20)      779 2024-05-17 15:45:22.000000 eurepoc-0.1.1/docs/build/_static/themetoggle.js
--rw-r--r--   0 camille    (501) staff       (20)    11699 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/date_type.html
--rw-r--r--   0 camille    (501) staff       (20)    10999 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/flag_type.html
--rw-r--r--   0 camille    (501) staff       (20)    16955 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/genindex.html
--rw-r--r--   0 camille    (501) staff       (20)    14905 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/index.html
--rw-r--r--   0 camille    (501) staff       (20)    18852 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/initiator_country.html
--rw-r--r--   0 camille    (501) staff       (20)      661 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/objects.inv
--rw-r--r--   0 camille    (501) staff       (20)    10167 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/py-modindex.html
--rw-r--r--   0 camille    (501) staff       (20)    13261 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/read_token.html
--rw-r--r--   0 camille    (501) staff       (20)    12144 2024-05-18 11:24:00.000000 eurepoc-0.1.1/docs/build/receiver_category.html
--rw-r--r--   0 camille    (501) staff       (20)    18880 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/receiver_country.html
--rw-r--r--   0 camille    (501) staff       (20)    12935 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/receiver_region.html
--rw-r--r--   0 camille    (501) staff       (20)     7117 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/search.html
--rw-r--r--   0 camille    (501) staff       (20)    19845 2024-05-18 11:24:01.000000 eurepoc-0.1.1/docs/build/searchindex.js
--rw-r--r--   0 camille    (501) staff       (20)      804 2024-05-17 13:41:39.000000 eurepoc-0.1.1/docs/make.bat
--rw-r--r--   0 camille    (501) staff       (20)       41 2024-05-18 13:08:29.000000 eurepoc-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.722240 eurepoc-0.1.1/docs/source/
--rw-r--r--   0 camille    (501) staff       (20)      506 2024-05-18 11:23:56.000000 eurepoc-0.1.1/docs/source/DatabaseQuery.rst
--rw-r--r--   0 camille    (501) staff       (20)      129 2024-05-17 15:35:02.000000 eurepoc-0.1.1/docs/source/IncidentDataFrames.rst
--rw-r--r--   0 camille    (501) staff       (20)      825 2024-05-17 15:45:34.000000 eurepoc-0.1.1/docs/source/conf.py
--rw-r--r--   0 camille    (501) staff       (20)      580 2024-05-18 11:23:56.000000 eurepoc-0.1.1/docs/source/date_type.rst
--rw-r--r--   0 camille    (501) staff       (20)       19 2024-05-18 10:46:49.000000 eurepoc-0.1.1/docs/source/flag_type.rst
--rw-r--r--   0 camille    (501) staff       (20)     1722 2024-05-18 12:57:33.000000 eurepoc-0.1.1/docs/source/index.rst
--rw-r--r--   0 camille    (501) staff       (20)     4085 2024-05-18 11:09:52.000000 eurepoc-0.1.1/docs/source/initiator_country.rst
--rw-r--r--   0 camille    (501) staff       (20)      104 2024-05-18 10:18:35.000000 eurepoc-0.1.1/docs/source/read_token.rst
--rw-r--r--   0 camille    (501) staff       (20)      708 2024-05-18 11:23:56.000000 eurepoc-0.1.1/docs/source/receiver_category.rst
--rw-r--r--   0 camille    (501) staff       (20)     4059 2024-05-18 11:09:52.000000 eurepoc-0.1.1/docs/source/receiver_country.rst
--rw-r--r--   0 camille    (501) staff       (20)      980 2024-05-18 11:23:56.000000 eurepoc-0.1.1/docs/source/receiver_region.rst
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.753167 eurepoc-0.1.1/eurepoc/
--rw-r--r--   0 camille    (501) staff       (20)      238 2024-05-18 11:46:20.000000 eurepoc-0.1.1/eurepoc/__init__.py
--rw-r--r--   0 camille    (501) staff       (20)    36013 2024-05-18 10:16:25.000000 eurepoc-0.1.1/eurepoc/data_cleaning_utils.py
--rw-r--r--   0 camille    (501) staff       (20)     9265 2024-05-17 12:10:59.000000 eurepoc-0.1.1/eurepoc/data_query_utils.py
--rw-r--r--   0 camille    (501) staff       (20)     3284 2024-05-18 11:45:21.000000 eurepoc-0.1.1/eurepoc/database_query.py
--rw-r--r--   0 camille    (501) staff       (20)    10686 2024-05-18 11:45:21.000000 eurepoc-0.1.1/eurepoc/incident_dataframes.py
--rw-r--r--   0 camille    (501) staff       (20)      924 2024-05-18 10:24:49.000000 eurepoc-0.1.1/eurepoc/read_token.py
--rw-r--r--   0 camille    (501) staff       (20)     8832 2024-05-17 09:56:40.000000 eurepoc-0.1.1/eurepoc/table_models.py
--rw-r--r--   0 camille    (501) staff       (20)    31923 2024-05-18 11:44:14.000000 eurepoc-0.1.1/eurepoc/tables.py
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:24:08.774324 eurepoc-0.1.1/eurepoc.egg-info/
--rw-r--r--   0 camille    (501) staff       (20)     1798 2024-05-18 13:24:08.000000 eurepoc-0.1.1/eurepoc.egg-info/PKG-INFO
--rw-r--r--   0 camille    (501) staff       (20)     2960 2024-05-18 13:24:08.000000 eurepoc-0.1.1/eurepoc.egg-info/SOURCES.txt
--rw-r--r--   0 camille    (501) staff       (20)        1 2024-05-18 13:24:08.000000 eurepoc-0.1.1/eurepoc.egg-info/dependency_links.txt
--rw-r--r--   0 camille    (501) staff       (20)       61 2024-05-18 13:24:08.000000 eurepoc-0.1.1/eurepoc.egg-info/requires.txt
--rw-r--r--   0 camille    (501) staff       (20)        8 2024-05-18 13:24:08.000000 eurepoc-0.1.1/eurepoc.egg-info/top_level.txt
--rw-r--r--   0 camille    (501) staff       (20)       38 2024-05-18 13:24:08.785066 eurepoc-0.1.1/setup.cfg
--rw-r--r--   0 camille    (501) staff       (20)      758 2024-05-18 13:23:56.000000 eurepoc-0.1.1/setup.py
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.995826 eurepoc-0.1.2/
+-rw-r--r--   0 camille    (501) staff       (20)     1068 2024-05-18 11:49:09.000000 eurepoc-0.1.2/LICENSE
+-rw-r--r--   0 camille    (501) staff       (20)      310 2024-05-18 11:42:32.000000 eurepoc-0.1.2/MANIFEST.in
+-rw-r--r--   0 camille    (501) staff       (20)     1916 2024-05-18 13:34:03.994721 eurepoc-0.1.2/PKG-INFO
+-rw-r--r--   0 camille    (501) staff       (20)     1268 2024-05-18 13:32:15.000000 eurepoc-0.1.2/README.md
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.592659 eurepoc-0.1.2/docs/
+-rw-r--r--   0 camille    (501) staff       (20)      638 2024-05-17 13:41:39.000000 eurepoc-0.1.2/docs/Makefile
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.627304 eurepoc-0.1.2/docs/build/
+-rw-r--r--   0 camille    (501) staff       (20)      230 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/.buildinfo
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.672861 eurepoc-0.1.2/docs/build/.doctrees/
+-rw-r--r--   0 camille    (501) staff       (20)    37350 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/DatabaseQuery.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    48029 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/IncidentDataFrames.doctree
+-rw-r--r--   0 camille    (501) staff       (20)     4978 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/date_type.doctree
+-rw-r--r--   0 camille    (501) staff       (20)   370061 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0 camille    (501) staff       (20)     2438 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/flag_type.doctree
+-rw-r--r--   0 camille    (501) staff       (20)     8255 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/index.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    52464 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/initiator_country.doctree
+-rw-r--r--   0 camille    (501) staff       (20)     9106 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/read_token.doctree
+-rw-r--r--   0 camille    (501) staff       (20)     6564 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/receiver_category.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    52411 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/receiver_country.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    13421 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/.doctrees/receiver_region.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    21104 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/DatabaseQuery.html
+-rw-r--r--   0 camille    (501) staff       (20)    38404 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/IncidentDataFrames.html
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.682187 eurepoc-0.1.2/docs/build/_modules/
+-rw-r--r--   0 camille    (501) staff       (20)    19320 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/_modules/database_query.html
+-rw-r--r--   0 camille    (501) staff       (20)    46603 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/_modules/incident_dataframes.html
+-rw-r--r--   0 camille    (501) staff       (20)     9178 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/_modules/index.html
+-rw-r--r--   0 camille    (501) staff       (20)    12071 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/_modules/read_token.html
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.715249 eurepoc-0.1.2/docs/build/_sources/
+-rw-r--r--   0 camille    (501) staff       (20)      506 2024-05-18 11:23:56.000000 eurepoc-0.1.2/docs/build/_sources/DatabaseQuery.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      129 2024-05-17 15:35:02.000000 eurepoc-0.1.2/docs/build/_sources/IncidentDataFrames.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      580 2024-05-18 11:23:56.000000 eurepoc-0.1.2/docs/build/_sources/date_type.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)       19 2024-05-18 10:46:49.000000 eurepoc-0.1.2/docs/build/_sources/flag_type.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)     1714 2024-05-18 10:48:12.000000 eurepoc-0.1.2/docs/build/_sources/index.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)     4085 2024-05-18 11:09:52.000000 eurepoc-0.1.2/docs/build/_sources/initiator_country.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      104 2024-05-18 10:18:35.000000 eurepoc-0.1.2/docs/build/_sources/read_token.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      708 2024-05-18 11:23:56.000000 eurepoc-0.1.2/docs/build/_sources/receiver_category.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)     4059 2024-05-18 11:09:52.000000 eurepoc-0.1.2/docs/build/_sources/receiver_country.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      980 2024-05-18 11:23:56.000000 eurepoc-0.1.2/docs/build/_sources/receiver_region.rst.txt
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.910467 eurepoc-0.1.2/docs/build/_static/
+-rw-r--r--   0 camille    (501) staff       (20)    15094 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/_static/basic.css
+-rw-r--r--   0 camille    (501) staff       (20)     4913 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/_static/classic.css
+-rw-r--r--   0 camille    (501) staff       (20)     3508 2024-05-17 15:45:22.000000 eurepoc-0.1.2/docs/build/_static/copybutton.js
+-rw-r--r--   0 camille    (501) staff       (20)       28 2024-05-17 13:40:31.000000 eurepoc-0.1.2/docs/build/_static/default.css
+-rw-r--r--   0 camille    (501) staff       (20)     4472 2024-05-17 13:40:31.000000 eurepoc-0.1.2/docs/build/_static/doctools.js
+-rw-r--r--   0 camille    (501) staff       (20)      328 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/_static/documentation_options.js
+-rw-r--r--   0 camille    (501) staff       (20)      286 2024-05-17 13:40:31.000000 eurepoc-0.1.2/docs/build/_static/file.png
+-rw-r--r--   0 camille    (501) staff       (20)     4758 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/_static/language_data.js
+-rw-r--r--   0 camille    (501) staff       (20)     2137 2024-05-17 15:45:22.000000 eurepoc-0.1.2/docs/build/_static/menu.js
+-rw-r--r--   0 camille    (501) staff       (20)       90 2024-05-17 13:40:31.000000 eurepoc-0.1.2/docs/build/_static/minus.png
+-rw-r--r--   0 camille    (501) staff       (20)       90 2024-05-17 13:40:31.000000 eurepoc-0.1.2/docs/build/_static/plus.png
+-rw-r--r--   0 camille    (501) staff       (20)      695 2024-05-17 15:45:22.000000 eurepoc-0.1.2/docs/build/_static/py.png
+-rw-r--r--   0 camille    (501) staff       (20)     2041 2024-05-17 15:45:22.000000 eurepoc-0.1.2/docs/build/_static/py.svg
+-rw-r--r--   0 camille    (501) staff       (20)    13101 2024-05-17 15:45:22.000000 eurepoc-0.1.2/docs/build/_static/pydoctheme.css
+-rw-r--r--   0 camille    (501) staff       (20)     2371 2024-05-17 15:45:22.000000 eurepoc-0.1.2/docs/build/_static/pydoctheme_dark.css
+-rw-r--r--   0 camille    (501) staff       (20)     4902 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/_static/pygments.css
+-rw-r--r--   0 camille    (501) staff       (20)     5055 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/_static/pygments_dark.css
+-rw-r--r--   0 camille    (501) staff       (20)      559 2024-05-17 15:45:22.000000 eurepoc-0.1.2/docs/build/_static/search-focus.js
+-rw-r--r--   0 camille    (501) staff       (20)    20731 2024-05-17 13:40:31.000000 eurepoc-0.1.2/docs/build/_static/searchtools.js
+-rw-r--r--   0 camille    (501) staff       (20)     2617 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/_static/sidebar.js
+-rw-r--r--   0 camille    (501) staff       (20)     5123 2024-05-17 13:40:31.000000 eurepoc-0.1.2/docs/build/_static/sphinx_highlight.js
+-rw-r--r--   0 camille    (501) staff       (20)      779 2024-05-17 15:45:22.000000 eurepoc-0.1.2/docs/build/_static/themetoggle.js
+-rw-r--r--   0 camille    (501) staff       (20)    11699 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/date_type.html
+-rw-r--r--   0 camille    (501) staff       (20)    10999 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/flag_type.html
+-rw-r--r--   0 camille    (501) staff       (20)    16955 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/genindex.html
+-rw-r--r--   0 camille    (501) staff       (20)    14905 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/index.html
+-rw-r--r--   0 camille    (501) staff       (20)    18852 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/initiator_country.html
+-rw-r--r--   0 camille    (501) staff       (20)      661 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/objects.inv
+-rw-r--r--   0 camille    (501) staff       (20)    10167 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/py-modindex.html
+-rw-r--r--   0 camille    (501) staff       (20)    13261 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/read_token.html
+-rw-r--r--   0 camille    (501) staff       (20)    12144 2024-05-18 11:24:00.000000 eurepoc-0.1.2/docs/build/receiver_category.html
+-rw-r--r--   0 camille    (501) staff       (20)    18880 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/receiver_country.html
+-rw-r--r--   0 camille    (501) staff       (20)    12935 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/receiver_region.html
+-rw-r--r--   0 camille    (501) staff       (20)     7117 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/search.html
+-rw-r--r--   0 camille    (501) staff       (20)    19845 2024-05-18 11:24:01.000000 eurepoc-0.1.2/docs/build/searchindex.js
+-rw-r--r--   0 camille    (501) staff       (20)      804 2024-05-17 13:41:39.000000 eurepoc-0.1.2/docs/make.bat
+-rw-r--r--   0 camille    (501) staff       (20)       41 2024-05-18 13:08:29.000000 eurepoc-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.947265 eurepoc-0.1.2/docs/source/
+-rw-r--r--   0 camille    (501) staff       (20)      506 2024-05-18 11:23:56.000000 eurepoc-0.1.2/docs/source/DatabaseQuery.rst
+-rw-r--r--   0 camille    (501) staff       (20)      129 2024-05-17 15:35:02.000000 eurepoc-0.1.2/docs/source/IncidentDataFrames.rst
+-rw-r--r--   0 camille    (501) staff       (20)      825 2024-05-17 15:45:34.000000 eurepoc-0.1.2/docs/source/conf.py
+-rw-r--r--   0 camille    (501) staff       (20)      580 2024-05-18 11:23:56.000000 eurepoc-0.1.2/docs/source/date_type.rst
+-rw-r--r--   0 camille    (501) staff       (20)       19 2024-05-18 10:46:49.000000 eurepoc-0.1.2/docs/source/flag_type.rst
+-rw-r--r--   0 camille    (501) staff       (20)     1761 2024-05-18 13:32:37.000000 eurepoc-0.1.2/docs/source/index.rst
+-rw-r--r--   0 camille    (501) staff       (20)     4085 2024-05-18 11:09:52.000000 eurepoc-0.1.2/docs/source/initiator_country.rst
+-rw-r--r--   0 camille    (501) staff       (20)      104 2024-05-18 10:18:35.000000 eurepoc-0.1.2/docs/source/read_token.rst
+-rw-r--r--   0 camille    (501) staff       (20)      708 2024-05-18 11:23:56.000000 eurepoc-0.1.2/docs/source/receiver_category.rst
+-rw-r--r--   0 camille    (501) staff       (20)     4059 2024-05-18 11:09:52.000000 eurepoc-0.1.2/docs/source/receiver_country.rst
+-rw-r--r--   0 camille    (501) staff       (20)      980 2024-05-18 11:23:56.000000 eurepoc-0.1.2/docs/source/receiver_region.rst
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.972772 eurepoc-0.1.2/eurepoc/
+-rw-r--r--   0 camille    (501) staff       (20)      238 2024-05-18 11:46:20.000000 eurepoc-0.1.2/eurepoc/__init__.py
+-rw-r--r--   0 camille    (501) staff       (20)    36013 2024-05-18 10:16:25.000000 eurepoc-0.1.2/eurepoc/data_cleaning_utils.py
+-rw-r--r--   0 camille    (501) staff       (20)     9265 2024-05-17 12:10:59.000000 eurepoc-0.1.2/eurepoc/data_query_utils.py
+-rw-r--r--   0 camille    (501) staff       (20)     3284 2024-05-18 11:45:21.000000 eurepoc-0.1.2/eurepoc/database_query.py
+-rw-r--r--   0 camille    (501) staff       (20)    10686 2024-05-18 11:45:21.000000 eurepoc-0.1.2/eurepoc/incident_dataframes.py
+-rw-r--r--   0 camille    (501) staff       (20)      924 2024-05-18 10:24:49.000000 eurepoc-0.1.2/eurepoc/read_token.py
+-rw-r--r--   0 camille    (501) staff       (20)     8832 2024-05-17 09:56:40.000000 eurepoc-0.1.2/eurepoc/table_models.py
+-rw-r--r--   0 camille    (501) staff       (20)    31923 2024-05-18 11:44:14.000000 eurepoc-0.1.2/eurepoc/tables.py
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-18 13:34:03.993260 eurepoc-0.1.2/eurepoc.egg-info/
+-rw-r--r--   0 camille    (501) staff       (20)     1916 2024-05-18 13:34:03.000000 eurepoc-0.1.2/eurepoc.egg-info/PKG-INFO
+-rw-r--r--   0 camille    (501) staff       (20)     2960 2024-05-18 13:34:03.000000 eurepoc-0.1.2/eurepoc.egg-info/SOURCES.txt
+-rw-r--r--   0 camille    (501) staff       (20)        1 2024-05-18 13:34:03.000000 eurepoc-0.1.2/eurepoc.egg-info/dependency_links.txt
+-rw-r--r--   0 camille    (501) staff       (20)       61 2024-05-18 13:34:03.000000 eurepoc-0.1.2/eurepoc.egg-info/requires.txt
+-rw-r--r--   0 camille    (501) staff       (20)        8 2024-05-18 13:34:03.000000 eurepoc-0.1.2/eurepoc.egg-info/top_level.txt
+-rw-r--r--   0 camille    (501) staff       (20)       38 2024-05-18 13:34:03.996175 eurepoc-0.1.2/setup.cfg
+-rw-r--r--   0 camille    (501) staff       (20)      766 2024-05-18 13:30:20.000000 eurepoc-0.1.2/setup.py
```

### Comparing `eurepoc-0.1.1/LICENSE` & `eurepoc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/PKG-INFO` & `eurepoc-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: eurepoc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wrapper for the EuRepoC API
 Author: Camille Borrett
 Author-email: camille.borrett@posteo.net
 License: MIT
 Project-URL: Documentation, https://eurepoc.readthedocs.io/
 Project-URL: Source, https://github.com/camilleborrett/eurepoc
 Project-URL: Tracker, https://github.com/camilleborrett/eurepoc/issues
-Project-URL: Project, https://eurepoc.eu/
+Project-URL: EuRepoC Project, https://eurepoc.eu/
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: nested_query_string
 Requires-Dist: pandas
 Requires-Dist: datetime
 Requires-Dist: pydantic
 Requires-Dist: typing
 
 # eurepoc
 
-The EuRepoC package is a wrapper around the main EuRepoC Strapi API. It is designed to streamline data queries through a set of filters and to preprocess, unnest and clean the Strapi output. The IncidentDataFrames class automatically converts the data into multiple pandas dataframes (dfs) for easier manipulation and analysis. These dfs can be easily joined using the incidents_id column.
+🚀 The EuRepoC package is a wrapper around the main EuRepoC Strapi API. It is designed to streamline data queries through a set of filters and to preprocess, unnest and clean the Strapi output. The IncidentDataFrames class automatically converts the data into multiple pandas dataframes (dfs) for easier manipulation and analysis. These dfs can be easily joined using the incidents_id column.
+
+🔎 Refer to the main [EuRepoC website](https://www.eurepoc.eu/) for more information about the data collection methodology. 
+The EuRepoC Codebook provides detailed information about the substantive meaning of each of the variables in the data [here](https://eurepoc.eu/methodology/).
+
+📖 **The package documentation is available [here](https://eurepoc.readthedocs.io/en/latest/)**
 
-Refer to the main [EuRepoC website](https://www.eurepoc.eu/) for more information about the data collection methodology. 
-The EuRepoC Codebook provides detailed information about the substantive meaning of each of the variables in the data [here](https://www.eurepoc.eu/codebook).
 ## Installation
 
 ```bash
 pip install eurepoc
 ```
 
 ## Quickstart
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eurepoc-0.1.1/README.md` & `eurepoc-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # eurepoc
 
-The EuRepoC package is a wrapper around the main EuRepoC Strapi API. It is designed to streamline data queries through a set of filters and to preprocess, unnest and clean the Strapi output. The IncidentDataFrames class automatically converts the data into multiple pandas dataframes (dfs) for easier manipulation and analysis. These dfs can be easily joined using the incidents_id column.
+🚀 The EuRepoC package is a wrapper around the main EuRepoC Strapi API. It is designed to streamline data queries through a set of filters and to preprocess, unnest and clean the Strapi output. The IncidentDataFrames class automatically converts the data into multiple pandas dataframes (dfs) for easier manipulation and analysis. These dfs can be easily joined using the incidents_id column.
+
+🔎 Refer to the main [EuRepoC website](https://www.eurepoc.eu/) for more information about the data collection methodology. 
+The EuRepoC Codebook provides detailed information about the substantive meaning of each of the variables in the data [here](https://eurepoc.eu/methodology/).
+
+📖 **The package documentation is available [here](https://eurepoc.readthedocs.io/en/latest/)**
 
-Refer to the main [EuRepoC website](https://www.eurepoc.eu/) for more information about the data collection methodology. 
-The EuRepoC Codebook provides detailed information about the substantive meaning of each of the variables in the data [here](https://www.eurepoc.eu/codebook).
 ## Installation
 
 ```bash
 pip install eurepoc
 ```
 
 ## Quickstart
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eurepoc-0.1.1/docs/Makefile` & `eurepoc-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/DatabaseQuery.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/DatabaseQuery.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/IncidentDataFrames.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/IncidentDataFrames.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/date_type.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/date_type.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/environment.pickle` & `eurepoc-0.1.2/docs/build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/flag_type.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/flag_type.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/index.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/initiator_country.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/initiator_country.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/read_token.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/read_token.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/receiver_category.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/receiver_category.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/receiver_country.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/receiver_country.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/.doctrees/receiver_region.doctree` & `eurepoc-0.1.2/docs/build/.doctrees/receiver_region.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/DatabaseQuery.html` & `eurepoc-0.1.2/docs/build/DatabaseQuery.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/IncidentDataFrames.html` & `eurepoc-0.1.2/docs/build/IncidentDataFrames.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_modules/database_query.html` & `eurepoc-0.1.2/docs/build/_modules/database_query.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_modules/incident_dataframes.html` & `eurepoc-0.1.2/docs/build/_modules/incident_dataframes.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_modules/index.html` & `eurepoc-0.1.2/docs/build/_modules/index.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_modules/read_token.html` & `eurepoc-0.1.2/docs/build/_modules/read_token.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_sources/date_type.rst.txt` & `eurepoc-0.1.2/docs/build/_sources/date_type.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_sources/index.rst.txt` & `eurepoc-0.1.2/docs/build/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_sources/initiator_country.rst.txt` & `eurepoc-0.1.2/docs/build/_sources/initiator_country.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_sources/receiver_category.rst.txt` & `eurepoc-0.1.2/docs/build/_sources/receiver_category.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_sources/receiver_country.rst.txt` & `eurepoc-0.1.2/docs/build/_sources/receiver_country.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_sources/receiver_region.rst.txt` & `eurepoc-0.1.2/docs/build/_sources/receiver_region.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/basic.css` & `eurepoc-0.1.2/docs/build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/classic.css` & `eurepoc-0.1.2/docs/build/_static/classic.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/copybutton.js` & `eurepoc-0.1.2/docs/build/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/doctools.js` & `eurepoc-0.1.2/docs/build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/language_data.js` & `eurepoc-0.1.2/docs/build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/menu.js` & `eurepoc-0.1.2/docs/build/_static/menu.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/py.png` & `eurepoc-0.1.2/docs/build/_static/py.png`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/py.svg` & `eurepoc-0.1.2/docs/build/_static/py.svg`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/pydoctheme.css` & `eurepoc-0.1.2/docs/build/_static/pydoctheme.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/pydoctheme_dark.css` & `eurepoc-0.1.2/docs/build/_static/pydoctheme_dark.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/pygments.css` & `eurepoc-0.1.2/docs/build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/pygments_dark.css` & `eurepoc-0.1.2/docs/build/_static/pygments_dark.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/search-focus.js` & `eurepoc-0.1.2/docs/build/_static/search-focus.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/searchtools.js` & `eurepoc-0.1.2/docs/build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/sidebar.js` & `eurepoc-0.1.2/docs/build/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/sphinx_highlight.js` & `eurepoc-0.1.2/docs/build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/_static/themetoggle.js` & `eurepoc-0.1.2/docs/build/_static/themetoggle.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/date_type.html` & `eurepoc-0.1.2/docs/build/date_type.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/flag_type.html` & `eurepoc-0.1.2/docs/build/flag_type.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/genindex.html` & `eurepoc-0.1.2/docs/build/genindex.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/index.html` & `eurepoc-0.1.2/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/initiator_country.html` & `eurepoc-0.1.2/docs/build/initiator_country.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/objects.inv` & `eurepoc-0.1.2/docs/build/objects.inv`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/py-modindex.html` & `eurepoc-0.1.2/docs/build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/read_token.html` & `eurepoc-0.1.2/docs/build/read_token.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/receiver_category.html` & `eurepoc-0.1.2/docs/build/receiver_category.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/receiver_country.html` & `eurepoc-0.1.2/docs/build/receiver_country.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/receiver_region.html` & `eurepoc-0.1.2/docs/build/receiver_region.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/search.html` & `eurepoc-0.1.2/docs/build/search.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/build/searchindex.js` & `eurepoc-0.1.2/docs/build/searchindex.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/make.bat` & `eurepoc-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/source/conf.py` & `eurepoc-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/source/date_type.rst` & `eurepoc-0.1.2/docs/source/date_type.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/source/index.rst` & `eurepoc-0.1.2/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 The EuRepoC package is a wrapper around the main EuRepoC Strapi API. It is designed to streamline
 data queries through a set of filters and to preprocess, unnest and clean the Strapi output. The
 `IncidentDataFrames` class automatically converts the data into multiple pandas dataframes (dfs) for easier
 manipulation and analysis. These dfs can be easily joined using the `incidents_id` column.
 
 Refer to the main EuRepoC website (https://www.eurepoc.eu/) for more information about the data collection
 methodology. The EuRepoC Codebook provides detailed information about the substantive meaning of each of the
-variables in the data here: https://www.eurepoc.eu/codebook.
+variables in the data here: https://eurepoc.eu/wp-content/uploads/2023/07/EuRepoC_Codebook_1_2.pdf.
 
 Quickstart
 ==========
 
 Install the package:
 
 .. code-block:: bash
```

### Comparing `eurepoc-0.1.1/docs/source/initiator_country.rst` & `eurepoc-0.1.2/docs/source/initiator_country.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/source/receiver_category.rst` & `eurepoc-0.1.2/docs/source/receiver_category.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/source/receiver_country.rst` & `eurepoc-0.1.2/docs/source/receiver_country.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/docs/source/receiver_region.rst` & `eurepoc-0.1.2/docs/source/receiver_region.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/eurepoc/data_cleaning_utils.py` & `eurepoc-0.1.2/eurepoc/data_cleaning_utils.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/eurepoc/data_query_utils.py` & `eurepoc-0.1.2/eurepoc/data_query_utils.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/eurepoc/database_query.py` & `eurepoc-0.1.2/eurepoc/database_query.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/eurepoc/incident_dataframes.py` & `eurepoc-0.1.2/eurepoc/incident_dataframes.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/eurepoc/read_token.py` & `eurepoc-0.1.2/eurepoc/read_token.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/eurepoc/table_models.py` & `eurepoc-0.1.2/eurepoc/table_models.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/eurepoc/tables.py` & `eurepoc-0.1.2/eurepoc/tables.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/eurepoc.egg-info/PKG-INFO` & `eurepoc-0.1.2/eurepoc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: eurepoc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wrapper for the EuRepoC API
 Author: Camille Borrett
 Author-email: camille.borrett@posteo.net
 License: MIT
 Project-URL: Documentation, https://eurepoc.readthedocs.io/
 Project-URL: Source, https://github.com/camilleborrett/eurepoc
 Project-URL: Tracker, https://github.com/camilleborrett/eurepoc/issues
-Project-URL: Project, https://eurepoc.eu/
+Project-URL: EuRepoC Project, https://eurepoc.eu/
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: nested_query_string
 Requires-Dist: pandas
 Requires-Dist: datetime
 Requires-Dist: pydantic
 Requires-Dist: typing
 
 # eurepoc
 
-The EuRepoC package is a wrapper around the main EuRepoC Strapi API. It is designed to streamline data queries through a set of filters and to preprocess, unnest and clean the Strapi output. The IncidentDataFrames class automatically converts the data into multiple pandas dataframes (dfs) for easier manipulation and analysis. These dfs can be easily joined using the incidents_id column.
+🚀 The EuRepoC package is a wrapper around the main EuRepoC Strapi API. It is designed to streamline data queries through a set of filters and to preprocess, unnest and clean the Strapi output. The IncidentDataFrames class automatically converts the data into multiple pandas dataframes (dfs) for easier manipulation and analysis. These dfs can be easily joined using the incidents_id column.
+
+🔎 Refer to the main [EuRepoC website](https://www.eurepoc.eu/) for more information about the data collection methodology. 
+The EuRepoC Codebook provides detailed information about the substantive meaning of each of the variables in the data [here](https://eurepoc.eu/methodology/).
+
+📖 **The package documentation is available [here](https://eurepoc.readthedocs.io/en/latest/)**
 
-Refer to the main [EuRepoC website](https://www.eurepoc.eu/) for more information about the data collection methodology. 
-The EuRepoC Codebook provides detailed information about the substantive meaning of each of the variables in the data [here](https://www.eurepoc.eu/codebook).
 ## Installation
 
 ```bash
 pip install eurepoc
 ```
 
 ## Quickstart
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eurepoc-0.1.1/eurepoc.egg-info/SOURCES.txt` & `eurepoc-0.1.2/eurepoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.1/setup.py` & `eurepoc-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurepoc',
-    version='0.1.1',
+    version='0.1.2',
     author='Camille Borrett',
     author_email='camille.borrett@posteo.net',
     description='Wrapper for the EuRepoC API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     project_urls={
         'Documentation': 'https://eurepoc.readthedocs.io/',
         'Source': 'https://github.com/camilleborrett/eurepoc',
         'Tracker': 'https://github.com/camilleborrett/eurepoc/issues',
-        'Project': 'https://eurepoc.eu/'
+        'EuRepoC Project': 'https://eurepoc.eu/'
     },
     license='MIT',
     packages=find_packages(),
     install_requires=['requests', 'nested_query_string', 'pandas', 'datetime', 'pydantic', 'typing'],
     python_requires='>=3.6',
 )
```

