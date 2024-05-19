# Comparing `tmp/cnparser-1.5.4.tar.gz` & `tmp/cnparser-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnparser-1.5.4.tar", last modified: Sat May 18 13:43:16 2024, max compression
+gzip compressed data, was "cnparser-1.5.5.tar", last modified: Sat May 18 14:17:30 2024, max compression
```

## Comparing `cnparser-1.5.4.tar` & `cnparser-1.5.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.117541 cnparser-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-18 13:43:06.000000 cnparser-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 13:43:16.117541 cnparser-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-18 13:43:06.000000 cnparser-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.109541 cnparser-1.5.4/cnparser/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.113541 cnparser-1.5.4/cnparser/config/
--rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/eng_kana.json
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/file_id.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/header.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/kind.json
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/config/legal_entity.json
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-18 13:43:06.000000 cnparser-1.5.4/cnparser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.117541 cnparser-1.5.4/cnparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 13:43:16.000000 cnparser-1.5.4/cnparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 13:43:16.117541 cnparser-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-18 13:43:06.000000 cnparser-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:16.117541 cnparser-1.5.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 13:43:06.000000 cnparser-1.5.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-18 13:43:06.000000 cnparser-1.5.4/test/test_enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-18 13:43:06.000000 cnparser-1.5.4/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:17:30.151475 cnparser-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-18 14:17:19.000000 cnparser-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-18 14:17:30.147475 cnparser-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-18 14:17:19.000000 cnparser-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:17:30.143475 cnparser-1.5.5/cnparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:17:30.147475 cnparser-1.5.5/cnparser/config/
+-rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/config/eng_kana.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/config/file_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/config/header.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/config/kind.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/config/legal_entity.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-18 14:17:19.000000 cnparser-1.5.5/cnparser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:17:30.147475 cnparser-1.5.5/cnparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-18 14:17:30.000000 cnparser-1.5.5/cnparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 14:17:30.000000 cnparser-1.5.5/cnparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:17:30.000000 cnparser-1.5.5/cnparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 14:17:30.000000 cnparser-1.5.5/cnparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 14:17:30.000000 cnparser-1.5.5/cnparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:17:30.151475 cnparser-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-18 14:17:19.000000 cnparser-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:17:30.147475 cnparser-1.5.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:17:19.000000 cnparser-1.5.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-18 14:17:19.000000 cnparser-1.5.5/test/test_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-18 14:17:19.000000 cnparser-1.5.5/test/test_load.py
```

### Comparing `cnparser-1.5.4/LICENSE` & `cnparser-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.4/PKG-INFO` & `cnparser-1.5.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.4
+Version: 1.5.5
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -59,17 +59,19 @@
 The functions perform all processing, but it is possible to apply only specific processing by defining specific processing as an argument.
 ```python:
 >>> import cnparser
 >>> df = cnparser.enrich(df, "enrich_kana" ...)
 ```
 
 The processes supported by the `enrich` function are as follows:
-- `enrich_kana`: function adding a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversion is not supported.  
-- `enrich_kind`: function adding label of `kind` to `std_legal_entity`.  
-  
+- `enrich_kana`: Function that adds a standardized furigana column `std_furigana` to the DataFrame. It handles data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversions are not supported.  
+- `enrich_kind`: Function that adds the `kind` label to the `std_legal_entity`.  
+- `enrich_post_code`: Function that adds the formatted postcode as XXX-XXX to `std_post_code`.  
+
+
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
 ```shell:
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.4/README.md` & `cnparser-1.5.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,17 +45,19 @@
 The functions perform all processing, but it is possible to apply only specific processing by defining specific processing as an argument.
 ```python:
 >>> import cnparser
 >>> df = cnparser.enrich(df, "enrich_kana" ...)
 ```
 
 The processes supported by the `enrich` function are as follows:
-- `enrich_kana`: function adding a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversion is not supported.  
-- `enrich_kind`: function adding label of `kind` to `std_legal_entity`.  
-  
+- `enrich_kana`: Function that adds a standardized furigana column `std_furigana` to the DataFrame. It handles data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversions are not supported.  
+- `enrich_kind`: Function that adds the `kind` label to the `std_legal_entity`.  
+- `enrich_post_code`: Function that adds the formatted postcode as XXX-XXX to `std_post_code`.  
+
+
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
 ```shell:
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.4/cnparser/config/eng_kana.json` & `cnparser-1.5.5/cnparser/config/eng_kana.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.4/cnparser/config/file_id.json` & `cnparser-1.5.5/cnparser/config/file_id.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.4/cnparser/config/header.json` & `cnparser-1.5.5/cnparser/config/header.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.4/cnparser/config/legal_entity.json` & `cnparser-1.5.5/cnparser/config/legal_entity.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.4/cnparser/enrich.py` & `cnparser-1.5.5/cnparser/enrich.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     Returns:
         pd.DataFrame: The enriched DataFrame.
     """
     default_functions = {
         'enrich_kana': enrich_kana,
         'enrich_kind': enrich_kind,
+        'enrich_post_code': enrich_post_code,
     }
 
     if processes:
         default_functions = {key: default_functions[key] for key in processes if key in default_functions}
 
     if default_functions:
         return _parallel_process(df, default_functions)
@@ -96,7 +97,20 @@
 
     Returns:
         pd.DataFrame: The DataFrame with the 'std_legal_entity' column added, containing standardized legal entity descriptions.
     """
     kind = load_config("kind")
     df['std_legal_entity'] = df['kind'].map(kind)
     return df
+
+def enrich_post_code(df: pd.DataFrame) -> pd.DataFrame:
+    """
+    Adds a standardized postal code column to the DataFrame.
+
+    Args:
+        df (pd.DataFrame): The DataFrame to be enriched.
+
+    Returns:
+        pd.DataFrame: The DataFrame with the 'std_post_code' column added, where postal codes are formatted as 'XXX-XXX'.
+    """
+    df['std_post_code'] = df['post_code'].apply(lambda x: f"{str(x)[:3]}-{str(x)[3:]}" if pd.notna(x) else None)
+    return df
```

### Comparing `cnparser-1.5.4/cnparser/load.py` & `cnparser-1.5.5/cnparser/load.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.4/cnparser/utility.py` & `cnparser-1.5.5/cnparser/utility.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.4/cnparser.egg-info/PKG-INFO` & `cnparser-1.5.5/cnparser.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.4
+Version: 1.5.5
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -59,17 +59,19 @@
 The functions perform all processing, but it is possible to apply only specific processing by defining specific processing as an argument.
 ```python:
 >>> import cnparser
 >>> df = cnparser.enrich(df, "enrich_kana" ...)
 ```
 
 The processes supported by the `enrich` function are as follows:
-- `enrich_kana`: function adding a standardized furigana column `std_furigana` to the DataFrame. It processes data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversion is not supported.  
-- `enrich_kind`: function adding label of `kind` to `std_legal_entity`.  
-  
+- `enrich_kana`: Function that adds a standardized furigana column `std_furigana` to the DataFrame. It handles data entry by converting `name` to kana, if `furigana` is NaN. Note that currently only kanji and katakana conversions are supported. Alphabet conversions are not supported.  
+- `enrich_kind`: Function that adds the `kind` label to the `std_legal_entity`.  
+- `enrich_post_code`: Function that adds the formatted postcode as XXX-XXX to `std_post_code`.  
+
+
 ## Tools
 ### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
 This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
 ```shell:
 $ cd /home/<USER>/analysis
 $ python enrich.py <FILE_PATH>
 ```
```

### Comparing `cnparser-1.5.4/setup.py` & `cnparser-1.5.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cnparser',
-    version='1.5.4',
+    version='1.5.5',
     author='new-village',
     url='https://github.com/new-village/cnparser',
     description='cnparser is a parser library of Corporate Number Publication Site data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPLv3+',
     install_requires=['requests', 'bs4', 'pandas', 'pykakasi'],
```

### Comparing `cnparser-1.5.4/test/test_enrich.py` & `cnparser-1.5.5/test/test_enrich.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ test_enrich.py
 """
 import pandas as pd
 import unittest
-from cnparser.enrich import enrich, enrich_kana, enrich_kind
+from cnparser.enrich import enrich, enrich_kana, enrich_kind, enrich_post_code
 from cnparser.load import read_csv
 
 class TestEnrich(unittest.TestCase):
     def setUp(self):
         """Set up the test environment by loading test data from a CSV file."""
         self.df = read_csv('./test/data/31_tottori_test_20240329.csv')
 
@@ -22,19 +22,28 @@
         """Test the enrich_kind function to ensure it correctly maps 'kind' to 'std_legal_entity'."""
         result = enrich_kind(self.df.copy())
         self.assertIn('std_legal_entity', result.columns)
         expected_entities = ['National Agency', 'K.K.', 'K.K.', 'K.K.', 'Y.K.']
         for i, entity in enumerate(expected_entities):
             self.assertEqual(result.iloc[i]['std_legal_entity'], entity)
 
+    def test_enrich_postcode(self):
+        """Test the enrich_kind function to ensure it correctly maps 'kind' to 'std_legal_entity'."""
+        result = enrich_post_code(self.df.copy())
+        self.assertIn('std_post_code', result.columns)
+        expected_entities = ['680-0011', None, '692-0011', '699-0101', '693-0005']
+        for i, entity in enumerate(expected_entities):
+            self.assertEqual(result.iloc[i]['std_post_code'], entity)
+
     def test_enrich_all_processes(self):
         """Test the enrich function with all processes to ensure it processes correctly."""
         result = enrich(self.df.copy())
         self.assertIn('std_furigana', result.columns)
         self.assertIn('std_legal_entity', result.columns)
+        self.assertIn('std_post_code', result.columns)
 
     def test_enrich_with_invalid_process(self):
         """Test the enrich function with an invalid process name to ensure it returns the original DataFrame unchanged and raises a warning."""
         with self.assertWarns(Warning) as warning:
             result = enrich(self.df.copy(), 'enrich_error')
             self.assertEqual(str(warning.warnings[0].message), "No valid processing functions specified in ('enrich_error',). Returning the original DataFrame unchanged.")
         pd.testing.assert_frame_equal(self.df, result)
```

### Comparing `cnparser-1.5.4/test/test_load.py` & `cnparser-1.5.5/test/test_load.py`

 * *Files identical despite different names*

