# Comparing `tmp/themoviedb_lib-0.0.3.tar.gz` & `tmp/themoviedb_lib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themoviedb_lib-0.0.3.tar", last modified: Tue May  7 16:37:18 2024, max compression
+gzip compressed data, was "themoviedb_lib-0.0.4.tar", last modified: Sun May 19 17:50:41 2024, max compression
```

## Comparing `themoviedb_lib-0.0.3.tar` & `themoviedb_lib-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/tmdb/
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/tmdb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:50:41.553277 themoviedb_lib-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 17:50:34.000000 themoviedb_lib-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-19 17:50:41.553277 themoviedb_lib-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-19 17:50:34.000000 themoviedb_lib-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:50:41.553277 themoviedb_lib-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-19 17:50:34.000000 themoviedb_lib-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:50:41.553277 themoviedb_lib-0.0.4/themoviedb_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-19 17:50:41.000000 themoviedb_lib-0.0.4/themoviedb_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-19 17:50:41.000000 themoviedb_lib-0.0.4/themoviedb_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:50:41.000000 themoviedb_lib-0.0.4/themoviedb_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 17:50:41.000000 themoviedb_lib-0.0.4/themoviedb_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-19 17:50:41.000000 themoviedb_lib-0.0.4/themoviedb_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:50:41.553277 themoviedb_lib-0.0.4/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    17637 2024-05-19 17:50:34.000000 themoviedb_lib-0.0.4/tmdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:50:41.553277 themoviedb_lib-0.0.4/tmdb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:50:34.000000 themoviedb_lib-0.0.4/tmdb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-19 17:50:34.000000 themoviedb_lib-0.0.4/tmdb/tests/test_tmdb_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-19 17:50:34.000000 themoviedb_lib-0.0.4/tmdb/tests/test_tmdb_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-19 17:50:34.000000 themoviedb_lib-0.0.4/tmdb/tests/test_tmdb_request.py
```

### Comparing `themoviedb_lib-0.0.3/LICENSE` & `themoviedb_lib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `themoviedb_lib-0.0.3/PKG-INFO` & `themoviedb_lib-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themoviedb-lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library providing useful tools for The Movie Database (TMDb). Not dependent on API-keys.
 Home-page: https://github.com/inwerk/themoviedb-lib
 Author: 
 Author-email: 
 Keywords: tmdb,themoviedb,the movie database,the movie db,movie,movies,tv,tv show,tv shows
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `themoviedb_lib-0.0.3/README.md` & `themoviedb_lib-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `themoviedb_lib-0.0.3/setup.py` & `themoviedb_lib-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Setting up
 setup(
     name="themoviedb-lib",  # Required
-    version="0.0.3",  # Required
+    version="0.0.4",  # Required
     description="Library providing useful tools for The Movie Database (TMDb). Not dependent on API-keys.",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional
     url="https://github.com/inwerk/themoviedb-lib",  # Optional
     author="",  # Optional
     author_email="",  # Optional
     classifiers=[  # Optional (https://pypi.org/classifiers/)
```

### Comparing `themoviedb_lib-0.0.3/themoviedb_lib.egg-info/PKG-INFO` & `themoviedb_lib-0.0.4/themoviedb_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themoviedb-lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library providing useful tools for The Movie Database (TMDb). Not dependent on API-keys.
 Home-page: https://github.com/inwerk/themoviedb-lib
 Author: 
 Author-email: 
 Keywords: tmdb,themoviedb,the movie database,the movie db,movie,movies,tv,tv show,tv shows
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `themoviedb_lib-0.0.3/tmdb/__init__.py` & `themoviedb_lib-0.0.4/tmdb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             if div_title.find('a') is not None:
                 tmdb_entry.category = div_title.find('a').get('data-media-type')
 
             if div_title.find('a') is not None:
                 tmdb_entry.tmdb_id = re.search(r'(\d+)', div_title.find('a').get('href')).group()
 
             if div_title.find('h2') is not None:
-                tmdb_entry.title = div_title.find('h2').get_text().replace('amp;', '')
+                result.title = div_title.find('h2').next_element.strip().replace('amp;', '')
 
             if div_title.find('span', {'class': 'release_date'}) is not None:
                 tmdb_entry.release_year = re.search(r'(\d){4}', div_title
                                                     .find('span', {'class': 'release_date'}).get_text()).group()
 
             if div_card.find('p') is not None:
                 tmdb_entry.description = div_card.find('p').get_text()
```

### Comparing `themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_api.py` & `themoviedb_lib-0.0.4/tmdb/tests/test_tmdb_api.py`

 * *Files identical despite different names*

### Comparing `themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_entry.py` & `themoviedb_lib-0.0.4/tmdb/tests/test_tmdb_entry.py`

 * *Files identical despite different names*

### Comparing `themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_request.py` & `themoviedb_lib-0.0.4/tmdb/tests/test_tmdb_request.py`

 * *Files identical despite different names*

