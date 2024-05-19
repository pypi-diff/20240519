# Comparing `tmp/banner-storedot-2.3.3.tar.gz` & `tmp/banner_storedot-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banner-storedot-2.3.3.tar", last modified: Mon Dec 18 09:41:48 2023, max compression
+gzip compressed data, was "banner_storedot-2.3.4.tar", last modified: Sun May 19 10:43:36 2024, max compression
```

## Comparing `banner-storedot-2.3.3.tar` & `banner_storedot-2.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 danielg   (1019) developers  (1234)        0 2023-12-18 09:41:48.285137 banner-storedot-2.3.3/
--rw-r--r--   0 danielg   (1019) developers  (1234)     1073 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/LICENSE
--rw-r--r--   0 danielg   (1019) developers  (1234)     8763 2023-12-18 09:41:48.285137 banner-storedot-2.3.3/PKG-INFO
--rw-r--r--   0 danielg   (1019) developers  (1234)     8138 2023-12-13 12:28:29.000000 banner-storedot-2.3.3/README.md
--rw-r--r--   0 danielg   (1019) developers  (1234)      122 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/pyproject.toml
--rw-r--r--   0 danielg   (1019) developers  (1234)      679 2023-12-18 09:41:48.285137 banner-storedot-2.3.3/setup.cfg
-drwxr-xr-x   0 danielg   (1019) developers  (1234)        0 2023-12-18 09:41:48.281137 banner-storedot-2.3.3/src/
-drwxr-xr-x   0 danielg   (1019) developers  (1234)        0 2023-12-18 09:41:48.285137 banner-storedot-2.3.3/src/banner/
--rw-r--r--   0 danielg   (1019) developers  (1234)      161 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/__init__.py
--rw-r--r--   0 danielg   (1019) developers  (1234)    30331 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/connection.py
--rw-r--r--   0 danielg   (1019) developers  (1234)     6632 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/pandas_decorator.py
--rw-r--r--   0 danielg   (1019) developers  (1234)     2121 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/pandas_wrap.py
--rw-r--r--   0 danielg   (1019) developers  (1234)    52814 2023-07-04 05:13:25.000000 banner-storedot-2.3.3/src/banner/queries.py
-drwxr-xr-x   0 danielg   (1019) developers  (1234)        0 2023-12-18 09:41:48.285137 banner-storedot-2.3.3/src/banner/utils/
--rw-r--r--   0 danielg   (1019) developers  (1234)        0 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/utils/__init__.py
--rw-r--r--   0 danielg   (1019) developers  (1234)     3798 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/utils/const.py
--rw-r--r--   0 danielg   (1019) developers  (1234)     2042 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/utils/misc.py
--rw-r--r--   0 danielg   (1019) developers  (1234)    10256 2023-12-11 12:29:36.000000 banner-storedot-2.3.3/src/banner/utils/neware.py
--rw-r--r--   0 danielg   (1019) developers  (1234)     1952 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/utils/pandas.py
--rw-r--r--   0 danielg   (1019) developers  (1234)   182362 2023-06-20 09:18:28.000000 banner-storedot-2.3.3/src/banner/utils/web2py.py
-drwxr-xr-x   0 danielg   (1019) developers  (1234)        0 2023-12-18 09:41:48.285137 banner-storedot-2.3.3/src/banner_storedot.egg-info/
--rw-r--r--   0 danielg   (1019) developers  (1234)     8763 2023-12-18 09:41:48.000000 banner-storedot-2.3.3/src/banner_storedot.egg-info/PKG-INFO
--rw-r--r--   0 danielg   (1019) developers  (1234)      544 2023-12-18 09:41:48.000000 banner-storedot-2.3.3/src/banner_storedot.egg-info/SOURCES.txt
--rw-r--r--   0 danielg   (1019) developers  (1234)        1 2023-12-18 09:41:48.000000 banner-storedot-2.3.3/src/banner_storedot.egg-info/dependency_links.txt
--rw-r--r--   0 danielg   (1019) developers  (1234)       75 2023-12-18 09:41:48.000000 banner-storedot-2.3.3/src/banner_storedot.egg-info/requires.txt
--rw-r--r--   0 danielg   (1019) developers  (1234)        7 2023-12-18 09:41:48.000000 banner-storedot-2.3.3/src/banner_storedot.egg-info/top_level.txt
+drwxrwsr-x   0 adoram    (1002) adoram    (1002)        0 2024-05-19 10:43:36.076873 banner_storedot-2.3.4/
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)     1073 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/LICENSE
+-rw-r--r--   0 adoram    (1002) adoram    (1002)     8763 2024-05-19 10:43:36.076873 banner_storedot-2.3.4/PKG-INFO
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)     8138 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/README.md
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)      122 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/pyproject.toml
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)      679 2024-05-19 10:43:36.076873 banner_storedot-2.3.4/setup.cfg
+drwxrwsr-x   0 adoram    (1002) adoram    (1002)        0 2024-05-19 10:43:36.076873 banner_storedot-2.3.4/src/
+drwxrwsr-x   0 adoram    (1002) adoram    (1002)        0 2024-05-19 10:43:36.076873 banner_storedot-2.3.4/src/banner/
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)      161 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/__init__.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)    30331 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/connection.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)     6632 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/pandas_decorator.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)     2121 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/pandas_wrap.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)    52804 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/queries.py
+drwxrwsr-x   0 adoram    (1002) adoram    (1002)        0 2024-05-19 10:43:36.076873 banner_storedot-2.3.4/src/banner/utils/
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)        0 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/utils/__init__.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)     3798 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/utils/const.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)     2042 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/utils/misc.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)    10287 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/utils/neware.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)     1952 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/utils/pandas.py
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)   182362 2024-05-19 08:35:02.000000 banner_storedot-2.3.4/src/banner/utils/web2py.py
+drwxrwsr-x   0 adoram    (1002) adoram    (1002)        0 2024-05-19 10:43:36.076873 banner_storedot-2.3.4/src/banner_storedot.egg-info/
+-rw-r--r--   0 adoram    (1002) adoram    (1002)     8763 2024-05-19 10:43:36.000000 banner_storedot-2.3.4/src/banner_storedot.egg-info/PKG-INFO
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)      544 2024-05-19 10:43:36.000000 banner_storedot-2.3.4/src/banner_storedot.egg-info/SOURCES.txt
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)        1 2024-05-19 10:43:36.000000 banner_storedot-2.3.4/src/banner_storedot.egg-info/dependency_links.txt
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)       75 2024-05-19 10:43:36.000000 banner_storedot-2.3.4/src/banner_storedot.egg-info/requires.txt
+-rw-rw-r--   0 adoram    (1002) adoram    (1002)        7 2024-05-19 10:43:36.000000 banner_storedot-2.3.4/src/banner_storedot.egg-info/top_level.txt
```

### Comparing `banner-storedot-2.3.3/LICENSE` & `banner_storedot-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/PKG-INFO` & `banner_storedot-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banner-storedot
-Version: 2.3.3
+Version: 2.3.4
 Summary: light dal package
 Home-page: https://https://github.com/storedot/banner
 Author: GB
 Author-email: techsupport@store-dot.com
 Project-URL: Bug Tracker, https://https://github.com/storedot/banner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `banner-storedot-2.3.3/README.md` & `banner_storedot-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/setup.cfg` & `banner_storedot-2.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = banner-storedot
-version = 2.3.3
+version = 2.3.4
 author = GB
 author_email = techsupport@store-dot.com
 description = light dal package
 long_description = file: README.md
 url = https://https://github.com/storedot/banner
 project_urls = 
 	Bug Tracker = https://https://github.com/storedot/banner/issues
```

### Comparing `banner-storedot-2.3.3/src/banner/connection.py` & `banner_storedot-2.3.4/src/banner/connection.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/src/banner/pandas_decorator.py` & `banner_storedot-2.3.4/src/banner/pandas_decorator.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/src/banner/pandas_wrap.py` & `banner_storedot-2.3.4/src/banner/pandas_wrap.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/src/banner/queries.py` & `banner_storedot-2.3.4/src/banner/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
             data = data.group_by_auxchl() # Banner method, neware.group_by_auxchl
             nw_columns.extend([column for column in data.columns if column.startswith(NW_TEMP)]) # nw_columns add temp columns
             
         except KeyError:
             pass
         
         if not raw:
-            data = calculate_neware_columns(data, cache_df=cachejoin_table_data) # Calculate neware columns
+            data = calculate_neware_columns(data, cache_df=cache_data) # Calculate neware columns
 
         if dqdv:
             data['dqdv'] = calculate_dqdv(data, raw=raw) # Calculate dqdv
             nw_columns.append('dqdv')
 
         try:
             data = merge_cache(data, cache_data, columns=nw_cache_columns) # Merge requested cache columns
```

### Comparing `banner-storedot-2.3.3/src/banner/utils/const.py` & `banner_storedot-2.3.4/src/banner/utils/const.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/src/banner/utils/misc.py` & `banner_storedot-2.3.4/src/banner/utils/misc.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/src/banner/utils/neware.py` & `banner_storedot-2.3.4/src/banner/utils/neware.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     if NW_VOLTAGE in df:
         df[NW_VOLTAGE] = calculate_voltage(df)
     
     if NW_CURRENT in df and NW_STEP_RANGE in df:
         df[NW_CURRENT] = calculate_current(df)
     
     if NW_TIMESTAMP in df:
-        df[NW_TIMESTAMP] = calculate_neware_timestamp(df, cache_df=cache_df)
+        result = calculate_neware_timestamp(df, cache_df=cache_df)
+        df[NW_TIMESTAMP] = result.values
     
     temp_columns = [column for column in df.columns if column.startswith(NW_TEMP)] # Temperature columns
     
     if temp_columns:
         df[temp_columns] = df[temp_columns].apply(lambda obj: obj / 10)
     
     return df
```

### Comparing `banner-storedot-2.3.3/src/banner/utils/pandas.py` & `banner_storedot-2.3.4/src/banner/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/src/banner/utils/web2py.py` & `banner_storedot-2.3.4/src/banner/utils/web2py.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.3/src/banner_storedot.egg-info/PKG-INFO` & `banner_storedot-2.3.4/src/banner_storedot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banner-storedot
-Version: 2.3.3
+Version: 2.3.4
 Summary: light dal package
 Home-page: https://https://github.com/storedot/banner
 Author: GB
 Author-email: techsupport@store-dot.com
 Project-URL: Bug Tracker, https://https://github.com/storedot/banner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `banner-storedot-2.3.3/src/banner_storedot.egg-info/SOURCES.txt` & `banner_storedot-2.3.4/src/banner_storedot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

