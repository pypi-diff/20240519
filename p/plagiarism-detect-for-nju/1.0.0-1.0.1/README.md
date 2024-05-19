# Comparing `tmp/plagiarism_detect_for_nju-1.0.0.tar.gz` & `tmp/plagiarism_detect_for_nju-1.0.1.tar.gz`

## Comparing `plagiarism_detect_for_nju-1.0.0.tar` & `plagiarism_detect_for_nju-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.0/plagiarism_detect_for_nju/__init__.py
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.0/plagiarism_detect_for_nju/detect_from_logfile_batch.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.0/.gitignore
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.0/LICENSE
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.0/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11223 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/plagiarism_detect_for_nju/__init__.py
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/plagiarism_detect_for_nju/detect_from_logfile_batch.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/.gitignore
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 plagiarism_detect_for_nju-1.0.1/PKG-INFO
```

### Comparing `plagiarism_detect_for_nju-1.0.0/plagiarism_detect_for_nju/detect_from_logfile_batch.py` & `plagiarism_detect_for_nju-1.0.1/plagiarism_detect_for_nju/detect_from_logfile_batch.py`

 * *Files identical despite different names*

### Comparing `plagiarism_detect_for_nju-1.0.0/LICENSE` & `plagiarism_detect_for_nju-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plagiarism_detect_for_nju-1.0.0/README.md` & `plagiarism_detect_for_nju-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,14 @@
                         where jplag jar is. u need to manage java environment yourself
 ```
 
 ## JPlag
 
 jplag仓库: [jplag](https://github.com/jplag/JPlag).
 
-直接下载了一份, 需要java17运行.
+需要自己下载。作者自己用4.3.0测试过，更新的版本需要自己测试。
 
 ## 怎么看报告
 
 运行后会首先创建文件夹存储切分出来的代码文件, 在这个文件夹下随后会产生一个`results-%dtoks`的文件夹, 名字的意思是在`%d`的敏感度下查重的结果. 文件夹里面会有若干个以题目编号为名字的`zip`格式文件, 每个代表那一题的查重结果.
 
 访问[这个网站](https://jplag.github.io/JPlag/), 把`zip`文件拖进去就可以看查重结果了.
```

### Comparing `plagiarism_detect_for_nju-1.0.0/PKG-INFO` & `plagiarism_detect_for_nju-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: plagiarism_detect_for_nju
-Version: 1.0.0
+Version: 1.0.1
 Summary: Plagiarism detection tool for C Programming Language course in Nanjing University using HUSTOJ as Online Judge. Makes my life easier.
 Author-email: UshioA <shiosshio@outlook.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -205,14 +205,14 @@
                         where jplag jar is. u need to manage java environment yourself
 ```
 
 ## JPlag
 
 jplag仓库: [jplag](https://github.com/jplag/JPlag).
 
-直接下载了一份, 需要java17运行.
+需要自己下载。作者自己用4.3.0测试过，更新的版本需要自己测试。
 
 ## 怎么看报告
 
 运行后会首先创建文件夹存储切分出来的代码文件, 在这个文件夹下随后会产生一个`results-%dtoks`的文件夹, 名字的意思是在`%d`的敏感度下查重的结果. 文件夹里面会有若干个以题目编号为名字的`zip`格式文件, 每个代表那一题的查重结果.
 
 访问[这个网站](https://jplag.github.io/JPlag/), 把`zip`文件拖进去就可以看查重结果了.
```

