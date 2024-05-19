# Comparing `tmp/sportswrangler-0.1.6.tar.gz` & `tmp/sportswrangler-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportswrangler-0.1.6.tar", max compression
+gzip compressed data, was "sportswrangler-0.1.7.tar", max compression
```

## Comparing `sportswrangler-0.1.6.tar` & `sportswrangler-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      454 2024-05-19 05:35:59.137287 sportswrangler-0.1.6/README.md
--rw-r--r--   0        0        0      422 2024-05-19 05:35:59.137287 sportswrangler-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      218 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/generic/__init__.py
--rw-r--r--   0        0        0     2070 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/generic/wrangler.py
--rw-r--r--   0        0        0      129 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/global_configs.py
--rw-r--r--   0        0        0       28 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/__init__.py
--rw-r--r--   0        0        0      206 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/utils/__init__.py
--rw-r--r--   0        0        0     3747 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/utils/classes.py
--rw-r--r--   0        0        0      238 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/utils/constants.py
--rw-r--r--   0        0        0     4739 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/utils/enums.py
--rw-r--r--   0        0        0      252 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/__init__.py
--rw-r--r--   0        0        0    20194 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/base.py
--rw-r--r--   0        0        0     2059 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/epl.py
--rw-r--r--   0        0        0     2109 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/mlb.py
--rw-r--r--   0        0        0     1979 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/nba.py
--rw-r--r--   0        0        0     2306 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/nfl.py
--rw-r--r--   0        0        0     1382 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/nhl.py
--rw-r--r--   0        0        0       51 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/sports/__init__.py
--rw-r--r--   0        0        0       40 2024-05-19 05:35:59.141287 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/__init__.py
--rw-r--r--   0        0        0   531535 2024-05-19 05:35:59.145288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/MLB/players.csv
--rw-r--r--   0        0        0     5204 2024-05-19 05:35:59.145288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
--rw-r--r--   0        0        0   144790 2024-05-19 05:35:59.145288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NBA/players.csv
--rw-r--r--   0        0        0     3101 2024-05-19 05:35:59.145288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
--rw-r--r--   0        0        0   774056 2024-05-19 05:35:59.153288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NFL/players.csv
--rw-r--r--   0        0        0     8878 2024-05-19 05:35:59.153288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
--rw-r--r--   0        0        0   293594 2024-05-19 05:35:59.153288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NHL/players.csv
--rw-r--r--   0        0        0     3313 2024-05-19 05:35:59.153288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
--rw-r--r--   0        0        0    12392 2024-05-19 05:35:59.153288 sportswrangler-0.1.6/sportswrangler/sports/data_feeds/wrangler.py
--rw-r--r--   0        0        0        0 2024-05-19 05:35:59.153288 sportswrangler-0.1.6/sportswrangler/utils/__init__.py
--rw-r--r--   0        0        0      250 2024-05-19 05:35:59.153288 sportswrangler-0.1.6/sportswrangler/utils/enums.py
--rw-r--r--   0        0        0      142 2024-05-19 05:35:59.153288 sportswrangler-0.1.6/sportswrangler/utils/helpers.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 sportswrangler-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      454 2024-05-19 06:06:44.384918 sportswrangler-0.1.7/README.md
+-rw-r--r--   0        0        0      422 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      218 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/generic/__init__.py
+-rw-r--r--   0        0        0     2070 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/generic/wrangler.py
+-rw-r--r--   0        0        0      129 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/global_configs.py
+-rw-r--r--   0        0        0       28 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/utils/__init__.py
+-rw-r--r--   0        0        0     3747 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/utils/classes.py
+-rw-r--r--   0        0        0      238 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/utils/constants.py
+-rw-r--r--   0        0        0     4739 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/utils/enums.py
+-rw-r--r--   0        0        0      252 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/__init__.py
+-rw-r--r--   0        0        0    20320 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/base.py
+-rw-r--r--   0        0        0     2059 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/epl.py
+-rw-r--r--   0        0        0     2109 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/mlb.py
+-rw-r--r--   0        0        0     1979 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/nba.py
+-rw-r--r--   0        0        0     2306 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/nfl.py
+-rw-r--r--   0        0        0     1382 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/nhl.py
+-rw-r--r--   0        0        0       51 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/sports/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-19 06:06:44.388918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/__init__.py
+-rw-r--r--   0        0        0   531535 2024-05-19 06:06:44.392918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/MLB/players.csv
+-rw-r--r--   0        0        0     5204 2024-05-19 06:06:44.392918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
+-rw-r--r--   0        0        0   144790 2024-05-19 06:06:44.392918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NBA/players.csv
+-rw-r--r--   0        0        0     3101 2024-05-19 06:06:44.392918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
+-rw-r--r--   0        0        0   774056 2024-05-19 06:06:44.400918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NFL/players.csv
+-rw-r--r--   0        0        0     8878 2024-05-19 06:06:44.400918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
+-rw-r--r--   0        0        0   293594 2024-05-19 06:06:44.400918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NHL/players.csv
+-rw-r--r--   0        0        0     3313 2024-05-19 06:06:44.400918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
+-rw-r--r--   0        0        0    12392 2024-05-19 06:06:44.400918 sportswrangler-0.1.7/sportswrangler/sports/data_feeds/wrangler.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:06:44.400918 sportswrangler-0.1.7/sportswrangler/utils/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-19 06:06:44.400918 sportswrangler-0.1.7/sportswrangler/utils/enums.py
+-rw-r--r--   0        0        0      142 2024-05-19 06:06:44.404918 sportswrangler-0.1.7/sportswrangler/utils/helpers.py
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 sportswrangler-0.1.7/PKG-INFO
```

### Comparing `sportswrangler-0.1.6/sportswrangler/generic/wrangler.py` & `sportswrangler-0.1.7/sportswrangler/generic/wrangler.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/utils/classes.py` & `sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/utils/classes.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/utils/enums.py` & `sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/utils/enums.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/base.py` & `sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,14 +419,16 @@
     def standardize_odds(
         self, df: list | pd.DataFrame | pl.LazyFrame
     ) -> list | pd.DataFrame | pl.LazyFrame:
         # Only standardize DataFrames
         if isinstance(df, list):
             return df
         elif isinstance(df, pd.DataFrame):
+            if df.empty:
+                return df
             melted_df = pd.melt(
                 df,
                 id_vars=self.standardization_config.id_vars,
                 var_name=self.standardization_config.variable_name,
                 value_name=self.standardization_config.value_name,
             )
             return (
@@ -441,14 +443,16 @@
                         )
                     )
                 ]
                 if self.standardization_config.filter_na_odds
                 else melted_df
             )
         elif isinstance(df, pl.LazyFrame):
+            if df.limit(1).collect().is_empty():
+                return df
             melted_df = df.melt(
                 id_vars=self.standardization_config.id_vars,
                 variable_name=self.standardization_config.variable_name,
                 value_name=self.standardization_config.value_name,
             )
             return (
                 melted_df.filter(
```

### Comparing `sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/epl.py` & `sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/epl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/mlb.py` & `sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/mlb.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/nba.py` & `sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/nba.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/nfl.py` & `sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/nfl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/odds/the_odds_api/wranglers/nhl.py` & `sportswrangler-0.1.7/sportswrangler/odds/the_odds_api/wranglers/nhl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/MLB/players.csv` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/MLB/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/MLB/teams.csv` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/MLB/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NBA/players.csv` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NBA/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NBA/teams.csv` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NBA/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NFL/players.csv` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NFL/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NFL/teams.csv` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NFL/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NHL/players.csv` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NHL/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/assets/NHL/teams.csv` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/assets/NHL/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/sportswrangler/sports/data_feeds/wrangler.py` & `sportswrangler-0.1.7/sportswrangler/sports/data_feeds/wrangler.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.6/PKG-INFO` & `sportswrangler-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sportswrangler
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for wranglin' sports and sports odds data
 Author: Dejon
 Author-email: dejon.wright@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

