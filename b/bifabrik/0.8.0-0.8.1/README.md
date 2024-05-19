# Comparing `tmp/bifabrik-0.8.0.tar.gz` & `tmp/bifabrik-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bifabrik-0.8.0.tar", max compression
+gzip compressed data, was "bifabrik-0.8.1.tar", max compression
```

## Comparing `bifabrik-0.8.0.tar` & `bifabrik-0.8.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1073 2024-05-09 13:17:58.797451 bifabrik-0.8.0/LICENSE
--rw-r--r--   0        0        0     4678 2024-05-09 13:17:58.797451 bifabrik-0.8.0/README.md
--rw-r--r--   0        0        0      575 2024-05-09 13:17:58.797451 bifabrik-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6451 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/__init__.py
--rw-r--r--   0        0        0     2896 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/base/Pipeline.py
--rw-r--r--   0        0        0     1798 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/base/Task.py
--rw-r--r--   0        0        0     5285 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/CompleteConfiguration.py
--rw-r--r--   0        0        0        0 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/Configuration.py
--rw-r--r--   0        0        0      755 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/CsvSourceConfiguration.py
--rw-r--r--   0        0        0      570 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py
--rw-r--r--   0        0        0      525 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/DataSourceConfigurationBase.py
--rw-r--r--   0        0        0      729 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/ExcelSourceConfiguration.py
--rw-r--r--   0        0        0      715 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/JsonSourceConfiguration.py
--rw-r--r--   0        0        0      512 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py
--rw-r--r--   0        0        0      605 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/TableDestinationConfiguration.py
--rw-r--r--   0        0        0      481 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/ValidationTransformationConfiguration.py
--rw-r--r--   0        0        0        0 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/__init__.py
--rw-r--r--   0        0        0     5626 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/engine/ConfigContainer.py
--rw-r--r--   0        0        0      411 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/engine/Configuration.py
--rw-r--r--   0        0        0     3895 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/CsvConfiguration.py
--rw-r--r--   0        0        0     2617 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
--rw-r--r--   0        0        0     4700 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/ExcelConfiguration.py
--rw-r--r--   0        0        0     2699 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py
--rw-r--r--   0        0        0     7254 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/JsonConfiguration.py
--rw-r--r--   0        0        0     3420 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/LogConfiguration.py
--rw-r--r--   0        0        0     2154 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
--rw-r--r--   0        0        0     2457 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/SecurityConfiguration.py
--rw-r--r--   0        0        0     2421 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
--rw-r--r--   0        0        0     5109 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/TableConfiguration.py
--rw-r--r--   0        0        0     4280 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/ValidationConfiguration.py
--rw-r--r--   0        0        0      970 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/CommonDestinationUtils.py
--rw-r--r--   0        0        0      379 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/DataDestination.py
--rw-r--r--   0        0        0    14889 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/LakehouseTableDestination.py
--rw-r--r--   0        0        0      909 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/PandasDfDestination.py
--rw-r--r--   0        0        0      834 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/SparkDfDestination.py
--rw-r--r--   0        0        0    29470 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/WarehouseTableDestination.py
--rw-r--r--   0        0        0        0 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/__init__.py
--rw-r--r--   0        0        0     3916 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/CsvSource.py
--rw-r--r--   0        0        0     4229 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/DataSource.py
--rw-r--r--   0        0        0     3925 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/ExcelSource.py
--rw-r--r--   0        0        0     3447 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/JsonSource.py
--rw-r--r--   0        0        0      919 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/PandasDfSource.py
--rw-r--r--   0        0        0     3588 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/SharePointListSource.py
--rw-r--r--   0        0        0      914 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/SparkDfSource.py
--rw-r--r--   0        0        0      941 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/SparkSqlSource.py
--rw-r--r--   0        0        0     3945 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/WarehouseSqlSource.py
--rw-r--r--   0        0        0        0 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/__init__.py
--rw-r--r--   0        0        0     3918 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/tsf/DataTransformation.py
--rw-r--r--   0        0        0     1086 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/tsf/PandasDfTransformation.py
--rw-r--r--   0        0        0      916 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/tsf/SparkDfTransformation.py
--rw-r--r--   0        0        0     5538 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/tsf/ValidationTransformation.py
--rw-r--r--   0        0        0    16111 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/utils/fsUtils.py
--rw-r--r--   0        0        0     7064 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/utils/log.py
--rw-r--r--   0        0        0     5371 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/utils/tableUtils.py
--rw-r--r--   0        0        0     6158 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/utils/tmslUtils.py
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 bifabrik-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-19 14:01:44.553798 bifabrik-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4678 2024-05-19 14:01:44.553798 bifabrik-0.8.1/README.md
+-rw-r--r--   0        0        0      575 2024-05-19 14:01:44.553798 bifabrik-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6451 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/__init__.py
+-rw-r--r--   0        0        0     2896 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/base/Pipeline.py
+-rw-r--r--   0        0        0     1798 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/base/Task.py
+-rw-r--r--   0        0        0     5285 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/CompleteConfiguration.py
+-rw-r--r--   0        0        0        0 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/Configuration.py
+-rw-r--r--   0        0        0      755 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/CsvSourceConfiguration.py
+-rw-r--r--   0        0        0      570 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py
+-rw-r--r--   0        0        0      525 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/DataSourceConfigurationBase.py
+-rw-r--r--   0        0        0      729 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/ExcelSourceConfiguration.py
+-rw-r--r--   0        0        0      715 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/JsonSourceConfiguration.py
+-rw-r--r--   0        0        0      512 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py
+-rw-r--r--   0        0        0      605 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/TableDestinationConfiguration.py
+-rw-r--r--   0        0        0      481 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/ValidationTransformationConfiguration.py
+-rw-r--r--   0        0        0        0 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/__init__.py
+-rw-r--r--   0        0        0     5626 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/engine/ConfigContainer.py
+-rw-r--r--   0        0        0      411 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/engine/Configuration.py
+-rw-r--r--   0        0        0     3895 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/CsvConfiguration.py
+-rw-r--r--   0        0        0     2617 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
+-rw-r--r--   0        0        0     4700 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/ExcelConfiguration.py
+-rw-r--r--   0        0        0     2699 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py
+-rw-r--r--   0        0        0     7254 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/JsonConfiguration.py
+-rw-r--r--   0        0        0     3420 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/LogConfiguration.py
+-rw-r--r--   0        0        0     2154 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
+-rw-r--r--   0        0        0     2457 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/SecurityConfiguration.py
+-rw-r--r--   0        0        0     2421 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
+-rw-r--r--   0        0        0     5109 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/TableConfiguration.py
+-rw-r--r--   0        0        0     4280 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/cfg/specific/ValidationConfiguration.py
+-rw-r--r--   0        0        0      970 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/dst/CommonDestinationUtils.py
+-rw-r--r--   0        0        0      379 2024-05-19 14:01:44.553798 bifabrik-0.8.1/src/bifabrik/dst/DataDestination.py
+-rw-r--r--   0        0        0    14889 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/dst/LakehouseTableDestination.py
+-rw-r--r--   0        0        0      909 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/dst/PandasDfDestination.py
+-rw-r--r--   0        0        0      834 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/dst/SparkDfDestination.py
+-rw-r--r--   0        0        0    29470 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/dst/WarehouseTableDestination.py
+-rw-r--r--   0        0        0        0 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/dst/__init__.py
+-rw-r--r--   0        0        0     4089 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/CsvSource.py
+-rw-r--r--   0        0        0     4229 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/DataSource.py
+-rw-r--r--   0        0        0     3925 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/ExcelSource.py
+-rw-r--r--   0        0        0     3447 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/JsonSource.py
+-rw-r--r--   0        0        0      919 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/PandasDfSource.py
+-rw-r--r--   0        0        0     3588 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/SharePointListSource.py
+-rw-r--r--   0        0        0      914 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/SparkDfSource.py
+-rw-r--r--   0        0        0      941 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/SparkSqlSource.py
+-rw-r--r--   0        0        0     3945 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/WarehouseSqlSource.py
+-rw-r--r--   0        0        0        0 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/src/__init__.py
+-rw-r--r--   0        0        0     3918 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/tsf/DataTransformation.py
+-rw-r--r--   0        0        0     1086 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/tsf/PandasDfTransformation.py
+-rw-r--r--   0        0        0      916 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/tsf/SparkDfTransformation.py
+-rw-r--r--   0        0        0     5538 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/tsf/ValidationTransformation.py
+-rw-r--r--   0        0        0    16111 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/utils/fsUtils.py
+-rw-r--r--   0        0        0     7064 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/utils/log.py
+-rw-r--r--   0        0        0     5371 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/utils/tableUtils.py
+-rw-r--r--   0        0        0     6158 2024-05-19 14:01:44.557798 bifabrik-0.8.1/src/bifabrik/utils/tmslUtils.py
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 bifabrik-0.8.1/PKG-INFO
```

### Comparing `bifabrik-0.8.0/LICENSE` & `bifabrik-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/README.md` & `bifabrik-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/pyproject.toml` & `bifabrik-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bifabrik"
-version = "0.8.0"
+version = "0.8.1"
 description = "Microsoft Fabric ETL toolbox"
 authors = ["Radovan Jankovič"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rjankovic.github.io/bifabrik/"
 documentation = "https://rjankovic.github.io/bifabrik/"
 repository = "https://github.com/rjankovic/bifabrik/"
```

### Comparing `bifabrik-0.8.0/src/bifabrik/__init__.py` & `bifabrik-0.8.1/src/bifabrik/__init__.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/base/Pipeline.py` & `bifabrik-0.8.1/src/bifabrik/base/Pipeline.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/base/Task.py` & `bifabrik-0.8.1/src/bifabrik/base/Task.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/CompleteConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/CompleteConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/CsvSourceConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/CsvSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py` & `bifabrik-0.8.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/DataSourceConfigurationBase.py` & `bifabrik-0.8.1/src/bifabrik/cfg/DataSourceConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/ExcelSourceConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/ExcelSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/JsonSourceConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/JsonSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/TableDestinationConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/TableDestinationConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/engine/ConfigContainer.py` & `bifabrik-0.8.1/src/bifabrik/cfg/engine/ConfigContainer.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/CsvConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/CsvConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/ExcelConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/ExcelConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/JsonConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/JsonConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/LogConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/LogConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/SecurityConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/SecurityConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/TableConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/TableConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/cfg/specific/ValidationConfiguration.py` & `bifabrik-0.8.1/src/bifabrik/cfg/specific/ValidationConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/dst/CommonDestinationUtils.py` & `bifabrik-0.8.1/src/bifabrik/dst/CommonDestinationUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/dst/LakehouseTableDestination.py` & `bifabrik-0.8.1/src/bifabrik/dst/LakehouseTableDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/dst/PandasDfDestination.py` & `bifabrik-0.8.1/src/bifabrik/dst/PandasDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/dst/SparkDfDestination.py` & `bifabrik-0.8.1/src/bifabrik/dst/SparkDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/dst/WarehouseTableDestination.py` & `bifabrik-0.8.1/src/bifabrik/dst/WarehouseTableDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/src/CsvSource.py` & `bifabrik-0.8.1/src/bifabrik/src/CsvSource.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,19 @@
                 header = mergedConfig.csv.header,
                 thousands = mergedConfig.csv.thousands,
                 decimal = mergedConfig.csv.decimal,
                 quotechar = mergedConfig.csv.quotechar,
                 quoting = mergedConfig.csv.quoting,
                 escapechar = mergedConfig.csv.escapechar
                 )
+            if pd_df.empty:
+                w = f'File {src_file} has no data - skipping'
+                lgr.warn(w)
+                print(w)
+                continue
             df = self._spark.createDataFrame(pd_df)
             fileDfs.append(df)
         if len(fileDfs) == 0:
             return None
         df = fileDfs[0]
         if len(fileDfs) > 1:
             for i in range(1, len(fileDfs)):
```

### Comparing `bifabrik-0.8.0/src/bifabrik/src/DataSource.py` & `bifabrik-0.8.1/src/bifabrik/src/DataSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/src/ExcelSource.py` & `bifabrik-0.8.1/src/bifabrik/src/ExcelSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/src/JsonSource.py` & `bifabrik-0.8.1/src/bifabrik/src/JsonSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/src/PandasDfSource.py` & `bifabrik-0.8.1/src/bifabrik/src/PandasDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/src/SharePointListSource.py` & `bifabrik-0.8.1/src/bifabrik/src/SharePointListSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/src/SparkDfSource.py` & `bifabrik-0.8.1/src/bifabrik/src/SparkDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/src/SparkSqlSource.py` & `bifabrik-0.8.1/src/bifabrik/src/SparkSqlSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/src/WarehouseSqlSource.py` & `bifabrik-0.8.1/src/bifabrik/src/WarehouseSqlSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/tsf/DataTransformation.py` & `bifabrik-0.8.1/src/bifabrik/tsf/DataTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/tsf/PandasDfTransformation.py` & `bifabrik-0.8.1/src/bifabrik/tsf/PandasDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/tsf/SparkDfTransformation.py` & `bifabrik-0.8.1/src/bifabrik/tsf/SparkDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/tsf/ValidationTransformation.py` & `bifabrik-0.8.1/src/bifabrik/tsf/ValidationTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/utils/fsUtils.py` & `bifabrik-0.8.1/src/bifabrik/utils/fsUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/utils/log.py` & `bifabrik-0.8.1/src/bifabrik/utils/log.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/utils/tableUtils.py` & `bifabrik-0.8.1/src/bifabrik/utils/tableUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/src/bifabrik/utils/tmslUtils.py` & `bifabrik-0.8.1/src/bifabrik/utils/tmslUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.8.0/PKG-INFO` & `bifabrik-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifabrik
-Version: 0.8.0
+Version: 0.8.1
 Summary: Microsoft Fabric ETL toolbox
 Home-page: https://rjankovic.github.io/bifabrik/
 License: MIT
 Author: Radovan Jankovič
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

