# Comparing `tmp/plagiarism_detect_for_nju-1.0.2.tar.gz` & `tmp/plagiarism_detect_for_nju-1.0.3.tar.gz`

## Comparing `plagiarism_detect_for_nju-1.0.2.tar` & `plagiarism_detect_for_nju-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/plagiarism_detect_for_nju/__init__.py
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/plagiarism_detect_for_nju/detect_from_logfile_batch.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/.gitignore
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/LICENSE
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    11259 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.3/plagiarism_detect_for_nju/__init__.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.3/plagiarism_detect_for_nju/detect_from_logfile_batch.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.3/.gitignore
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.3/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.3/PKG-INFO
```

### Comparing `plagiarism_detect_for_nju-1.0.2/plagiarism_detect_for_nju/detect_from_logfile_batch.py` & `plagiarism_detect_for_nju-1.0.3/plagiarism_detect_for_nju/detect_from_logfile_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 
 def main():
   parser = argparse.ArgumentParser(
       prog="plag4nju4cprog", description="plagiarism detect from hustoj's logfile, multi-process")
   parser.add_argument('log', type=str, action="store",
                       help='log file u want to cut')
   parser.add_argument('-d', '--dir', type=str, default=None,
-                      help='target directory u want to place the cut files in, default to the same name as the log file')
+                      help='target directory u want to place the cut files in. default to the same name as the log file')
   parser.add_argument('-s', '--suffix', type=str,
-                      default=None, help='suffix you want to add')
+                      default=None, help='suffix you want to add. i have no idea what this will do.')
   parser.add_argument('-a', '--all', help='whether to include all pairs in result',
                       action='store_true', default=False)
   parser.add_argument("-o", "--old", default=False,
                       action='store_true', help="use old method for cpp code")
   parser.add_argument('-r', '--remove', action='store_true',
                       default=False, help='remove existing directory if set to true')
   parser.add_argument('-p', "--parallel", action="store_true",
                       default=False, help='turn on to parallel')
   parser.add_argument('-n', '--ntoks', type=int, default=100,
-                      help='how many identical tokens will be recognized as copy. higher means more tolerant')
+                      help='how many identical tokens will be recognized as copy. higher means more tolerant. default to -1')
   parser.add_argument('-j', '--jar_path', type=str,
-                      default='./jplag.jar', help='where jplag jar is. u need to manage java environment yourself')
+                      default='./jplag.jar', help='where jplag jar is. u need to manage java environment yourself. default to "./jplag.jar"')
   args = parser.parse_args()
   logfile = args.log
   directory = args.dir
   include_all = args.all
   if args.suffix:
     global suffix
     suffix = args.suffix
```

### Comparing `plagiarism_detect_for_nju-1.0.2/LICENSE` & `plagiarism_detect_for_nju-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plagiarism_detect_for_nju-1.0.2/README.md` & `plagiarism_detect_for_nju-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 plagiarism detect from hustoj's logfile, multi-process
 
 positional arguments:
   log                   log file u want to cut
 
 options:
   -h, --help            show this help message and exit
-  -d DIR, --dir DIR     target directory u want to place the cut files in, default to the same name as the log file
+  -d DIR, --dir DIR     target directory u want to place the cut files in. default to the same name as the log file
   -s SUFFIX, --suffix SUFFIX
-                        suffix you want to add
+                        suffix you want to add. i have no idea what this will do.
   -a, --all             whether to include all pairs in result
   -o, --old             use old method for cpp code
   -r, --remove          remove existing directory if set to true
   -p, --parallel        turn on to parallel
   -n NTOKS, --ntoks NTOKS
-                        how many identical tokens will be recognized as copy. higher means more tolerant
+                        how many identical tokens will be recognized as copy. higher means more tolerant. default to -1
   -j JAR_PATH, --jar_path JAR_PATH
-                        where jplag jar is. u need to manage java environment yourself
+                        where jplag jar is. u need to manage java environment yourself. default to "./jplag.jar"
 ```
 
 ## JPlag
 
 jplag仓库: [jplag](https://github.com/jplag/JPlag).
 
 需要自己下载。作者自己用4.3.0测试过，更新的版本需要自己测试。
```

### Comparing `plagiarism_detect_for_nju-1.0.2/pyproject.toml` & `plagiarism_detect_for_nju-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "plagiarism_detect_for_nju"
-version = "1.0.2"
+version = "1.0.3"
 authors = [{ name = 'UshioA', email = "shiosshio@outlook.com" }]
 description = "Plagiarism detection tool for C Programming Language course in Nanjing University using HUSTOJ as Online Judge. Makes my life easier."
 requires-python = ">=3.6"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `plagiarism_detect_for_nju-1.0.2/PKG-INFO` & `plagiarism_detect_for_nju-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: plagiarism_detect_for_nju
-Version: 1.0.2
+Version: 1.0.3
 Summary: Plagiarism detection tool for C Programming Language course in Nanjing University using HUSTOJ as Online Judge. Makes my life easier.
 Author-email: UshioA <shiosshio@outlook.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -188,25 +188,25 @@
 plagiarism detect from hustoj's logfile, multi-process
 
 positional arguments:
   log                   log file u want to cut
 
 options:
   -h, --help            show this help message and exit
-  -d DIR, --dir DIR     target directory u want to place the cut files in, default to the same name as the log file
+  -d DIR, --dir DIR     target directory u want to place the cut files in. default to the same name as the log file
   -s SUFFIX, --suffix SUFFIX
-                        suffix you want to add
+                        suffix you want to add. i have no idea what this will do.
   -a, --all             whether to include all pairs in result
   -o, --old             use old method for cpp code
   -r, --remove          remove existing directory if set to true
   -p, --parallel        turn on to parallel
   -n NTOKS, --ntoks NTOKS
-                        how many identical tokens will be recognized as copy. higher means more tolerant
+                        how many identical tokens will be recognized as copy. higher means more tolerant. default to -1
   -j JAR_PATH, --jar_path JAR_PATH
-                        where jplag jar is. u need to manage java environment yourself
+                        where jplag jar is. u need to manage java environment yourself. default to "./jplag.jar"
 ```
 
 ## JPlag
 
 jplag仓库: [jplag](https://github.com/jplag/JPlag).
 
 需要自己下载。作者自己用4.3.0测试过，更新的版本需要自己测试。
```

