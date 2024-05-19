# Comparing `tmp/wwpdb.utils.oe_util-0.8.tar.gz` & `tmp/wwpdb_utils_oe_util-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.oe_util-0.8.tar", last modified: Sat Jun 17 11:32:17 2023, max compression
+gzip compressed data, was "wwpdb_utils_oe_util-0.8.1.tar", last modified: Sun May 19 11:44:17 2024, max compression
```

## Comparing `wwpdb.utils.oe_util-0.8.tar` & `wwpdb_utils_oe_util-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/
--rw-r--r--   0 vsts      (1001) docker     (123)      730 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1222 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2397 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.393557 wwpdb.utils.oe_util-0.8/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.393557 wwpdb.utils.oe_util-0.8/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.393557 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/
--rw-r--r--   0 vsts      (1001) docker     (123)      149 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/
--rw-r--r--   0 vsts      (1001) docker     (123)    10746 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeBuildModelMol.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19744 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeBuildMol.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4150 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeChemCompIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1366 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeDescriptorUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16791 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OePersist.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14062 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/PdbxBuildChemComp.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/
--rw-r--r--   0 vsts      (1001) docker     (123)    28515 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeAlignDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    45990 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeAlignDepictUtils.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     9099 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2719 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/modMCSAlign.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3373 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/simple-example.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.393557 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      730 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      931 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-17 11:31:45.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 11:44:17.649416 wwpdb_utils_oe_util-0.8.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1067 2024-05-19 11:44:17.649416 wwpdb_utils_oe_util-0.8.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-19 11:44:17.649416 wwpdb_utils_oe_util-0.8.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2397 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 11:44:17.645415 wwpdb_utils_oe_util-0.8.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 11:44:17.645415 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 11:44:17.645415 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/
+-rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 11:44:17.649416 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10746 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OeBuildModelMol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19744 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OeBuildMol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4150 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OeChemCompIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1366 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OeDescriptorUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16791 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OePersist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/PdbxBuildChemComp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 11:44:17.649416 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/
+-rw-r--r--   0 vsts      (1001) docker     (127)    28515 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/OeAlignDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45990 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/OeAlignDepictUtils.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     9099 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/OeDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2719 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/modMCSAlign.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3373 2024-05-19 11:42:46.000000 wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/simple-example.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 11:44:17.649416 wwpdb_utils_oe_util-0.8.1/wwpdb.utils.oe_util.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1067 2024-05-19 11:44:17.000000 wwpdb_utils_oe_util-0.8.1/wwpdb.utils.oe_util.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-19 11:44:17.000000 wwpdb_utils_oe_util-0.8.1/wwpdb.utils.oe_util.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-19 11:44:17.000000 wwpdb_utils_oe_util-0.8.1/wwpdb.utils.oe_util.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-19 11:43:50.000000 wwpdb_utils_oe_util-0.8.1/wwpdb.utils.oe_util.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      233 2024-05-19 11:44:17.000000 wwpdb_utils_oe_util-0.8.1/wwpdb.utils.oe_util.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-19 11:44:17.000000 wwpdb_utils_oe_util-0.8.1/wwpdb.utils.oe_util.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.oe_util-0.8/README.md` & `wwpdb_utils_oe_util-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/setup.py` & `wwpdb_utils_oe_util-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeBuildModelMol.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OeBuildModelMol.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeBuildMol.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OeBuildMol.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeChemCompIoUtils.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OeChemCompIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeDescriptorUtils.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OeDescriptorUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OePersist.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/OePersist.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/PdbxBuildChemComp.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/build/PdbxBuildChemComp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeAlignDepict.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/OeAlignDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeAlignDepictUtils.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/OeAlignDepictUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeDepict.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/OeDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/modMCSAlign.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/modMCSAlign.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/simple-example.py` & `wwpdb_utils_oe_util-0.8.1/wwpdb/utils/oe_util/oedepict/simple-example.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/SOURCES.txt` & `wwpdb_utils_oe_util-0.8.1/wwpdb.utils.oe_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

