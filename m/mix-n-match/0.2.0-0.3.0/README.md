# Comparing `tmp/mix-n-match-0.2.0.tar.gz` & `tmp/mix_n_match-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mix-n-match-0.2.0.tar", last modified: Wed Nov 29 13:16:19 2023, max compression
+gzip compressed data, was "mix_n_match-0.3.0.tar", last modified: Sun May 19 14:32:37 2024, max compression
```

## Comparing `mix-n-match-0.2.0.tar` & `mix_n_match-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 13:16:19.838755 mix-n-match-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-11-29 13:16:19.838755 mix-n-match-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 13:16:19.834755 mix-n-match-0.2.0/mix_n_match/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/mix_n_match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/mix_n_match/correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    19151 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/mix_n_match/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/mix_n_match/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 13:16:19.838755 mix-n-match-0.2.0/mix_n_match.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-11-29 13:16:19.000000 mix-n-match-0.2.0/mix_n_match.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-11-29 13:16:19.000000 mix-n-match-0.2.0/mix_n_match.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 13:16:19.000000 mix-n-match-0.2.0/mix_n_match.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-29 13:16:19.000000 mix-n-match-0.2.0/mix_n_match.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-29 13:16:19.000000 mix-n-match-0.2.0/mix_n_match.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 13:16:19.838755 mix-n-match-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/requirements/extra.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/requirements/private.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/requirements/public.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 13:16:19.838755 mix-n-match-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2023-11-29 13:16:05.000000 mix-n-match-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/mix_n_match/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/mix_n_match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/mix_n_match/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19103 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/mix_n_match/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/mix_n_match/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/mix_n_match.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/requirements/extra.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/requirements/private.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/requirements/public.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/setup.py
```

### Comparing `mix-n-match-0.2.0/LICENSE` & `mix_n_match-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mix-n-match-0.2.0/mix_n_match/correlations.py` & `mix_n_match-0.3.0/mix_n_match/correlations.py`

 * *Files identical despite different names*

### Comparing `mix-n-match-0.2.0/mix_n_match/main.py` & `mix_n_match-0.3.0/mix_n_match/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             include_boundaries=True,  # TODO by default we dont need this tbh,
             # but for partial check this must be set to true
             closed=self.closed_boundaries,  # how to treat values at the
             # boundaries. Also affects the boundarties themselves.
             # If left, starts looking at [left, )
             label=self.labelling_strategy,
             start_by="window",
-            by=self.group_by_columns,
+            group_by=self.group_by_columns,
         )
 
         # -- start window takes a datapoint, then normalises it by "every",
         # applies the offset!
         # -- closed affects how the boundaru is created!!!
         # -- for each datapoint,
 
@@ -312,16 +312,14 @@
 
             target_columns = list(target_columns)
         else:
             target_columns = self.target_columns
 
         # -- sorting is necessary
         groupby_obj = self._groupby(X)
-        # for item in groupby_obj:
-        #    print(item)
         agg_func_list = []
         multiple_resampling_functions = len(self.resampling_function) > 1
         for target_column in target_columns:
             for resampling_function_metadata in self.resampling_function:
                 func_name = resampling_function_metadata["name"]
                 # TODO add support for arguments to these, e.g.
                 # "sum with truncation" if these are native!
@@ -369,15 +367,15 @@
                 X, self.time_column, "mode"
             )
 
             df_agg = df_agg.with_columns(
                 pl.col("_upper_boundary")
                 .sub(pl.col("_lower_boundary"))
                 .alias("_date_diff")
-                .dt.seconds()
+                .dt.total_seconds()
                 .truediv(frequency)
             )
 
             df_agg = df_agg.with_columns(
                 pl.col("_count").lt(pl.col("_date_diff")).alias("_is_partial")
             )
```

### Comparing `mix-n-match-0.2.0/setup.py` & `mix_n_match-0.3.0/setup.py`

 * *Files identical despite different names*

