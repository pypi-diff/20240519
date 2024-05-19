# Comparing `tmp/csv2notion_neo-1.2.5.tar.gz` & `tmp/csv2notion_neo-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv2notion_neo-1.2.5.tar", max compression
+gzip compressed data, was "csv2notion_neo-1.2.6.tar", max compression
```

## Comparing `csv2notion_neo-1.2.5.tar` & `csv2notion_neo-1.2.6.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0     2933 2024-05-11 07:26:46.563915 csv2notion_neo-1.2.5/CHANGELOG.md
--rw-r--r--   0        0        0     1068 2024-05-11 07:26:46.563915 csv2notion_neo-1.2.5/LICENSE
--rw-r--r--   0        0        0    27658 2024-05-11 07:26:46.563915 csv2notion_neo-1.2.5/README.md
--rw-r--r--   0        0        0        0 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/__init__.py
--rw-r--r--   0        0        0      119 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/__main__.py
--rw-r--r--   0        0        0     3195 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/cli.py
--rw-r--r--   0        0        0    11825 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/cli_args.py
--rw-r--r--   0        0        0     2348 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/cli_steps.py
--rw-r--r--   0        0        0     5533 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/local_data.py
--rw-r--r--   0        0        0        0 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/__init__.py
--rw-r--r--   0        0        0    24846 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/block.py
--rw-r--r--   0        0        0    16051 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/client.py
--rw-r--r--   0        0        0    27147 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/collection.py
--rw-r--r--   0        0        0     1107 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/logger.py
--rw-r--r--   0        0        0     3725 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/maps.py
--rw-r--r--   0        0        0     9350 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/markdown.py
--rw-r--r--   0        0        0     8200 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/monitor.py
--rw-r--r--   0        0        0     1021 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/operations.py
--rw-r--r--   0        0        0     4898 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/records.py
--rw-r--r--   0        0        0      671 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/settings.py
--rw-r--r--   0        0        0     9398 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/smoke_test.py
--rw-r--r--   0        0        0     1636 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/space.py
--rw-r--r--   0        0        0    14842 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/store.py
--rw-r--r--   0        0        0      546 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/user.py
--rw-r--r--   0        0        0     2851 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion/utils.py
--rw-r--r--   0        0        0     2279 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion/utils_ssl.py
--rw-r--r--   0        0        0    12437 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_convert.py
--rw-r--r--   0        0        0     1922 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_convert_map.py
--rw-r--r--   0        0        0     6697 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_db.py
--rw-r--r--   0        0        0     2072 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_db_client.py
--rw-r--r--   0        0        0     5092 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_db_collection.py
--rw-r--r--   0        0        0     9697 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_preparator.py
--rw-r--r--   0        0        0     9799 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_row.py
--rw-r--r--   0        0        0     4151 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_row_image_block.py
--rw-r--r--   0        0        0     2908 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_row_upload_file.py
--rw-r--r--   0        0        0     1126 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_type_guess.py
--rw-r--r--   0        0        0     1759 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_uploader.py
--rw-r--r--   0        0        0     1276 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_db.py
--rw-r--r--   0        0        0      305 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_exceptions.py
--rw-r--r--   0        0        0      331 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_file.py
--rw-r--r--   0        0        0      679 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_rand_id.py
--rw-r--r--   0        0        0     1792 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_static.py
--rw-r--r--   0        0        0      249 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_str.py
--rw-r--r--   0        0        0     1387 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_threading.py
--rw-r--r--   0        0        0       22 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/version.py
--rw-r--r--   0        0        0     5334 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/pyproject.toml
--rw-r--r--   0        0        0    29622 1970-01-01 00:00:00.000000 csv2notion_neo-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3070 2024-05-19 01:26:54.960995 csv2notion_neo-1.2.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1068 2024-05-19 01:26:54.960995 csv2notion_neo-1.2.6/LICENSE
+-rw-r--r--   0        0        0    27897 2024-05-19 01:26:54.960995 csv2notion_neo-1.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:26:55.401000 csv2notion_neo-1.2.6/csv2notion_neo/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-19 01:26:55.401000 csv2notion_neo-1.2.6/csv2notion_neo/__main__.py
+-rw-r--r--   0        0        0     3139 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/cli.py
+-rw-r--r--   0        0        0    11825 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/cli_args.py
+-rw-r--r--   0        0        0     2353 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/cli_steps.py
+-rw-r--r--   0        0        0     5533 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/local_data.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/__init__.py
+-rw-r--r--   0        0        0    24846 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/block.py
+-rw-r--r--   0        0        0    16051 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/client.py
+-rw-r--r--   0        0        0    27147 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/collection.py
+-rw-r--r--   0        0        0     1107 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/logger.py
+-rw-r--r--   0        0        0     3725 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/maps.py
+-rw-r--r--   0        0        0     9350 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/markdown.py
+-rw-r--r--   0        0        0     8200 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/monitor.py
+-rw-r--r--   0        0        0     1021 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/operations.py
+-rw-r--r--   0        0        0     4898 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/records.py
+-rw-r--r--   0        0        0      671 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/settings.py
+-rw-r--r--   0        0        0     9398 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/smoke_test.py
+-rw-r--r--   0        0        0     1636 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/space.py
+-rw-r--r--   0        0        0    14842 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/store.py
+-rw-r--r--   0        0        0      546 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/user.py
+-rw-r--r--   0        0        0     2851 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/utils.py
+-rw-r--r--   0        0        0     2279 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/utils_ssl.py
+-rw-r--r--   0        0        0    12666 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_convert.py
+-rw-r--r--   0        0        0     1922 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_convert_map.py
+-rw-r--r--   0        0        0     6697 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_db.py
+-rw-r--r--   0        0        0     2072 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_db_client.py
+-rw-r--r--   0        0        0     5092 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_db_collection.py
+-rw-r--r--   0        0        0     9697 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_preparator.py
+-rw-r--r--   0        0        0     9799 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_row.py
+-rw-r--r--   0        0        0     4151 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_row_image_block.py
+-rw-r--r--   0        0        0     2908 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_row_upload_file.py
+-rw-r--r--   0        0        0     1126 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_type_guess.py
+-rw-r--r--   0        0        0     1759 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_uploader.py
+-rw-r--r--   0        0        0     1503 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_ai.py
+-rw-r--r--   0        0        0     1276 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_db.py
+-rw-r--r--   0        0        0      305 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_exceptions.py
+-rw-r--r--   0        0        0      331 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_file.py
+-rw-r--r--   0        0        0      679 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_rand_id.py
+-rw-r--r--   0        0        0     1792 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_static.py
+-rw-r--r--   0        0        0      249 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_str.py
+-rw-r--r--   0        0        0     1387 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_threading.py
+-rw-r--r--   0        0        0       22 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/version.py
+-rw-r--r--   0        0        0     5334 2024-05-19 01:26:55.409000 csv2notion_neo-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0    29861 1970-01-01 00:00:00.000000 csv2notion_neo-1.2.6/PKG-INFO
```

### Comparing `csv2notion_neo-1.2.5/CHANGELOG.md` & `csv2notion_neo-1.2.6/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+### 1.2.6
+
+**🎉 Released:**
+- 19th May 2024
+
+**🔨 Improvements:**
+- Improved log output for `--rename-notion-key-column` (#35)
+
+---
+
 ### 1.2.5
 
 **🎉 Released:**
 - 10th May 2024
 
 **🔨 Improvements:**
 - Improved image and icon upload logic (#32)
```

### Comparing `csv2notion_neo-1.2.5/LICENSE` & `csv2notion_neo-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/README.md` & `csv2notion_neo-1.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -524,14 +524,24 @@
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_10.gif?raw=true"> </p>
 
 </p>
 </details>
 
 ## Utilised By
 
+### Marker Data
+
+<details><summary>Marker Data's Notion Panel</summary>
+<p>
+
+<p align="center"> <img src="https://github.com/TheAcharya/MarkerData-Website/blob/main/docs/assets/md-database-settings_01.png?raw=true"> </p>
+
+</p>
+</details>
+
 ### [CommandPost](https://commandpost.io)
 
 <details><summary>CommandPost's Notion Toolbox</summary>
 <p>
 
 <p align="center"> <img src="https://github.com/CommandPost/CommandPost-Website/blob/main/docs/static/toolbox-notion.png?raw=true"> </p>
```

#### html2text {}

```diff
@@ -308,16 +308,18 @@
 Importing JSON into Existing Database with a Different Key Column
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
 YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-
 column "Cat ID" --rename-notion-key-column "Cat ID" "Anything ID" --merge JSON-
 Demo.json ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_10.gif?raw=true]
-## Utilised By ### [CommandPost](https://commandpost.io) CommandPost's Notion
-Toolbox
+## Utilised By ### Marker Data Marker Data's Notion Panel
+  [https://github.com/TheAcharya/MarkerData-Website/blob/main/docs/assets/md-
+                      database-settings_01.png?raw=true]
+### [CommandPost](https://commandpost.io) CommandPost's Notion Toolbox
   [https://github.com/CommandPost/CommandPost-Website/blob/main/docs/static/
                          toolbox-notion.png?raw=true]
 ## Credits Original Idea and Workflow Architecture by [Vigneswaran Rajkumar]
 (https://twitter.com/IAmVigneswaran) Maintained by [Arjun Prakash](https://
 github.com/arjunprakash027) (1.0.0 ...) Original Work by [Vladilen Zhdanov]
 (https://github.com/vzhd1701) Icon Design by [Bor Jen Goh](https://
 www.artstation.com/borjengoh) ## License Licensed under the MIT license. See
```

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/cli.py` & `csv2notion_neo-1.2.6/csv2notion_neo/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         logger.info("Done!")
 
     except Exception as e:
         if args.verbose:
             logger.error('Error at %s', 'division', exc_info=e)
         else:
-            logger.error("An error has occured! use --verbose switch to know more")
+            logger.error(e)
 
 
 def setup_logging(is_verbose: bool = False, log_file: Optional[Path] = None) -> None:
     logging.basicConfig(format="%(levelname)s: %(message)s")
 
     logging.getLogger("csv2notion_neo").setLevel(
         logging.DEBUG if is_verbose else logging.INFO
```

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/cli_args.py` & `csv2notion_neo-1.2.6/csv2notion_neo/cli_args.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/cli_steps.py` & `csv2notion_neo-1.2.6/csv2notion_neo/cli_steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
     conversion_rules = ConversionRules.from_args(args)
 
     NotionPreparator(notion_db, csv_data, conversion_rules).prepare()
 
 
     converter = NotionRowConverter(notion_db, conversion_rules)
+    
     return converter.convert_to_notion_rows(csv_data)
 
 
 def upload_rows(
     notion_rows: List[NotionUploadRow],
     client: NotionClientExtended,
     collection_id: str,
```

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/local_data.py` & `csv2notion_neo-1.2.6/csv2notion_neo/local_data.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/block.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/block.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/client.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/client.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/collection.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/collection.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/logger.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/logger.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/maps.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/maps.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/markdown.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/markdown.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/monitor.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/monitor.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/operations.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/operations.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/records.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/records.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/settings.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/settings.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/smoke_test.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/smoke_test.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/space.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/space.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/store.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/store.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/user.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/user.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/utils.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/utils.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion/utils_ssl.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion/utils_ssl.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_convert.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     map_number,
     map_url_or_file,
 )
 from csv2notion_neo.notion_db import NotionDB
 from csv2notion_neo.notion_row import CollectionRowBlockExtended
 from csv2notion_neo.notion_type_guess import is_email
 from csv2notion_neo.notion_uploader import NotionUploadRow
-from csv2notion_neo.utils_exceptions import NotionError, TypeConversionError
+from csv2notion_neo.utils_exceptions import NotionError, TypeConversionError, CriticalError
 from csv2notion_neo.utils_static import ConversionRules, FileType
 from csv2notion_neo.utils_str import split_str
 from icecream import ic
 
 logger = logging.getLogger(__name__)
 
 
@@ -35,15 +35,18 @@
 
     def convert_to_notion_rows(self, csv_data: LocalData) -> List[NotionUploadRow]:
         notion_rows = []
         # starting with 2nd row, because first is header
         self._current_row = 2
 
         for row in csv_data:
+
             if self.rules.rename_notion_key_column:
+                if self.rules.rename_notion_key_column[1] == self.rules.rename_notion_key_column[0]:
+                    raise CriticalError(f"Please do not provide same column name in rename-payload-key-column")
                 new_id = self.rules.rename_notion_key_column[1]
                 old_id = self.rules.rename_notion_key_column[0]
                 row[new_id] = row[old_id]
                 del row[old_id]
 
             try:
                 notion_rows.append(self._convert_row(row))
```

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_convert_map.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_convert_map.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_db.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_db.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_db_client.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_db_client.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_db_collection.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_db_collection.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_preparator.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_preparator.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_row.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_row.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_row_image_block.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_row_image_block.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_row_upload_file.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_row_upload_file.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_type_guess.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_type_guess.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/notion_uploader.py` & `csv2notion_neo-1.2.6/csv2notion_neo/notion_uploader.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/utils_db.py` & `csv2notion_neo-1.2.6/csv2notion_neo/utils_db.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/utils_rand_id.py` & `csv2notion_neo-1.2.6/csv2notion_neo/utils_rand_id.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/utils_static.py` & `csv2notion_neo-1.2.6/csv2notion_neo/utils_static.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/csv2notion_neo/utils_threading.py` & `csv2notion_neo-1.2.6/csv2notion_neo/utils_threading.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.5/pyproject.toml` & `csv2notion_neo-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "csv2notion_neo"
-version = "1.2.5"
+version = "1.2.6"
 description = "Upload & Merge CSV Data with Images to Notion Database"
 authors = ["vzhd1701 <vzhd1701@gmail.com>", "Arjun <arjunprakash027@gmail.com>"]
 readme = "README.md"
 include = ["CHANGELOG.md"]
 license = "MIT"
 homepage = "https://github.com/TheAcharya/csv2notion-neo"
 repository = "https://github.com/TheAcharya/csv2notion-neo"
```

### Comparing `csv2notion_neo-1.2.5/PKG-INFO` & `csv2notion_neo-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv2notion-neo
-Version: 1.2.5
+Version: 1.2.6
 Summary: Upload & Merge CSV Data with Images to Notion Database
 Home-page: https://github.com/TheAcharya/csv2notion-neo
 License: MIT
 Keywords: csv,notion,import,merge
 Author: vzhd1701
 Author-email: vzhd1701@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -571,14 +571,24 @@
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_10.gif?raw=true"> </p>
 
 </p>
 </details>
 
 ## Utilised By
 
+### Marker Data
+
+<details><summary>Marker Data's Notion Panel</summary>
+<p>
+
+<p align="center"> <img src="https://github.com/TheAcharya/MarkerData-Website/blob/main/docs/assets/md-database-settings_01.png?raw=true"> </p>
+
+</p>
+</details>
+
 ### [CommandPost](https://commandpost.io)
 
 <details><summary>CommandPost's Notion Toolbox</summary>
 <p>
 
 <p align="center"> <img src="https://github.com/CommandPost/CommandPost-Website/blob/main/docs/static/toolbox-notion.png?raw=true"> </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: csv2notion-neo Version: 1.2.5 Summary: Upload &
+Metadata-Version: 2.1 Name: csv2notion-neo Version: 1.2.6 Summary: Upload &
 Merge CSV Data with Images to Notion Database Home-page: https://github.com/
 TheAcharya/csv2notion-neo License: MIT Keywords: csv,notion,import,merge
 Author: vzhd1701 Author-email: vzhd1701@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft Classifier:
@@ -334,16 +334,18 @@
 Importing JSON into Existing Database with a Different Key Column
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
 YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-
 column "Cat ID" --rename-notion-key-column "Cat ID" "Anything ID" --merge JSON-
 Demo.json ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_10.gif?raw=true]
-## Utilised By ### [CommandPost](https://commandpost.io) CommandPost's Notion
-Toolbox
+## Utilised By ### Marker Data Marker Data's Notion Panel
+  [https://github.com/TheAcharya/MarkerData-Website/blob/main/docs/assets/md-
+                      database-settings_01.png?raw=true]
+### [CommandPost](https://commandpost.io) CommandPost's Notion Toolbox
   [https://github.com/CommandPost/CommandPost-Website/blob/main/docs/static/
                          toolbox-notion.png?raw=true]
 ## Credits Original Idea and Workflow Architecture by [Vigneswaran Rajkumar]
 (https://twitter.com/IAmVigneswaran) Maintained by [Arjun Prakash](https://
 github.com/arjunprakash027) (1.0.0 ...) Original Work by [Vladilen Zhdanov]
 (https://github.com/vzhd1701) Icon Design by [Bor Jen Goh](https://
 www.artstation.com/borjengoh) ## License Licensed under the MIT license. See
```

