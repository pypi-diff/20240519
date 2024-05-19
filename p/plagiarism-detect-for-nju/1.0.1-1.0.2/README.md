# Comparing `tmp/plagiarism_detect_for_nju-1.0.1.tar.gz` & `tmp/plagiarism_detect_for_nju-1.0.2.tar.gz`

## Comparing `plagiarism_detect_for_nju-1.0.1.tar` & `plagiarism_detect_for_nju-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/plagiarism_detect_for_nju/__init__.py
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/plagiarism_detect_for_nju/detect_from_logfile_batch.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/.gitignore
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/LICENSE
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/plagiarism_detect_for_nju/__init__.py
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/plagiarism_detect_for_nju/detect_from_logfile_batch.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/.gitignore
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11259 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/PKG-INFO
```

### Comparing `plagiarism_detect_for_nju-1.0.1/plagiarism_detect_for_nju/detect_from_logfile_batch.py` & `plagiarism_detect_for_nju-1.0.2/plagiarism_detect_for_nju/detect_from_logfile_batch.py`

 * *Files identical despite different names*

### Comparing `plagiarism_detect_for_nju-1.0.1/LICENSE` & `plagiarism_detect_for_nju-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plagiarism_detect_for_nju-1.0.1/README.md` & `plagiarism_detect_for_nju-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 查重工具
 
 本工具可以根据从`hustoj`后台导出的竞赛log文件, 自动分离出每个人的最后一次ac提交并存储, 之后使用`jplag`查重.
 
 ## 用法
 
 ```text
-usage: detech_from_logfile_batch [-h] [-d DIR] [-s SUFFIX] [-a] [-o] [-r] [-p] [-n NTOKS] [-j JAR_PATH] log
+usage: plag4nju4cprog [-h] [-d DIR] [-s SUFFIX] [-a] [-o] [-r] [-p] [-n NTOKS] [-j JAR_PATH] log
 
 plagiarism detect from hustoj's logfile, multi-process
 
 positional arguments:
   log                   log file u want to cut
 
 options:
```

### Comparing `plagiarism_detect_for_nju-1.0.1/pyproject.toml` & `plagiarism_detect_for_nju-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "plagiarism_detect_for_nju"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{ name = 'UshioA', email = "shiosshio@outlook.com" }]
 description = "Plagiarism detection tool for C Programming Language course in Nanjing University using HUSTOJ as Online Judge. Makes my life easier."
 requires-python = ">=3.6"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `plagiarism_detect_for_nju-1.0.1/PKG-INFO` & `plagiarism_detect_for_nju-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: plagiarism_detect_for_nju
-Version: 1.0.1
+Version: 1.0.2
 Summary: Plagiarism detection tool for C Programming Language course in Nanjing University using HUSTOJ as Online Judge. Makes my life easier.
 Author-email: UshioA <shiosshio@outlook.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -179,15 +179,15 @@
 # 查重工具
 
 本工具可以根据从`hustoj`后台导出的竞赛log文件, 自动分离出每个人的最后一次ac提交并存储, 之后使用`jplag`查重.
 
 ## 用法
 
 ```text
-usage: detech_from_logfile_batch [-h] [-d DIR] [-s SUFFIX] [-a] [-o] [-r] [-p] [-n NTOKS] [-j JAR_PATH] log
+usage: plag4nju4cprog [-h] [-d DIR] [-s SUFFIX] [-a] [-o] [-r] [-p] [-n NTOKS] [-j JAR_PATH] log
 
 plagiarism detect from hustoj's logfile, multi-process
 
 positional arguments:
   log                   log file u want to cut
 
 options:
```

