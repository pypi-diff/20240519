# Comparing `tmp/am2r_yams-2.1.2.tar.gz` & `tmp/am2r_yams-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "am2r_yams-2.1.2.tar", last modified: Mon May 13 16:24:21 2024, max compression
+gzip compressed data, was "am2r_yams-2.2.0.tar", last modified: Sun May 19 17:38:59 2024, max compression
```

## Comparing `am2r_yams-2.1.2.tar` & `am2r_yams-2.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.144720 am2r_yams-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 16:23:59.000000 am2r_yams-2.1.2/LICENSE-CODE
--rw-r--r--   0 runner    (1001) docker     (127)    42372 2024-05-13 16:24:21.144720 am2r_yams-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-13 16:23:59.000000 am2r_yams-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.132720 am2r_yams-2.1.2/am2r_yams/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-13 16:24:00.000000 am2r_yams-2.1.2/am2r_yams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.136720 am2r_yams-2.1.2/am2r_yams/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 16:24:00.000000 am2r_yams-2.1.2/am2r_yams/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 16:24:00.000000 am2r_yams-2.1.2/am2r_yams/__pyinstaller/hook-am2r_yams.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-13 16:24:00.000000 am2r_yams-2.1.2/am2r_yams/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.144720 am2r_yams-2.1.2/am2r_yams/yams/
--rwxr--r--   0 runner    (1001) docker     (127)   204800 2021-09-19 09:20:24.000000 am2r_yams-2.1.2/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
--rwxr--r--   0 runner    (1001) docker     (127)    42496 2022-06-15 03:36:02.000000 am2r_yams-2.1.2/am2r_yams/yams/Macross.Json.Extensions.dll
--rwxr--r--   0 runner    (1001) docker     (127)    27528 2020-10-19 18:40:26.000000 am2r_yams-2.1.2/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (127)    14336 2024-04-14 16:50:48.000000 am2r_yams-2.1.2/am2r_yams/yams/NaturalSort.Extension.dll
--rwxr--r--   0 runner    (1001) docker     (127)     6656 2021-03-13 10:51:42.000000 am2r_yams-2.1.2/am2r_yams/yams/PropertyChanged.dll
--rwxr--r--   0 runner    (1001) docker     (127)  2091520 2024-04-11 06:51:00.000000 am2r_yams-2.1.2/am2r_yams/yams/SixLabors.ImageSharp.dll
--rwxr--r--   0 runner    (1001) docker     (127)   173432 2021-10-22 20:57:42.000000 am2r_yams-2.1.2/am2r_yams/yams/System.Drawing.Common.dll
--rw-r--r--   0 runner    (1001) docker     (127)   947200 2024-05-13 16:24:16.000000 am2r_yams-2.1.2/am2r_yams/yams/UndertaleModLib.dll
--rw-r--r--   0 runner    (1001) docker     (127)   330863 2024-05-13 16:24:14.000000 am2r_yams-2.1.2/am2r_yams/yams/UndertaleModLib.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-13 16:24:18.000000 am2r_yams-2.1.2/am2r_yams/yams/YAMS-LIB.deps.json
--rw-r--r--   0 runner    (1001) docker     (127)   283648 2024-05-13 16:24:18.000000 am2r_yams-2.1.2/am2r_yams/yams/YAMS-LIB.dll
--rw-r--r--   0 runner    (1001) docker     (127)    29084 2024-05-13 16:24:18.000000 am2r_yams-2.1.2/am2r_yams/yams/YAMS-LIB.pdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.132720 am2r_yams-2.1.2/am2r_yams/yams/runtimes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.132720 am2r_yams-2.1.2/am2r_yams/yams/runtimes/unix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.132720 am2r_yams-2.1.2/am2r_yams/yams/runtimes/unix/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.144720 am2r_yams-2.1.2/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (127)   419720 2021-10-22 20:57:34.000000 am2r_yams-2.1.2/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.132720 am2r_yams-2.1.2/am2r_yams/yams/runtimes/win/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.132720 am2r_yams-2.1.2/am2r_yams/yams/runtimes/win/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.144720 am2r_yams-2.1.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (127)    52104 2020-10-19 18:52:12.000000 am2r_yams-2.1.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (127)   436600 2021-10-22 20:58:02.000000 am2r_yams-2.1.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.144720 am2r_yams-2.1.2/am2r_yams/yams/sprites/
--rw-r--r--   0 runner    (1001) docker     (127)   284547 2024-05-13 16:24:08.000000 am2r_yams-2.1.2/am2r_yams/yams/sprites/texturepage.png
--rw-r--r--   0 runner    (1001) docker     (127)    74598 2024-05-13 16:24:08.000000 am2r_yams-2.1.2/am2r_yams/yams/sprites/texturepageiteminfo.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:24:21.144720 am2r_yams-2.1.2/am2r_yams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42372 2024-05-13 16:24:21.000000 am2r_yams-2.1.2/am2r_yams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-13 16:24:21.000000 am2r_yams-2.1.2/am2r_yams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:24:21.000000 am2r_yams-2.1.2/am2r_yams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 16:24:21.000000 am2r_yams-2.1.2/am2r_yams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 16:24:21.000000 am2r_yams-2.1.2/am2r_yams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 16:24:21.000000 am2r_yams-2.1.2/am2r_yams.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 16:24:00.000000 am2r_yams-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:24:21.144720 am2r_yams-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.422862 am2r_yams-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 17:38:31.000000 am2r_yams-2.2.0/LICENSE-CODE
+-rw-r--r--   0 runner    (1001) docker     (127)    42372 2024-05-19 17:38:59.422862 am2r_yams-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-19 17:38:31.000000 am2r_yams-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.410862 am2r_yams-2.2.0/am2r_yams/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 17:38:32.000000 am2r_yams-2.2.0/am2r_yams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.410862 am2r_yams-2.2.0/am2r_yams/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-19 17:38:32.000000 am2r_yams-2.2.0/am2r_yams/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-19 17:38:32.000000 am2r_yams-2.2.0/am2r_yams/__pyinstaller/hook-am2r_yams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-19 17:38:32.000000 am2r_yams-2.2.0/am2r_yams/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.418862 am2r_yams-2.2.0/am2r_yams/yams/
+-rwxr--r--   0 runner    (1001) docker     (127)   204800 2021-09-19 09:20:24.000000 am2r_yams-2.2.0/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
+-rwxr--r--   0 runner    (1001) docker     (127)    42496 2022-06-15 03:36:02.000000 am2r_yams-2.2.0/am2r_yams/yams/Macross.Json.Extensions.dll
+-rwxr--r--   0 runner    (1001) docker     (127)    27528 2020-10-19 18:40:26.000000 am2r_yams-2.2.0/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (127)    14336 2024-04-14 16:50:48.000000 am2r_yams-2.2.0/am2r_yams/yams/NaturalSort.Extension.dll
+-rwxr--r--   0 runner    (1001) docker     (127)     6656 2021-03-13 10:51:42.000000 am2r_yams-2.2.0/am2r_yams/yams/PropertyChanged.dll
+-rwxr--r--   0 runner    (1001) docker     (127)  2091520 2024-04-11 06:51:00.000000 am2r_yams-2.2.0/am2r_yams/yams/SixLabors.ImageSharp.dll
+-rwxr--r--   0 runner    (1001) docker     (127)   173432 2021-10-22 20:57:42.000000 am2r_yams-2.2.0/am2r_yams/yams/System.Drawing.Common.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   947200 2024-05-19 17:38:53.000000 am2r_yams-2.2.0/am2r_yams/yams/UndertaleModLib.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   330863 2024-05-19 17:38:52.000000 am2r_yams-2.2.0/am2r_yams/yams/UndertaleModLib.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-19 17:38:56.000000 am2r_yams-2.2.0/am2r_yams/yams/YAMS-LIB.deps.json
+-rw-r--r--   0 runner    (1001) docker     (127)   303104 2024-05-19 17:38:56.000000 am2r_yams-2.2.0/am2r_yams/yams/YAMS-LIB.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    29376 2024-05-19 17:38:56.000000 am2r_yams-2.2.0/am2r_yams/yams/YAMS-LIB.pdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.406862 am2r_yams-2.2.0/am2r_yams/yams/runtimes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.406862 am2r_yams-2.2.0/am2r_yams/yams/runtimes/unix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.406862 am2r_yams-2.2.0/am2r_yams/yams/runtimes/unix/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.418862 am2r_yams-2.2.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (127)   419720 2021-10-22 20:57:34.000000 am2r_yams-2.2.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.406862 am2r_yams-2.2.0/am2r_yams/yams/runtimes/win/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.406862 am2r_yams-2.2.0/am2r_yams/yams/runtimes/win/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.418862 am2r_yams-2.2.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (127)    52104 2020-10-19 18:52:12.000000 am2r_yams-2.2.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (127)   436600 2021-10-22 20:58:02.000000 am2r_yams-2.2.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.418862 am2r_yams-2.2.0/am2r_yams/yams/sprites/
+-rw-r--r--   0 runner    (1001) docker     (127)   294678 2024-05-19 17:38:45.000000 am2r_yams-2.2.0/am2r_yams/yams/sprites/texturepage.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77784 2024-05-19 17:38:45.000000 am2r_yams-2.2.0/am2r_yams/yams/sprites/texturepageiteminfo.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:38:59.418862 am2r_yams-2.2.0/am2r_yams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42372 2024-05-19 17:38:59.000000 am2r_yams-2.2.0/am2r_yams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 17:38:59.000000 am2r_yams-2.2.0/am2r_yams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:38:59.000000 am2r_yams-2.2.0/am2r_yams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-19 17:38:59.000000 am2r_yams-2.2.0/am2r_yams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 17:38:59.000000 am2r_yams-2.2.0/am2r_yams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 17:38:59.000000 am2r_yams-2.2.0/am2r_yams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 17:38:32.000000 am2r_yams-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:38:59.422862 am2r_yams-2.2.0/setup.cfg
```

### Comparing `am2r_yams-2.1.2/LICENSE-CODE` & `am2r_yams-2.2.0/LICENSE-CODE`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/PKG-INFO` & `am2r_yams-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 2.1.2
+Version: 2.2.0
 Summary: An open source randomizer patcher for AM2R.
 Author: Miepee
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `am2r_yams-2.1.2/README.md` & `am2r_yams-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/wrapper.py` & `am2r_yams-2.2.0/am2r_yams/wrapper.py`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/ICSharpCode.SharpZipLib.dll` & `am2r_yams-2.2.0/am2r_yams/yams/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/Macross.Json.Extensions.dll` & `am2r_yams-2.2.0/am2r_yams/yams/Macross.Json.Extensions.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-2.2.0/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/NaturalSort.Extension.dll` & `am2r_yams-2.2.0/am2r_yams/yams/NaturalSort.Extension.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/PropertyChanged.dll` & `am2r_yams-2.2.0/am2r_yams/yams/PropertyChanged.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/SixLabors.ImageSharp.dll` & `am2r_yams-2.2.0/am2r_yams/yams/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/System.Drawing.Common.dll` & `am2r_yams-2.2.0/am2r_yams/yams/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/UndertaleModLib.dll` & `am2r_yams-2.2.0/am2r_yams/yams/UndertaleModLib.dll`

 * *Files 6% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xefaecfdf
+	             Time stamp: 0xc0f1daeb
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2102
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
 	              Code Size: 0x000e6c00
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x000e8ade
+	        Entry Point RVA: 0x000e8a8e
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00000000
 
 
 NT Header:
 	   Image Base (0x400000): 0x00400000
 	Section Alignment (8192): 0x00002000
@@ -41,31 +41,31 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x000e8a8c [0x0000004f]
+	     Import Table: 0x000e8a40 [0x0000004b]
 	   Resource Table: 0x000ea000 [0x000003b4]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x000ec000 [0x0000000c]
-	            Debug: 0x000d1e54 [0x00000054]
+	            Debug: 0x000d1e00 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x000e6ae4
+	   Virtual Size: 0x000e6a94
 	Virtual Address: 0x00002000
 	  Raw Data Size: 0x000e6c00
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
@@ -92,58 +92,58 @@
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0005bf94 [0x00075ec0]
+	         Metadata: 0x0005bf54 [0x00075eac]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0005bb98 [0x00000018]
+	     Resources at: 0x0005bb58 [0x00000018]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name: none
 
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x0002ae88 [175644 == 0x0002ae1c]
-	    Strings: 0x0002ae88 - 0x0003b5e4 [67420 == 0x0001075c]
-	       Blob: 0x0006e48c - 0x00075ec0 [31284 == 0x00007a34]
-	User string: 0x0003b5e4 - 0x0006e47c [208536 == 0x00032e98]
-	       GUID: 0x0006e47c - 0x0006e48c [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x0002ae80 [175636 == 0x0002ae14]
+	    Strings: 0x0002ae80 - 0x0003b5dc [67420 == 0x0001075c]
+	       Blob: 0x0006e484 - 0x00075eac [31272 == 0x00007a28]
+	User string: 0x0003b5dc - 0x0006e474 [208536 == 0x00032e98]
+	       GUID: 0x0006e474 - 0x0006e484 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (12 bytes, at 5a288)
-Table TypeRef: 206 records (10 bytes, at 5a294)
-Table TypeDef: 437 records (18 bytes, at 5aaa0)
-Table Field: 2714 records (8 bytes, at 5c95a)
-Table Method: 3582 records (16 bytes, at 61e2a)
-Table Param: 2600 records (8 bytes, at 6fe0a)
-Table InterfaceImpl: 394 records (4 bytes, at 74f4a)
-Table MemberRef: 1672 records (8 bytes, at 75572)
-Table Constant: 1122 records (6 bytes, at 789b2)
-Table CustomAttribute: 2309 records (8 bytes, at 7a3fe)
-Table DeclSecurity: 1 records (6 bytes, at 7ec26)
-Table ClassLayout: 14 records (8 bytes, at 7ec2c)
-Table StandaloneSig: 357 records (2 bytes, at 7ec9c)
-Table EventMap: 84 records (4 bytes, at 7ef66)
-Table Event: 84 records (8 bytes, at 7f0b6)
-Table PropertyMap: 171 records (4 bytes, at 7f356)
-Table Property: 931 records (8 bytes, at 7f602)
-Table MethodSemantics: 1846 records (6 bytes, at 8131a)
-Table MethodImpl: 4 records (6 bytes, at 83e5e)
-Table TypeSpec: 502 records (2 bytes, at 83e76)
-Table FieldRVA: 26 records (6 bytes, at 84262)
-Table Assembly: 1 records (26 bytes, at 842fe)
-Table AssemblyRef: 18 records (24 bytes, at 84318)
-Table ManifestResource: 1 records (14 bytes, at 844c8)
-Table NestedClass: 220 records (4 bytes, at 844d6)
-Table GenericParam: 31 records (10 bytes, at 84846)
-Table MethodSpec: 394 records (4 bytes, at 8497c)
-Table GenericParamConstraint: 30 records (4 bytes, at 84fa4)
+Table Module: 1 records (12 bytes, at 5a248)
+Table TypeRef: 206 records (10 bytes, at 5a254)
+Table TypeDef: 437 records (18 bytes, at 5aa60)
+Table Field: 2714 records (8 bytes, at 5c91a)
+Table Method: 3582 records (16 bytes, at 61dea)
+Table Param: 2600 records (8 bytes, at 6fdca)
+Table InterfaceImpl: 394 records (4 bytes, at 74f0a)
+Table MemberRef: 1671 records (8 bytes, at 75532)
+Table Constant: 1122 records (6 bytes, at 7896a)
+Table CustomAttribute: 2309 records (8 bytes, at 7a3b6)
+Table DeclSecurity: 1 records (6 bytes, at 7ebde)
+Table ClassLayout: 14 records (8 bytes, at 7ebe4)
+Table StandaloneSig: 357 records (2 bytes, at 7ec54)
+Table EventMap: 84 records (4 bytes, at 7ef1e)
+Table Event: 84 records (8 bytes, at 7f06e)
+Table PropertyMap: 171 records (4 bytes, at 7f30e)
+Table Property: 931 records (8 bytes, at 7f5ba)
+Table MethodSemantics: 1846 records (6 bytes, at 812d2)
+Table MethodImpl: 4 records (6 bytes, at 83e16)
+Table TypeSpec: 502 records (2 bytes, at 83e2e)
+Table FieldRVA: 26 records (6 bytes, at 8421a)
+Table Assembly: 1 records (26 bytes, at 842b6)
+Table AssemblyRef: 18 records (24 bytes, at 842d0)
+Table ManifestResource: 1 records (14 bytes, at 84480)
+Table NestedClass: 220 records (4 bytes, at 8448e)
+Table GenericParam: 31 records (10 bytes, at 847fe)
+Table MethodSpec: 394 records (4 bytes, at 84934)
+Table GenericParamConstraint: 30 records (4 bytes, at 84f5c)
```

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/UndertaleModLib.xml` & `am2r_yams-2.2.0/am2r_yams/yams/UndertaleModLib.xml`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/YAMS-LIB.deps.json` & `am2r_yams-2.2.0/am2r_yams/yams/YAMS-LIB.deps.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'libraries'": "{'YAMS-LIB/2.2.0': OrderedDict([('type', 'project'), ('serviceable', False), "*

 * *                "('sha512', '')]), delete: ['YAMS-LIB/2.1.2']}",*

 * * "'targets'": "{'.NETCoreApp,Version=v6.0': {'YAMS-LIB/2.2.0': OrderedDict([('dependencies', "*

 * *              "OrderedDict([('Macross.Json.Extensions', '3.0.0'), ('NaturalSort.Extension', "*

 * *              "'4.3.0'), ('SixLabors.ImageSharp', '3.1.4'), ('UndertaleModLib', '1.0.0')])), "*

 * *              "('runtime', OrderedDict([('YAMS-LIB.dll', OrderedDic […]*

```diff
@@ -65,15 +65,15 @@
             "type": "package"
         },
         "UndertaleModLib/1.0.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
-        "YAMS-LIB/2.1.2": {
+        "YAMS-LIB/2.2.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         }
     },
     "runtimeTarget": {
         "name": ".NETCoreApp,Version=v6.0",
@@ -174,15 +174,15 @@
                     "SharpZipLib": "1.3.3",
                     "System.Drawing.Common": "5.0.3"
                 },
                 "runtime": {
                     "UndertaleModLib.dll": {}
                 }
             },
-            "YAMS-LIB/2.1.2": {
+            "YAMS-LIB/2.2.0": {
                 "dependencies": {
                     "Macross.Json.Extensions": "3.0.0",
                     "NaturalSort.Extension": "4.3.0",
                     "SixLabors.ImageSharp": "3.1.4",
                     "UndertaleModLib": "1.0.0"
                 },
                 "runtime": {
```

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/YAMS-LIB.dll` & `am2r_yams-2.2.0/am2r_yams/yams/YAMS-LIB.dll`

 * *Files 2% similar despite different names*

#### pedump {}

```diff
@@ -1,106 +1,106 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xfaa3cd87
+	             Time stamp: 0x98f5b476
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x00044c00
+	              Code Size: 0x00049800
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x00046b8e
+	        Entry Point RVA: 0x0004b6d6
 	 	  Code Base RVA: 0x00002000
-		  Data Base RVA: 0x00048000
+		  Data Base RVA: 0x0004c000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
 	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
-	 	      Image Size: 0x0004c000
+	 	      Image Size: 0x00050000
 	 	     Header Size: 0x00000200
 	            Checksum (0): 0x00000000
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x00046b3c [0x0000004f]
-	   Resource Table: 0x00048000 [0x00000370]
+	     Import Table: 0x0004b684 [0x0000004f]
+	   Resource Table: 0x0004c000 [0x00000370]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
-	      Reloc Table: 0x0004a000 [0x0000000c]
-	            Debug: 0x00046a64 [0x00000054]
+	      Reloc Table: 0x0004e000 [0x0000000c]
+	            Debug: 0x0004b5ac [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00044bc0
+	   Virtual Size: 0x00049708
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x00044c00
+	  Raw Data Size: 0x00049800
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x00000370
-	Virtual Address: 0x00048000
+	Virtual Address: 0x0004c000
 	  Raw Data Size: 0x00000400
-	   Raw Data Ptr: 0x00044e00
+	   Raw Data Ptr: 0x00049a00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
-	Virtual Address: 0x0004a000
+	Virtual Address: 0x0004e000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x00045200
+	   Raw Data Ptr: 0x00049e00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0000f220 [0x00037844]
+	         Metadata: 0x0000f504 [0x0003c0a8]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
@@ -109,32 +109,32 @@
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x00002cc8 [11356 == 0x00002c5c]
-	    Strings: 0x00002cc8 - 0x00004e94 [8652 == 0x000021cc]
-	       Blob: 0x0003542c - 0x00037844 [9240 == 0x00002418]
-	User string: 0x00004e94 - 0x0003541c [198024 == 0x00030588]
-	       GUID: 0x0003541c - 0x0003542c [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x00002d1c [11440 == 0x00002cb0]
+	    Strings: 0x00002d1c - 0x00004f00 [8676 == 0x000021e4]
+	       Blob: 0x00039c70 - 0x0003c0a8 [9272 == 0x00002438]
+	User string: 0x00004f00 - 0x00039c60 [216416 == 0x00034d60]
+	       GUID: 0x00039c60 - 0x00039c70 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at d4f0)
-Table TypeRef: 128 records (6 bytes, at d4fa)
-Table TypeDef: 48 records (14 bytes, at d7fa)
-Table Field: 267 records (6 bytes, at da9a)
-Table Method: 103 records (14 bytes, at e0dc)
-Table Param: 109 records (6 bytes, at e67e)
-Table MemberRef: 348 records (6 bytes, at e90c)
-Table Constant: 145 records (6 bytes, at f134)
-Table CustomAttribute: 424 records (6 bytes, at f49a)
-Table ClassLayout: 1 records (8 bytes, at fe8a)
-Table StandaloneSig: 21 records (2 bytes, at fe92)
-Table TypeSpec: 67 records (2 bytes, at febc)
-Table FieldRVA: 1 records (6 bytes, at ff42)
-Table Assembly: 1 records (22 bytes, at ff48)
-Table AssemblyRef: 11 records (20 bytes, at ff5e)
-Table NestedClass: 11 records (4 bytes, at 1003a)
-Table GenericParam: 2 records (8 bytes, at 10066)
-Table MethodSpec: 26 records (4 bytes, at 10076)
-Table GenericParamConstraint: 2 records (4 bytes, at 100de)
+Table Module: 1 records (10 bytes, at d7d4)
+Table TypeRef: 128 records (6 bytes, at d7de)
+Table TypeDef: 49 records (14 bytes, at dade)
+Table Field: 268 records (6 bytes, at dd8c)
+Table Method: 105 records (14 bytes, at e3d4)
+Table Param: 112 records (6 bytes, at e992)
+Table MemberRef: 348 records (6 bytes, at ec32)
+Table Constant: 146 records (6 bytes, at f45a)
+Table CustomAttribute: 426 records (6 bytes, at f7c6)
+Table ClassLayout: 1 records (8 bytes, at 101c2)
+Table StandaloneSig: 21 records (2 bytes, at 101ca)
+Table TypeSpec: 67 records (2 bytes, at 101f4)
+Table FieldRVA: 1 records (6 bytes, at 1027a)
+Table Assembly: 1 records (22 bytes, at 10280)
+Table AssemblyRef: 11 records (20 bytes, at 10296)
+Table NestedClass: 11 records (4 bytes, at 10372)
+Table GenericParam: 2 records (8 bytes, at 1039e)
+Table MethodSpec: 26 records (4 bytes, at 103ae)
+Table GenericParamConstraint: 2 records (4 bytes, at 10416)
```

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/YAMS-LIB.pdb` & `am2r_yams-2.2.0/am2r_yams/yams/YAMS-LIB.pdb`

 * *Files 12% similar despite different names*

```diff
@@ -1,1818 +1,1836 @@
 00000000: 4253 4a42 0100 0100 0000 0000 0c00 0000  BSJB............
 00000010: 5044 4220 7631 2e30 0000 0000 0000 0600  PDB v1.0........
 00000020: 7c00 0000 6c00 0000 2350 6462 0000 0000  |...l...#Pdb....
-00000030: e800 0000 2411 0000 237e 0000 0c12 0000  ....$...#~......
-00000040: 0808 0000 2353 7472 696e 6773 0000 0000  ....#Strings....
-00000050: 141a 0000 0400 0000 2355 5300 181a 0000  ........#US.....
-00000060: 7000 0000 2347 5549 4400 0000 881a 0000  p...#GUID.......
-00000070: 1457 0000 2342 6c6f 6200 0000 1705 ce6f  .W..#Blob......o
-00000080: c6d8 194b b355 9f14 96f4 edd0 2b11 e0f4  ...K.U......+...
+00000030: e800 0000 7011 0000 237e 0000 5812 0000  ....p...#~..X...
+00000040: 1408 0000 2353 7472 696e 6773 0000 0000  ....#Strings....
+00000050: 6c1a 0000 0400 0000 2355 5300 701a 0000  l.......#US.p...
+00000060: 7000 0000 2347 5549 4400 0000 e01a 0000  p...#GUID.......
+00000070: e057 0000 2342 6c6f 6200 0000 b004 40b9  .W..#Blob.....@.
+00000080: aa5b 0848 8ec7 7948 da7d 505c bf02 57c5  .[.H..yH.}P\..W.
 00000090: 0000 0000 579d 0228 091e 0000 0100 0000  ....W..(........
-000000a0: 8000 0000 3000 0000 0b01 0000 6700 0000  ....0.......g...
-000000b0: 6d00 0000 5c01 0000 9100 0000 a801 0000  m...\...........
+000000a0: 8000 0000 3100 0000 0c01 0000 6900 0000  ....1.......i...
+000000b0: 7000 0000 5c01 0000 9200 0000 aa01 0000  p...\...........
 000000c0: 0100 0000 1500 0000 4300 0000 0100 0000  ........C.......
 000000d0: 0100 0000 0b00 0000 0b00 0000 0200 0000  ................
 000000e0: 1a00 0000 0200 0000 0000 0000 0200 0001  ................
 000000f0: 0000 0000 0000 bf00 0000 0000 0000 8400  ................
-00000100: 1200 0000 6700 0000 9300 0000 c200 0000  ....g...........
+00000100: 1300 0000 6900 0000 9600 0000 c400 0000  ....i...........
 00000110: 0700 0000 2400 0000 0f00 0000 2e00 0100  ....$...........
 00000120: 3800 0200 6d00 0100 7700 0200 a800 0100  8...m...w.......
 00000130: b300 0200 e000 0100 eb00 0200 2601 0100  ............&...
-00000140: 3301 0200 6301 0100 7001 0200 a201 0100  3...c...p.......
-00000150: af01 0200 de01 0100 eb01 0200 2802 0100  ............(...
-00000160: 3702 0200 7102 0100 8002 0200 b702 0100  7...q...........
-00000170: c602 0200 0103 0100 1003 0200 3c03 0100  ............<...
-00000180: 4903 0200 7503 0100 8003 0200 af03 0100  I...u...........
-00000190: ba03 0200 0904 0100 1a04 0200 db04 0100  ................
-000001a0: ec04 0200 f105 0100 0206 0200 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001c0: 0100 be2e 0100 502f 0100 5c2f 0200 682f  ......P/..\/..h/
-000001d0: 0200 0f30 0200 1630 0200 4030 0200 5630  ...0...0..@0..V0
-000001e0: 0200 6c30 0200 7830 0200 8430 0200 9030  ..l0..x0...0...0
-000001f0: 0200 9a30 0300 e230 0000 0000 0400 a331  ...0...0.......1
-00000200: 0e00 e231 0e00 3133 0000 0000 0e00 3947  ...1..13......9G
-00000210: 0f00 4047 0000 0000 0f00 a547 0f00 ad47  ..@G.......G...G
-00000220: 0f00 ba47 0000 0000 0000 0000 0f00 d647  ...G...........G
-00000230: 0f00 de47 0f00 eb47 0f00 fd47 0500 0548  ...G...G...G...H
-00000240: 0500 4748 0500 f248 0000 0000 0600 0449  ..GH...H.......I
-00000250: 0600 6149 0000 0000 0700 cc49 0000 0000  ..aI.......I....
-00000260: 0800 6b4d 0000 0000 0d00 264e 0000 0000  ..kM......&N....
-00000270: 0d00 7553 0d00 ad53 0900 ba53 0000 0000  ..uS...S...S....
-00000280: 0a00 2155 0000 0000 0b00 9f55 0000 0000  ..!U.......U....
-00000290: 0c00 c855 0000 0000 0000 0000 0200 1456  ...U...........V
-000002a0: 0000 0000 0000 0000 0e00 1b56 0e00 2356  ...........V..#V
-000002b0: 0e00 2b56 0e00 3356 0e00 3b56 0e00 4356  ..+V..3V..;V..CV
-000002c0: 0e00 4b56 0e00 5356 0e00 5b56 0e00 6456  ..KV..SV..[V..dV
-000002d0: 0e00 6c56 0e00 7456 0e00 7d56 0e00 8556  ..lV..tV..}V...V
-000002e0: 0e00 8d56 0e00 9556 0e00 9d56 0e00 a556  ...V...V...V...V
-000002f0: 0e00 ad56 0e00 b556 0000 0000 0e00 bd56  ...V...V.......V
-00000300: 0e00 c556 0000 0000 0600 cd56 0000 0000  ...V.......V....
-00000310: 0000 0000 0700 d456 0700 db56 0000 0000  .......V...V....
-00000320: 0700 e356 0700 ea56 0000 0000 0000 0000  ...V...V........
-00000330: 0d00 f156 0000 0000 0d00 f856 0d00 ff56  ...V.......V...V
-00000340: 0d00 0657 0d00 0d57 0600 0300 0100 0100  ...W...W........
-00000350: 0000 0000 0700 0000 0700 0300 0100 0100  ................
-00000360: 0000 0000 0800 0000 0800 0300 0100 0100  ................
-00000370: 0000 0000 0900 0000 0900 0500 0100 0100  ................
-00000380: 0000 0000 1500 0000 0a00 0500 0100 0100  ................
-00000390: 0000 0000 0d00 0000 0b00 0500 0100 0100  ................
-000003a0: 0000 0000 8500 0000 0c00 0500 0200 0100  ................
-000003b0: 0000 0000 2700 0000 0d00 0500 0300 0100  ....'...........
-000003c0: 0000 0000 2700 0000 0e00 0500 0400 0100  ....'...........
-000003d0: 0000 0000 0d00 0000 0f00 0500 0400 0100  ................
-000003e0: 0000 0000 8300 0000 1000 0500 0400 0100  ................
-000003f0: 0000 0000 7500 0000 1100 0500 0400 0100  ....u...........
-00000400: 0000 0000 4a00 0000 1200 0500 0500 0100  ....J...........
-00000410: 0000 0000 d000 0000 1300 0700 0900 0100  ................
-00000420: 0000 0000 8901 0000 1300 0700 0a00 0100  ................
-00000430: c900 0000 5900 0000 1300 0700 0c00 0100  ....Y...........
-00000440: 4b01 0000 3300 0000 1300 0700 0d00 0100  K...3...........
-00000450: 5001 0000 2e00 0000 1500 0900 0e00 0100  P...............
-00000460: 0000 0000 1200 0000 1600 0b00 0e00 0100  ................
-00000470: 0000 0000 6900 0000 1700 0b00 0f00 0100  ....i...........
-00000480: 0000 0000 7068 0000 1700 0b00 3800 0800  ....ph......8...
-00000490: 2700 0000 2a00 0000 1700 0b00 3900 0800  '...*.......9...
-000004a0: 5105 0000 4b00 0000 1700 0b00 3a00 0800  Q...K.......:...
-000004b0: f006 0000 2300 0000 1700 0b00 3b00 0800  ....#.......;...
-000004c0: a209 0000 2300 0000 1700 0b00 3c00 0800  ....#.......<...
-000004d0: 2d0b 0000 2600 0000 1700 0b00 3d00 0800  -...&.......=...
-000004e0: a60b 0000 4500 0000 1700 0b00 3e00 0800  ....E.......>...
-000004f0: 7f0c 0000 4500 0000 1700 0b00 3f00 0800  ....E.......?...
-00000500: 230e 0000 2900 0000 1700 0b00 4000 0800  #...).......@...
-00000510: 4312 0000 c401 0000 1700 0b00 4100 0800  C...........A...
-00000520: 4f12 0000 a601 0000 1700 0b00 4600 0800  O...........F...
-00000530: 3315 0000 2900 0000 1700 0b00 4700 0800  3...).......G...
-00000540: a715 0000 6000 0000 1700 0b00 4800 0800  ....`.......H...
-00000550: ae15 0000 5900 0000 1700 0b00 4900 0800  ....Y.......I...
-00000560: 5d17 0000 890e 0000 1700 0b00 5600 0800  ]...........V...
-00000570: 5d2f 0000 2900 0000 1700 0b00 5700 0800  ]/..).......W...
-00000580: 4d32 0000 2900 0000 1700 0b00 5800 0800  M2..).......X...
-00000590: 5834 0000 2900 0000 1700 0b00 5900 0800  X4..).......Y...
-000005a0: 3f35 0000 2900 0000 1700 0b00 5a00 0800  ?5..).......Z...
-000005b0: 0236 0000 2900 0000 1700 0b00 5b00 0800  .6..).......[...
-000005c0: 5e3c 0000 2900 0000 1700 0b00 5c00 0800  ^<..).......\...
-000005d0: da3d 0000 ac09 0000 1700 0b00 5e00 0800  .=..........^...
-000005e0: f63d 0000 9009 0000 1700 0b00 5f00 0800  .=.........._...
-000005f0: fa3d 0000 3909 0000 1700 0b00 6500 0800  .=..9.......e...
-00000600: 2341 0000 3700 0000 1700 0b00 6600 0800  #A..7.......f...
-00000610: c44f 0000 7107 0000 1700 0b00 6800 0800  .O..q.......h...
-00000620: e04f 0000 5507 0000 1700 0b00 6b00 0800  .O..U.......k...
-00000630: 0754 0000 2200 0000 1700 0b00 6c00 0800  .T..".......l...
-00000640: 045b 0000 2300 0000 1700 0b00 6d00 0800  .[..#.......m...
-00000650: 5d5b 0000 8b00 0000 1700 0b00 6e00 0800  ][..........n...
-00000660: a85b 0000 2900 0000 1700 0b00 6f00 0800  .[..).......o...
-00000670: f95b 0000 5e00 0000 1700 0b00 7000 0800  .[..^.......p...
-00000680: a55d 0000 4a00 0000 1700 0b00 7100 0800  .]..J.......q...
-00000690: 4d5e 0000 3600 0000 1700 0b00 7200 0800  M^..6.......r...
-000006a0: 5b5f 0000 3600 0000 1700 0b00 7300 0800  [_..6.......s...
-000006b0: ef5f 0000 4a00 0000 1700 0b00 7400 0800  ._..J.......t...
-000006c0: 8c60 0000 2900 0000 1700 0b00 7500 0800  .`..).......u...
-000006d0: 5866 0000 2800 0000 1700 0b00 7600 0800  Xf..(.......v...
-000006e0: a066 0000 0d01 0000 1700 0b00 7700 0800  .f..........w...
-000006f0: d766 0000 a200 0000 1700 0b00 7800 0800  .f..........x...
-00000700: 2d68 0000 4200 0000 1900 0b00 7900 0800  -h..B.......y...
-00000710: 0000 0000 0b00 0000 1a00 0d00 7900 0800  ............y...
-00000720: 0000 0000 3e00 0000 1c00 0d00 7900 0800  ....>.......y...
-00000730: 0000 0000 1200 0000 1d00 0d00 7900 0800  ............y...
-00000740: 0000 0000 1600 0000 1e00 0d00 7900 0800  ............y...
-00000750: 0000 0000 3e00 0000 2100 0d00 7900 0800  ....>...!...y...
-00000760: 0000 0000 1200 0000 2200 0d00 7900 0800  ........"...y...
-00000770: 0000 0000 1d00 0000 2300 0d00 7900 0800  ........#...y...
-00000780: 0000 0000 2800 0000 2400 0d00 7900 0800  ....(...$...y...
-00000790: 0000 0000 1200 0000 2500 1000 7900 0800  ........%...y...
-000007a0: 0000 0000 b600 0000 2600 1000 7900 0800  ........&...y...
-000007b0: 0000 0000 5906 0000 2700 1000 7a00 0800  ....Y...'...z...
-000007c0: 0000 0000 1100 0000 2900 1300 7a00 0800  ........)...z...
-000007d0: 0000 0000 8a00 0000 2a00 1300 7d00 0800  ........*...}...
-000007e0: 0000 0000 5501 0000 2a00 1300 7d00 0800  ....U...*...}...
-000007f0: 2b00 0000 1d00 0000 2a00 1300 7e00 0800  +.......*...~...
-00000800: a200 0000 1d00 0000 2a00 1300 7f00 0800  ........*.......
-00000810: 1b01 0000 2000 0000 2c00 1600 8000 0800  .... ...,.......
-00000820: 0000 0000 320e 0000 2c00 1600 8300 0800  ....2...,.......
-00000830: 3801 0000 6501 0000 2c00 1600 8400 0800  8...e...,.......
-00000840: 3f01 0000 5e01 0000 2c00 1600 8500 0800  ?...^...,.......
-00000850: ea01 0000 1800 0000 2c00 1600 8600 0800  ........,.......
-00000860: c602 0000 4f0b 0000 2c00 1600 8800 0800  ....O...,.......
-00000870: e202 0000 330b 0000 2c00 1600 8900 0800  ....3...,.......
-00000880: f602 0000 cc0a 0000 2c00 1600 8a00 0800  ........,.......
-00000890: 1103 0000 910a 0000 2c00 1600 8b00 0800  ........,.......
-000008a0: 1a03 0000 880a 0000 2c00 1600 9200 0800  ........,.......
-000008b0: 2c04 0000 9b01 0000 2c00 1600 9400 0800  ,.......,.......
-000008c0: db04 0000 8b00 0000 2c00 1600 9500 0800  ........,.......
-000008d0: e004 0000 7800 0000 2c00 1600 9600 0800  ....x...,.......
-000008e0: d605 0000 8000 0000 2c00 1600 9700 0800  ........,.......
-000008f0: 4d0a 0000 b100 0000 2c00 1600 9900 0800  M.......,.......
-00000900: 610b 0000 fa00 0000 2c00 1600 9a00 0800  a.......,.......
-00000910: 2a0c 0000 1800 0000 2c00 1600 9b00 0800  *.......,.......
-00000920: 770c 0000 e200 0000 2e00 1900 9c00 0800  w...............
-00000930: 0000 0000 9805 0000 3000 1c00 a100 0800  ........0.......
-00000940: 0000 0000 7a32 0000 3000 1c00 a300 0800  ....z2..0.......
-00000950: 1a00 0000 6c00 0000 3000 1c00 a400 0800  ....l...0.......
-00000960: 2000 0000 5a00 0000 3000 1c00 a500 0800   ...Z...0.......
-00000970: c700 0000 b600 0000 3000 1c00 a600 0800  ........0.......
-00000980: d000 0000 ad00 0000 3000 1c00 a700 0800  ........0.......
-00000990: 9901 0000 0502 0000 3000 1c00 aa00 0800  ........0.......
-000009a0: 5f02 0000 4000 0000 3000 1c00 ab00 0800  _...@...0.......
-000009b0: 5e03 0000 4000 0000 3000 1c00 ac00 0800  ^...@...0.......
-000009c0: 5b2d 0000 4700 0000 3200 1c00 ad00 0800  [-..G...2.......
-000009d0: 0000 0000 af00 0000 3200 1c00 ae00 0800  ........2.......
-000009e0: 4300 0000 3d00 0000 3300 1c00 af00 0800  C...=...3.......
-000009f0: 0000 0000 7400 0000 3400 2000 af00 0800  ....t...4. .....
-00000a00: 0000 0000 9003 0000 3400 2000 b900 0800  ........4. .....
-00000a10: 1500 0000 7000 0000 3600 2000 bb00 0800  ....p...6. .....
-00000a20: 0000 0000 d601 0000 3600 2000 c000 0800  ........6. .....
-00000a30: 1d00 0000 dd00 0000 3600 2000 c100 0800  ........6. .....
-00000a40: 4800 0000 9600 0000 3800 2400 c200 0800  H.......8.$.....
-00000a50: 0000 0000 2200 0000 3a00 2400 c200 0800  ...."...:.$.....
-00000a60: 0000 0000 6901 0000 3d00 0500 c300 0800  ....i...=.......
-00000a70: 0000 0000 1d00 0000 4000 0b00 c300 0800  ........@.......
-00000a80: 0000 0000 1d00 0000 4100 0b00 c300 0800  ........A.......
-00000a90: 0000 0000 1a00 0000 4200 0b00 c300 0800  ........B.......
-00000aa0: 0000 0000 1a00 0000 4300 0b00 c300 0800  ........C.......
-00000ab0: 0000 0000 1a00 0000 4400 0b00 c300 0800  ........D.......
-00000ac0: 0000 0000 1d00 0000 4500 0b00 c300 0800  ........E.......
-00000ad0: 0000 0000 1d00 0000 4600 0b00 c300 0800  ........F.......
-00000ae0: 0000 0000 1d00 0000 4700 0b00 c300 0800  ........G.......
-00000af0: 0000 0000 1d00 0000 4800 0b00 c300 0800  ........H.......
-00000b00: 0000 0000 4300 0000 4900 0b00 c300 0800  ....C...I.......
-00000b10: 0000 0000 5a00 0000 4a00 0b00 c300 0800  ....Z...J.......
-00000b20: 0000 0000 5a00 0000 4b00 0b00 c300 0800  ....Z...K.......
-00000b30: 0000 0000 4300 0000 4c00 0b00 c300 0800  ....C...L.......
-00000b40: 0000 0000 1600 0000 4d00 0b00 c300 0800  ........M.......
-00000b50: 0000 0000 1b00 0000 4e00 0b00 c300 0800  ........N.......
-00000b60: 0000 0000 1b00 0000 4f00 0b00 c300 0800  ........O.......
-00000b70: 0000 0000 1b00 0000 5000 0b00 c300 0800  ........P.......
-00000b80: 0000 0000 1b00 0000 5100 0b00 c300 0800  ........Q.......
-00000b90: 0000 0000 3300 0000 5200 0b00 c300 0800  ....3...R.......
-00000ba0: 0000 0000 1b00 0000 5300 0b00 c300 0800  ........S.......
-00000bb0: 0000 0000 1b00 0000 5500 0b00 c300 0800  ........U.......
-00000bc0: 0000 0000 1d00 0000 5600 0b00 c300 0800  ........V.......
-00000bd0: 0000 0000 1d00 0000 5800 1300 c300 0800  ........X.......
-00000be0: 0000 0000 4000 0000 5b00 1600 c300 0800  ....@...[.......
-00000bf0: 0000 0000 1b00 0000 5c00 1600 c300 0800  ........\.......
-00000c00: 0000 0000 6100 0000 5e00 1600 c300 0800  ....a...^.......
-00000c10: 0000 0000 3300 0000 5f00 1600 c300 0800  ....3..._.......
-00000c20: 0000 0000 1a00 0000 6200 1c00 c300 0800  ........b.......
-00000c30: 0000 0000 0200 0000 6400 1c00 c300 0800  ........d.......
-00000c40: 0000 0000 3900 0000 6500 1c00 c300 0800  ....9...e.......
-00000c50: 0000 0000 3100 0000 6600 1c00 c300 0800  ....1...f.......
-00000c60: 0000 0000 3900 0000 6700 1c00 c300 0800  ....9...g.......
-00000c70: 0000 0000 3100 0000 0000 0000 bf06 0000  ....1...........
-00000c80: 0000 bf06 0000 0000 bf06 0000 0000 0100  ................
-00000c90: 0000 0000 6607 0000 0100 b704 0000 0200  ....f...........
-00000ca0: 2803 0000 0300 9e06 0000 0000 f802 0000  (...............
-00000cb0: 0400 5e02 0000 0500 5102 0000 0900 2502  ..^.....Q.....%.
-00000cc0: 0000 0a00 4802 0000 0000 4a07 0000 0000  ....H.....J.....
-00000cd0: 0100 0000 0100 d404 0000 0200 ba02 0000  ................
-00000ce0: 0300 9602 0000 0400 9d03 0000 0500 0706  ................
-00000cf0: 0000 0600 2004 0000 0700 cb01 0000 0800  .... ...........
-00000d00: f006 0000 0900 6703 0000 0a00 c003 0000  ......g.........
-00000d10: 0b00 8106 0000 0c00 c806 0000 0d00 e903  ................
-00000d20: 0000 0e00 d503 0000 0f00 4200 0000 1000  ..........B.....
-00000d30: 5200 0000 1100 2f00 0000 1200 d705 0000  R...../.........
-00000d40: 1300 5705 0000 1400 0104 0000 1500 8401  ..W.............
-00000d50: 0000 1600 1f03 0000 1700 9001 0000 1800  ................
-00000d60: 5706 0000 1900 3c06 0000 1a00 2806 0000  W.....<.....(...
-00000d70: 1b00 6d06 0000 1c00 3204 0000 1d00 df06  ..m.....2.......
-00000d80: 0000 1e00 f706 0000 1f00 0907 0000 2000  .............. .
-00000d90: 8e06 0000 2100 bb01 0000 2200 ab01 0000  ....!.....".....
-00000da0: 2300 9f04 0000 2400 c104 0000 2500 8c04  #.....$.....%...
-00000db0: 0000 2600 3707 0000 2700 1b07 0000 2800  ..&.7...'.....(.
-00000dc0: 6305 0000 2900 b404 0000 2c00 ed01 0000  c...).....,.....
-00000dd0: 2d00 3402 0000 2e00 3402 0000 2f00 3402  -.4.....4.../.4.
-00000de0: 0000 3100 d100 0000 3300 d100 0000 3400  ..1.....3.....4.
-00000df0: 3402 0000 3600 1d03 0000 3700 0d04 0000  4...6.....7.....
-00000e00: 3800 aa02 0000 3900 ce03 0000 3a00 1306  8.....9.....:...
-00000e10: 0000 3b00 7a03 0000 3c00 8c02 0000 3d00  ..;.z...<.....=.
-00000e20: 8c02 0000 3e00 6607 0000 3f00 c405 0000  ....>.f...?.....
-00000e30: 4000 7e05 0000 4100 ae05 0000 4200 9805  @.~...A.....B...
-00000e40: 0000 4300 7005 0000 4400 df04 0000 4500  ..C.p...D.....E.
-00000e50: 1705 0000 4600 7401 0000 4700 6701 0000  ....F.t...G.g...
-00000e60: 4800 4003 0000 4900 4501 0000 4a00 4f03  H.@...I.E...J.O.
-00000e70: 0000 4b00 5401 0000 4e00 ed01 0000 5300  ..K.T...N.....S.
-00000e80: ed01 0000 5400 ed01 0000 5500 ed01 0000  ....T.....U.....
-00000e90: 5600 ed01 0000 5700 ed01 0000 5900 3b03  V.....W.....Y.;.
-00000ea0: 0000 5a00 ff07 0000 5d00 cf07 0000 5e00  ..Z.....].....^.
-00000eb0: a907 0000 5f00 bf07 0000 6000 dd07 0000  ...._.....`.....
-00000ec0: 6100 f107 0000 6200 8707 0000 6300 9b07  a.....b.....c...
-00000ed0: 0000 6400 4407 0000 6600 7302 0000 6700  ..d.D...f.s...g.
-00000ee0: 4404 0000 6b00 3605 0000 6c00 9d01 0000  D...k.6...l.....
-00000ef0: 6d00 3301 0000 6e00 4407 0000 6f00 3402  m.3...n.D...o.4.
-00000f00: 0000 7000 6a02 0000 7100 f904 0000 7200  ..p.j...q.....r.
-00000f10: 1d03 0000 7300 f904 0000 7400 f904 0000  ....s.....t.....
-00000f20: 7500 f904 0000 7600 f904 0000 7700 3402  u.....v.....w.4.
-00000f30: 0000 7800 6a02 0000 7a00 9102 0000 7b00  ..x.j...z.....{.
-00000f40: f904 0000 7c00 b404 0000 0000 ba02 0000  ....|...........
-00000f50: 0000 0100 0000 0100 0002 0000 0200 be04  ................
-00000f60: 0000 0100 7007 0000 0200 7007 0000 0400  ....p.....p.....
-00000f70: b702 0000 0000 0100 0000 0100 8004 0000  ................
-00000f80: 0200 2807 0000 0700 6a02 0000 0800 6203  ..(.....j.....b.
-00000f90: 0000 0c00 2f02 0000 0f00 2401 0000 1000  ..../.....$.....
-00000fa0: 7d07 0000 1400 2701 0000 1500 6203 0000  }.....'.....b...
-00000fb0: 1600 f904 0000 1700 3f05 0000 1800 e802  ........?.......
-00000fc0: 0000 1900 8704 0000 1a00 4c05 0000 1b00  ..........L.....
-00000fd0: 0405 0000 1c00 2205 0000 1d00 bf06 0000  ......".........
-00000fe0: 1f00 0203 0000 2000 d705 0000 2300 1d03  ...... .....#...
-00000ff0: 0000 2400 7104 0000 2500 ed01 0000 2800  ..$.q...%.....(.
-00001000: 0401 0000 2900 d705 0000 2a00 c902 0000  ....).....*.....
-00001010: 2b00 2f02 0000 2c00 e305 0000 0000 0c01  +./...,.........
-00001020: 0000 0100 b704 0000 0200 2803 0000 0300  ..........(.....
-00001030: b103 0000 0400 1a06 0000 0000 0100 0000  ................
-00001040: 0100 f201 0000 0200 be04 0000 0300 0002  ................
-00001050: 0000 0500 3b03 0000 0600 3203 0000 0900  ....;.....2.....
-00001060: 1100 0000 0a00 1902 0000 0b00 0c02 0000  ................
-00001070: 0c00 be04 0000 0d00 be04 0000 1000 3d02  ..............=.
-00001080: 0000 0000 ba06 0000 0200 4607 0000 0000  ..........F.....
-00001090: 5c04 0000 0100 d402 0000 0200 2100 0000  \...........!...
-000010a0: 0300 5307 0000 0400 0c03 0000 0500 a506  ..S.............
-000010b0: 0000 0600 1004 0000 0700 eb04 0000 0800  ................
-000010c0: 8f03 0000 0900 fa05 0000 0b00 6a02 0000  ............j...
-000010d0: 0c00 fb00 0000 0000 4b04 0000 0100 7e02  ........K.....~.
-000010e0: 0000 0200 dd01 0000 0300 8403 0000 0400  ................
-000010f0: f005 0000 0600 b102 0000 0b00 2d01 0000  ............-...
-00001100: 0000 cb01 8b00 0f47 ba00 1547 a100 1b47  .......G...G...G
-00001110: eb00 2147 7700 2747 6300 2d47 d800 3347  ..!Gw.'Gc.-G..3G
-00001120: 0000 0000 0100 3a2f 0200 0000 0100 ea2f  ......:/......./
-00001130: 0400 0000 0100 8a31 0600 0000 0100 c931  .......1.......1
-00001140: 0800 0000 0100 ef32 0a00 0000 0100 8147  .......2.......G
-00001150: 0c00 0000 0100 2948 0e00 0000 0f00 0000  ......)H........
-00001160: 0100 3949 1100 0000 1200 0000 0100 454d  ..9I..........EM
-00001170: 1400 0000 1500 0000 0100 074e 1700 0000  ...........N....
-00001180: 1800 0000 0100 4453 1a00 0000 1b00 0000  ......DS........
-00001190: 0100 fd54 1d00 0000 1e00 0000 1f00 0000  ...T............
-000011a0: 0100 ac55 2100 0000 2200 0000 2300 0000  ...U!..."...#...
-000011b0: 2700 0500 7e07 2700 0600 a708 2700 0700  '...~.'.....'...
-000011c0: ce0a 8301 0400 7c07 a301 0400 7c07 c301  ......|.....|...
-000011d0: 0400 7c07 e301 0400 7c07 0302 0400 7c07  ..|.....|.....|.
-000011e0: 1602 0300 3b04 3602 0300 0d05 5602 0300  ....;.6.....V...
-000011f0: 2306 8302 0400 7c07 a302 0400 7c07 c302  #.....|.....|...
-00001200: 0400 7c07 6303 0400 7c07 0000 0043 5324  ..|.c...|....CS$
-00001210: 3c3e 385f 5f6c 6f63 616c 7330 0043 5324  <>8__locals0.CS$
-00001220: 3c3e 385f 5f6c 6f63 616c 7331 0072 6f6f  <>8__locals1.roo
-00001230: 6d4e 616d 6548 7564 4343 0077 6174 6572  mNameHudCC.water
-00001240: 5475 7262 696e 6544 6f6f 7243 4300 7468  TurbineDoorCC.th
-00001250: 6f74 684c 6566 7444 6f6f 7243 4300 7468  othLeftDoorCC.th
-00001260: 6f74 6852 6967 6874 446f 6f72 4343 0050  othRightDoorCC.P
-00001270: 6970 6549 6e44 6570 7468 7355 7070 6572  ipeInDepthsUpper
-00001280: 4944 0050 6970 6549 6e44 6570 7468 734c  ID.PipeInDepthsL
-00001290: 6f77 6572 4944 0054 686f 7468 4272 6964  owerID.ThothBrid
-000012a0: 6765 4c65 6674 446f 6f72 4944 0041 3257  geLeftDoorID.A2W
-000012b0: 6174 6572 5475 7262 696e 654c 6566 7444  aterTurbineLeftD
-000012c0: 6f6f 7249 4400 5468 6f74 6842 7269 6467  oorID.ThothBridg
-000012d0: 6552 6967 6874 446f 6f72 4944 0064 6f6f  eRightDoorID.doo
-000012e0: 7249 4400 5069 7065 496e 5761 7465 7266  rID.PipeInWaterf
-000012f0: 616c 6c73 4944 0050 6970 6549 6e48 6964  allsID.PipeInHid
-00001300: 656f 7574 4944 0072 6f6f 6d44 6174 6100  eoutID.roomData.
-00001310: 666c 6970 7065 6400 6f43 6f6e 7472 6f6c  flipped.oControl
-00001320: 4e65 7477 6f72 6b52 6563 6569 7665 6400  NetworkReceived.
-00001330: 6964 0066 6f75 6e64 0063 6f6f 7264 0063  id.found.coord.c
-00001340: 6f6c 6c69 7369 6f6e 436f 6465 546f 4265  ollisionCodeToBe
-00001350: 0064 6570 7468 7350 6970 6543 6f64 6500  .depthsPipeCode.
-00001360: 7761 7465 7266 616c 6c73 5069 7065 436f  waterfallsPipeCo
-00001370: 6465 006e 6573 7450 6970 6543 6f64 6500  de.nestPipeCode.
-00001380: 6869 6465 6f75 7450 6970 6543 6f64 6500  hideoutPipeCode.
-00001390: 6472 6177 4775 6943 6f64 6500 6c61 6242  drawGuiCode.labB
-000013a0: 6c6f 636b 436f 6465 0063 6f6c 6c69 7369  lockCode.collisi
-000013b0: 6f6e 436f 6465 006c 6f61 6447 6c6f 6261  onCode.loadGloba
-000013c0: 6c73 436f 6465 0073 6176 6547 6c6f 6261  lsCode.saveGloba
-000013d0: 6c73 436f 6465 0063 6861 7261 6374 6572  lsCode.character
-000013e0: 5661 7273 436f 6465 0073 7346 4744 6573  VarsCode.ssFGDes
-000013f0: 7472 6f79 436f 6465 0063 6f64 6500 7574  troyCode.code.ut
-00001400: 5465 7874 7572 6550 6167 6500 7465 7874  TexturePage.text
-00001410: 7572 6550 6167 6500 6134 5061 6765 3249  urePage.a4Page2I
-00001420: 6d61 6765 0061 3450 6167 6549 6d61 6765  mage.a4PageImage
-00001430: 006d 7573 6963 4669 6c65 0074 696c 6500  .musicFile.tile.
-00001440: 636f 6465 4e61 6d65 0073 7072 6974 654e  codeName.spriteN
-00001450: 616d 6500 6f72 6967 4e61 6d65 006f 7269  ame.origName.ori
-00001460: 6753 6f6e 674e 616d 6500 6e65 7753 6f6e  gSongName.newSon
-00001470: 674e 616d 6500 726f 6f6d 4e61 6d65 0070  gName.roomName.p
-00001480: 6963 6b75 704e 616d 6500 4453 4d61 7043  ickupName.DSMapC
-00001490: 6f6f 7264 526f 6f6d 6e61 6d65 0070 6970  oordRoomname.pip
-000014a0: 6500 7769 7364 6f6d 5365 7074 6f67 6743  e.wisdomSeptoggC
-000014b0: 7265 6174 6500 6372 6561 7465 0076 616c  reate.create.val
-000014c0: 7565 0062 6700 6f57 6973 646f 6d53 6570  ue.bg.oWisdomSep
-000014d0: 746f 6767 006c 6566 7446 6163 696e 6700  togg.leftFacing.
-000014e0: 726f 6f6d 4e61 6d65 4453 4d61 7053 7472  roomNameDSMapStr
-000014f0: 696e 6700 6973 5265 7365 6172 6368 4861  ing.isResearchHa
-00001500: 7463 6800 6d75 7369 6350 6174 6800 7469  tch.musicPath.ti
-00001510: 6c65 4465 7074 6800 726f 6f6d 4e61 6d65  leDepth.roomName
-00001520: 4875 6444 7261 7747 7569 006c 6162 426c  HudDrawGui.labBl
-00001530: 6f63 6b00 6172 6773 4c6f 6361 6c00 7061  ock.argsLocal.pa
-00001540: 6765 4974 656d 0069 7465 6d00 6465 7074  geItem.item.dept
-00001550: 6873 5069 7065 526f 6f6d 0077 6174 6572  hsPipeRoom.water
-00001560: 6661 6c6c 7350 6970 6552 6f6f 6d00 726f  fallsPipeRoom.ro
-00001570: 6f6d 0064 6f6f 7253 616d 7573 436f 6c6c  om.doorSamusColl
-00001580: 6973 696f 6e00 636f 6c6c 6973 696f 6e00  ision.collision.
-00001590: 7373 4647 4163 7469 6f6e 0072 6f6f 6d48  ssFGAction.roomH
-000015a0: 7564 4163 7469 6f6e 0077 6973 646f 6d53  udAction.wisdomS
-000015b0: 6570 746f 6767 4163 7469 6f6e 006f 436f  eptoggAction.oCo
-000015c0: 6e74 726f 6c41 6374 696f 6e00 7661 7244  ntrolAction.varD
-000015d0: 6f6f 7241 6374 696f 6e00 6163 7469 6f6e  oorAction.action
-000015e0: 0061 3541 6374 6976 6174 6543 6f6e 6469  .a5ActivateCondi
-000015f0: 7469 6f6e 0065 6d70 4261 7474 6572 7943  tion.empBatteryC
-00001600: 656c 6c43 6f6e 6469 7469 6f6e 0073 6372  ellCondition.scr
-00001610: 444e 4153 7061 776e 0067 6f00 726f 6f6d  DNASpawn.go.room
-00001620: 4e61 6d65 4875 6453 7465 7000 7769 7364  NameHudStep.wisd
-00001630: 6f6d 5365 7074 6f67 6753 7465 7000 7375  omSeptoggStep.su
-00001640: 6273 6372 6565 6e4d 656e 7553 7465 7000  bscreenMenuStep.
-00001650: 7069 636b 7570 0064 734d 6170 436f 7264  pickup.dsMapCord
-00001660: 4275 696c 6465 7200 726f 6f6d 4e61 6d65  Builder.roomName
-00001670: 4453 4d61 7042 7569 6c64 6572 0074 696c  DSMapBuilder.til
-00001680: 6573 6574 436f 756e 7465 7200 6135 446f  esetCounter.a5Do
-00001690: 6f72 0064 6f6f 7200 616c 7265 6164 7941  or.door.alreadyA
-000016a0: 6464 6564 5042 6f6d 6273 0061 6c72 6561  ddedPBombs.alrea
-000016b0: 6479 4164 6465 644d 6973 7369 6c65 7300  dyAddedMissiles.
-000016c0: 6673 006c 6f63 616c 7300 6d73 0061 6c72  fs.locals.ms.alr
-000016d0: 6561 6479 4164 6465 6453 7570 6572 7300  eadyAddedSupers.
-000016e0: 7365 6564 4f62 6a65 6374 0073 6f6c 6964  seedObject.solid
-000016f0: 4f62 6a65 6374 0072 6f6f 6d48 7564 4f62  Object.roomHudOb
-00001700: 6a65 6374 0067 616d 654f 626a 6563 7400  ject.gameObject.
-00001710: 7761 7465 7254 7572 6269 6e65 4f62 6a65  waterTurbineObje
-00001720: 6374 0070 6970 654f 626a 6563 7400 7265  ct.pipeObject.re
-00001730: 7365 6172 6368 4861 7463 684f 626a 6563  searchHatchObjec
-00001740: 7400 676d 4f62 6a65 6374 0069 7347 6f74  t.gmObject.isGot
-00001750: 6f4f 626a 6563 7400 646f 6f72 4f62 6a65  oObject.doorObje
-00001760: 6374 0065 6e65 6d79 4f62 6a65 6374 0065  ct.enemyObject.e
-00001770: 7461 6e6b 536e 6970 7065 7400 7069 7065  tankSnippet.pipe
-00001780: 4247 5469 6c65 7365 7400 6465 7074 6873  BGTileset.depths
-00001790: 456e 7472 616e 6365 5069 7065 5469 6c65  EntrancePipeTile
-000017a0: 7365 7400 7761 7465 7266 616c 6c73 5069  set.waterfallsPi
-000017b0: 7065 5469 6c65 7365 7400 6465 7074 6873  peTileset.depths
-000017c0: 4578 6974 5069 7065 5469 6c65 7365 7400  ExitPipeTileset.
-000017d0: 6869 6465 6f75 7450 6970 6554 696c 6573  hideoutPipeTiles
-000017e0: 6574 0064 6f6f 7254 696c 6573 6574 006d  et.doorTileset.m
-000017f0: 6f76 696e 674f 6666 7365 7400 7373 4647  ovingOffset.ssFG
-00001800: 4576 656e 7400 726f 6f6d 4875 6445 7665  Event.roomHudEve
-00001810: 6e74 0077 6973 646f 6d53 6570 746f 6767  nt.wisdomSeptogg
-00001820: 4576 656e 7400 6f43 6f6e 7472 6f6c 4576  Event.oControlEv
-00001830: 656e 7400 7042 6f6d 6243 6861 7261 6374  ent.pBombCharact
-00001840: 6572 4576 656e 7400 7375 7065 724d 6973  erEvent.superMis
-00001850: 7369 6c65 4368 6172 6163 7465 7245 7665  sileCharacterEve
-00001860: 6e74 006d 6973 7369 6c65 4368 6172 6163  nt.missileCharac
-00001870: 7465 7245 7665 6e74 0065 5461 6e6b 4368  terEvent.eTankCh
-00001880: 6172 6163 7465 7245 7665 6e74 0076 6172  aracterEvent.var
-00001890: 446f 6f72 4576 656e 7400 6974 656d 7353  DoorEvent.itemsS
-000018a0: 7761 7053 6372 6970 7400 7363 7269 7074  wapScript.script
-000018b0: 0072 6f6f 6d4e 616d 6548 7564 526f 6f6d  .roomNameHudRoom
-000018c0: 5374 6172 7400 6c69 7374 0063 6f64 6554  Start.list.codeT
-000018d0: 6578 7400 6e65 7744 6f6f 7252 6570 6c61  ext.newDoorRepla
-000018e0: 6365 6d65 6e74 5465 7874 0073 7562 7363  cementText.subsc
-000018f0: 7265 656e 4d69 7363 4461 7700 7373 4472  reenMiscDaw.ssDr
-00001900: 6177 0073 7562 6372 6565 6e42 6f6f 7473  aw.subcreenBoots
-00001910: 4472 6177 0073 7562 7363 7265 656e 5375  Draw.subscreenSu
-00001920: 6974 4472 6177 0064 7261 7745 6e64 496e  itDraw.drawEndIn
-00001930: 6465 7800 646f 6f72 4576 656e 7449 6e64  dex.doorEventInd
-00001940: 6578 0064 7261 7753 7461 7274 496e 6465  ex.drawStartInde
-00001950: 7800 6b65 7900 6173 7365 6d62 6c79 0072  x.key.assembly.r
-00001960: 6f6f 6d4e 616d 6548 7564 4465 7374 726f  oomNameHudDestro
-00001970: 7900 636f 6465 456e 7472 7900 7465 7874  y.codeEntry.text
-00001980: 7572 6545 6e74 7279 0064 6f6f 7245 6e74  ureEntry.doorEnt
-00001990: 7279 006c 6f63 6b65 6450 426f 6d62 5175  ry.lockedPBombQu
-000019a0: 616e 7469 7479 0070 426f 6d62 5175 616e  antity.pBombQuan
-000019b0: 7469 7479 006c 6f63 6b65 644d 6973 7369  tity.lockedMissi
-000019c0: 6c65 5175 616e 7469 7479 006d 6973 7369  leQuantity.missi
-000019d0: 6c65 5175 616e 7469 7479 0066 696e 616c  leQuantity.final
-000019e0: 5175 616e 7469 7479 006c 6f63 6b65 6453  Quantity.lockedS
-000019f0: 7570 6572 5175 616e 7469 7479 0073 7570  uperQuantity.sup
-00001a00: 6572 5175 616e 7469 7479 0071 7561 6e74  erQuantity.quant
-00001a10: 6974 7900 0000 0000 0fd0 2988 b811 1342  ity.......)....B
-00001a20: 878b 770e 8597 ac16 f862 513f c607 d311  ..w......bQ?....
-00001a30: 9053 00c0 4fa3 02a1 1b57 8a0e 2669 6e46  .S..O....W..&inF
-00001a40: b4ad 8ab0 4611 f5fe bc74 2e93 a9db 7844  ....F....t....xD
-00001a50: 8d46 0f32 a7ba b3d3 5605 11cc 91a0 384d  .F.2....V.....8M
-00001a60: 9fec 25ab 9a35 1a6a 05ec feb5 d08c 834a  ..%..5.j.......J
-00001a70: 96da 4662 84bb 4bd8 0847 4d7e 6e09 5c4c  ..Fb..K..GM~n.\L
-00001a80: aeda cb10 ba6a 740d 0004 686f 6d65 0672  .....jt...home.r
-00001a90: 756e 6e65 7204 776f 726b 0459 414d 5308  unner.work.YAMS.
-00001aa0: 5941 4d53 2d4c 4942 0d45 7863 6570 7469  YAMS-LIB.Excepti
-00001ab0: 6f6e 732e 6373 092f 0001 060d 1212 1720  ons.cs./....... 
-00001ac0: 2045 cf63 12b5 33a2 5dfc 4dce b431 5040   E.c..3.].M..1P@
-00001ad0: 06cb b9c4 4b95 8487 2f00 aa0c 69ad 7c7b  ....K.../...i.|{
-00001ae0: 7913 4578 7465 6e73 696f 6e4d 6574 686f  y.ExtensionMetho
-00001af0: 6473 2e63 7309 2f00 0106 0d12 1217 5920  ds.cs./.......Y 
-00001b00: 8e60 29b7 ed9a 0b1a 1a46 f770 be95 760e  .`)......F.p..v.
-00001b10: ea0e 8ec0 45b2 e613 b318 395a 43ae 57f7  ....E.....9ZC.W.
-00001b20: 0f4d 7573 6963 5368 7566 666c 652e 6373  .MusicShuffle.cs
-00001b30: 0a2f 0001 060d 1212 1780 9820 3c0a 97ef  ./......... <...
-00001b40: 3aba 9a95 23f6 7f5c 7a9b 8254 fac4 f5de  :...#..\z..T....
-00001b50: dc3e 0a75 a15d d33b dcc7 45e4 0b50 6167  .>.u.].;..E..Pag
-00001b60: 6549 7465 6d2e 6373 0a2f 0001 060d 1212  eItem.cs./......
-00001b70: 1780 d420 b8f4 0c63 e376 41df 859c 9e67  ... ...c.vA....g
-00001b80: 96f9 3ff7 c2ee f73b bfa8 ba8e 5fa9 fa91  ..?....;...._...
-00001b90: 408f 2dda 0770 6174 6368 6573 1141 6464  @.-..patches.Add
-00001ba0: 496e 4761 6d65 4869 6e74 732e 6373 0c2f  InGameHints.cs./
-00001bb0: 0001 060d 1212 1781 0c81 1420 6e02 69a1  ........... n.i.
-00001bc0: 68e9 d66f e7cc 3811 95b7 b370 bf14 88e1  h..o..8....p....
-00001bd0: e2a0 5b53 5d2c f554 b77d acd2 0e43 6f73  ..[S],.T.}...Cos
-00001be0: 6d65 7469 6348 7564 2e63 730c 2f00 0106  meticHud.cs./...
-00001bf0: 0d12 1217 810c 8154 2021 0e9e e208 512b  .......T !....Q+
-00001c00: df26 8fe7 4a3d 859d 6171 9813 5331 5cb5  .&..J=..aq..S1\.
-00001c10: 3dfc e038 894d ca8a e010 446f 6f72 4c6f  =..8.M....DoorLo
-00001c20: 636b 5261 6e64 6f2e 6373 0c2f 0001 060d  ckRando.cs./....
-00001c30: 1212 1781 0c81 9120 d7dc d53e db98 6e3e  ....... ...>..n>
-00001c40: f456 7805 f7e9 cb8f 1701 aa23 22fd d775  .Vx........#"..u
-00001c50: a34b d63d 0444 3afc 0d4d 756c 7469 776f  .K.=.D:..Multiwo
-00001c60: 726c 642e 6373 0c2f 0001 060d 1212 1781  rld.cs./........
-00001c70: 0c81 d020 fcd7 7d7d 7dfe 1110 6e46 2898  ... ..}}}...nF(.
-00001c80: 20fe 5717 e5be fc76 c337 eaa8 024c 6bd4   .W....v.7...Lk.
-00001c90: 6a52 afcd 0371 6f6c 1744 6973 706c 6179  jR...qol.Display
-00001ca0: 526f 6f6d 4e61 6d65 4f6e 4855 442e 6373  RoomNameOnHUD.cs
-00001cb0: 0e2f 0001 060d 1212 1781 0c82 0c82 1020  ./............. 
-00001cc0: 4d23 0e05 5638 4766 9700 43bc 2d01 9dcb  M#..V8Gf..C.-...
-00001cd0: c8ef f918 c361 86d3 f16f c89a 1bfb ec85  .....a...o......
-00001ce0: 1844 6973 706c 6179 526f 6f6d 4e61 6d65  .DisplayRoomName
-00001cf0: 734f 6e4d 6170 2e63 730e 2f00 0106 0d12  sOnMap.cs./.....
-00001d00: 1217 810c 820c 8258 2099 1928 51d6 abde  .......X ..(Q...
-00001d10: 1669 e226 83bb 64d4 46ec 545d 2c37 82f1  .i.&..d.F.T],7..
-00001d20: 3415 3b56 6cd5 e2b5 3d15 526f 6f6d 4665  4.;Vl...=.RoomFe
-00001d30: 6174 7572 654d 6170 5465 7874 2e63 730e  atureMapText.cs.
-00001d40: 2f00 0106 0d12 1217 810c 820c 82a1 20c4  /............. .
-00001d50: 8253 0a0a 876a 5cfe 6919 2a2c 85e5 ccb9  .S...j\.i.*,....
-00001d60: d59e 17e1 94a1 d4dc e7ab 234c 0ed7 c719  ..........#L....
-00001d70: 5368 6f77 4675 6c6c 7955 6e65 7870 6c6f  ShowFullyUnexplo
-00001d80: 7265 644d 6170 2e63 730e 2f00 0106 0d12  redMap.cs./.....
-00001d90: 1217 810c 820c 82e7 204b 3897 7778 2bb2  ........ K8.wx+.
-00001da0: 56ca 6138 17db bdb9 b4ee cc3d 52c6 5a60  V.a8.......=R.Z`
-00001db0: a4aa 48c2 7668 3ad2 af0a 5370 7269 7465  ..H.vh:...Sprite
-00001dc0: 732e 6373 0c2f 0001 060d 1212 1781 0c83  s.cs./..........
-00001dd0: 3120 e68e 493f bad2 08df 4416 aed4 063e  1 ..I?....D....>
-00001de0: 4034 4559 7dab 15a6 01db 4696 7fa2 a514  @4EY}.....F.....
-00001df0: 7ff1 0a50 726f 6772 616d 2e63 730a 2f00  ...Program.cs./.
-00001e00: 0106 0d12 1217 836a 2075 edac 1fc8 b276  .......j u.....v
-00001e10: 56c1 f278 8209 817a 387c e786 e6a2 db76  V..x...z8|.....v
-00001e20: 1695 8203 682e 1df3 d20d 5365 6564 4f62  ....h.....SeedOb
-00001e30: 6a65 6374 2e63 730a 2f00 0106 0d12 1217  ject.cs./.......
-00001e40: 83a1 20ca 4616 7be8 3aaa e496 3643 4d33  .. .F.{.:...6CM3
-00001e50: 9630 49a3 8b6a 3951 2761 b2db 9032 c644  .0I..j9Q'a...2.D
-00001e60: 2b8a bf03 6f62 6a07 5265 6c65 6173 6506  +...obj.Release.
-00001e70: 6e65 7436 2e30 1a59 414d 532d 4c49 422e  net6.0.YAMS-LIB.
-00001e80: 476c 6f62 616c 5573 696e 6773 2e67 2e63  GlobalUsings.g.c
-00001e90: 7310 2f00 0106 0d12 1217 83db 83df 83e7  s./.............
-00001ea0: 83ee 20ad db14 3f8c 43b9 5f1b b73a 0cba  .. ...?.C._..:..
-00001eb0: 7c79 3281 935c 4ab8 ccab bdf6 b04d 3e0f  |y2..\J......M>.
-00001ec0: 809e 0e70 1f01 0000 d3d7 57b0 492c 2dc9  ...p......W.I,-.
-00001ed0: d74d 4fcd 4b2d 4a2c 494d d1b7 e34a cfc9  .MO.K-J,IM...J..
-00001ee0: 4f4a cc51 282d cecc 4b57 8070 acac 822b  OJ.Q(-..KW.p...+
-00001ef0: 8b4b 5273 adf1 49ea 39e7 e7e4 a426 9764  .KRs..I.9....&.d
-00001f00: e6e7 15eb b983 0ccc 4cc6 afc1 d31f bfbc  ........L.......
-00001f10: 4f66 5e21 7e15 7ea9 257a 1e25 2505 f855  Of^!~.~.%z.%%..U
-00001f20: 8564 14a5 26a6 0025 8854 a617 9258 9c5d  .d..&..%.T...X.]
-00001f30: 6ccd 0500 2e2e 4e45 5443 6f72 6541 7070  l.....NETCoreApp
-00001f40: 2c56 6572 7369 6f6e 3d76 362e 302e 4173  ,Version=v6.0.As
-00001f50: 7365 6d62 6c79 4174 7472 6962 7574 6573  semblyAttributes
-00001f60: 2e63 7310 2f00 0106 0d12 1217 83db 83df  .cs./...........
-00001f70: 83e7 84ac 2078 97e5 953c b5cd 5131 509b  .... x...<..Q1P.
-00001f80: 3504 2186 34c2 4b9c e7a6 8b98 4ffb 5a16  5.!.4.K.....O.Z.
-00001f90: 686e b5af 5c80 c900 0000 002f 2f20 3c61  hn..\......// <a
-00001fa0: 7574 6f67 656e 6572 6174 6564 202f 3e0d  utogenerated />.
-00001fb0: 0a75 7369 6e67 2053 7973 7465 6d3b 0d0a  .using System;..
-00001fc0: 7573 696e 6720 5379 7374 656d 2e52 6566  using System.Ref
-00001fd0: 6c65 6374 696f 6e3b 0d0a 5b61 7373 656d  lection;..[assem
-00001fe0: 626c 793a 2067 6c6f 6261 6c3a 3a53 7973  bly: global::Sys
-00001ff0: 7465 6d2e 5275 6e74 696d 652e 5665 7273  tem.Runtime.Vers
-00002000: 696f 6e69 6e67 2e54 6172 6765 7446 7261  ioning.TargetFra
-00002010: 6d65 776f 726b 4174 7472 6962 7574 6528  meworkAttribute(
-00002020: 222e 4e45 5443 6f72 6541 7070 2c56 6572  ".NETCoreApp,Ver
-00002030: 7369 6f6e 3d76 362e 3022 2c20 4672 616d  sion=v6.0", Fram
-00002040: 6577 6f72 6b44 6973 706c 6179 4e61 6d65  eworkDisplayName
-00002050: 203d 2022 2e4e 4554 2036 2e30 2229 5d0a   = ".NET 6.0")].
-00002060: 1859 414d 532d 4c49 422e 4173 7365 6d62  .YAMS-LIB.Assemb
-00002070: 6c79 496e 666f 2e63 7310 2f00 0106 0d12  lyInfo.cs./.....
-00002080: 1217 83db 83df 83e7 85d8 20a8 1e99 9946  .......... ....F
-00002090: 3eae 7c06 b08c 3570 6bb6 b9f0 f104 9673  >.|...5pk......s
-000020a0: 7291 9236 7973 d7b0 468f 1a81 57d2 0300  r..6ys..F...W...
-000020b0: 00ad 9351 4bc3 3010 c7df fb29 8e3d 29b2  ...QK.0....).=).
-000020c0: b676 75dd 9c08 db60 3270 20db 5044 7cb8  .vu....`2p .PD|.
-000020d0: b6d7 3690 2692 a48e 7e7b d3e9 c6c6 500a  ..6.&...~{....P.
-000020e0: eede 7277 f9fd ef2e 17cf eb9e d51c cf83  ..rw............
-000020f0: 3bac 8cec e624 48a1 a1f4 bef1 35b6 2e98  ;....$H.....5...
-00002100: 8644 a604 1bd4 b08f 435c 0382 9192 bb36  .D......C\.....6
-00002110: 7397 3c2d 50e4 a4ad 1f4c 732f 639c a0c4  s.<-P....Ls/c...
-00002120: 1a12 ac34 0113 8954 8a12 0331 15f8 c9a4  ...4...T...1....
-00002130: 0214 296c 18e7 d603 5c6a 032c dbc1 4c41  ..)l....\j.,..LA
-00002140: dfc2 16a4 68af ec6e abf5 4ecb 3df3 4c9c  ....h..n..N.=.L.
-00002150: 4a33 91c3 aad6 86ca d1d1 c95d 52c6 6d1b  J3.........]R.m.
-00002160: 4c8a 91e3 bca1 d654 c6bc be3d 0dbb e39f  L......T...=....
-00002170: d854 961f 28ea b131 8ac5 95a1 8bce eb78  .T..(..1.......x
-00002180: b1ea 3ece 279d cbf7 b608 91b1 bcb2 fd5a  ..>.'..........Z
-00002190: ef01 6849 9c50 536b cecc 3eca 3329 7d4c  ..hI.PSk..>.3)}L
-000021a0: 09dc 6b37 70fd d694 b9c8 a42a b7b5 20ff  ..k7p......*.. .
-000021b0: 0577 150d 0788 4936 203f f4fb 8390 fa71  .w....I6 ?.....q
-000021c0: 10f4 87a1 1f44 712f 89c3 5e1a 0f23 8cfc  .....Dq/..^..#..
-000021d0: 9bd6 aa4f 4aa6 5562 fe33 c635 339c fe03  ...OJ.Ub.3.53...
-000021e0: f873 76cd 723e 1c7e 9266 8b17 ab49 c578  .sv.r>.~.f...I.x
-000021f0: 0a2f 8a19 9ada 959e 29cc 4b12 0612 6e15  ./......).K...n.
-00002200: 5dc7 f902 010f 8127 7b22 646f 6375 6d65  ]......'{"docume
-00002210: 6e74 7322 3a7b 222f 686f 6d65 2f72 756e  nts":{"/home/run
-00002220: 6e65 722f 776f 726b 2f59 414d 532f 5941  ner/work/YAMS/YA
-00002230: 4d53 2f2a 223a 2268 7474 7073 3a2f 2f72  MS/*":"https://r
-00002240: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00002250: 7465 6e74 2e63 6f6d 2f72 616e 646f 7661  tent.com/randova
-00002260: 6e69 612f 5941 4d53 2f37 3938 6161 6366  nia/YAMS/798aacf
-00002270: 3865 3034 3036 3834 6536 6232 3236 3934  8e040684e6b22694
-00002280: 3032 3762 3363 6234 3364 6239 3761 3730  027b3cb43db97a70
-00002290: 352f 2a22 2c22 2f68 6f6d 652f 7275 6e6e  5/*","/home/runn
-000022a0: 6572 2f77 6f72 6b2f 5941 4d53 2f59 414d  er/work/YAMS/YAM
-000022b0: 532f 556e 6465 7274 616c 654d 6f64 546f  S/UndertaleModTo
-000022c0: 6f6c 2f2a 223a 2268 7474 7073 3a2f 2f72  ol/*":"https://r
-000022d0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000022e0: 7465 6e74 2e63 6f6d 2f6b 727a 7973 2d68  tent.com/krzys-h
-000022f0: 2f55 6e64 6572 7461 6c65 4d6f 6454 6f6f  /UndertaleModToo
-00002300: 6c2f 3266 3065 3636 6530 3931 3034 3937  l/2f0e66e0910497
-00002310: 6435 3132 6331 3862 3434 3966 3735 6634  d512c18b449f75f4
-00002320: 3734 6133 3432 3566 3037 2f2a 227d 7d82  74a3425f07/*"}}.
-00002330: 2576 6572 7369 6f6e 0032 0063 6f6d 7069  %version.2.compi
-00002340: 6c65 722d 7665 7273 696f 6e00 342e 392e  ler-version.4.9.
-00002350: 322d 332e 3234 3132 392e 362b 3939 3334  2-3.24129.6+9934
-00002360: 6662 3965 3335 3237 6531 6330 6335 3133  fb9e3527e1c0c513
-00002370: 3134 6535 3764 3461 6162 3330 6639 3765  14e57d4aab30f97e
-00002380: 3866 3965 006c 616e 6775 6167 6500 4323  8f9e.language.C#
-00002390: 0073 6f75 7263 652d 6669 6c65 2d63 6f75  .source-file-cou
-000023a0: 6e74 0031 3800 6f75 7470 7574 2d6b 696e  nt.18.output-kin
-000023b0: 6400 4479 6e61 6d69 6361 6c6c 794c 696e  d.DynamicallyLin
-000023c0: 6b65 644c 6962 7261 7279 006f 7074 696d  kedLibrary.optim
-000023d0: 697a 6174 696f 6e00 7265 6c65 6173 6500  ization.release.
-000023e0: 706c 6174 666f 726d 0041 6e79 4370 7500  platform.AnyCpu.
-000023f0: 7275 6e74 696d 652d 7665 7273 696f 6e00  runtime-version.
-00002400: 382e 302e 342b 3264 3765 6561 3235 3239  8.0.4+2d7eea2529
-00002410: 3634 6536 3962 6539 3463 6239 6338 3437  64e69be94cb9c847
-00002420: 6233 3731 6232 3365 3464 6434 3730 006c  b371b23e4dd470.l
-00002430: 616e 6775 6167 652d 7665 7273 696f 6e00  anguage-version.
-00002440: 7072 6576 6965 7700 6e75 6c6c 6162 6c65  preview.nullable
-00002450: 0045 6e61 626c 6500 6465 6669 6e65 0054  .Enable.define.T
-00002460: 5241 4345 2c52 454c 4541 5345 2c4e 4554  RACE,RELEASE,NET
-00002470: 2c4e 4554 365f 302c 4e45 5443 4f52 4541  ,NET6_0,NETCOREA
-00002480: 5050 2c4e 4554 355f 305f 4f52 5f47 5245  PP,NET5_0_OR_GRE
-00002490: 4154 4552 2c4e 4554 365f 305f 4f52 5f47  ATER,NET6_0_OR_G
-000024a0: 5245 4154 4552 2c4e 4554 434f 5245 4150  REATER,NETCOREAP
-000024b0: 5031 5f30 5f4f 525f 4752 4541 5445 522c  P1_0_OR_GREATER,
-000024c0: 4e45 5443 4f52 4541 5050 315f 315f 4f52  NETCOREAPP1_1_OR
-000024d0: 5f47 5245 4154 4552 2c4e 4554 434f 5245  _GREATER,NETCORE
-000024e0: 4150 5032 5f30 5f4f 525f 4752 4541 5445  APP2_0_OR_GREATE
-000024f0: 522c 4e45 5443 4f52 4541 5050 325f 315f  R,NETCOREAPP2_1_
-00002500: 4f52 5f47 5245 4154 4552 2c4e 4554 434f  OR_GREATER,NETCO
-00002510: 5245 4150 5032 5f32 5f4f 525f 4752 4541  REAPP2_2_OR_GREA
-00002520: 5445 522c 4e45 5443 4f52 4541 5050 335f  TER,NETCOREAPP3_
-00002530: 305f 4f52 5f47 5245 4154 4552 2c4e 4554  0_OR_GREATER,NET
-00002540: 434f 5245 4150 5033 5f31 5f4f 525f 4752  COREAPP3_1_OR_GR
-00002550: 4541 5445 5200 a3ee 4943 5368 6172 7043  EATER...ICSharpC
-00002560: 6f64 652e 5368 6172 705a 6970 4c69 622e  ode.SharpZipLib.
-00002570: 646c 6c00 0001 6c99 0498 0080 0300 87d2  dll...l.........
-00002580: 8216 a495 d14a bd3f 1fc4 0213 b4ed 4d61  .....J.?......Ma
-00002590: 6372 6f73 732e 4a73 6f6e 2e45 7874 656e  cross.Json.Exten
-000025a0: 7369 6f6e 732e 646c 6c00 0001 55c4 78ba  sions.dll...U.x.
-000025b0: 0000 0100 b209 bad9 cad5 dc4e 93a4 2a22  ...........N..*"
-000025c0: b117 ec34 4d69 6372 6f73 6f66 742e 4353  ...4Microsoft.CS
-000025d0: 6861 7270 2e64 6c6c 0000 017c 2204 d600  harp.dll...|"...
-000025e0: 8000 0016 7189 67e2 0d98 499f e4b6 958b  ....q.g...I.....
-000025f0: 6529 264d 6963 726f 736f 6674 2e56 6973  e)&Microsoft.Vis
-00002600: 7561 6c42 6173 6963 2e43 6f72 652e 646c  ualBasic.Core.dl
-00002610: 6c00 0001 07b0 43b4 0020 0100 5570 1e38  l.....C.. ..Up.8
-00002620: 3a65 5047 920c db2f 521d e660 4d69 6372  :ePG.../R..`Micr
-00002630: 6f73 6f66 742e 5669 7375 616c 4261 7369  osoft.VisualBasi
-00002640: 632e 646c 6c00 0001 59d2 0ea3 0080 0000  c.dll...Y.......
-00002650: 345d 84dd 2e75 834e 8967 4190 6e86 58f3  4]...u.N.gA.n.X.
-00002660: 4d69 6372 6f73 6f66 742e 5769 6e33 322e  Microsoft.Win32.
-00002670: 5072 696d 6974 6976 6573 2e64 6c6c 0000  Primitives.dll..
-00002680: 0100 b02d e800 8000 00df 7a3b 0081 c19a  ...-......z;....
-00002690: 4399 9482 c7ee 7f37 744d 6963 726f 736f  C......7tMicroso
-000026a0: 6674 2e57 696e 3332 2e52 6567 6973 7472  ft.Win32.Registr
-000026b0: 792e 646c 6c00 0001 5ace 0088 00a0 0000  y.dll...Z.......
-000026c0: 9f25 45de 1bbe eb41 b891 e17a b367 eccc  .%E....A...z.g..
-000026d0: 6d73 636f 726c 6962 2e64 6c6c 0000 013d  mscorlib.dll...=
-000026e0: 1d0b d500 2001 002c 27ac 2e93 fac2 4297  .... ..,'.....B.
-000026f0: 7aeb e0b5 e264 f34e 6174 7572 616c 536f  z....d.NaturalSo
-00002700: 7274 2e45 7874 656e 7369 6f6e 2e64 6c6c  rt.Extension.dll
-00002710: 0000 01f8 cdb5 9e00 a000 005c dfe3 2353  ...........\..#S
-00002720: f79a 4bb5 43e2 52f8 16d1 b96e 6574 7374  ..K.C.R....netst
-00002730: 616e 6461 7264 2e64 6c6c 0000 0135 8697  andard.dll...5..
-00002740: 8400 c001 0033 f8a7 542f 006c 4a84 3dc1  .....3..T/.lJ.=.
-00002750: e3d2 2b67 3b50 726f 7065 7274 7943 6861  ..+g;PropertyCha
-00002760: 6e67 6564 2e64 6c6c 0000 018b 5a97 8a00  nged.dll....Z...
-00002770: 8000 0031 74ff 35d3 a634 4c90 ea21 b0de  ...1t.5..4L..!..
-00002780: 577f e053 6978 4c61 626f 7273 2e49 6d61  W..SixLabors.Ima
-00002790: 6765 5368 6172 702e 646c 6c00 0001 2e78  geSharp.dll....x
-000027a0: c49f 0040 2000 1201 6d04 683c 5747 b755  ...@ ...m.h<WG.U
-000027b0: 9c23 1bf1 cf27 5379 7374 656d 2e41 7070  .#...'System.App
-000027c0: 436f 6e74 6578 742e 646c 6c00 0001 4d50  Context.dll...MP
-000027d0: a8d9 0080 0000 aff0 ccfc 1832 c545 b316  ...........2.E..
-000027e0: 922e 84af 5430 5379 7374 656d 2e42 7566  ....T0System.Buf
-000027f0: 6665 7273 2e64 6c6c 0000 01b1 be65 ed00  fers.dll.....e..
-00002800: 8000 0047 af5f ce12 fd8f 4796 3f7e 0f26  ...G._....G.?~.&
-00002810: 3136 a653 7973 7465 6d2e 436f 6c6c 6563  16.System.Collec
-00002820: 7469 6f6e 732e 436f 6e63 7572 7265 6e74  tions.Concurrent
-00002830: 2e64 6c6c 0000 01ca def0 ff00 a000 0094  .dll............
-00002840: 4c75 4035 0226 44a7 a998 8fce e67a 8253  Lu@5.&D......z.S
-00002850: 7973 7465 6d2e 436f 6c6c 6563 7469 6f6e  ystem.Collection
-00002860: 732e 646c 6c00 0001 61d0 9f89 0000 0100  s.dll...a.......
-00002870: 13d2 f48b 8c41 aa44 84d8 d0d2 c9c3 0c03  .....A.D........
-00002880: 5379 7374 656d 2e43 6f6c 6c65 6374 696f  System.Collectio
-00002890: 6e73 2e49 6d6d 7574 6162 6c65 2e64 6c6c  ns.Immutable.dll
-000028a0: 0000 018a eea7 d100 4001 0001 2767 b021  ........@...'g.!
-000028b0: ff97 49ab e180 a5fa 2f86 f253 7973 7465  ..I...../..Syste
-000028c0: 6d2e 436f 6c6c 6563 7469 6f6e 732e 4e6f  m.Collections.No
-000028d0: 6e47 656e 6572 6963 2e64 6c6c 0000 01ae  nGeneric.dll....
-000028e0: 9af4 9600 a000 0025 7405 ad26 5084 41bc  .......%t..&P.A.
-000028f0: 1515 48f1 2d81 8453 7973 7465 6d2e 436f  ..H.-..System.Co
-00002900: 6c6c 6563 7469 6f6e 732e 5370 6563 6961  llections.Specia
-00002910: 6c69 7a65 642e 646c 6c00 0001 ff07 55fc  lized.dll.....U.
-00002920: 00a0 0000 4f28 e908 c4d2 ae45 a67e ab71  ....O(.....E.~.q
-00002930: 55c2 4b93 5379 7374 656d 2e43 6f6d 706f  U.K.System.Compo
-00002940: 6e65 6e74 4d6f 6465 6c2e 416e 6e6f 7461  nentModel.Annota
-00002950: 7469 6f6e 732e 646c 6c00 0001 0c51 26af  tions.dll....Q&.
-00002960: 00c0 0000 efe3 dfb3 26fb 3448 80cb b228  ........&.4H...(
-00002970: 3ad2 49f2 5379 7374 656d 2e43 6f6d 706f  :.I.System.Compo
-00002980: 6e65 6e74 4d6f 6465 6c2e 4461 7461 416e  nentModel.DataAn
-00002990: 6e6f 7461 7469 6f6e 732e 646c 6c00 0001  notations.dll...
-000029a0: 4d13 9da1 0080 0000 aba3 4449 7c47 bd41  M.........DI|G.A
-000029b0: 8c08 67c1 622e bd39 5379 7374 656d 2e43  ..g.b..9System.C
-000029c0: 6f6d 706f 6e65 6e74 4d6f 6465 6c2e 646c  omponentModel.dl
-000029d0: 6c00 0001 5264 cfd2 0080 0000 2bfd 8001  l...Rd......+...
-000029e0: c597 694f a94b f878 8b1c 59df 5379 7374  ..iO.K.x..Y.Syst
-000029f0: 656d 2e43 6f6d 706f 6e65 6e74 4d6f 6465  em.ComponentMode
-00002a00: 6c2e 4576 656e 7442 6173 6564 4173 796e  l.EventBasedAsyn
-00002a10: 632e 646c 6c00 0001 b5d5 e6fa 0080 0000  c.dll...........
-00002a20: eb54 62cf 5be2 9c4a 9b7c 33aa ace4 0115  .Tb.[..J.|3.....
-00002a30: 5379 7374 656d 2e43 6f6d 706f 6e65 6e74  System.Component
-00002a40: 4d6f 6465 6c2e 5072 696d 6974 6976 6573  Model.Primitives
-00002a50: 2e64 6c6c 0000 01b5 702e 9200 a000 002a  .dll....p......*
-00002a60: 50cd 0787 ca46 4c89 fb13 a899 5816 4f53  P....FL.....X.OS
-00002a70: 7973 7465 6d2e 436f 6d70 6f6e 656e 744d  ystem.ComponentM
-00002a80: 6f64 656c 2e54 7970 6543 6f6e 7665 7274  odel.TypeConvert
-00002a90: 6572 2e64 6c6c 0000 01ad 0772 dd00 c001  er.dll.....r....
-00002aa0: 00b0 7832 023d fdbd 4596 e3dd fe88 a5a5  ..x2.=..E.......
-00002ab0: 8453 7973 7465 6d2e 436f 6e66 6967 7572  .System.Configur
-00002ac0: 6174 696f 6e2e 646c 6c00 0001 72ca 1df7  ation.dll...r...
-00002ad0: 0080 0000 35ba 4be7 c40f af43 9eb0 a71e  ....5.K....C....
-00002ae0: 21bb ac3f 5379 7374 656d 2e43 6f6e 736f  !..?System.Conso
-00002af0: 6c65 2e64 6c6c 0000 01ac 8fcd c600 a000  le.dll..........
-00002b00: 00ce e7f4 7b4b cf4f 40aa 5f9f f8c0 653e  ....{K.O@._...e>
-00002b10: e153 7973 7465 6d2e 436f 7265 2e64 6c6c  .System.Core.dll
-00002b20: 0000 01eb 351e 8b00 a000 00f2 3d70 71e1  ....5.......=pq.
-00002b30: 4935 47ae 49f8 6f63 d6e4 3253 7973 7465  I5G.I.oc..2Syste
-00002b40: 6d2e 4461 7461 2e43 6f6d 6d6f 6e2e 646c  m.Data.Common.dl
-00002b50: 6c00 0001 6609 a2b0 0080 0200 a097 f52b  l...f..........+
-00002b60: ac3b 234f a897 8d88 27cd 7183 5379 7374  .;#O....'.q.Syst
-00002b70: 656d 2e44 6174 612e 4461 7461 5365 7445  em.Data.DataSetE
-00002b80: 7874 656e 7369 6f6e 732e 646c 6c00 0001  xtensions.dll...
-00002b90: 5190 7af7 0080 0000 dd38 6b86 8111 3b44  Q.z......8k...;D
-00002ba0: 99db aee2 7fa6 2e40 5379 7374 656d 2e44  .......@System.D
-00002bb0: 6174 612e 646c 6c00 0001 02eb 4cd5 00a0  ata.dll.....L...
-00002bc0: 0000 d077 d334 88c1 594e 87d3 9485 24a1  ...w.4..YN....$.
-00002bd0: 4bcd 5379 7374 656d 2e44 6961 676e 6f73  K.System.Diagnos
-00002be0: 7469 6373 2e43 6f6e 7472 6163 7473 2e64  tics.Contracts.d
-00002bf0: 6c6c 0000 01cb 95e7 e300 8000 0045 403e  ll...........E@>
-00002c00: 01b0 ae66 43b5 73a6 f0bd 072b 8c53 7973  ...fC.s....+.Sys
-00002c10: 7465 6d2e 4469 6167 6e6f 7374 6963 732e  tem.Diagnostics.
-00002c20: 4465 6275 672e 646c 6c00 0001 ef6e f4ab  Debug.dll....n..
-00002c30: 0080 0000 446d d735 770d 7e4a 86f1 b6ad  ....Dm.5w.~J....
-00002c40: e2fc b545 5379 7374 656d 2e44 6961 676e  ...ESystem.Diagn
-00002c50: 6f73 7469 6373 2e44 6961 676e 6f73 7469  ostics.Diagnosti
-00002c60: 6353 6f75 7263 652e 646c 6c00 0001 6cc9  cSource.dll...l.
-00002c70: 31e7 00c0 0000 7cb8 30b8 de3a 7d46 9897  1.....|.0..:}F..
-00002c80: 543d 4da7 a255 5379 7374 656d 2e44 6961  T=M..USystem.Dia
-00002c90: 676e 6f73 7469 6373 2e46 696c 6556 6572  gnostics.FileVer
-00002ca0: 7369 6f6e 496e 666f 2e64 6c6c 0000 0194  sionInfo.dll....
-00002cb0: 30c1 a000 8000 008a d9d0 1cf2 902a 4195  0............*A.
-00002cc0: 5ef8 f8bc 6c1b 7953 7973 7465 6d2e 4469  ^...l.ySystem.Di
-00002cd0: 6167 6e6f 7374 6963 732e 5072 6f63 6573  agnostics.Proces
-00002ce0: 732e 646c 6c00 0001 9bc0 a5e3 00c0 0000  s.dll...........
-00002cf0: 780f 998a 29ad cc44 a618 471a 7044 b3c6  x...)..D..G.pD..
-00002d00: 5379 7374 656d 2e44 6961 676e 6f73 7469  System.Diagnosti
-00002d10: 6373 2e53 7461 636b 5472 6163 652e 646c  cs.StackTrace.dl
-00002d20: 6c00 0001 8a88 a0dd 00a0 0000 08e3 1679  l..............y
-00002d30: 64e7 ee4f 9315 eac7 8e43 b29b 5379 7374  d..O.....C..Syst
-00002d40: 656d 2e44 6961 676e 6f73 7469 6373 2e54  em.Diagnostics.T
-00002d50: 6578 7457 7269 7465 7254 7261 6365 4c69  extWriterTraceLi
-00002d60: 7374 656e 6572 2e64 6c6c 0000 01df 6fbe  stener.dll....o.
-00002d70: ac00 8000 0097 ef5a e78c 5724 4abe e6df  .......Z..W$J...
-00002d80: 315f b57c d153 7973 7465 6d2e 4469 6167  1_.|.System.Diag
-00002d90: 6e6f 7374 6963 732e 546f 6f6c 732e 646c  nostics.Tools.dl
-00002da0: 6c00 0001 96fd d2ad 0080 0000 9511 a170  l..............p
-00002db0: ca4f e74c a131 e506 a771 3d06 5379 7374  .O.L.1...q=.Syst
-00002dc0: 656d 2e44 6961 676e 6f73 7469 6373 2e54  em.Diagnostics.T
-00002dd0: 7261 6365 536f 7572 6365 2e64 6c6c 0000  raceSource.dll..
-00002de0: 0112 4e28 8b00 a000 003d eef4 b9ec da39  ..N(.....=.....9
-00002df0: 4189 ec4f 89d5 62a7 1253 7973 7465 6d2e  A..O..b..System.
-00002e00: 4469 6167 6e6f 7374 6963 732e 5472 6163  Diagnostics.Trac
-00002e10: 696e 672e 646c 6c00 0001 7427 47de 00a0  ing.dll...t'G...
-00002e20: 0000 afc5 2f8a 7c63 564f adf5 c142 03aa  ..../.|cVO...B..
-00002e30: 3f9d 5379 7374 656d 2e64 6c6c 0000 01ff  ?.System.dll....
-00002e40: 56ed 8f00 0001 0039 ec84 68a7 c2f0 459e  V......9..h...E.
-00002e50: 7b60 2836 d5a8 8253 7973 7465 6d2e 4472  {`(6...System.Dr
-00002e60: 6177 696e 672e 436f 6d6d 6f6e 2e64 6c6c  awing.Common.dll
-00002e70: 0000 0121 8d42 d500 2002 0008 43fe c06a  ...!.B.. ...C..j
-00002e80: 78bb 469f 62dc 8ac5 b55a bc53 7973 7465  x.F.b....Z.Syste
-00002e90: 6d2e 4472 6177 696e 672e 646c 6c00 0001  m.Drawing.dll...
-00002ea0: 2a2a 6a8e 0080 0000 1f08 2022 54a5 9540  **j....... "T..@
-00002eb0: b3fd 69a8 528f 5cb8 5379 7374 656d 2e44  ..i.R.\.System.D
-00002ec0: 7261 7769 6e67 2e50 7269 6d69 7469 7665  rawing.Primitive
-00002ed0: 732e 646c 6c00 0001 f325 bbcc 00c0 0000  s.dll....%......
-00002ee0: b6c1 508a eb03 9c45 a956 cc45 1059 358d  ..P....E.V.E.Y5.
-00002ef0: 5379 7374 656d 2e44 796e 616d 6963 2e52  System.Dynamic.R
-00002f00: 756e 7469 6d65 2e64 6c6c 0000 0173 6bc1  untime.dll...sk.
-00002f10: fa00 8000 004d 534f 0722 30f6 4aa5 79e3  .....MSO."0.J.y.
-00002f20: ed4d ffa1 9153 7973 7465 6d2e 466f 726d  .M...System.Form
-00002f30: 6174 732e 4173 6e31 2e64 6c6c 0000 01b0  ats.Asn1.dll....
-00002f40: de6f c500 a000 002a 8801 9410 fc70 49ba  .o.....*.....pI.
-00002f50: dae8 8f98 0037 b853 7973 7465 6d2e 476c  .....7.System.Gl
-00002f60: 6f62 616c 697a 6174 696f 6e2e 4361 6c65  obalization.Cale
-00002f70: 6e64 6172 732e 646c 6c00 0001 5591 bd96  ndars.dll...U...
-00002f80: 0080 0000 b850 3341 a970 ee4a 95ad 287a  .....P3A.p.J..(z
-00002f90: cc4e 3079 5379 7374 656d 2e47 6c6f 6261  .N0ySystem.Globa
-00002fa0: 6c69 7a61 7469 6f6e 2e64 6c6c 0000 01d3  lization.dll....
-00002fb0: 93c2 a200 8000 00b5 fa72 22d5 c191 48ab  .........r"...H.
-00002fc0: c142 d510 62f9 ad53 7973 7465 6d2e 476c  .B..b..System.Gl
-00002fd0: 6f62 616c 697a 6174 696f 6e2e 4578 7465  obalization.Exte
-00002fe0: 6e73 696f 6e73 2e64 6c6c 0000 0156 572b  nsions.dll...VW+
-00002ff0: fb00 8000 0036 75c6 196a 81da 4b96 8ea5  .....6u..j..K...
-00003000: 9f98 49ff 1353 7973 7465 6d2e 494f 2e43  ..I..System.IO.C
-00003010: 6f6d 7072 6573 7369 6f6e 2e42 726f 746c  ompression.Brotl
-00003020: 692e 646c 6c00 0001 6fa6 6c90 0080 0000  i.dll...o.l.....
-00003030: 876f 5409 fff8 cf40 ba93 e63a e707 cb11  .oT....@...:....
-00003040: 5379 7374 656d 2e49 4f2e 436f 6d70 7265  System.IO.Compre
-00003050: 7373 696f 6e2e 646c 6c00 0001 3343 f1b8  ssion.dll...3C..
-00003060: 00a0 0000 5996 e666 875d 664f 8ae6 1a43  ....Y..f.]fO...C
-00003070: 931a 4794 5379 7374 656d 2e49 4f2e 436f  ..G.System.IO.Co
-00003080: 6d70 7265 7373 696f 6e2e 4669 6c65 5379  mpression.FileSy
-00003090: 7374 656d 2e64 6c6c 0000 0197 c05e af00  stem.dll.....^..
-000030a0: 8000 0003 510c 2eb9 976c 49af 7934 44de  ....Q....lI.y4D.
-000030b0: 47ec 7153 7973 7465 6d2e 494f 2e43 6f6d  G.qSystem.IO.Com
-000030c0: 7072 6573 7369 6f6e 2e5a 6970 4669 6c65  pression.ZipFile
-000030d0: 2e64 6c6c 0000 0181 9db4 a800 8000 0007  .dll............
-000030e0: 8c19 34db 832e 4fbd 0b34 ca13 74cd bb53  ..4...O..4..t..S
-000030f0: 7973 7465 6d2e 494f 2e64 6c6c 0000 01e2  ystem.IO.dll....
-00003100: 9925 e600 8000 0007 98f2 3dd8 4272 46bd  .%........=.BrF.
-00003110: 1391 1604 6aa6 a353 7973 7465 6d2e 494f  ....j..System.IO
-00003120: 2e46 696c 6553 7973 7465 6d2e 4163 6365  .FileSystem.Acce
-00003130: 7373 436f 6e74 726f 6c2e 646c 6c00 0001  ssControl.dll...
-00003140: 3fd0 5597 00a0 0000 17d4 ec7f b5e8 b14c  ?.U............L
-00003150: bb03 1e52 ff02 d440 5379 7374 656d 2e49  ...R...@System.I
-00003160: 4f2e 4669 6c65 5379 7374 656d 2e64 6c6c  O.FileSystem.dll
-00003170: 0000 011c d495 e600 8000 0014 424e 9f45  ............BN.E
-00003180: ebcc 4fae 2133 7581 1bf3 7353 7973 7465  ..O.!3u...sSyste
-00003190: 6d2e 494f 2e46 696c 6553 7973 7465 6d2e  m.IO.FileSystem.
-000031a0: 4472 6976 6549 6e66 6f2e 646c 6c00 0001  DriveInfo.dll...
-000031b0: fd4e a4c3 0080 0000 ab96 b45c 7c8c 7442  .N.........\|.tB
-000031c0: 8136 3c24 d204 2696 5379 7374 656d 2e49  .6<$..&.System.I
-000031d0: 4f2e 4669 6c65 5379 7374 656d 2e50 7269  O.FileSystem.Pri
-000031e0: 6d69 7469 7665 732e 646c 6c00 0001 8a78  mitives.dll....x
-000031f0: b296 0080 0000 9d2c 347d b319 8246 b5cb  .......,4}...F..
-00003200: 9462 2859 72da 5379 7374 656d 2e49 4f2e  .b(Yr.System.IO.
-00003210: 4669 6c65 5379 7374 656d 2e57 6174 6368  FileSystem.Watch
-00003220: 6572 2e64 6c6c 0000 01ab 2c4c f200 a000  er.dll....,L....
-00003230: 0002 e409 8ed7 6a56 4299 bcca df1b 62f7  ......jVB.....b.
-00003240: 0a53 7973 7465 6d2e 494f 2e49 736f 6c61  .System.IO.Isola
-00003250: 7465 6453 746f 7261 6765 2e64 6c6c 0000  tedStorage.dll..
-00003260: 01e6 371c bd00 a000 00ff e50c 2fa0 7ae5  ..7........./.z.
-00003270: 4292 536a 977c 8798 4053 7973 7465 6d2e  B.Sj.|..@System.
-00003280: 494f 2e4d 656d 6f72 794d 6170 7065 6446  IO.MemoryMappedF
-00003290: 696c 6573 2e64 6c6c 0000 01b7 5217 9b00  iles.dll....R...
-000032a0: 8000 002b 3bd8 f4b4 835f 4cab d034 4f2b  ...+;...._L..4O+
-000032b0: fff1 2353 7973 7465 6d2e 494f 2e50 6970  ..#System.IO.Pip
-000032c0: 6573 2e41 6363 6573 7343 6f6e 7472 6f6c  es.AccessControl
-000032d0: 2e64 6c6c 0000 01ea 29da e400 8000 0053  .dll....)......S
-000032e0: ff95 6671 0e69 45ad 3154 de9d 5279 8453  ..fq.iE.1T..Ry.S
-000032f0: 7973 7465 6d2e 494f 2e50 6970 6573 2e64  ystem.IO.Pipes.d
-00003300: 6c6c 0000 0151 3f62 b000 a000 006f 2048  ll...Q?b.....o H
-00003310: 042d 2462 4b9b 13fb f078 9048 f453 7973  .-$bK....x.H.Sys
-00003320: 7465 6d2e 494f 2e55 6e6d 616e 6167 6564  tem.IO.Unmanaged
-00003330: 4d65 6d6f 7279 5374 7265 616d 2e64 6c6c  MemoryStream.dll
-00003340: 0000 0107 2bd2 fd00 8000 001b c381 5b54  ....+.........[T
-00003350: 1bda 499e f5b6 5ff6 b0f9 7853 7973 7465  ..I..._...xSyste
-00003360: 6d2e 4c69 6e71 2e64 6c6c 0000 0177 e4a2  m.Linq.dll...w..
-00003370: 9700 c000 0063 bf95 d3d7 c50c 4cb9 4bcc  .....c......L.K.
-00003380: 773c 5268 4b53 7973 7465 6d2e 4c69 6e71  w<RhKSystem.Linq
-00003390: 2e45 7870 7265 7373 696f 6e73 2e64 6c6c  .Expressions.dll
-000033a0: 0000 0193 93df a700 4001 007c d583 c885  ........@..|....
-000033b0: 3466 4b9e 7925 60c6 ad7a 0253 7973 7465  4fK.y%`..z.Syste
-000033c0: 6d2e 4c69 6e71 2e50 6172 616c 6c65 6c2e  m.Linq.Parallel.
-000033d0: 646c 6c00 0001 6732 79da 00c0 0000 c027  dll...g2y......'
-000033e0: afbe ce3c 8b46 8eff fa93 f614 5b23 5379  ...<.F......[#Sy
-000033f0: 7374 656d 2e4c 696e 712e 5175 6572 7961  stem.Linq.Querya
-00003400: 626c 652e 646c 6c00 0001 5b75 c9c4 00c0  ble.dll...[u....
-00003410: 0000 ff79 ec75 6680 4f49 9dbb 90e4 e4eb  ...y.uf.OI......
-00003420: 04ff 5379 7374 656d 2e4d 656d 6f72 792e  ..System.Memory.
-00003430: 646c 6c00 0001 4b13 3ec2 00e0 0000 dc97  dll...K.>.......
-00003440: ddaa 672a 3943 b478 7343 8693 5ee5 5379  ..g*9C.xsC..^.Sy
-00003450: 7374 656d 2e4e 6574 2e64 6c6c 0000 0166  stem.Net.dll...f
-00003460: 55a4 d400 8000 0022 fe7b 1bd4 32cc 4b8a  U......".{..2.K.
-00003470: 4983 ec73 ba3c f053 7973 7465 6d2e 4e65  I..s.<.System.Ne
-00003480: 742e 4874 7470 2e64 6c6c 0000 01f4 f7b2  t.Http.dll......
-00003490: e900 2001 0092 8754 8bdb 94c0 4486 a268  .. ....T....D..h
-000034a0: 7c79 f1bd ad53 7973 7465 6d2e 4e65 742e  |y...System.Net.
-000034b0: 4874 7470 2e4a 736f 6e2e 646c 6c00 0001  Http.Json.dll...
-000034c0: 2a11 bef4 0080 0000 0a15 1b13 bfc1 544e  *.............TN
-000034d0: ab15 89e7 1147 5efb 5379 7374 656d 2e4e  .....G^.System.N
-000034e0: 6574 2e48 7474 704c 6973 7465 6e65 722e  et.HttpListener.
-000034f0: 646c 6c00 0001 784e e4b3 00a0 0000 0949  dll...xN.......I
-00003500: 3ab6 82cc cc4c 9fa0 29cd 9336 88a9 5379  :....L..)..6..Sy
-00003510: 7374 656d 2e4e 6574 2e4d 6169 6c2e 646c  stem.Net.Mail.dl
-00003520: 6c00 0001 0a76 fbf4 00c0 0000 368f d753  l....v......6..S
-00003530: 1c03 0940 8269 218c 08d9 18ee 5379 7374  ...@.i!.....Syst
-00003540: 656d 2e4e 6574 2e4e 616d 6552 6573 6f6c  em.Net.NameResol
-00003550: 7574 696f 6e2e 646c 6c00 0001 6237 30c0  ution.dll...b70.
-00003560: 0080 0000 2bf6 bd89 228b d24e 817b e3a8  ....+..."..N.{..
-00003570: 4211 7d39 5379 7374 656d 2e4e 6574 2e4e  B.}9System.Net.N
-00003580: 6574 776f 726b 496e 666f 726d 6174 696f  etworkInformatio
-00003590: 6e2e 646c 6c00 0001 acdf aba3 00c0 0000  n.dll...........
-000035a0: 5172 c718 c3ca a84d ad97 e585 f8c2 46f5  Qr.....M......F.
-000035b0: 5379 7374 656d 2e4e 6574 2e50 696e 672e  System.Net.Ping.
-000035c0: 646c 6c00 0001 8a29 5d99 0080 0000 ef33  dll....)]......3
-000035d0: 029e 4180 3f4d b11e a57e 9583 488a 5379  ..A.?M...~..H.Sy
-000035e0: 7374 656d 2e4e 6574 2e50 7269 6d69 7469  stem.Net.Primiti
-000035f0: 7665 732e 646c 6c00 0001 fc53 6acc 00c0  ves.dll....Sj...
-00003600: 0000 3cca 5e61 60de 824f 9eab 45c6 5361  ..<.^a`..O..E.Sa
-00003610: 5635 5379 7374 656d 2e4e 6574 2e52 6571  V5System.Net.Req
-00003620: 7565 7374 732e 646c 6c00 0001 329d 63f3  uests.dll...2.c.
-00003630: 00e0 0000 a6e5 e890 4c14 874b 9f1a 5b64  ........L..K..[d
-00003640: f896 83cc 5379 7374 656d 2e4e 6574 2e53  ....System.Net.S
-00003650: 6563 7572 6974 792e 646c 6c00 0001 b13b  ecurity.dll....;
-00003660: dec4 0000 0100 125e 7a1b 1b0e dc4f bb61  .......^z....O.a
-00003670: 01f5 368f f0a6 5379 7374 656d 2e4e 6574  ..6...System.Net
-00003680: 2e53 6572 7669 6365 506f 696e 742e 646c  .ServicePoint.dl
-00003690: 6c00 0001 cb80 da94 0080 0000 6f67 4290  l...........ogB.
-000036a0: b49a d542 bbbe c31a 37ff c556 5379 7374  ...B....7..VSyst
-000036b0: 656d 2e4e 6574 2e53 6f63 6b65 7473 2e64  em.Net.Sockets.d
-000036c0: 6c6c 0000 01f8 14c4 e600 0001 006b d208  ll...........k..
-000036d0: 6afd d730 4882 580b b31d f7ee c153 7973  j..0H.X......Sys
-000036e0: 7465 6d2e 4e65 742e 5765 6243 6c69 656e  tem.Net.WebClien
-000036f0: 742e 646c 6c00 0001 003f 9bdc 00a0 0000  t.dll....?......
-00003700: 1944 f1e5 da53 264d bd95 9b29 3227 34b4  .D...S&M...)2'4.
-00003710: 5379 7374 656d 2e4e 6574 2e57 6562 4865  System.Net.WebHe
-00003720: 6164 6572 436f 6c6c 6563 7469 6f6e 2e64  aderCollection.d
-00003730: 6c6c 0000 01d2 7c25 ae00 8000 005f c943  ll....|%....._.C
-00003740: c103 d805 48b7 1a77 3f16 bb73 d053 7973  ....H..w?..s.Sys
-00003750: 7465 6d2e 4e65 742e 5765 6250 726f 7879  tem.Net.WebProxy
-00003760: 2e64 6c6c 0000 01df 3a5d f200 8000 007e  .dll....:].....~
-00003770: f5e9 4599 7649 4882 c33c 2154 2506 6153  ..E.vIH..<!T%.aS
-00003780: 7973 7465 6d2e 4e65 742e 5765 6253 6f63  ystem.Net.WebSoc
-00003790: 6b65 7473 2e43 6c69 656e 742e 646c 6c00  kets.Client.dll.
-000037a0: 0001 9ab6 d0f0 0080 0000 ef4b 528a 0af8  ...........KR...
-000037b0: db40 a280 5731 c31f 2c8c 5379 7374 656d  .@..W1..,.System
-000037c0: 2e4e 6574 2e57 6562 536f 636b 6574 732e  .Net.WebSockets.
-000037d0: 646c 6c00 0001 88e3 ebbe 00a0 0000 c61e  dll.............
-000037e0: 499b 5f9a 2241 ae0c e8d6 ab97 6672 5379  I._."A......frSy
-000037f0: 7374 656d 2e4e 756d 6572 6963 732e 646c  stem.Numerics.dl
-00003800: 6c00 0001 7e2b e3e1 0080 0000 af9b fb46  l...~+.........F
-00003810: feaa eb4f 82da 1085 6f2a e185 5379 7374  ...O....o*..Syst
-00003820: 656d 2e4e 756d 6572 6963 732e 5665 6374  em.Numerics.Vect
-00003830: 6f72 732e 646c 6c00 0001 3758 e2ca 00c0  ors.dll...7X....
-00003840: 0000 4031 8c61 396e 8142 ab1c 2c46 1daf  ..@1.a9n.B..,F..
-00003850: b931 5379 7374 656d 2e4f 626a 6563 744d  .1System.ObjectM
-00003860: 6f64 656c 2e64 6c6c 0000 0174 62e5 9000  odel.dll...tb...
-00003870: c000 0077 f973 8329 f67f 468d d56b 5131  ...w.s.)..F..kQ1
-00003880: 2ccc d853 7973 7465 6d2e 5265 666c 6563  ,..System.Reflec
-00003890: 7469 6f6e 2e44 6973 7061 7463 6850 726f  tion.DispatchPro
-000038a0: 7879 2e64 6c6c 0000 014b ae13 b200 8000  xy.dll...K......
-000038b0: 008a 29a1 2275 5510 4b9e d40d c66e e1cb  ..)."uU.K....n..
-000038c0: ed53 7973 7465 6d2e 5265 666c 6563 7469  .System.Reflecti
-000038d0: 6f6e 2e64 6c6c 0000 0186 1a3f 8b00 8000  on.dll.....?....
-000038e0: 0040 eaf1 8d30 37c4 44a8 2c08 af7b 2c79  .@...07.D.,..{,y
-000038f0: d053 7973 7465 6d2e 5265 666c 6563 7469  .System.Reflecti
-00003900: 6f6e 2e45 6d69 742e 646c 6c00 0001 6226  on.Emit.dll...b&
-00003910: 01ad 00e0 0000 4994 5b80 b83f 384c a6a5  ......I.[..?8L..
-00003920: 9ac5 d465 987f 5379 7374 656d 2e52 6566  ...e..System.Ref
-00003930: 6c65 6374 696f 6e2e 456d 6974 2e49 4c47  lection.Emit.ILG
-00003940: 656e 6572 6174 696f 6e2e 646c 6c00 0001  eneration.dll...
-00003950: 7efb 1fe4 00a0 0000 7cfa 0633 58f3 204c  ~.......|..3X. L
-00003960: 9c0e e801 6a04 d954 5379 7374 656d 2e52  ....j..TSystem.R
-00003970: 6566 6c65 6374 696f 6e2e 456d 6974 2e4c  eflection.Emit.L
-00003980: 6967 6874 7765 6967 6874 2e64 6c6c 0000  ightweight.dll..
-00003990: 015e 1869 9700 8000 006c 0566 7e62 7699  .^.i.....l.f~bv.
-000039a0: 4e9f bad4 c335 f59c da53 7973 7465 6d2e  N....5...System.
-000039b0: 5265 666c 6563 7469 6f6e 2e45 7874 656e  Reflection.Exten
-000039c0: 7369 6f6e 732e 646c 6c00 0001 a887 73dd  sions.dll.....s.
-000039d0: 0080 0000 5ca1 30be 0a3b 6144 85f3 a098  ....\.0..;aD....
-000039e0: c8eb 5157 5379 7374 656d 2e52 6566 6c65  ..QWSystem.Refle
-000039f0: 6374 696f 6e2e 4d65 7461 6461 7461 2e64  ction.Metadata.d
-00003a00: 6c6c 0000 01bb ffe9 a400 2002 0085 75e0  ll........ ...u.
-00003a10: 7b44 8af3 489a c5ea 78e7 23b1 f753 7973  {D..H...x.#..Sys
-00003a20: 7465 6d2e 5265 666c 6563 7469 6f6e 2e50  tem.Reflection.P
-00003a30: 7269 6d69 7469 7665 732e 646c 6c00 0001  rimitives.dll...
-00003a40: 61db 35b9 00a0 0000 897c c354 20a5 ca49  a.5......|.T ..I
-00003a50: b721 c276 ac7e c601 5379 7374 656d 2e52  .!.v.~..System.R
-00003a60: 6566 6c65 6374 696f 6e2e 5479 7065 4578  eflection.TypeEx
-00003a70: 7465 6e73 696f 6e73 2e64 6c6c 0000 017d  tensions.dll...}
-00003a80: f567 ce00 8000 00e4 64f2 52ae 5a19 41bc  .g......d.R.Z.A.
-00003a90: 8225 a3c2 4a98 2c53 7973 7465 6d2e 5265  .%..J.,System.Re
-00003aa0: 736f 7572 6365 732e 5265 6164 6572 2e64  sources.Reader.d
-00003ab0: 6c6c 0000 014f 41bb e100 8000 00e8 6885  ll...OA.......h.
-00003ac0: c73f e7dc 418e 57eb 7a20 85eb 1a53 7973  .?..A.W.z ...Sys
-00003ad0: 7465 6d2e 5265 736f 7572 6365 732e 5265  tem.Resources.Re
-00003ae0: 736f 7572 6365 4d61 6e61 6765 722e 646c  sourceManager.dl
-00003af0: 6c00 0001 0b09 3b8c 0080 0000 c2ca 7b53  l.....;.......{S
-00003b00: de67 ad4b 8ce7 f5b9 b775 884e 5379 7374  .g.K.....u.NSyst
-00003b10: 656d 2e52 6573 6f75 7263 6573 2e57 7269  em.Resources.Wri
-00003b20: 7465 722e 646c 6c00 0001 6c27 5fba 0080  ter.dll...l'_...
-00003b30: 0000 e213 a7ec 90af e34c 9ade 4267 1993  .........L..Bg..
-00003b40: ec7e 5379 7374 656d 2e52 756e 7469 6d65  .~System.Runtime
-00003b50: 2e43 6f6d 7069 6c65 7253 6572 7669 6365  .CompilerService
-00003b60: 732e 556e 7361 6665 2e64 6c6c 0000 0157  s.Unsafe.dll...W
-00003b70: fd68 a800 8000 008b ba2d fd2f f22b 448e  .h.......-./.+D.
-00003b80: 7fa0 2cb5 8be2 9453 7973 7465 6d2e 5275  ..,....System.Ru
-00003b90: 6e74 696d 652e 436f 6d70 696c 6572 5365  ntime.CompilerSe
-00003ba0: 7276 6963 6573 2e56 6973 7561 6c43 2e64  rvices.VisualC.d
-00003bb0: 6c6c 0000 0157 defb b100 8000 007a 364e  ll...W.......z6N
-00003bc0: f34e 6d1d 4780 27b3 1fc2 af71 eb53 7973  .Nm.G.'....q.Sys
-00003bd0: 7465 6d2e 5275 6e74 696d 652e 646c 6c00  tem.Runtime.dll.
-00003be0: 0001 efd8 25e4 0080 0700 8eb2 458f c943  ....%.......E..C
-00003bf0: b846 bdae a734 3e7b bf4a 5379 7374 656d  .F...4>{.JSystem
-00003c00: 2e52 756e 7469 6d65 2e45 7874 656e 7369  .Runtime.Extensi
-00003c10: 6f6e 732e 646c 6c00 0001 264d c184 0080  ons.dll...&M....
-00003c20: 0000 838d f7c1 6b7d 194f bd3a 128f 7bed  ......k}.O.:..{.
-00003c30: 227c 5379 7374 656d 2e52 756e 7469 6d65  "|System.Runtime
-00003c40: 2e48 616e 646c 6573 2e64 6c6c 0000 0195  .Handles.dll....
-00003c50: c14b e700 8000 00fa 9de2 d789 11f5 45ae  .K............E.
-00003c60: f1fe 5969 b6c8 8653 7973 7465 6d2e 5275  ..Yi...System.Ru
-00003c70: 6e74 696d 652e 496e 7465 726f 7053 6572  ntime.InteropSer
-00003c80: 7669 6365 732e 646c 6c00 0001 d8e0 55a1  vices.dll.....U.
-00003c90: 0040 0100 2198 a5f3 c676 6343 b827 dba7  .@..!....vcC.'..
-00003ca0: f0da b3a7 5379 7374 656d 2e52 756e 7469  ....System.Runti
-00003cb0: 6d65 2e49 6e74 6572 6f70 5365 7276 6963  me.InteropServic
-00003cc0: 6573 2e52 756e 7469 6d65 496e 666f 726d  es.RuntimeInform
-00003cd0: 6174 696f 6e2e 646c 6c00 0001 6dab f68c  ation.dll...m...
-00003ce0: 0080 0000 7ff2 aa55 2110 eb4e a470 398a  .......U!..N.p9.
-00003cf0: 5c01 2375 5379 7374 656d 2e52 756e 7469  \.#uSystem.Runti
-00003d00: 6d65 2e49 6e74 7269 6e73 6963 732e 646c  me.Intrinsics.dl
-00003d10: 6c00 0001 6ed7 f3ef 00c0 0200 ea72 6015  l...n........r`.
-00003d20: 0c00 8349 bccb e1c6 5d40 e38e 5379 7374  ...I....]@..Syst
-00003d30: 656d 2e52 756e 7469 6d65 2e4c 6f61 6465  em.Runtime.Loade
-00003d40: 722e 646c 6c00 0001 e7e1 35d1 0080 0000  r.dll.....5.....
-00003d50: c16d b42a 5814 754d aae5 51c6 709e c712  .m.*X.uM..Q.p...
-00003d60: 5379 7374 656d 2e52 756e 7469 6d65 2e4e  System.Runtime.N
-00003d70: 756d 6572 6963 732e 646c 6c00 0001 5d01  umerics.dll...].
-00003d80: ffc5 00a0 0000 f2fc 093c 2ba0 a945 b015  .........<+..E..
-00003d90: e4e4 d55f bbc0 5379 7374 656d 2e52 756e  ..._..System.Run
-00003da0: 7469 6d65 2e53 6572 6961 6c69 7a61 7469  time.Serializati
-00003db0: 6f6e 2e64 6c6c 0000 010c aaea fb00 8000  on.dll..........
-00003dc0: 003b cf23 3076 fb00 449d 84bb b517 3ed7  .;.#0v..D.....>.
-00003dd0: 2f53 7973 7465 6d2e 5275 6e74 696d 652e  /System.Runtime.
-00003de0: 5365 7269 616c 697a 6174 696f 6e2e 466f  Serialization.Fo
-00003df0: 726d 6174 7465 7273 2e64 6c6c 0000 0136  rmatters.dll...6
-00003e00: e772 ec00 a000 0049 d957 3758 deef 4fa6  .r.....I.W7X..O.
-00003e10: a2ea 1baa 5587 9d53 7973 7465 6d2e 5275  ....U..System.Ru
-00003e20: 6e74 696d 652e 5365 7269 616c 697a 6174  ntime.Serializat
-00003e30: 696f 6e2e 4a73 6f6e 2e64 6c6c 0000 0168  ion.Json.dll...h
-00003e40: b853 aa00 8000 0087 14ab 0a28 a87d 4cbe  .S.........(.}L.
-00003e50: 6ffb 2b93 8cb6 e553 7973 7465 6d2e 5275  o.+....System.Ru
-00003e60: 6e74 696d 652e 5365 7269 616c 697a 6174  ntime.Serializat
-00003e70: 696f 6e2e 5072 696d 6974 6976 6573 2e64  ion.Primitives.d
-00003e80: 6c6c 0000 017c ecaf c700 8000 0075 d3af  ll...|.......u..
-00003e90: a1f8 a9d3 4391 7c8b cfea 01e6 f453 7973  ....C.|......Sys
-00003ea0: 7465 6d2e 5275 6e74 696d 652e 5365 7269  tem.Runtime.Seri
-00003eb0: 616c 697a 6174 696f 6e2e 586d 6c2e 646c  alization.Xml.dl
-00003ec0: 6c00 0001 3150 2aa5 00c0 0000 e171 1117  l...1P*......q..
-00003ed0: dff5 b446 980b 1190 b086 a5d9 5379 7374  ...F........Syst
-00003ee0: 656d 2e53 6563 7572 6974 792e 4163 6365  em.Security.Acce
-00003ef0: 7373 436f 6e74 726f 6c2e 646c 6c00 0001  ssControl.dll...
-00003f00: 74a8 e9eb 00e0 0000 96e5 f328 3df5 b745  t..........(=..E
-00003f10: 94c1 b85d 78ec cd23 5379 7374 656d 2e53  ...]x..#System.S
-00003f20: 6563 7572 6974 792e 436c 6169 6d73 2e64  ecurity.Claims.d
-00003f30: 6c6c 0000 01c4 835c 8f00 c000 00e8 dfd1  ll.....\........
-00003f40: 112a 02a0 4d9e b434 33d2 7682 8953 7973  .*..M..43.v..Sys
-00003f50: 7465 6d2e 5365 6375 7269 7479 2e43 7279  tem.Security.Cry
-00003f60: 7074 6f67 7261 7068 792e 416c 676f 7269  ptography.Algori
-00003f70: 7468 6d73 2e64 6c6c 0000 01e7 1389 b800  thms.dll........
-00003f80: 0001 009a 0898 a128 c4e5 4bbc 10c0 1622  .......(..K...."
-00003f90: c43e c853 7973 7465 6d2e 5365 6375 7269  .>.System.Securi
-00003fa0: 7479 2e43 7279 7074 6f67 7261 7068 792e  ty.Cryptography.
-00003fb0: 436e 672e 646c 6c00 0001 4cdf 61d0 00c0  Cng.dll...L.a...
-00003fc0: 0000 63b9 c39b 068a d043 8d3f 9194 8ac4  ..c......C.?....
-00003fd0: d431 5379 7374 656d 2e53 6563 7572 6974  .1System.Securit
-00003fe0: 792e 4372 7970 746f 6772 6170 6879 2e43  y.Cryptography.C
-00003ff0: 7370 2e64 6c6c 0000 0102 a5a2 ce00 a000  sp.dll..........
-00004000: 0070 c61f 9839 a34a 49b5 8b10 d078 07ac  .p...9.JI....x..
-00004010: 1853 7973 7465 6d2e 5365 6375 7269 7479  .System.Security
-00004020: 2e43 7279 7074 6f67 7261 7068 792e 456e  .Cryptography.En
-00004030: 636f 6469 6e67 2e64 6c6c 0000 012a 0af7  coding.dll...*..
-00004040: c400 a000 0036 9210 c2cc ed84 4eb4 a8f3  .....6......N...
-00004050: d95a 6142 7153 7973 7465 6d2e 5365 6375  .ZaBqSystem.Secu
-00004060: 7269 7479 2e43 7279 7074 6f67 7261 7068  rity.Cryptograph
-00004070: 792e 4f70 656e 5373 6c2e 646c 6c00 0001  y.OpenSsl.dll...
-00004080: 4d3a f095 0080 0000 5fc4 5fb5 eb1e 8641  M:......_._....A
-00004090: 9bae 72c2 b788 b456 5379 7374 656d 2e53  ..r....VSystem.S
-000040a0: 6563 7572 6974 792e 4372 7970 746f 6772  ecurity.Cryptogr
-000040b0: 6170 6879 2e50 7269 6d69 7469 7665 732e  aphy.Primitives.
-000040c0: 646c 6c00 0001 1fcd 8582 00a0 0000 9140  dll............@
-000040d0: 05a2 4d89 ba4b 81f2 f3e2 9382 6372 5379  ..M..K......crSy
-000040e0: 7374 656d 2e53 6563 7572 6974 792e 4372  stem.Security.Cr
-000040f0: 7970 746f 6772 6170 6879 2e58 3530 3943  yptography.X509C
-00004100: 6572 7469 6669 6361 7465 732e 646c 6c00  ertificates.dll.
-00004110: 0001 756a 98e6 00e0 0000 318f bfbf 3224  ..uj......1...2$
-00004120: 7742 8a67 b0f0 4d50 00c2 5379 7374 656d  wB.g..MP..System
-00004130: 2e53 6563 7572 6974 792e 646c 6c00 0001  .Security.dll...
-00004140: 79a7 41e0 0080 0000 d3aa 5198 f404 d742  y.A.......Q....B
-00004150: 9981 16eb ffff 2e83 5379 7374 656d 2e53  ........System.S
-00004160: 6563 7572 6974 792e 5072 696e 6369 7061  ecurity.Principa
-00004170: 6c2e 646c 6c00 0001 296d 1586 0080 0000  l.dll...)m......
-00004180: f366 488e 3887 794c 8800 6abb 1daa c2b2  .fH.8.yL..j.....
-00004190: 5379 7374 656d 2e53 6563 7572 6974 792e  System.Security.
-000041a0: 5072 696e 6369 7061 6c2e 5769 6e64 6f77  Principal.Window
-000041b0: 732e 646c 6c00 0001 eda1 e8ee 00a0 0000  s.dll...........
-000041c0: 3fcb 9736 efa0 bd49 8aac b171 f892 4916  ?..6...I...q..I.
-000041d0: 5379 7374 656d 2e53 6563 7572 6974 792e  System.Security.
-000041e0: 5365 6375 7265 5374 7269 6e67 2e64 6c6c  SecureString.dll
-000041f0: 0000 017c 7bf7 cf00 8000 00e8 5160 734a  ...|{.......Q`sJ
-00004200: 8386 4a8d 436b 02c3 aef8 a753 7973 7465  ..J.Ck.....Syste
-00004210: 6d2e 5365 7276 6963 654d 6f64 656c 2e57  m.ServiceModel.W
-00004220: 6562 2e64 6c6c 0000 0185 cb7f f100 8000  eb.dll..........
-00004230: 0049 f78d c70e 896b 48b7 399f 270e eb5f  .I.....kH.9.'.._
-00004240: fb53 7973 7465 6d2e 5365 7276 6963 6550  .System.ServiceP
-00004250: 726f 6365 7373 2e64 6c6c 0000 016b 36e2  rocess.dll...k6.
-00004260: 9400 8000 008a c80a f204 32ec 429a 521f  ..........2.B.R.
-00004270: a5cb 81ef d553 7973 7465 6d2e 5465 7874  .....System.Text
-00004280: 2e45 6e63 6f64 696e 672e 436f 6465 5061  .Encoding.CodePa
-00004290: 6765 732e 646c 6c00 0001 98e0 72ab 0080  ges.dll.....r...
-000042a0: 0000 8da1 7385 74c7 624e b5e9 2889 a8e8  ....s.t.bN..(...
-000042b0: b61b 5379 7374 656d 2e54 6578 742e 456e  ..System.Text.En
-000042c0: 636f 6469 6e67 2e64 6c6c 0000 019d b404  coding.dll......
-000042d0: be00 8000 004c a879 7d1c 598b 49b3 6f7b  .....L.y}.Y.I.o{
-000042e0: a60f f6b6 4b53 7973 7465 6d2e 5465 7874  ....KSystem.Text
-000042f0: 2e45 6e63 6f64 696e 672e 4578 7465 6e73  .Encoding.Extens
-00004300: 696f 6e73 2e64 6c6c 0000 017c ac3c bc00  ions.dll...|.<..
-00004310: a000 00f0 a040 bc4d 09fa 42b8 c2a1 ce69  .....@.M..B....i
-00004320: 8718 5653 7973 7465 6d2e 5465 7874 2e45  ..VSystem.Text.E
-00004330: 6e63 6f64 696e 6773 2e57 6562 2e64 6c6c  ncodings.Web.dll
-00004340: 0000 0165 baf3 a600 a000 0024 6b95 05d4  ...e.......$k...
-00004350: 3f7e 4b8b 4e54 3e1a 58a9 8d53 7973 7465  ?~K.NT>.X..Syste
-00004360: 6d2e 5465 7874 2e4a 736f 6e2e 646c 6c00  m.Text.Json.dll.
-00004370: 0001 ca89 b181 0020 0100 f931 66e2 cf8e  ....... ...1f...
-00004380: ea46 aa7a 2319 c582 4739 5379 7374 656d  .F.z#...G9System
-00004390: 2e54 6578 742e 5265 6775 6c61 7245 7870  .Text.RegularExp
-000043a0: 7265 7373 696f 6e73 2e64 6c6c 0000 013f  ressions.dll...?
-000043b0: ba4b ca00 c000 00dc 194f 503f 05eb 4783  .K.......OP?..G.
-000043c0: 541e c241 4f79 ae53 7973 7465 6d2e 5468  T..AOy.System.Th
-000043d0: 7265 6164 696e 672e 4368 616e 6e65 6c73  reading.Channels
-000043e0: 2e64 6c6c 0000 0138 5d8b e500 8000 00de  .dll...8].......
-000043f0: 82b1 1dca ef07 42b4 c8e5 7083 38e2 5b53  ......B...p.8.[S
-00004400: 7973 7465 6d2e 5468 7265 6164 696e 672e  ystem.Threading.
-00004410: 646c 6c00 0001 368b f8ba 00c0 0000 0a34  dll...6........4
-00004420: ad89 f304 794c a695 9105 d140 3c92 5379  ....yL.....@<.Sy
-00004430: 7374 656d 2e54 6872 6561 6469 6e67 2e4f  stem.Threading.O
-00004440: 7665 726c 6170 7065 642e 646c 6c00 0001  verlapped.dll...
-00004450: 987d 5387 0080 0000 802d f65d 0f50 584a  .}S......-.].PXJ
-00004460: 8996 a612 3cd1 cff2 5379 7374 656d 2e54  ....<...System.T
-00004470: 6872 6561 6469 6e67 2e54 6173 6b73 2e44  hreading.Tasks.D
-00004480: 6174 6166 6c6f 772e 646c 6c00 0001 1577  ataflow.dll....w
-00004490: c8f4 00c0 0000 3fc8 a3e8 15f5 e44b b06c  ......?......K.l
-000044a0: becf ee6f 9331 5379 7374 656d 2e54 6872  ...o.1System.Thr
-000044b0: 6561 6469 6e67 2e54 6173 6b73 2e64 6c6c  eading.Tasks.dll
-000044c0: 0000 012a fc9f 9600 8000 0056 c2a1 bd8c  ...*.......V....
-000044d0: ff4e 4081 ee86 d5ed 9e88 1f53 7973 7465  .N@........Syste
-000044e0: 6d2e 5468 7265 6164 696e 672e 5461 736b  m.Threading.Task
-000044f0: 732e 4578 7465 6e73 696f 6e73 2e64 6c6c  s.Extensions.dll
-00004500: 0000 01ab 5ba5 eb00 8000 005b ac34 9315  ....[......[.4..
-00004510: 4aac 4d84 8c58 0881 36bf 9a53 7973 7465  J.M..X..6..Syste
-00004520: 6d2e 5468 7265 6164 696e 672e 5461 736b  m.Threading.Task
-00004530: 732e 5061 7261 6c6c 656c 2e64 6c6c 0000  s.Parallel.dll..
-00004540: 010f 4825 bf00 8000 00d6 cdf7 9f9f 8291  ..H%............
-00004550: 489f 685e 8065 4710 4e53 7973 7465 6d2e  H.h^.eG.NSystem.
-00004560: 5468 7265 6164 696e 672e 5468 7265 6164  Threading.Thread
-00004570: 2e64 6c6c 0000 0119 d3ef b200 a000 0012  .dll............
-00004580: f5b8 9d2f 85a9 4ab7 4222 1617 9d62 0053  .../..J.B"...b.S
-00004590: 7973 7465 6d2e 5468 7265 6164 696e 672e  ystem.Threading.
-000045a0: 5468 7265 6164 506f 6f6c 2e64 6c6c 0000  ThreadPool.dll..
-000045b0: 0149 8cf1 a400 8000 0056 bac3 41dc 5411  .I.......V..A.T.
-000045c0: 4ebe e0f4 eb48 af9d 5953 7973 7465 6d2e  N....H..YSystem.
-000045d0: 5468 7265 6164 696e 672e 5469 6d65 722e  Threading.Timer.
-000045e0: 646c 6c00 0001 784d c1ba 0080 0000 18a1  dll...xM........
-000045f0: 8a38 62fb c44c 81bd 7462 4551 99de 5379  .8b..L..tbEQ..Sy
-00004600: 7374 656d 2e54 7261 6e73 6163 7469 6f6e  stem.Transaction
-00004610: 732e 646c 6c00 0001 6b65 1f82 0080 0000  s.dll...ke......
-00004620: 5c5f a066 8f5d dc4c 8be2 d8f4 d210 2063  \_.f.].L...... c
-00004630: 5379 7374 656d 2e54 7261 6e73 6163 7469  System.Transacti
-00004640: 6f6e 732e 4c6f 6361 6c2e 646c 6c00 0001  ons.Local.dll...
-00004650: 332d a0a7 00a0 0000 648e a71d 6845 ae4f  3-......d...hE.O
-00004660: 8437 55ff e3c8 f559 5379 7374 656d 2e56  .7U....YSystem.V
-00004670: 616c 7565 5475 706c 652e 646c 6c00 0001  alueTuple.dll...
-00004680: f602 d1c7 0080 0000 2b95 2276 34df 0f45  ........+."v4..E
-00004690: a8a3 4475 3782 e0b7 5379 7374 656d 2e57  ..Du7...System.W
-000046a0: 6562 2e64 6c6c 0000 01cb 8df5 b400 8000  eb.dll..........
-000046b0: 0060 79dd da96 6005 4e80 246b 911d 7bd8  .`y...`.N.$k..{.
-000046c0: 3253 7973 7465 6d2e 5765 622e 4874 7470  2System.Web.Http
-000046d0: 5574 696c 6974 792e 646c 6c00 0001 a03b  Utility.dll....;
-000046e0: fdd1 0080 0000 b32b 0461 e2c5 4848 bd1d  .......+.a..HH..
-000046f0: c1dc 58ed 9a5e 5379 7374 656d 2e57 696e  ..X..^System.Win
-00004700: 646f 7773 2e64 6c6c 0000 0136 1668 f900  dows.dll...6.h..
-00004710: 8000 00fe 4ef8 f678 14e5 42a3 c9b7 9887  ....N..x..B.....
-00004720: 393d ea53 7973 7465 6d2e 586d 6c2e 646c  9=.System.Xml.dl
-00004730: 6c00 0001 64d4 39b2 00a0 0000 fa1c 8067  l...d.9........g
-00004740: b6b1 5345 95f4 c6d3 32dd 0103 5379 7374  ..SE....2...Syst
-00004750: 656d 2e58 6d6c 2e4c 696e 712e 646c 6c00  em.Xml.Linq.dll.
-00004760: 0001 7a1f 83d2 0080 0000 40a3 9586 86bc  ..z.......@.....
-00004770: 8146 8ec2 3003 3602 9677 5379 7374 656d  .F..0.6..wSystem
-00004780: 2e58 6d6c 2e52 6561 6465 7257 7269 7465  .Xml.ReaderWrite
-00004790: 722e 646c 6c00 0001 692b 28ac 0000 0200  r.dll...i+(.....
-000047a0: fc5b f327 e1cd 9e46 b7dd 2c6e f27b 2acd  .[.'...F..,n.{*.
-000047b0: 5379 7374 656d 2e58 6d6c 2e53 6572 6961  System.Xml.Seria
-000047c0: 6c69 7a61 7469 6f6e 2e64 6c6c 0000 0147  lization.dll...G
-000047d0: 58fc 9500 8000 00ad 11a7 bffb d043 4aa0  X............CJ.
-000047e0: 9e73 3751 5f92 0053 7973 7465 6d2e 586d  .s7Q_..System.Xm
-000047f0: 6c2e 5844 6f63 756d 656e 742e 646c 6c00  l.XDocument.dll.
-00004800: 0001 8518 bca2 00c0 0000 21ab fb3f 62a8  ..........!..?b.
-00004810: c045 8314 f90a d894 7d07 5379 7374 656d  .E......}.System
-00004820: 2e58 6d6c 2e58 6d6c 446f 6375 6d65 6e74  .Xml.XmlDocument
-00004830: 2e64 6c6c 0000 01b6 14b5 8600 8000 00ef  .dll............
-00004840: f42b c0a1 6d35 4a98 a112 be1a f403 6a53  .+..m5J.......jS
-00004850: 7973 7465 6d2e 586d 6c2e 586d 6c53 6572  ystem.Xml.XmlSer
-00004860: 6961 6c69 7a65 722e 646c 6c00 0001 1c19  ializer.dll.....
-00004870: e78c 0000 0100 2c92 b403 2fc6 b847 9cc3  ......,.../..G..
-00004880: eebc 4779 dfae 5379 7374 656d 2e58 6d6c  ..Gy..System.Xml
-00004890: 2e58 5061 7468 2e64 6c6c 0000 01c9 480f  .XPath.dll....H.
-000048a0: a000 8000 0034 bfc9 f493 c836 4e97 be0c  .....4.....6N...
-000048b0: 9206 3bb8 e453 7973 7465 6d2e 586d 6c2e  ..;..System.Xml.
-000048c0: 5850 6174 682e 5844 6f63 756d 656e 742e  XPath.XDocument.
-000048d0: 646c 6c00 0001 4e06 9e92 0080 0000 d859  dll...N........Y
-000048e0: fc91 576e 9347 8947 d5e4 d4a1 aebb 556e  ..Wn.G.G......Un
-000048f0: 6465 7274 616c 654d 6f64 4c69 622e 646c  dertaleModLib.dl
-00004900: 6c00 0001 62f2 9ae3 0020 0300 c184 c359  l...b.... .....Y
-00004910: 6d76 1f49 976e bf23 e575 fde7 5769 6e64  mv.I.n.#.u..Wind
-00004920: 6f77 7342 6173 652e 646c 6c00 0001 9245  owsBase.dll....E
-00004930: 4a8f 0080 0000 966c a4ea 5188 7642 a8d0  J......l..Q.vB..
-00004940: 6ea1 c579 98e8 0b00 0000 2405 0506 0001  n..y......$.....
-00004950: 0400 0653 7973 7465 6d1a 5379 7374 656d  ...System.System
-00004960: 2e43 6f6c 6c65 6374 696f 6e73 2e47 656e  .Collections.Gen
-00004970: 6572 6963 0953 7973 7465 6d2e 494f 0b53  eric.System.IO.S
-00004980: 7973 7465 6d2e 4c69 6e71 0f53 7973 7465  ystem.Linq.Syste
-00004990: 6d2e 4e65 742e 4874 7470 1053 7973 7465  m.Net.Http.Syste
-000049a0: 6d2e 5468 7265 6164 696e 6716 5379 7374  m.Threading.Syst
-000049b0: 656d 2e54 6872 6561 6469 6e67 2e54 6173  em.Threading.Tas
-000049c0: 6b73 1501 aeca 01ae d101 aeec 01ae f601  ks..............
-000049d0: af02 01af 1201 af23 0b00 0000 0d0a 0b07  .......#........
-000049e0: 0001 0475 0b00 0000 140f 0b08 0001 0475  ...u...........u
-000049f0: 1000 0000 1810 090a 002c 0200 0a00 0102  .........,......
-00004a00: 790f 556e 6465 7274 616c 654d 6f64 4c69  y.UndertaleModLi
-00004a10: 621a 556e 6465 7274 616c 654d 6f64 4c69  b.UndertaleModLi
-00004a20: 622e 4465 636f 6d70 696c 6572 1655 6e64  b.Decompiler.Und
-00004a30: 6572 7461 6c65 4d6f 644c 6962 2e4d 6f64  ertaleModLib.Mod
-00004a40: 656c 7311 5379 7374 656d 2e52 6566 6c65  els.System.Refle
-00004a50: 6374 696f 6e1c 5379 7374 656d 2e52 756e  ction.System.Run
-00004a60: 7469 6d65 2e53 6572 6961 6c69 7a61 7469  time.Serializati
-00004a70: 6f6e 2401 aeca 01ae d101 aeec 01ae f601  on$.............
-00004a80: af02 01af 1201 af23 01af 7901 af89 01af  .......#..y.....
-00004a90: a401 afbb 01af cd06 0000 0034 1709 2901  ...........4..).
-00004aa0: 0000 3c1c 090d 0026 0200 0900 1104 0803  ..<....&........
-00004ab0: 0007 0208 0100 6a04 7955 003c 0479 0900  ......j.yU.<.y..
-00004ac0: 2202 000c 0001 0279 1502 0000 3c2a 090d  "......y....<*..
-00004ad0: 002b 0200 0d00 2202 000c 0001 0279 1502  .+...."......y..
-00004ae0: 0000 3c31 090d 002a 0200 0d00 2202 000c  ..<1...*...."...
-00004af0: 0001 0279 0b00 0000 2438 090c 0001 0279  ...y....$8.....y
-00004b00: 0b03 0000 253d 0934 0b04 0200 0b03 0000  ....%=.4........
-00004b10: 244e 0934 0904 0200 0904 0000 000d 0518  $N.4............
-00004b20: 5e09 4705 0000 5f68 0927 001b 0200 1000  ^.G..._h.'......
-00004b30: 3704 0006 001d 0200 0c00 4c02 0006 0038  7.........L....8
-00004b40: 0200 1b00 1402 0007 001d 0200 0c00 1a02  ................
-00004b50: 0007 001e 0200 1000 2204 0007 005f 0200  ........"...._..
-00004b60: 2400 1b02 0010 0001 0279 8086 0600 0019  $........y......
-00004b70: 0909 0800 0702 0801 003c 0679 0700 6f06  .........<.y..o.
-00004b80: 0024 0059 0208 1b00 6904 7924 0053 0208  .$.Y....i.y$.S..
-00004b90: 1b00 1b06 2c0e 0000 0200 0d00 5f03 002b  ....,......._..+
-00004ba0: 0277 1500 0004 0002 7f26 0600 0908 3207  .w.......&....2.
-00004bb0: 0000 0200 2300 331c 003b 0477 1900 5902  ....#.3..;.w..Y.
-00004bc0: 0824 0002 7b4a 0b00 000e 001c 0e5b 0e00  .$..{J.......[..
-00004bd0: 0002 000d 005f 0500 2b04 771c 001b 0200  ....._..+.w.....
-00004be0: 0900 1b02 0809 0000 0400 0279 1e06 0001  ...........y....
-00004bf0: 0c4b 1f53 7973 7465 6d2e 4469 6167 6e6f  .K.System.Diagno
-00004c00: 7374 6963 732e 436f 6465 416e 616c 7973  stics.CodeAnalys
-00004c10: 6973 1801 aeca 01ae d101 aeec 01ae f601  is..............
-00004c20: af02 01af 1201 af23 01b1 6a06 0000 0018  .......#..j.....
-00004c30: 0805 1e53 7973 7465 6d2e 5465 7874 2e4a  ...System.Text.J
-00004c40: 736f 6e2e 5365 7269 616c 697a 6174 696f  son.Serializatio
-00004c50: 6e18 01ae ca01 aed1 01ae ec01 aef6 01af  n...............
-00004c60: 0201 af12 01af 2301 b1aa 1507 0000 461b  ......#.......F.
-00004c70: 0910 0015 0200 0300 0a00 2c06 003d 0455  ..........,..=.U
-00004c80: 1c53 7973 7465 6d2e 436f 6d70 6f6e 656e  .System.Componen
-00004c90: 744d 6f64 656c 2e44 6573 6967 6e14 5379  tModel.Design.Sy
-00004ca0: 7374 656d 2e47 6c6f 6261 6c69 7a61 7469  stem.Globalizati
-00004cb0: 6f6e 1053 7973 7465 6d2e 5465 7874 2e4a  on.System.Text.J
-00004cc0: 736f 6e15 4e61 7475 7261 6c53 6f72 742e  son.NaturalSort.
-00004cd0: 4578 7465 6e73 696f 6e14 5369 784c 6162  Extension.SixLab
-00004ce0: 6f72 732e 496d 6167 6553 6861 7270 2053  ors.ImageSharp S
-00004cf0: 6978 4c61 626f 7273 2e49 6d61 6765 5368  ixLabors.ImageSh
-00004d00: 6172 702e 466f 726d 6174 732e 506e 6721  arp.Formats.Png!
-00004d10: 5369 784c 6162 6f72 732e 496d 6167 6553  SixLabors.ImageS
-00004d20: 6861 7270 2e50 6978 656c 466f 726d 6174  harp.PixelFormat
-00004d30: 731f 5369 784c 6162 6f72 732e 496d 6167  s.SixLabors.Imag
-00004d40: 6553 6861 7270 2e50 726f 6365 7373 696e  eSharp.Processin
-00004d50: 6710 5941 4d53 5f4c 4942 2e70 6174 6368  g.YAMS_LIB.patch
-00004d60: 6573 1459 414d 535f 4c49 422e 7061 7463  es.YAMS_LIB.patc
-00004d70: 6865 732e 716f 6c41 01ae ca01 aed1 01ae  hes.qolA........
-00004d80: ec01 aef6 01af 0201 af12 01af 2301 b1f8  ............#...
-00004d90: 01b2 1501 afbb 01b2 2a01 b23b 01b2 5101  ........*..;..Q.
-00004da0: b266 01b2 8701 b2a9 01af 7901 af89 01af  .f........y.....
-00004db0: a401 b2c9 01b2 da03 1c93 dc08 0000 0006  ................
-00004dc0: 003a 2e09 0a00 5c04 000d 001d 0e00 0a00  .:....\.........
-00004dd0: 3104 0e0d 001e 047b 0f00 0102 7902 0000  1......{....y...
-00004de0: 0b00 0001 0025 0400 0a00 3d02 0010 0057  .....%....=....W
-00004df0: 0600 1a00 4002 000c 004e 0080 820b 0034  ....@....N.....4
-00004e00: 06bf 7f10 0038 0400 1000 6806 0016 0080  .....8....h.....
-00004e10: 8204 001f 0067 0200 2505 0408 0044 0080  .....g..%....D..
-00004e20: 810c 0021 0055 0200 0b00 2502 0010 0037  ...!.U....%....7
-00004e30: 0200 0c00 5c02 0007 0031 0200 0800 4f02  ....\....1....O.
-00004e40: 0007 0024 0200 0800 3402 000e 0030 0200  ...$....4....0..
-00004e50: 0700 7d02 0022 0074 0200 0c00 2302 0011  ..}..".t....#...
-00004e60: 0035 0200 0c00 3c02 0007 002f 0200 0900  .5....<..../....
-00004e70: 3502 0007 0024 0200 0800 3402 000e 002e  5....$....4.....
-00004e80: 0200 0700 2702 0010 0058 0400 1700 5a06  ....'....X....Z.
-00004e90: 0015 0056 0200 1001 80d2 0200 2501 81ca  ...V........%...
-00004ea0: 0800 2500 8087 0800 1f00 5906 001f 0053  ..%.......Y....S
-00004eb0: 0600 1500 5e02 000a 0058 0200 1f00 5506  ....^....X....U.
-00004ec0: 001f 0080 8f06 0025 0080 8802 0025 0280  .......%.....%..
-00004ed0: a606 0025 0280 a60a 0025 0077 0a00 2500  ...%.....%.w..%.
-00004ee0: 8087 0400 2500 809d 0600 2500 5c06 001f  ....%.....%.\...
-00004ef0: 005a 0200 1f00 4706 0017 0080 8902 0012  .Z....G.........
-00004f00: 0080 8102 0012 0080 8302 0012 007e 0200  .............~..
-00004f10: 1200 6002 322a 0000 0200 0c00 6107 0047  ..`.2*......a..G
-00004f20: 0477 2200 4702 0022 0000 0600 027b 2408  .w".G..".....{$.
-00004f30: 0180 9a0e 5525 0067 0600 2500 5806 001f  ....U%.g..%.X...
-00004f40: 0080 8402 0025 0073 0600 1f00 7302 001f  .....%.s....s...
-00004f50: 0073 0200 1f00 6e02 001f 0073 0200 1f00  .s....n....s....
-00004f60: 4e06 381b 0000 0200 0f00 5b07 003c 0477  N.8.......[..<.w
-00004f70: 1c00 0006 0002 7d2a 0800 80a6 0c4f 1f0e  ......}*.....O..
-00004f80: 1202 0025 0181 041e 0025 1112 0400 2500  ...%.....%....%.
-00004f90: 2d28 0012 0067 005c 2501 80da 0625 1f00  -(...g.\%....%..
-00004fa0: 6804 001f 0076 0600 2500 7d02 0025 0074  h....v..%.}..%.t
-00004fb0: 0200 2500 809c 0600 1f00 8097 0200 1f00  ..%.............
-00004fc0: 8097 0200 1f00 5e06 0025 0060 0200 2505  ......^..%.`..%.
-00004fd0: 5d06 3866 0000 0200 0f00 5b07 0033 0e77  ].8f......[..3.w
-00004fe0: 1c00 0006 0002 732a 0800 808f 144f 1f01  ......s*.....O..
-00004ff0: 811a 0600 2503 80e2 0800 2500 710e 0025  ....%.....%.q..%
-00005000: 0037 0200 0700 5602 001c 026c 0200 0c00  .7....V....l....
-00005010: 2406 0011 0045 0200 2000 5602 0007 002a  $....E.. .V....*
-00005020: 0200 0900 4902 0007 0020 0200 0c00 2802  ....I.... ....(.
-00005030: 000e 0024 0200 0707 8122 0c00 0701 80f6  ...$....."......
-00005040: 1238 2b00 0002 000f 005b 0700 5306 771f  .8+......[..S.w.
-00005050: 0000 0600 027b 2a08 006a 0e4f 2500 2906  .....{*..j.O%.).
-00005060: 0007 005d 0230 1700 0002 000b 0063 0700  ...].0.......c..
-00005070: 2e04 770f 0031 005e 2f00 0006 0002 7d45  ..w..1.^/.....}E
-00005080: 0804 8090 0a57 3104 8086 0a00 3100 250c  .....W1.....1.%.
-00005090: 0007 001d 0230 1b00 0002 000b 0063 0700  .....0.......c..
-000050a0: 2e04 770f 002d 005e 2f00 0006 0002 7d45  ..w..-.^/.....}E
-000050b0: 0804 8088 0a57 3104 7e0a 0031 0980 8a10  .....W1.~..1....
-000050c0: 001f 005d 1600 2500 5d02 0025 0060 0600  ...]..%.]..%.`..
-000050d0: 2500 809d 0600 2500 4e06 001f 0055 0638  %.....%.N....U.8
-000050e0: 1b00 0002 000f 005b 0700 7b04 7722 0000  .......[..{.w"..
-000050f0: 0600 027d 2a08 0080 8c0c 4f25 0174 0600  ...}*.....O%.t..
-00005100: 2517 809e 0800 2500 7a34 0022 007c 0200  %.....%.z4.".|..
-00005110: 2200 2102 0011 0022 0200 1109 0602 0078  ".!....".......x
-00005120: 0906 1400 7b00 5c18 001f 0080 8008 0022  ....{.\........"
-00005130: 0024 0200 1100 3a02 0015 0080 8b02 0037  .$....:........7
-00005140: 0047 0600 1700 4802 002d 0048 0200 2d00  .G....H..-.H..-.
-00005150: 4802 002a 0046 0200 2900 4602 002c 0046  H..*.F..).F..,.F
-00005160: 0200 2c00 4602 0029 0044 0200 2700 4608  ..,.F..).D..'.F.
-00005170: 0017 000b 020a 0700 0005 0033 047f 0700  ...........3....
-00005180: 3502 0028 001a 0200 0900 2b04 0007 004d  5..(......+....M
-00005190: 0200 4900 4302 001d 0018 0200 1100 2302  ..I.C.........#.
-000051a0: 000d 004f 0200 0700 1702 0009 0043 0200  ...O.........C..
-000051b0: 0700 1b02 000e 001c 0200 0700 2e04 0007  ................
-000051c0: 0055 0200 4900 1b02 0011 0026 0200 0d00  .U..I......&....
-000051d0: 2f02 0007 001a 0200 0900 2902 0007 001a  /.........).....
-000051e0: 0200 0c00 1b02 000e 001f 0200 0700 1b02  ................
-000051f0: 0011 0003 4b30 0600 0800 6d0c 0e5a 3e5d  ....K0....m..Z>]
-00005200: 1200 4e1e 0025 004e 0200 2500 3006 0007  ..N..%.N..%.0...
-00005210: 0048 0200 1c5d 4602 000c 001d 80bc 0011  .H...]F.........
-00005220: 0071 0200 3701 817a 0600 1201 817a 0400  .q..7..z.....z..
-00005230: 1204 6508 3033 0000 0200 0b00 6307 003b  ..e.03......c..;
-00005240: 0c77 2200 0006 0002 7522 0804 6514 063b  .w".....u"..e..;
-00005250: 0000 0200 0b00 6307 0029 0c77 1400 5302  ......c..).w..S.
-00005260: 0012 031a 0200 1308 120e 0812 0000 0205  ................
-00005270: 0a18 000c 0000 0600 024b 1a08 0047 4a57  .........K...GJW
-00005280: 1700 4202 0012 0054 0200 1200 8092 0200  ..B....T........
-00005290: 2500 8092 0200 2501 6802 0025 005f 0400  %.....%.h..%._..
-000052a0: 1500 7102 0011 006f 0200 1100 8088 0200  ..q....o........
-000052b0: 1101 809e 0200 1100 808c 0400 1000 6d02  ..............m.
-000052c0: 0025 0021 0600 1000 4106 0815 005c 0200  .%.!....A....\..
-000052d0: 1700 5c02 0017 005a 0200 1700 5b02 0017  ..\....Z....[...
-000052e0: 004e 0200 1700 4802 0017 0050 0200 1700  .N....H....P....
-000052f0: 5c02 002f 0055 0200 2f00 5602 0030 0055  \../.U../.V..0.U
-00005300: 0200 2f00 5502 002f 0056 0200 3000 5602  ../.U../.V..0.V.
-00005310: 0030 0056 0200 3000 5602 002c 0052 0400  .0.V..0.V..,.R..
-00005320: 2900 4902 0029 0052 0200 2900 7a04 0022  ).I..).R..).z.."
-00005330: 0065 0200 0c00 2102 0011 0070 0200 2a00  .e....!....p..*.
-00005340: 6802 000f 003e 0600 1500 6002 002f 0058  h....>....`../.X
-00005350: 0200 2e00 5a02 0030 0059 0200 2f00 5a02  ....Z..0.Y../.Z.
-00005360: 0030 0059 0200 2f00 5a02 0030 005a 0200  .0.Y../.Z..0.Z..
-00005370: 3000 4f06 0029 0046 0200 2900 4f02 0029  0.O..).F..).O..)
-00005380: 0045 0400 1000 7704 0022 0063 0200 0c00  .E....w..".c....
-00005390: 1e02 0011 006e 0200 2a00 5d06 0030 0040  .....n..*.]..0.@
-000053a0: 0800 1700 5d02 002d 0056 0200 2d00 5702  ....]..-.V..-.W.
-000053b0: 002e 0057 0200 2d00 5602 002d 0057 0200  ...W..-.V..-.W..
-000053c0: 2e00 5702 002e 0058 0200 2e00 5708 0038  ..W....X....W..8
-000053d0: 0056 0200 3800 5e02 0032 0050 0400 2700  .V..8.^..2.P..'.
-000053e0: 4702 0027 0050 0200 2700 4804 0011 0079  G..'.P..'.H....y
-000053f0: 0400 2200 6502 000c 0020 0200 1100 7102  ..".e.... ....q.
-00005400: 0028 0044 0600 1700 6202 0030 005a 0200  .(.D....b..0.Z..
-00005410: 2f00 5c02 0031 005b 0200 3000 5c02 0031  /.\..1.[..0.\..1
-00005420: 005b 0200 3000 5c02 0031 005c 0200 3100  .[..0.\..1.\..1.
-00005430: 5f08 0038 005f 0200 3800 5f02 0038 005f  _..8._..8._..8._
-00005440: 0200 3800 6f02 0043 0055 0400 2a00 4c02  ..8.o..C.U..*.L.
-00005450: 002a 0055 0200 2a00 7d04 0022 0067 0200  .*.U..*.}..".g..
-00005460: 0c00 2402 0011 0079 0200 2b00 4904 0011  ..$....y..+.I...
-00005470: 0080 8808 0025 0080 8802 0025 0180 9404  .....%.....%....
-00005480: 0025 0080 8806 0025 0080 8802 0025 0080  .%.....%.....%..
-00005490: 8802 0025 0080 8802 0025 0080 8802 0025  ...%.....%.....%
-000054a0: 0080 8604 0025 0080 8602 0025 0080 8602  .....%.....%....
-000054b0: 0025 0080 8802 0025 0181 9208 7925 0181  .%.....%....y%..
-000054c0: 9204 0025 0181 9204 0025 0181 9204 0025  ...%.....%.....%
-000054d0: 0281 7008 001f 003b 0a00 1500 4302 0007  ..p....;....C...
-000054e0: 0010 0200 0900 1002 0009 0014 0200 0c00  ................
-000054f0: 1402 000c 0033 0200 2400 4102 001c 0031  .....3..$.A....1
-00005500: 0200 0700 5602 001c 006e 0200 0c00 1e02  ....V....n......
-00005510: 0011 0025 0200 0900 2302 000d 0b06 0200  ...%....#.......
-00005520: 8088 0b06 1800 808a 007b 1c00 2502 8098  .........{..%...
-00005530: 0600 4b00 4a0a 0015 0063 0200 1100 6f06  ..K.J....c....o.
-00005540: 0010 005b 0600 2500 5b02 0025 0180 9406  ...[..%.[..%....
-00005550: 0025 0181 2a0e 000c 006c 0a00 1200 8080  .%..*....l......
-00005560: 0200 1200 5402 0012 0069 0200 1200 4e02  ....T....i....N.
-00005570: 0012 0060 0200 1200 6702 0012 0051 0600  ...`....g....Q..
-00005580: 1502 8156 0200 1000 4c06 0015 0068 0200  ...V....L....h..
-00005590: 100b 1208 0012 084e 1800 1208 4e12 0012  .......N....N...
-000055a0: 0a4e 1200 120b 121a 0012 084e 1800 1208  .N.........N....
-000055b0: 4e12 0012 0a4e 1200 120a 121a 0012 084e  N....N.........N
-000055c0: 1600 1208 4e12 0012 0a4e 1200 1200 521a  ....N....N....R.
-000055d0: 0015 0080 9502 0011 0180 b602 0011 0181  ................
-000055e0: 2408 0011 095a 0800 1100 5914 0010 0281  $....Z....Y.....
-000055f0: 280e 000c 003b 0a00 0c00 6a06 000c 007f  (....;....j.....
-00005600: 0600 2400 8083 0200 2a01 812a 0600 0c01  ..$.....*..*....
-00005610: 80cc 0800 0c00 6404 0017 0862 0200 1200  ......d....b....
-00005620: 6712 0012 006e 0400 1708 6c02 0012 0071  g....n....l....q
-00005630: 1200 1200 6404 0017 085e 0200 1200 6712  ....d....^....g.
-00005640: 0012 0065 0400 1708 5e02 0012 0064 1200  ...e....^....d..
-00005650: 1200 4e06 000c 0181 1002 0025 0080 a304  ..N........%....
-00005660: 0025 0f80 9e02 0025 007d 2400 0c00 80af  .%.....%.}$.....
-00005670: 0200 1f00 80be 0200 2500 3702 000d 0061  ........%.7....a
-00005680: 0408 1200 8093 0200 2c00 8094 0200 2c02  ........,.....,.
-00005690: 814a 0879 0c1e 5a0a 0012 0181 003e 0012  .J.y..Z......>..
-000056a0: 007a 0800 2500 5a06 0017 004e 0200 1200  .z..%.Z....N....
-000056b0: 5902 0017 0047 0200 1205 6504 304b 0000  Y....G....e.0K..
-000056c0: 0200 0b00 6307 004f 0e77 2200 0006 0002  ....c..O.w".....
-000056d0: 7322 0800 4f14 571b 000c 023e 1100 0002  s"..O.W....>....
-000056e0: 0012 0055 0700 6004 4632 0000 0200 1b00  ...U..`.F2......
-000056f0: 4307 004c 0477 1500 027d 420b 0000 0b00  C..L.w...}B.....
-00005700: 0001 0002 7d67 0b00 000b 0000 0100 4b14  ....}g........K.
-00005710: 4912 0052 0200 1200 4c06 0012 0053 0200  I..R....L....S..
-00005720: 1201 80da 023e 3500 0002 0012 0055 0700  .....>5......U..
-00005730: 4006 7710 0002 7b30 0b00 000b 0000 0100  @.w...{0........
-00005740: 4a0e 4912 0051 0200 1200 7502 0025 005b  J.I..Q....u..%.[
-00005750: 0600 1700 4902 0012 004f 0200 1202 8096  ....I....O......
-00005760: 0240 3500 0002 0013 0053 0700 3c08 7710  .@5......S..<.w.
-00005770: 0002 7932 0b00 000b 0000 0100 5a10 4717  ..y2........Z.G.
-00005780: 0048 0200 1200 4e02 0012 0465 0230 3300  .H....N....e.03.
-00005790: 0002 000b 0063 0700 4f0c 7722 0000 0600  .....c..O.w"....
-000057a0: 0275 2208 004c 1457 1200 5202 0012 0280  .u"..L.W..R.....
-000057b0: 9602 4035 0000 0200 1300 5307 0045 0877  ..@5......S..E.w
-000057c0: 1000 0279 320b 0000 0b00 0001 004f 1047  ...y2........O.G
-000057d0: 1200 5502 0012 0180 d602 4035 0000 0200  ..U.......@5....
-000057e0: 1300 5307 0048 0677 1000 027b 320b 0000  ..S..H.w...{2...
-000057f0: 0b00 0001 004d 1047 1200 5402 0012 0765  .....M.G..T....e
-00005800: 0230 809c 0000 0200 0b00 6307 0055 1277  .0........c..U.w
-00005810: 2200 0006 0002 6f22 0800 4a1c 5712 0050  ".....o"..J.W..P
-00005820: 0200 1206 6504 3080 8a00 0002 000b 0063  ....e.0........c
-00005830: 0700 5110 7722 0000 0600 0271 2208 0055  ..Q.w".....q"..U
-00005840: 1857 1700 4702 0012 004f 0200 1200 4706  .W..G....O....G.
-00005850: 0012 004f 0200 1200 808c 0230 2b00 0002  ...O.......0+...
-00005860: 000b 0063 0700 5604 7722 0000 0600 027d  ...c..V.w".....}
-00005870: 2208 0047 0c57 1200 4f02 0012 0047 0600  "..G.W..O....G..
-00005880: 1200 4f02 0012 0047 0600 1200 4f02 0012  ..O....G....O...
-00005890: 0858 0600 1208 5a12 0012 085a 1200 1212  .X....Z....Z....
-000058a0: 5a12 0012 085a 2800 1200 3816 000c 0281  Z....Z(...8.....
-000058b0: 5802 0025 0039 0a00 0c00 7c02 001f 0c12  X..%.9....|.....
-000058c0: 0200 2500 80a8 1e00 7e00 6606 0025 0065  ..%.....~.f..%.e
-000058d0: 0200 1f00 5f02 001f 0065 0600 2500 8083  ...._....e..%...
-000058e0: 0400 1f00 3f06 000c 004e 0200 1504 80f6  ....?....N......
-000058f0: 0200 1010 80a6 0e00 1f00 6e22 0025 0780  ..........n".%..
-00005900: a202 001f 2780 aa10 0025 0780 a250 001f  ....'....%...P..
-00005910: 0067 1000 1f08 8092 0200 1f01 80a6 1200  .g..............
-00005920: 2500 3408 0007 0052 0200 1c2f 4e02 000c  %.4....R.../N...
-00005930: 0021 6000 1100 7b02 0037 0034 0400 0700  .!`...{..7.4....
-00005940: 5202 001c 384e 0200 0c00 2172 0011 007b  R...8N....!r...{
-00005950: 0200 3700 4304 0015 0080 8002 0011 002d  ..7.C..........-
-00005960: 0200 1100 3702 0010 0043 0400 1500 2d02  ....7....C....-.
-00005970: 0011 0074 0200 1100 7102 0011 0d44 0200  ...t....q....D..
-00005980: 1100 80a1 2000 7d04 6002 0010 0052 1000  .... .}.`....R..
-00005990: 1500 3402 0011 007b 0200 1000 6e04 302b  ..4....{....n.0+
-000059a0: 0000 0200 0b00 6307 003e 0477 2200 0006  ......c..>.w"...
-000059b0: 0002 7d22 0800 400c 5724 0044 0200 2400  ..}"..@.W$.D..$.
-000059c0: 8081 0600 4a00 809c 0200 3c00 4206 000c  ....J.....<.B...
-000059d0: 0064 0200 2508 1202 001f 0022 1600 0300  .d..%......"....
-000059e0: 2002 0003 0020 0200 0300 4802 000c 0018   .... ....H.....
-000059f0: 0254 0d00 0005 001d 003f 1c00 1d04 7704  .T.......?....w.
-00005a00: 000d 0200 0400 0080 be00 5806 103f 0180  ..........X..?..
-00005a10: e802 0080 8500 0604 0005 0019 0600 0700  ................
-00005a20: 7c04 0017 0027 0408 0700 7606 7917 0021  |....'....v.y..!
-00005a30: 0080 ee07 0061 04bf 133f 001c 0200 0300  .....a...?......
-00005a40: 0602 0005 0017 0600 0700 8084 0400 1700  ................
-00005a50: 2504 0807 007e 0679 1700 1f00 80fe 0700  %....~.y........
-00005a60: 6304 bf03 3f00 1a02 0003 0006 0200 0500  c...?...........
-00005a70: 1708 0007 0076 0400 1700 2500 80ee 0700  .....v....%.....
-00005a80: 7004 bf13 1700 1f00 80e2 0700 5d04 bf1f  p...........]...
-00005a90: 3f00 1a02 0003 0006 0200 0500 0004 0023  ?..............#
-00005aa0: 0e0e 1c00 4702 7312 0006 0200 0500 5c06  ....G.s.......\.
-00005ab0: 003f 0006 0200 0500 6404 003f 0006 0200  .?......d..?....
-00005ac0: 0500 6604 003f 0006 0200 0500 6204 003f  ..f..?......b..?
-00005ad0: 0006 0200 0500 5e04 003f 0006 0200 0500  ......^..?......
-00005ae0: 5c04 003f 0006 0200 0500 6404 003f 0006  \..?......d..?..
-00005af0: 0200 0500 1204 0005 0054 0026 1200 1204  .........T.&....
-00005b00: 5b08 005a 0026 1200 0604 5b05 006a 0400  [..Z.&....[..j..
-00005b10: 3f00 0602 0005 0068 0400 3f00 0602 0005  ?......h..?.....
-00005b20: 0060 0400 3f00 0602 0005 0012 0400 0500  .`..?...........
-00005b30: 5200 2612 0012 045b 0800 5600 2612 0006  R.&....[..V.&...
-00005b40: 045b 0500 5c0a 003f 0006 0200 0500 5c04  .[..\..?......\.
-00005b50: 003f 0006 0200 0500 5c04 003f 0006 0200  .?......\..?....
-00005b60: 0500 5c04 003f 0006 0200 0500 5c04 003f  ..\..?......\..?
-00005b70: 0006 0200 0500 5c04 003f 0006 0200 0500  ......\..?......
-00005b80: 6a04 003f 0006 0200 0500 6b04 003f 0006  j..?......k..?..
-00005b90: 0200 0500 8081 0400 3300 0602 0002 0055  ........3......U
-00005ba0: 0400 3300 0602 0002 0057 0400 3300 0602  ..3......W..3...
-00005bb0: 0002 0028 0800 0600 6b04 7153 0002 bee3  ...(....k.qS....
-00005bc0: 460e 0000 0e00 7581 2433 4800 7106 001c  F.....u.$3H.q...
-00005bd0: 005f 0408 1200 7406 791c 0061 0408 1200  ._....t.y..a....
-00005be0: 6a06 791c 005b 0408 1200 7f08 793c 0079  j.y..[......y<.y
-00005bf0: 0200 3c08 8090 0600 2500 6112 0025 2d7e  ..<.....%.a..%-~
-00005c00: 0400 1f00 5662 001f 017a 0200 2500 3a08  ....Vb...z..%.:.
-00005c10: 0010 0066 0600 1f00 4a06 0019 0182 2e02  ...f....J.......
-00005c20: 0080 a000 810f 0400 2a01 824a 0200 80a0  ........*..J....
-00005c30: 0081 1e04 002a 0182 2002 0080 a000 8100  .....*.. .......
-00005c40: 0400 2a00 4902 0019 004f 0200 1900 5d02  ..*.I....O....].
-00005c50: 0019 0060 0200 1900 5d02 0019 0080 8f02  ...`....].......
-00005c60: 0019 1756 0200 1900 8089 3000 1900 6602  ...V......0...f.
-00005c70: 0019 0053 0200 1900 8174 0200 6817 5a02  ...S.....t..h.Z.
-00005c80: 0019 2b6c 3000 6800 5658 0019 0054 0200  ..+l0.h.VX...T..
-00005c90: 1900 5402 0019 0056 0200 1900 5602 0019  ..T....V....V...
-00005ca0: 005a 0200 1900 80aa 0200 1900 80a8 0200  .Z..............
-00005cb0: 1900 809d 0200 1900 80a9 0200 1900 8096  ................
-00005cc0: 0200 1900 80d9 0200 1900 80d8 0200 1900  ................
-00005cd0: 6a02 0019 0046 0200 1900 4202 0019 0018  j....F....B.....
-00005ce0: 066a 0d00 0005 0028 0029 1c00 4604 7714  .j.....(.)..F.w.
-00005cf0: 0043 0200 2300 5502 001c 006a 0408 5700  .C..#.U....j..W.
-00005d00: 4408 7923 0181 3e02 0080 c400 4706 0025  D.y#..>.....G..%
-00005d10: 4504 0200 80d3 000d 0436 0c00 2b02 0c3e  E........6..+..>
-00005d20: 0180 8802 7f48 0031 040c 3e01 8094 027f  .....H.1..>.....
-00005d30: 4800 2604 753e 017e 027f 4800 2604 5916  H.&.u>.~..H.&.Y.
-00005d40: 002e 0054 0c00 4702 450c 0035 0208 0c00  ...T..G.E..5....
-00005d50: 4b02 020c 004c 0200 0c00 3802 020c 0606  K....L....8.....
-00005d60: 0275 0c00 370e 080c 0038 0206 0c00 3102  .u..7....8....1.
-00005d70: 750c 003d 0463 0c06 0602 200c 0606 0e10  u..=.c.... .....
-00005d80: 0c00 4c0e 6f0c 0033 027b 0c00 3402 020c  ..L.o..3.{..4...
-00005d90: 0036 0204 0c00 3602 000c 0035 0206 0c00  .6....6....5....
-00005da0: 5104 5d3e 004f 0400 3e00 4c04 003e 0052  Q.]>.O..>.L..>.R
-00005db0: 0400 3e00 4f04 003e 004a 0400 3e00 4904  ..>.O..>.J..>.I.
-00005dc0: 003b 0055 0238 3b00 3c02 6b09 0037 0210  .;.U.8;.<.k..7..
-00005dd0: 0900 1402 6f09 0049 0263 2200 0004 0033  ....o..I.c"....3
-00005de0: 046f 0900 02bf 575c 0e00 000e 0764 80b2  .o....W\.....d..
-00005df0: 1d12 076e 1200 1207 6012 0012 0780 9016  ...n....`.......
-00005e00: 0080 9900 4a16 000d 0044 0200 0d00 4902  ....J....D....I.
-00005e10: 000d 005b 0200 0e13 6402 0080 a100 262c  ...[....d.....&,
-00005e20: 000d 005d 004e 1200 4d04 7335 0000 0200  ...].N..M.s5....
-00005e30: 1300 5307 0055 0477 0a00 027d 320b 0000  ..S..U.w...}2...
-00005e40: 0b00 0001 000c 0a04 1100 0002 0012 0055  ...............U
-00005e50: 0700 6004 4632 0000 0200 1b00 4307 0148  ..`.F2......C..H
-00005e60: 0477 1500 027d 420b 0000 0b00 0001 0002  .w...}B.........
-00005e70: 7d67 0b00 000b 0000 0101 5012 4925 0073  }g........P.I%.s
-00005e80: 0600 2500 7302 0025 0073 0200 2500 270a  ..%.s..%.s..%.'.
-00005e90: 000d 005f 0050 1204 5d06 6943 0000 0200  ..._.P..].iC....
-00005ea0: 0f00 5b07 0076 0c77 1c00 0006 0002 752a  ..[..v.w......u*
-00005eb0: 0800 2c12 0623 0000 0500 0f00 5b07 0066  ..,..#......[..f
-00005ec0: 0458 4200 0002 0024 0031 0900 2404 7709  .XB....$.1..$.w.
-00005ed0: 0050 0400 1700 0279 540b 0000 0b00 0001  .P.....yT.......
-00005ee0: 0000 0600 027d 4f0b 000a 1659 0400 0002  .....}O....Y....
-00005ef0: 007e 047f 4c00 037d 2c06 0007 006f 0600  .~..L..},....o..
-00005f00: 280c 5f0d 0050 0408 1202 3806 7925 002a  (._..P....8.y%.*
-00005f10: 0a00 0d00 6600 5612 006f 087d 4500 0002  ....f.V..o.}E...
-00005f20: 001c 0041 0700 4304 771a 0002 7d44 0b00  ...A..C.w...}D..
-00005f30: 000b 0000 0129 8094 0a35 2500 3758 0015  .....)...5%.7X..
-00005f40: 004e 0262 3000 0002 0024 0031 0900 1706  .N.b0....$.1....
-00005f50: 770b 0364 0408 1700 180e 790e 005e 0032  w..d......y..^.2
-00005f60: 1100 0269 220b 0000 0b00 0001 0068 2006  ...i"........h .
-00005f70: 4500 0002 0024 0031 0900 2d04 7716 0142  E....$.1..-.w..B
-00005f80: 0408 1700 0279 4c0b 0000 0b00 0001 0078  .....yL........x
-00005f90: 1406 4500 0002 0024 0031 0701 4204 7715  ..E....$.1..B.w.
-00005fa0: 0002 7d54 0b00 000b 0000 0100 670e 0645  ..}T........g..E
-00005fb0: 0000 0200 2400 3109 002e 0477 1601 4204  ....$.1....w..B.
-00005fc0: 0817 0002 794c 0b00 000b 0000 0100 6c16  ....yL........l.
-00005fd0: 0645 0000 0200 2400 3109 0017 0677 0b04  .E....$.1....w..
-00005fe0: 6404 0817 0018 1079 0e00 5e00 3211 0002  d......y..^.2...
-00005ff0: 6722 0b00 000b 0000 0100 808b 2225 1f00  g".........."%..
-00006000: 4e06 381b 0000 0200 0f00 5b07 0080 8604  N.8.......[.....
-00006010: 7722 0000 0600 027d 2a08 0080 f80c 4f1f  w".....}*.....O.
-00006020: 0224 0600 2501 2406 0025 0080 9e08 001f  .$..%.$..%......
-00006030: 0075 0600 1f00 2906 000d 0063 0054 1200  .u....)....c.T..
-00006040: 80a6 062d 1f00 4306 0010 0026 0600 0d00  ...-..C....&....
-00006050: 5900 4e12 0180 cc04 331f 0025 0800 0d00  Y.N.....3..%....
-00006060: 5b00 4c12 0060 0635 1f00 4c04 000c 0b80  [.L..`.5..L.....
-00006070: b204 001f 004e 1a00 0c00 4e04 000c 1b80  .....N....N.....
-00006080: 9804 001f 0052 3a00 0c02 81f4 0400 1f02  .....R:.........
-00006090: 81f4 0800 1f00 5c08 001f 0181 1604 001f  ......\.........
-000060a0: 0e80 a206 0025 0180 ba1e 0025 0028 0800  .....%.....%.(..
-000060b0: 0d00 6100 5212 1b80 9e04 2f25 0028 3c00  ..a.R...../%.(<.
-000060c0: 0d00 5f00 5212 006e 062f 1f00 7606 0025  .._.R..n./..v..%
-000060d0: 0080 8404 0025 0812 0600 1f00 4116 0010  .....%......A...
-000060e0: 0080 8f06 0052 0680 9606 0080 b200 3212  .....R........2.
-000060f0: 000d 0075 0066 1200 3b0a 1b10 1763 0e32  ...u.f..;....c.2
-00006100: 80c0 0000 0200 0c00 6107 0080 9c32 7721  ........a....2w!
-00006110: 0000 0600 024f 2408 0016 3a7f 0d00 0005  .....O$...:.....
-00006120: 0008 0069 0900 0c04 3611 0000 0500 1300  ...i....6.......
-00006130: 5307 0010 0458 0c00 0005 0024 0031 0900  S....X.....$.1..
-00006140: 2604 7713 0080 9004 0080 8600 0279 540e  &.w..........yT.
-00006150: 0000 0b00 0001 0002 7d57 0e00 000b 0000  ........}W......
-00006160: 0100 027d 630e 0000 0e00 421c 5d10 0033  ...}c.....B.]..3
-00006170: 0600 0f01 8108 0800 3500 3708 0010 0038  ........5.7....8
-00006180: 060e 0d00 3104 7b27 0001 0279 0200 000b  ....1.{'...y....
-00006190: 0000 0100 0102 7905 0980 1a06 0005 0981  ......y.........
-000061a0: 1a06 0005 0982 1a06 0005 0983 1a06 0005  ................
-000061b0: 0984 1a06 0005 0985 1a06 0005 0986 1a06  ................
-000061c0: 0006 0000 0035 1505 1a00 0000 5f1b 050b  .....5......_...
-000061d0: 0059 0800 0b00 5508 000b 0051 0800 0b00  .Y....U....Q....
-000061e0: 5f10 0025 5379 7374 656d 2e43 6f6d 706f  _..%System.Compo
-000061f0: 6e65 6e74 4d6f 6465 6c2e 4461 7461 416e  nentModel.DataAn
-00006200: 6e6f 7461 7469 6f6e 7323 01ae ca01 aed1  notations#......
-00006210: 01ae ec01 aef6 01af 0201 af12 01af 2301  ..............#.
-00006220: c000 475b 01af cd01 b22a 01b1 aa07 0000  ..G[.....*......
-00006230: 0056 80da 050c 0000 002e 8110 0507 0021  .V.............!
-00006240: 4800 1b00 0000 1d81 3b05 0b00 2408 000b  H.......;...$...
-00006250: 0028 0800 0b00 2608 000b 001d 1200 0700  .(....&.........
-00006260: 0000 2482 3205 0c00 0000 2682 3c05 0b00  ..$.2.....&.<...
-00006270: 3208 0011 0000 001f 8247 050b 001e 0800  2........G......
-00006280: 0b00 3d08 0007 0000 0018 825e 0523 0000  ..=........^.#..
-00006290: 0069 0c09 2100 80a8 0400 2100 80bc 0400  .i..!.....!.....
-000062a0: 3100 808f 0400 2100 8085 0600 2100 0102  1.....!.....!...
-000062b0: 791d 01ae ca01 aed1 01ae ec01 aef6 01af  y...............
-000062c0: 0201 af12 01af 2301 af79 01af 8903 1c80  ......#..y......
-000062d0: a909 0000 5f1c 0921 005f 0200 2114 1204  ...._..!._..!...
-000062e0: 001b 0612 2c00 2107 1210 0021 0412 1200  ....,.!....!....
-000062f0: 2106 120c 0021 1d12 0e00 2117 123e 0082  !....!....!..>..
-00006300: 2800 4134 0012 005b 0600 3400 6e02 001b  (.A4...[..4.n...
-00006310: 005c 0400 3700 6f02 001b 005c 0400 3400  .\..7.o....\..4.
-00006320: 6f02 001b 005c 0400 3700 6f02 001b 005b  o....\..7.o....[
-00006330: 0400 3400 6e02 001b 005c 0400 3700 6f02  ..4.n....\..7.o.
-00006340: 001b 005c 0400 3700 6f02 001b 0080 870a  ...\..7.o.......
-00006350: 0021 0080 8706 0021 0080 8706 0021 0080  .!.....!.....!..
-00006360: 8706 0021 0080 8706 0021 0080 8706 0021  ...!.....!.....!
-00006370: 0080 8706 0021 0001 0279 1100 0000 3780  .....!...y....7.
-00006380: be09 0800 3e02 0008 0001 0279 340a 0000  ....>......y4...
-00006390: 0014 0052 0e09 2000 8087 0200 1200 2b04  ...R.. .......+.
-000063a0: 0006 0029 0200 0c00 3b02 001b 0001 0279  ...)....;......y
-000063b0: 0200 0009 0000 0100 0009 0000 0100 0100  ................
-000063c0: 0027 01ae ca01 aed1 01ae ec01 aef6 01af  .'..............
-000063d0: 0201 af12 01af 2301 b251 01b2 6601 b2a9  ......#..Q..f...
-000063e0: 01af 7901 af89 01af a46a 0b00 002f 1a09  ..y......j.../..
-000063f0: 0d00 2b04 761c 0000 0200 2a00 2507 005f  ..+.v.....*.%.._
-00006400: 0477 1600 027d 600a 0000 0900 0001 0030  .w...}`........0
-00006410: 0e11 0d00 6004 7637 0000 0200 2a00 2507  ....`.v7....*.%.
-00006420: 0060 0477 1600 027d 600a 0000 0900 0001  .`.w...}`.......
-00006430: 002d 0e11 0d00 8081 044e 3900 0002 0016  .-.......N9.....
-00006440: 004d 0900 5304 7717 0002 7d38 0b00 000e  .M..S.w...}8....
-00006450: 0001 0a31 835f 0c00 0000 0600 4d0d 0911  ...1._......M...
-00006460: 0e12 0600 1000 501e 0221 0050 0200 2100  ......P..!.P..!.
-00006470: 3206 7f12 000c 022a 0c00 0002 0008 0069  2......*.......i
-00006480: 0600 5204 2030 0000 0200 0800 6907 001f  ..R. 0......i...
-00006490: 0477 0600 027d 1c0b 0000 0b00 0001 0002  .w...}..........
-000064a0: 7d79 0a00 0009 0000 0100 1310 5d08 0033  }y..........]..3
-000064b0: 0600 1700 1e02 381b 0000 0500 0f00 5b07  ......8.......[.
-000064c0: 0029 0477 1005 0402 001e 004e 0424 3100  .).w.......N.$1.
-000064d0: 4302 0031 005c 026f 0b00 0002 0016 0418  C..1.\.o........
-000064e0: 0c00 0002 0008 0069 0900 1804 770f 0002  .......i....w...
-000064f0: 7d1c 0b00 000e 001b 0a5d 0e00 4504 0834  }........]..E..4
-00006500: 0000 0200 1b04 020e 0043 047f 3000 0006  .........C..0...
-00006510: 0002 5922 0b00 1932 4f06 0014 0248 0d00  ..Y"...2O....H..
-00006520: 0005 0017 004b 1c00 1304 7703 000c 022a  .....K....w....*
-00006530: 0c00 0005 0008 0069 0800 1004 2c0e 0000  .......i....,...
-00006540: 0500 0e00 5d09 0020 0477 0e00 4c04 001d  ....].. .w..L...
-00006550: 0050 0200 1d00 2602 000d 0080 9004 0838  .P....&........8
-00006560: 012a 0679 4200 5506 0838 002b 0679 0400  .*.yB.U..8.+.y..
-00006570: 1102 0007 0014 0608 0400 3602 0013 0080  ..........6.....
-00006580: eb02 0053 0404 0400 3200 0404 1c05 0005  ...S....2.......
-00006590: 0277 0300 0006 0016 066f 0500 0904 1203  .w.......o......
-000065a0: 0000 0200 5a04 7f12 0081 1d02 0066 0003  ....Z........f..
-000065b0: 7b28 0600 0600 7108 0080 ed10 5953 001b  {(....q.....YS..
-000065c0: 0200 0e00 0d06 7903 001e 0200 0c00 7304  ......y.......s.
-000065d0: 086a 0016 0200 0d00 1902 0009 0036 0679  .j...........6.y
-000065e0: 1300 4402 0013 0042 0200 1328 0404 0080  ..D....B...(....
-000065f0: 9d00 1704 360c 003b 0202 3800 3b02 0a38  ....6..;..8.;..8
-00006600: 003b 0273 3800 2d02 0a0c 002d 0279 0c00  .;.s8.-....-.y..
-00006610: 2d02 7d0c 002d 0204 0c00 2d02 000c 002d  -.}..-....-....-
-00006620: 027b 0c00 2d02 020c 002d 0204 0c00 2d02  .{..-....-....-.
-00006630: 7f0c 002d 020e 0c00 2d02 7d0c 002d 0204  ...-....-.}..-..
-00006640: 0c00 2d02 000c 002d 027d 0c00 2d02 000c  ..-....-.}..-...
-00006650: 002d 0202 0c00 2d02 7d0c 002d 0206 0c00  .-....-.}..-....
-00006660: 2d02 730c 002d 0200 0c00 2d02 000c 002d  -.s..-....-....-
-00006670: 0210 0c00 2d02 020c 002d 027f 0c00 2d02  ....-....-....-.
-00006680: 040c 002d 027b 0c00 2d02 0c0c 002d 0269  ...-.{..-....-.i
-00006690: 0c03 80b2 0210 5f00 5d08 7f4c 005e 024f  ......_.]..L.^.O
-000066a0: 5200 0004 0061 066f 1c00 2f04 080c 0031  R....a.o../....1
-000066b0: 0200 0c00 0c02 0004 0012 0408 1300 0d02  ................
-000066c0: 0010 0022 0879 1900 3602 0013 0080 8602  ...".y..6.......
-000066d0: 0046 0061 0879 1600 1404 080e 0024 0408  .F.a.y.......$..
-000066e0: 1300 0d02 0010 0061 0871 1c00 2204 0819  .......a.q.."...
-000066f0: 0012 0200 1300 2202 0010 0080 9602 0054  ......"........T
-00006700: 0080 9e02 0030 000d 022a 0700 0002 0008  .....0...*......
-00006710: 0069 0900 1802 770f 0002 7f1c 0b00 000e  .i....w.........
-00006720: 0061 0855 1c00 4a04 0813 002c 0200 1900  .a.U..J....,....
-00006730: 1202 0013 0017 0200 0c00 6202 0840 0000  ..........b..@..
-00006740: 0200 2002 0215 0062 027f 4000 3108 710b  .. ....b..@.1.q.
-00006750: 002c 0208 0900 0002 0032 0202 0b00 2b02  .,.......2....+.
-00006760: 7f09 0000 0200 2304 0009 002c 0479 0e00  ......#....,.y..
-00006770: 1102 0004 0006 0200 0200 02be c728 0e00  .............(..
-00006780: 000b 0000 0100 0a81 4051 0400 0600 1602  ........@Q......
-00006790: 0002 bebd 060d 0000 0900 0001 000b 814a  ...............J
-000067a0: 5d04 0043 0208 3800 02be af32 0e00 000e  ]..C..8....2....
-000067b0: 0001 8156 3717 5379 7374 656d 2e4e 6574  ...V7.System.Net
-000067c0: 2e48 7474 702e 4865 6164 6572 7325 01ae  .Http.Headers%..
-000067d0: ca01 aed1 01ae ec01 aef6 01af 0201 af12  ................
-000067e0: 01af 2301 c000 4d2d 01af 7901 af89 01af  ..#...M-..y.....
-000067f0: a403 1c80 9a0d 0000 4d0b 0911 080a 0800  ........M.......
-00006800: 1527 0a14 0030 040a 5400 0a1f 0a0e 0015  .'...0..T.......
-00006810: 060a 4600 2104 0a12 001b 140a 0e00 1503  ..F.!...........
-00006820: 0a2c 001b 150a 0c00 1b29 5430 001b 0077  .,.......)T0...w
-00006830: 5800 1d00 3702 0006 002b 0200 0c00 4c02  X...7....+....L.
-00006840: 0006 0038 0200 1700 1402 0007 001d 0200  ...8............
-00006850: 0c00 2802 0007 001e 0200 0c81 190a 0200  ..(.............
-00006860: 83b5 0029 8234 000c 004c 0200 1c00 3b02  ...).4...L....;.
-00006870: 0006 0030 0200 0700 3402 0007 0020 0200  ...0....4.... ..
-00006880: 0900 2a02 000d 0029 0200 0700 0102 791e  ..*....)......y.
-00006890: 01ae ca01 aed1 01ae ec01 aef6 01af 0201  ................
-000068a0: af12 01af 2301 af79 01af 8901 afa4 851c  ....#..y........
-000068b0: 0e00 0000 0800 3711 090c 0049 0200 0600  ......7....I....
-000068c0: 2404 0e06 007b 047b 1f00 2f02 000c 0031  $....{.{../....1
-000068d0: 0200 0c00 2902 000c 0060 0200 1700 0102  ....)....`......
-000068e0: 7902 0000 0900 0001 002b 0200 1100 80c2  y........+......
-000068f0: 0400 2400 0c02 2a07 0000 0500 0800 6909  ..$...*.......i.
-00006900: 0043 0477 0700 1a02 000e 001a 0200 0e00  .C.w............
-00006910: 5202 0026 0056 0200 2600 2502 0008 0026  R..&.V..&.%....&
-00006920: 0200 1200 4502 0024 0002 6f1c 0e00 000e  ....E..$..o.....
-00006930: 0000 0700 601c 6527 004e 0200 2700 8084  ....`.e'.N..'...
-00006940: 0200 1900 5302 0022 004a 0200 2200 6402  ....S..".J..".d.
-00006950: 0014 0024 020e 0700 2904 7b0e 0039 0200  ...$....).{..9..
-00006960: 1d00 0102 7902 0000 0b00 0001 0062 0400  ....y........b..
-00006970: 2700 5002 0027 0080 8902 0019 0055 0200  '.P..'.......U..
-00006980: 2200 4c02 0022 0068 0200 1400 2402 0e07  ".L..".h....$...
-00006990: 002a 047b 0e00 3a02 001d 0001 0279 0200  .*.{..:......y..
-000069a0: 000b 0000 0100 7222 793b 0078 0200 3b00  ......r"y;.x..;.
-000069b0: 7802 003b 007e 0200 3b00 6b02 003b 0080  x..;.~..;.k..;..
-000069c0: a602 0057 0080 a602 0057 0080 a602 0057  ...W.....W.....W
-000069d0: 0080 a602 0057 0080 a602 0057 0080 a602  .....W.....W....
-000069e0: 0057 0080 a602 0057 0181 3604 0057 0181  .W.....W..6..W..
-000069f0: 2204 0057 0181 1204 0057 0181 0e04 0057  "..W.....W.....W
-00006a00: 0080 a508 004b 0080 a702 004b 0080 a102  .....K.....K....
-00006a10: 004b 0080 a302 004b 0080 a502 004b 0080  .K.....K.....K..
-00006a20: 9f02 004b 0080 a802 004b 0080 aa02 004b  ...K.....K.....K
-00006a30: 0080 a402 004b 0075 0600 4600 7802 0046  .....K.u..F.x..F
-00006a40: 0076 0200 4600 7602 0046 007b 0200 4600  .v..F.v..F.{..F.
-00006a50: 80a2 0600 4b00 80a0 0200 4b00 80a2 0200  ....K.....K.....
-00006a60: 4b00 80a2 0200 4b00 809f 0200 4b00 809c  K.....K.....K...
-00006a70: 0200 4b00 809e 0200 4b00 809d 0200 4b00  ..K.....K.....K.
-00006a80: 80a4 0200 4b00 809e 0200 4b00 80a0 0200  ....K.....K.....
-00006a90: 4b00 80a0 0200 4b00 809e 0200 4b00 809e  K.....K.....K...
-00006aa0: 0200 4b00 809f 0200 4b00 809d 0200 4b00  ..K.....K.....K.
-00006ab0: 80a4 0200 4b00 809d 0200 4b00 809d 0200  ....K.....K.....
-00006ac0: 4b00 809d 0200 4b00 80a6 0200 4b00 80a6  K.....K.....K...
-00006ad0: 0200 4b00 80a5 0200 4b00 80ab 0200 4b00  ..K.....K.....K.
-00006ae0: 80a8 0200 4b00 80aa 0200 4b00 809e 0200  ....K.....K.....
-00006af0: 4b00 3206 0020 0080 9902 004b 0080 9902  K.2.. .....K....
-00006b00: 004b 0080 9902 004b 0080 9902 004b 0080  .K.....K.....K..
-00006b10: 9902 004b 0080 9902 004b 0080 9902 004b  ...K.....K.....K
-00006b20: 0080 9902 004b 0080 9902 004b 0506 1600  .....K.....K....
-00006b30: 8080 0406 0e00 7204 060c 0072 0406 0c00  ......r....r....
-00006b40: 7204 060c 0072 0406 0c00 7204 060c 0072  r....r....r....r
-00006b50: 0406 0a00 7204 060c 0072 0506 0c00 7204  ....r....r....r.
-00006b60: 060e 0072 0406 0c00 7204 060c 0072 0506  ...r....r....r..
-00006b70: 0c00 8080 0506 0e00 8080 0039 0e00 2000  ...........9.. .
-00006b80: 6702 0027 0034 0600 1c00 3502 001d 0039  g..'.4....5....9
-00006b90: 0400 2000 6702 0027 0080 9504 004b 0a06  .. .g..'.....K..
-00006ba0: 0400 8117 3706 1800 8a97 0406 7200 7204  ....7.......r.r.
-00006bb0: 060c 0072 0406 0c00 7204 060c 0072 002f  ...r....r....r./
-00006bc0: 0c00 0c00 2f02 000c 0506 0600 8082 0023  ..../..........#
-00006bd0: 1000 0d00 3404 4423 0000 0200 1100 5707  ....4.D#......W.
-00006be0: 003c 0477 1300 5502 002d 0000 0600 027b  .<.w..U..-.....{
-00006bf0: 2e08 0406 1043 6d00 2312 000c 002d 0600  .....Cm.#....-..
-00006c00: 0c00 3202 000c 0032 0200 0c00 3602 000c  ..2....2....6...
-00006c10: 0033 0200 0c00 3402 000c 0033 0200 0c00  .3....4....3....
-00006c20: 3502 000c 0030 0200 0c00 3202 000c 0034  5....0....2....4
-00006c30: 0200 0c00 3102 000c 0032 0200 0c00 2a02  ....1....2....*.
-00006c40: 000c 002e 0200 0c00 3002 000c 0031 0200  ........0....1..
-00006c50: 0c00 3002 000c 0030 0200 0c00 2c02 000c  ..0....0....,...
-00006c60: 0030 0200 0c00 2e02 000c 002f 0200 0c00  .0........./....
-00006c70: 2f02 000c 002e 0200 0c00 3602 000c 002e  /.........6.....
-00006c80: 0200 0c00 2f02 000c 0031 0200 0c00 3102  ..../....1....1.
-00006c90: 000c 002e 0200 0c00 2d02 000c 002f 0200  ........-..../..
-00006ca0: 0c00 2e02 000c 002b 0800 0c00 3102 000c  .......+....1...
-00006cb0: 002e 0200 0c00 3002 000c 002c 0200 0c00  ......0....,....
-00006cc0: 3102 000c 002e 0200 0c00 2e02 000c 002e  1...............
-00006cd0: 0200 0c00 3302 000c 002f 0200 0c00 2f02  ....3..../..../.
-00006ce0: 000c 002f 0200 0c00 2d02 000c 0030 0200  .../....-....0..
-00006cf0: 0c00 2f02 000c 002f 0200 0c00 2f02 000c  ../..../..../...
-00006d00: 0037 0200 0c00 3502 000c 0031 0200 0c00  .7....5....1....
-00006d10: 3302 000c 0032 0200 0c00 3202 000c 002f  3....2....2..../
-00006d20: 0200 0c00 2c02 000c 002f 0800 0c00 3202  ....,..../....2.
-00006d30: 000c 002a 0200 0c00 2a02 000c 002f 0200  ...*....*..../..
-00006d40: 0c00 3002 000c 0030 0200 0c00 3402 000c  ..0....0....4...
-00006d50: 0030 0200 0c00 3402 000c 002e 0200 0c00  .0....4.........
-00006d60: 3602 000c 0032 0200 0c00 3102 000c 002f  6....2....1..../
-00006d70: 0200 0c00 2e02 000c 0031 0200 0c00 3802  .........1....8.
-00006d80: 000c 0031 0200 0c00 2e02 000c 0032 0200  ...1.........2..
-00006d90: 0c00 3902 000c 002e 0200 0c00 2d02 000c  ..9.........-...
-00006da0: 0029 0800 0c00 2e08 000c 002c 0200 0c00  .).........,....
-00006db0: 3102 000c 002d 0200 0c00 2c02 000c 002d  1....-....,....-
-00006dc0: 0200 0c00 3008 000c 0001 0679 3001 aeca  ....0......y0...
-00006dd0: 01ae d101 aeec 01ae f601 af02 01af 1201  ................
-00006de0: af23 01af bb01 b22a 01b2 3b01 b251 01b2  .#.....*..;..Q..
-00006df0: 6601 b2a9 01af 7901 af89 01af a437 0f00  f.....y......7..
-00006e00: 0043 480d 0600 5d02 2e3b 0000 0200 0a00  .CH...]..;......
-00006e10: 6507 0019 0477 0900 6a00 342d 0002 7d6d  e....w..j.4-..}m
-00006e20: 0a00 0009 0000 0100 100a 5908 003e 0208  ..........Y..>..
-00006e30: 1100 0c04 790c 0000 0406 80a7 0d73 0001  ....y........s..
-00006e40: 0a79 8135 1000 0039 0c09 0600 1602 520d  .y.5...9......R.
-00006e50: 0000 0200 1c00 411c 0065 0277 5400 027f  ......A..e.wT...
-00006e60: 440b 0000 0e00 3d04 3507 0071 0400 1d0d  D.....=.5..q....
-00006e70: 0a02 004c 0077 1c00 1d00 5e02 000b 0075  ...L.w....^....u
-00006e80: 0200 1e05 0a02 000c 0075 0c00 1e09 0a02  .........u......
-00006e90: 000c 0071 1400 1e22 0a02 000c 001f 4600  ...q..."......F.
-00006ea0: 0c00 2402 000c 0024 0200 0d00 2602 000d  ..$....$....&...
-00006eb0: 0021 0200 0d00 8087 0600 3000 2602 000d  .!........0.&...
-00006ec0: 0080 9202 001b 0033 0400 0d00 3a02 0007  .......3....:...
-00006ed0: 0025 0200 0800 3302 0007 001e 0200 0800  .%....3.........
-00006ee0: 2802 000e 0027 0200 0700 2f04 000d 0036  (....'..../....6
-00006ef0: 0200 0700 2a02 0008 002f 0200 0700 1e02  ....*..../......
-00006f00: 0008 0028 0200 0e00 2702 0007 002f 0400  ...(....'..../..
-00006f10: 0d00 3602 0007 0027 0200 0900 2f02 0007  ..6....'..../...
-00006f20: 001e 0200 0800 2802 000e 0027 0200 0700  ......(....'....
-00006f30: 2f04 000d 0036 0200 0700 2c02 0009 002f  /....6....,..../
-00006f40: 0200 0700 1e02 0008 0028 0200 0e00 2702  .........(....'.
-00006f50: 0007 002f 0400 0d00 3602 0007 002a 0200  .../....6....*..
-00006f60: 0900 2f02 0007 001f 0200 0900 2802 000e  ../.........(...
-00006f70: 0027 0200 0700 0102 790b 5379 7374 656d  .'......y.System
-00006f80: 2e54 6578 7423 01ae ca01 aed1 01ae ec01  .Text#..........
-00006f90: aef6 01af 0201 af12 01af 2301 c000 54f1  ..........#...T.
-00006fa0: 01af 7901 af89 01af a47d 1100 005a 0c09  ..y......}...Z..
-00006fb0: 0b00 1602 560d 0000 0500 1e00 3d18 0011  ....V.......=...
-00006fc0: 0430 0e00 0005 0010 0059 0900 8084 0477  .0.......Y.....w
-00006fd0: 808d 0002 7d2c 0e00 000e 0002 7d14 0e00  ....},......}...
-00006fe0: 000e 0038 0e31 0700 5602 0017 110a 0200  ...8.1..V.......
-00006ff0: 2100 6e24 001d 0048 0200 0b00 2102 000c  !.n$...H....!...
-00007000: 0046 0200 1c00 3702 0006 0024 0200 0700  .F....7....$....
-00007010: 3002 0007 001b 0200 0800 2202 000d 0021  0........."....!
-00007020: 0200 0700 0102 790c 0000 0080 a30a 0921  ......y........!
-00007030: 0001 0279 1b01 aeca 01ae d101 aeec 01ae  ...y............
-00007040: f601 af02 01af 1201 af23 01af 7901 af89  .........#..y...
-00007050: 4b12 0000 4d0a 0912 005d 0600 2100 5f02  K...M....]..!._.
-00007060: 0021 002b 0600 0d00 5d04 0811 1412 0279  .!.+....]......y
-00007070: 2107 1a2c 0021 0080 af12 0021 0080 af02  !..,.!.....!....
-00007080: 0021 0080 8904 001b 0080 a304 0021 2a0a  .!...........!*.
-00007090: 0400 1b0d 0a5a 001b 0001 1c79 0600 0000  .....Z.....y....
-000070a0: 1a61 2307 0000 0018 82e7 3107 0000 0018  .a#.......1.....
-000070b0: 82f7 4907 0000 0017 82f8 4907 0000 0017  ..I.......I.....
-000070c0: 82f9 3307 0000 0018 8313 5107 0000 0018  ..3.......Q.....
-000070d0: 8314 5107 0000 0018 8315 5107 0000 0018  ..Q.......Q.....
-000070e0: 8316 5108 0000 0180 aa84 ee3f 0700 0002  ..Q........?....
-000070f0: 6684 fd40 0700 0002 6685 1440 0800 0001  f..@....f..@....
-00007100: 80a6 851e 4007 0000 0035 88e4 4007 0000  ....@....5..@...
-00007110: 0030 890a 7307 0000 0036 8927 6a07 0000  .0..s....6.'j...
-00007120: 0030 8959 5707 0000 0030 8969 7107 1300  .0.YW....0.iq...
-00007130: 0040 8973 7107 0000 002f 897a 7107 0000  .@.sq..../.zq...
-00007140: 0034 8985 7107 0000 0042 84e0 5207 0000  .4..q....B..R...
-00007150: 0042 88eb 5206 0000 006c 0f22 0600 0000  .B..R....l."....
-00007160: 3426 3f07 1400 0067 80d2 4406 1500 0037  4&?....g..D....7
-00007170: 3535 0600 0000 2c36 3506 0000 0001 4949  55....,65.....II
-00007180: 0600 0000 6a2f 2506 0000 004a 3225 0600  ....j/%....J2%..
-00007190: 0000 6e3b 2606 0000 004d 3e26            ..n;&....M>&
+00000140: 3301 0200 6601 0100 7301 0200 a301 0100  3...f...s.......
+00000150: b001 0200 e201 0100 ef01 0200 1e02 0100  ................
+00000160: 2b02 0200 6802 0100 7702 0200 b102 0100  +...h...w.......
+00000170: c002 0200 f702 0100 0603 0200 4103 0100  ............A...
+00000180: 5003 0200 7c03 0100 8903 0200 b503 0100  P...|...........
+00000190: c003 0200 ef03 0100 fa03 0200 4904 0100  ............I...
+000001a0: 5a04 0200 1b05 0100 2c05 0200 3106 0100  Z.......,...1...
+000001b0: 4206 0200 0000 0000 0000 0000 0000 0000  B...............
+000001c0: 0000 0000 0000 0000 0100 002f 0100 922f  .........../.../
+000001d0: 0100 9e2f 0200 aa2f 0200 5130 0200 5830  .../.../..Q0..X0
+000001e0: 0200 8230 0200 9830 0200 ae30 0200 ba30  ...0...0...0...0
+000001f0: 0200 c630 0200 d230 0200 dc30 0300 2431  ...0...0...0..$1
+00000200: 0000 0000 0400 e531 0f00 2432 0f00 7333  .......1..$2..s3
+00000210: 0000 0000 0f00 cd47 1000 d447 0000 0000  .......G...G....
+00000220: 1000 3948 1000 4148 1000 4e48 0000 0000  ..9H..AH..NH....
+00000230: 0000 0000 1000 6a48 1000 7248 1000 7f48  ......jH..rH...H
+00000240: 1000 9148 0500 9948 0500 db48 0500 8649  ...H...H...H...I
+00000250: 0000 0000 0600 9849 0000 0000 0700 d749  .......I.......I
+00000260: 0700 344a 0000 0000 0800 9f4a 0000 0000  ..4J.......J....
+00000270: 0900 3e4e 0000 0000 0e00 f94e 0000 0000  ..>N.......N....
+00000280: 0e00 5d54 0e00 9554 0a00 a254 0000 0000  ..]T...T...T....
+00000290: 0b00 0956 0000 0000 0c00 8756 0000 0000  ...V.......V....
+000002a0: 0d00 9456 0000 0000 0000 0000 0200 e056  ...V...........V
+000002b0: 0000 0000 0000 0000 0f00 e756 0f00 ef56  ...........V...V
+000002c0: 0f00 f756 0f00 ff56 0f00 0757 0f00 0f57  ...V...V...W...W
+000002d0: 0f00 1757 0f00 1f57 0f00 2757 0f00 3057  ...W...W..'W..0W
+000002e0: 0f00 3857 0f00 4057 0f00 4957 0f00 5157  ..8W..@W..IW..QW
+000002f0: 0f00 5957 0f00 6157 0f00 6957 0f00 7157  ..YW..aW..iW..qW
+00000300: 0f00 7957 0f00 8157 0000 0000 0f00 8957  ..yW...W.......W
+00000310: 0f00 9157 0000 0000 0700 9957 0000 0000  ...W.......W....
+00000320: 0000 0000 0800 a057 0800 a757 0000 0000  .......W...W....
+00000330: 0800 af57 0800 b657 0000 0000 0000 0000  ...W...W........
+00000340: 0e00 bd57 0000 0000 0e00 c457 0e00 cb57  ...W.......W...W
+00000350: 0e00 d257 0e00 d957 0600 0300 0100 0100  ...W...W........
+00000360: 0000 0000 0700 0000 0700 0300 0100 0100  ................
+00000370: 0000 0000 0800 0000 0800 0300 0100 0100  ................
+00000380: 0000 0000 0900 0000 0900 0500 0100 0100  ................
+00000390: 0000 0000 1500 0000 0a00 0500 0100 0100  ................
+000003a0: 0000 0000 0d00 0000 0b00 0500 0100 0100  ................
+000003b0: 0000 0000 8500 0000 0c00 0500 0200 0100  ................
+000003c0: 0000 0000 2700 0000 0d00 0500 0300 0100  ....'...........
+000003d0: 0000 0000 2700 0000 0e00 0500 0400 0100  ....'...........
+000003e0: 0000 0000 0d00 0000 0f00 0500 0400 0100  ................
+000003f0: 0000 0000 8300 0000 1000 0500 0400 0100  ................
+00000400: 0000 0000 7500 0000 1100 0500 0400 0100  ....u...........
+00000410: 0000 0000 4a00 0000 1200 0500 0500 0100  ....J...........
+00000420: 0000 0000 d000 0000 1300 0700 0900 0100  ................
+00000430: 0000 0000 8901 0000 1300 0700 0a00 0100  ................
+00000440: c900 0000 5900 0000 1300 0700 0c00 0100  ....Y...........
+00000450: 4b01 0000 3300 0000 1300 0700 0d00 0100  K...3...........
+00000460: 5001 0000 2e00 0000 1500 0900 0e00 0100  P...............
+00000470: 0000 0000 1200 0000 1600 0b00 0e00 0100  ................
+00000480: 0000 0000 6900 0000 1700 0b00 0f00 0100  ....i...........
+00000490: 0000 0000 eb69 0000 1700 0b00 3800 0800  .....i......8...
+000004a0: 2700 0000 2a00 0000 1700 0b00 3900 0800  '...*.......9...
+000004b0: 6105 0000 4b00 0000 1700 0b00 3a00 0800  a...K.......:...
+000004c0: 0007 0000 2300 0000 1700 0b00 3b00 0800  ....#.......;...
+000004d0: b209 0000 2300 0000 1700 0b00 3c00 0800  ....#.......<...
+000004e0: 3d0b 0000 2600 0000 1700 0b00 3d00 0800  =...&.......=...
+000004f0: b60b 0000 4500 0000 1700 0b00 3e00 0800  ....E.......>...
+00000500: 8f0c 0000 4500 0000 1700 0b00 3f00 0800  ....E.......?...
+00000510: 330e 0000 2900 0000 1700 0b00 4000 0800  3...).......@...
+00000520: 5312 0000 c401 0000 1700 0b00 4100 0800  S...........A...
+00000530: 5f12 0000 a601 0000 1700 0b00 4600 0800  _...........F...
+00000540: 4315 0000 2900 0000 1700 0b00 4700 0800  C...).......G...
+00000550: b715 0000 6000 0000 1700 0b00 4800 0800  ....`.......H...
+00000560: be15 0000 5900 0000 1700 0b00 4900 0800  ....Y.......I...
+00000570: 6d17 0000 890e 0000 1700 0b00 5600 0800  m...........V...
+00000580: 6d2f 0000 2900 0000 1700 0b00 5700 0800  m/..).......W...
+00000590: 5d32 0000 2900 0000 1700 0b00 5800 0800  ]2..).......X...
+000005a0: 6834 0000 2900 0000 1700 0b00 5900 0800  h4..).......Y...
+000005b0: 4f35 0000 2900 0000 1700 0b00 5a00 0800  O5..).......Z...
+000005c0: 1236 0000 2900 0000 1700 0b00 5b00 0800  .6..).......[...
+000005d0: d73c 0000 2900 0000 1700 0b00 5c00 0800  .<..).......\...
+000005e0: 533e 0000 e809 0000 1700 0b00 5e00 0800  S>..........^...
+000005f0: 6f3e 0000 cc09 0000 1700 0b00 5f00 0800  o>.........._...
+00000600: 733e 0000 7509 0000 1700 0b00 6500 0800  s>..u.......e...
+00000610: a041 0000 3700 0000 1700 0b00 6600 0800  .A..7.......f...
+00000620: 9250 0000 8107 0000 1700 0b00 6800 0800  .P..........h...
+00000630: ae50 0000 6507 0000 1700 0b00 6b00 0800  .P..e.......k...
+00000640: d954 0000 2200 0000 1700 0b00 6c00 0800  .T..".......l...
+00000650: e25b 0000 2300 0000 1700 0b00 6d00 0800  .[..#.......m...
+00000660: 3b5c 0000 8b00 0000 1700 0b00 6e00 0800  ;\..........n...
+00000670: 865c 0000 2900 0000 1700 0b00 6f00 0800  .\..).......o...
+00000680: d75c 0000 5e00 0000 1700 0b00 7000 0800  .\..^.......p...
+00000690: 835e 0000 4a00 0000 1700 0b00 7100 0800  .^..J.......q...
+000006a0: 2b5f 0000 3600 0000 1700 0b00 7200 0800  +_..6.......r...
+000006b0: 3960 0000 3600 0000 1700 0b00 7300 0800  9`..6.......s...
+000006c0: cd60 0000 4a00 0000 1700 0b00 7400 0800  .`..J.......t...
+000006d0: 6a61 0000 2900 0000 1700 0b00 7500 0800  ja..).......u...
+000006e0: 3967 0000 bf00 0000 1700 0b00 7600 0800  9g..........v...
+000006f0: 4067 0000 b800 0000 1700 0b00 7700 0800  @g..........w...
+00000700: 8067 0000 3300 0000 1700 0b00 7800 0800  .g..3.......x...
+00000710: 1b68 0000 0d01 0000 1700 0b00 7900 0800  .h..........y...
+00000720: 5268 0000 a200 0000 1700 0b00 7a00 0800  Rh..........z...
+00000730: a869 0000 4200 0000 1900 0b00 7b00 0800  .i..B.......{...
+00000740: 0000 0000 0b00 0000 1a00 0d00 7b00 0800  ............{...
+00000750: 0000 0000 3e00 0000 1c00 0d00 7b00 0800  ....>.......{...
+00000760: 0000 0000 1200 0000 1d00 0d00 7b00 0800  ............{...
+00000770: 0000 0000 1600 0000 1e00 0d00 7b00 0800  ............{...
+00000780: 0000 0000 3e00 0000 2100 0d00 7b00 0800  ....>...!...{...
+00000790: 0000 0000 1200 0000 2200 0d00 7b00 0800  ........"...{...
+000007a0: 0000 0000 1d00 0000 2300 0d00 7b00 0800  ........#...{...
+000007b0: 0000 0000 2800 0000 2400 0d00 7b00 0800  ....(...$...{...
+000007c0: 0000 0000 1200 0000 2500 1000 7b00 0800  ........%...{...
+000007d0: 0000 0000 b600 0000 2600 1000 7b00 0800  ........&...{...
+000007e0: 0000 0000 5906 0000 2700 1000 7c00 0800  ....Y...'...|...
+000007f0: 0000 0000 1100 0000 2900 1300 7c00 0800  ........)...|...
+00000800: 0000 0000 8e00 0000 2b00 1600 7c00 0800  ........+...|...
+00000810: 0000 0000 8a00 0000 2c00 1600 7f00 0800  ........,.......
+00000820: 0000 0000 5501 0000 2c00 1600 7f00 0800  ....U...,.......
+00000830: 2b00 0000 1d00 0000 2c00 1600 8000 0800  +.......,.......
+00000840: a200 0000 1d00 0000 2c00 1600 8100 0800  ........,.......
+00000850: 1b01 0000 2000 0000 2e00 1900 8200 0800  .... ...........
+00000860: 0000 0000 600e 0000 2e00 1900 8500 0800  ....`...........
+00000870: 3801 0000 6501 0000 2e00 1900 8600 0800  8...e...........
+00000880: 3f01 0000 5e01 0000 2e00 1900 8700 0800  ?...^...........
+00000890: ea01 0000 1800 0000 2e00 1900 8800 0800  ................
+000008a0: c602 0000 7d0b 0000 2e00 1900 8a00 0800  ....}...........
+000008b0: e202 0000 610b 0000 2e00 1900 8b00 0800  ....a...........
+000008c0: f602 0000 fa0a 0000 2e00 1900 8c00 0800  ................
+000008d0: 1103 0000 bf0a 0000 2e00 1900 8d00 0800  ................
+000008e0: 1a03 0000 b60a 0000 2e00 1900 9400 0800  ................
+000008f0: 2c04 0000 c901 0000 2e00 1900 9600 0800  ,...............
+00000900: 0805 0000 8c00 0000 2e00 1900 9700 0800  ................
+00000910: 0d05 0000 7900 0000 2e00 1900 9800 0800  ....y...........
+00000920: 0406 0000 8000 0000 2e00 1900 9900 0800  ................
+00000930: 7b0a 0000 b100 0000 2e00 1900 9b00 0800  {...............
+00000940: 8f0b 0000 fa00 0000 2e00 1900 9c00 0800  ................
+00000950: 580c 0000 1800 0000 2e00 1900 9d00 0800  X...............
+00000960: a50c 0000 e200 0000 3000 1c00 9e00 0800  ........0.......
+00000970: 0000 0000 b205 0000 3200 1f00 a300 0800  ........2.......
+00000980: 0000 0000 f532 0000 3200 1f00 a500 0800  .....2..2.......
+00000990: 1a00 0000 6c00 0000 3200 1f00 a600 0800  ....l...2.......
+000009a0: 2000 0000 5a00 0000 3200 1f00 a700 0800   ...Z...2.......
+000009b0: c700 0000 b600 0000 3200 1f00 a800 0800  ........2.......
+000009c0: d000 0000 ad00 0000 3200 1f00 a900 0800  ........2.......
+000009d0: 9901 0000 0502 0000 3200 1f00 ac00 0800  ........2.......
+000009e0: 5f02 0000 4000 0000 3200 1f00 ad00 0800  _...@...2.......
+000009f0: 5e03 0000 4000 0000 3200 1f00 ae00 0800  ^...@...2.......
+00000a00: d62d 0000 4700 0000 3400 1f00 af00 0800  .-..G...4.......
+00000a10: 0000 0000 af00 0000 3400 1f00 b000 0800  ........4.......
+00000a20: 4300 0000 3d00 0000 3500 1f00 b100 0800  C...=...5.......
+00000a30: 0000 0000 7400 0000 3600 2300 b100 0800  ....t...6.#.....
+00000a40: 0000 0000 9003 0000 3600 2300 bb00 0800  ........6.#.....
+00000a50: 1500 0000 7000 0000 3800 2300 bd00 0800  ....p...8.#.....
+00000a60: 0000 0000 d601 0000 3800 2300 c200 0800  ........8.#.....
+00000a70: 1d00 0000 dd00 0000 3800 2300 c300 0800  ........8.#.....
+00000a80: 4800 0000 9600 0000 3a00 2400 c400 0800  H.......:.$.....
+00000a90: 0000 0000 2200 0000 3c00 2400 c400 0800  ...."...<.$.....
+00000aa0: 0000 0000 6901 0000 3f00 0500 c500 0800  ....i...?.......
+00000ab0: 0000 0000 1d00 0000 4200 0b00 c500 0800  ........B.......
+00000ac0: 0000 0000 1d00 0000 4300 0b00 c500 0800  ........C.......
+00000ad0: 0000 0000 1a00 0000 4400 0b00 c500 0800  ........D.......
+00000ae0: 0000 0000 1a00 0000 4500 0b00 c500 0800  ........E.......
+00000af0: 0000 0000 1a00 0000 4600 0b00 c500 0800  ........F.......
+00000b00: 0000 0000 1d00 0000 4700 0b00 c500 0800  ........G.......
+00000b10: 0000 0000 1d00 0000 4800 0b00 c500 0800  ........H.......
+00000b20: 0000 0000 1d00 0000 4900 0b00 c500 0800  ........I.......
+00000b30: 0000 0000 1d00 0000 4a00 0b00 c500 0800  ........J.......
+00000b40: 0000 0000 4300 0000 4b00 0b00 c500 0800  ....C...K.......
+00000b50: 0000 0000 5a00 0000 4c00 0b00 c500 0800  ....Z...L.......
+00000b60: 0000 0000 5a00 0000 4d00 0b00 c500 0800  ....Z...M.......
+00000b70: 0000 0000 4300 0000 4e00 0b00 c500 0800  ....C...N.......
+00000b80: 0000 0000 1600 0000 4f00 0b00 c500 0800  ........O.......
+00000b90: 0000 0000 1b00 0000 5000 0b00 c500 0800  ........P.......
+00000ba0: 0000 0000 1b00 0000 5100 0b00 c500 0800  ........Q.......
+00000bb0: 0000 0000 1b00 0000 5200 0b00 c500 0800  ........R.......
+00000bc0: 0000 0000 1b00 0000 5300 0b00 c500 0800  ........S.......
+00000bd0: 0000 0000 3300 0000 5400 0b00 c500 0800  ....3...T.......
+00000be0: 0000 0000 1b00 0000 5500 0b00 c500 0800  ........U.......
+00000bf0: 0000 0000 1b00 0000 5700 0b00 c500 0800  ........W.......
+00000c00: 0000 0000 1d00 0000 5800 0b00 c500 0800  ........X.......
+00000c10: 0000 0000 1d00 0000 5a00 1600 c500 0800  ........Z.......
+00000c20: 0000 0000 4000 0000 5d00 1900 c500 0800  ....@...].......
+00000c30: 0000 0000 1b00 0000 5e00 1900 c500 0800  ........^.......
+00000c40: 0000 0000 6100 0000 6000 1900 c500 0800  ....a...`.......
+00000c50: 0000 0000 3300 0000 6100 1900 c500 0800  ....3...a.......
+00000c60: 0000 0000 1a00 0000 6400 1f00 c500 0800  ........d.......
+00000c70: 0000 0000 0200 0000 6600 1f00 c500 0800  ........f.......
+00000c80: 0000 0000 3900 0000 6700 1f00 c500 0800  ....9...g.......
+00000c90: 0000 0000 3100 0000 6800 1f00 c500 0800  ....1...h.......
+00000ca0: 0000 0000 3900 0000 6900 1f00 c500 0800  ....9...i.......
+00000cb0: 0000 0000 3100 0000 0000 0000 c906 0000  ....1...........
+00000cc0: 0000 c906 0000 0000 c906 0000 0000 0100  ................
+00000cd0: 0000 0000 7007 0000 0100 c104 0000 0200  ....p...........
+00000ce0: 3203 0000 0300 a806 0000 0000 0203 0000  2...............
+00000cf0: 0400 6802 0000 0500 5b02 0000 0900 2f02  ..h.....[...../.
+00000d00: 0000 0a00 5202 0000 0000 5407 0000 0000  ....R.....T.....
+00000d10: 0100 0000 0100 de04 0000 0200 c402 0000  ................
+00000d20: 0300 a002 0000 0400 a703 0000 0500 1106  ................
+00000d30: 0000 0600 2a04 0000 0700 d501 0000 0800  ....*...........
+00000d40: fa06 0000 0900 7103 0000 0a00 ca03 0000  ......q.........
+00000d50: 0b00 8b06 0000 0c00 d206 0000 0d00 f303  ................
+00000d60: 0000 0e00 df03 0000 0f00 4200 0000 1000  ..........B.....
+00000d70: 5200 0000 1100 2f00 0000 1200 e105 0000  R...../.........
+00000d80: 1300 6105 0000 1400 0b04 0000 1500 8e01  ..a.............
+00000d90: 0000 1600 2903 0000 1700 9a01 0000 1800  ....)...........
+00000da0: 6106 0000 1900 4606 0000 1a00 3206 0000  a.....F.....2...
+00000db0: 1b00 7706 0000 1c00 3c04 0000 1d00 e906  ..w.....<.......
+00000dc0: 0000 1e00 0107 0000 1f00 1307 0000 2000  .............. .
+00000dd0: 9806 0000 2100 c501 0000 2200 b501 0000  ....!.....".....
+00000de0: 2300 a904 0000 2400 cb04 0000 2500 9604  #.....$.....%...
+00000df0: 0000 2600 4107 0000 2700 2507 0000 2800  ..&.A...'.%...(.
+00000e00: 6d05 0000 2900 be04 0000 2c00 f701 0000  m...).....,.....
+00000e10: 2d00 3e02 0000 2e00 3e02 0000 2f00 3e02  -.>.....>.../.>.
+00000e20: 0000 3100 d100 0000 3300 d100 0000 3400  ..1.....3.....4.
+00000e30: 3e02 0000 3600 2703 0000 3700 1704 0000  >...6.'...7.....
+00000e40: 3800 b402 0000 3900 d803 0000 3a00 1d06  8.....9.....:...
+00000e50: 0000 3b00 8403 0000 3c00 9602 0000 3d00  ..;.....<.....=.
+00000e60: 9602 0000 3e00 7007 0000 3f00 ce05 0000  ....>.p...?.....
+00000e70: 4000 8805 0000 4100 b805 0000 4200 a205  @.....A.....B...
+00000e80: 0000 4300 7a05 0000 4400 e904 0000 4500  ..C.z...D.....E.
+00000e90: 2105 0000 4600 7e01 0000 4700 7101 0000  !...F.~...G.q...
+00000ea0: 4800 4a03 0000 4900 4f01 0000 4a00 5903  H.J...I.O...J.Y.
+00000eb0: 0000 4b00 5e01 0000 4e00 f701 0000 5300  ..K.^...N.....S.
+00000ec0: f701 0000 5400 f701 0000 5500 f701 0000  ....T.....U.....
+00000ed0: 5600 f701 0000 5700 f701 0000 5900 4503  V.....W.....Y.E.
+00000ee0: 0000 5a00 0908 0000 5d00 d907 0000 5e00  ..Z.....].....^.
+00000ef0: b307 0000 5f00 c907 0000 6000 e707 0000  ...._.....`.....
+00000f00: 6100 fb07 0000 6200 9107 0000 6300 a507  a.....b.....c...
+00000f10: 0000 6400 4e07 0000 6600 7d02 0000 6700  ..d.N...f.}...g.
+00000f20: 4e04 0000 6b00 4005 0000 6c00 a701 0000  N...k.@...l.....
+00000f30: 6d00 3301 0000 6e00 4e07 0000 6f00 3e02  m.3...n.N...o.>.
+00000f40: 0000 7000 7402 0000 7100 0305 0000 7200  ..p.t...q.....r.
+00000f50: 2703 0000 7300 0305 0000 7400 0305 0000  '...s.....t.....
+00000f60: 7500 0305 0000 7600 0305 0000 7700 3e02  u.....v.....w.>.
+00000f70: 0000 7800 7402 0000 7900 4501 0000 7a00  ..x.t...y.E...z.
+00000f80: dc04 0000 7c00 9b02 0000 7d00 0305 0000  ....|.....}.....
+00000f90: 7e00 be04 0000 0000 c402 0000 0000 0100  ~...............
+00000fa0: 0000 0100 0a02 0000 0200 c804 0000 0100  ................
+00000fb0: 7a07 0000 0200 7a07 0000 0400 c102 0000  z.....z.........
+00000fc0: 0000 0100 0000 0100 8a04 0000 0200 3207  ..............2.
+00000fd0: 0000 0700 7402 0000 0800 6c03 0000 0c00  ....t.....l.....
+00000fe0: 3902 0000 0f00 2401 0000 1000 8707 0000  9.....$.........
+00000ff0: 1400 2701 0000 1500 6c03 0000 1600 0305  ..'.....l.......
+00001000: 0000 1700 4905 0000 1800 f202 0000 1900  ....I...........
+00001010: 9104 0000 1a00 5605 0000 1b00 0e05 0000  ......V.........
+00001020: 1c00 2c05 0000 1d00 c906 0000 1f00 0c03  ..,.............
+00001030: 0000 2000 e105 0000 2300 2703 0000 2400  .. .....#.'...$.
+00001040: 7b04 0000 2500 f701 0000 2800 0401 0000  {...%.....(.....
+00001050: 2900 e105 0000 2a00 d302 0000 2b00 3902  ).....*.....+.9.
+00001060: 0000 2c00 ed05 0000 0000 0c01 0000 0100  ..,.............
+00001070: c104 0000 0200 3203 0000 0300 bb03 0000  ......2.........
+00001080: 0400 2406 0000 0000 0100 0000 0100 fc01  ..$.............
+00001090: 0000 0200 c804 0000 0300 0a02 0000 0500  ................
+000010a0: 4503 0000 0600 3c03 0000 0900 1100 0000  E.....<.........
+000010b0: 0a00 2302 0000 0b00 1602 0000 0c00 c804  ..#.............
+000010c0: 0000 0d00 c804 0000 1000 4702 0000 0000  ..........G.....
+000010d0: c406 0000 0200 5007 0000 0000 6604 0000  ......P.....f...
+000010e0: 0100 de02 0000 0200 2100 0000 0300 5d07  ........!.....].
+000010f0: 0000 0400 1603 0000 0500 af06 0000 0600  ................
+00001100: 1a04 0000 0700 f504 0000 0800 9903 0000  ................
+00001110: 0900 0406 0000 0b00 7402 0000 0c00 fb00  ........t.......
+00001120: 0000 0000 5504 0000 0100 8802 0000 0200  ....U...........
+00001130: e701 0000 0300 8e03 0000 0400 fa05 0000  ................
+00001140: 0600 bb02 0000 0b00 2d01 0000 0000 d501  ........-.......
+00001150: 8b00 a347 ba00 a947 a100 af47 eb00 b547  ...G...G...G...G
+00001160: 7700 bb47 6300 c147 d800 c747 0000 0000  w..Gc..G...G....
+00001170: 0100 7c2f 0200 0000 0100 2c30 0400 0000  ..|/......,0....
+00001180: 0100 cc31 0600 0000 0100 0b32 0800 0000  ...1.......2....
+00001190: 0100 3133 0a00 0000 0100 1548 0c00 0000  ..13.......H....
+000011a0: 0100 bd48 0e00 0000 0f00 0000 0100 bb49  ...H...........I
+000011b0: 1100 0000 1200 0000 0100 0c4a 1400 0000  ...........J....
+000011c0: 1500 0000 0100 184e 1700 0000 1800 0000  .......N........
+000011d0: 0100 da4e 1a00 0000 1b00 0000 0100 2c54  ...N..........,T
+000011e0: 1d00 0000 1e00 0000 0100 e555 2000 0000  ...........U ...
+000011f0: 2100 0000 2200 0000 1300 0000 2700 0500  !...".......'...
+00001200: be07 2700 0600 e708 2700 0700 100b 8301  ..'.....'.......
+00001210: 0400 bc07 a301 0400 bc07 c301 0400 bc07  ................
+00001220: e301 0400 bc07 0302 0400 bc07 3602 0300  ............6...
+00001230: 7b04 5602 0300 4d05 7602 0300 6306 8302  {.V...M.v...c...
+00001240: 0400 bc07 a302 0400 bc07 c302 0400 bc07  ................
+00001250: 6303 0400 bc07 0000 0043 5324 3c3e 385f  c........CS$<>8_
+00001260: 5f6c 6f63 616c 7330 0043 5324 3c3e 385f  _locals0.CS$<>8_
+00001270: 5f6c 6f63 616c 7331 0072 6f6f 6d4e 616d  _locals1.roomNam
+00001280: 6548 7564 4343 0077 6174 6572 5475 7262  eHudCC.waterTurb
+00001290: 696e 6544 6f6f 7243 4300 7468 6f74 684c  ineDoorCC.thothL
+000012a0: 6566 7444 6f6f 7243 4300 7468 6f74 6852  eftDoorCC.thothR
+000012b0: 6967 6874 446f 6f72 4343 0050 6970 6549  ightDoorCC.PipeI
+000012c0: 6e44 6570 7468 7355 7070 6572 4944 0050  nDepthsUpperID.P
+000012d0: 6970 6549 6e44 6570 7468 734c 6f77 6572  ipeInDepthsLower
+000012e0: 4944 0054 686f 7468 4272 6964 6765 4c65  ID.ThothBridgeLe
+000012f0: 6674 446f 6f72 4944 0041 3257 6174 6572  ftDoorID.A2Water
+00001300: 5475 7262 696e 654c 6566 7444 6f6f 7249  TurbineLeftDoorI
+00001310: 4400 5468 6f74 6842 7269 6467 6552 6967  D.ThothBridgeRig
+00001320: 6874 446f 6f72 4944 0064 6f6f 7249 4400  htDoorID.doorID.
+00001330: 5069 7065 496e 5761 7465 7266 616c 6c73  PipeInWaterfalls
+00001340: 4944 0050 6970 6549 6e48 6964 656f 7574  ID.PipeInHideout
+00001350: 4944 0072 6f6f 6d44 6174 6100 666c 6970  ID.roomData.flip
+00001360: 7065 6400 6f43 6f6e 7472 6f6c 4e65 7477  ped.oControlNetw
+00001370: 6f72 6b52 6563 6569 7665 6400 6964 0066  orkReceived.id.f
+00001380: 6f75 6e64 0063 6f6f 7264 0063 6f6c 6c69  ound.coord.colli
+00001390: 7369 6f6e 436f 6465 546f 4265 006d 7573  sionCodeToBe.mus
+000013a0: 6963 436f 6465 0064 6570 7468 7350 6970  icCode.depthsPip
+000013b0: 6543 6f64 6500 7761 7465 7266 616c 6c73  eCode.waterfalls
+000013c0: 5069 7065 436f 6465 006e 6573 7450 6970  PipeCode.nestPip
+000013d0: 6543 6f64 6500 6869 6465 6f75 7450 6970  eCode.hideoutPip
+000013e0: 6543 6f64 6500 6472 6177 4775 6943 6f64  eCode.drawGuiCod
+000013f0: 6500 6c61 6242 6c6f 636b 436f 6465 0063  e.labBlockCode.c
+00001400: 6f6c 6c69 7369 6f6e 436f 6465 006c 6f61  ollisionCode.loa
+00001410: 6447 6c6f 6261 6c73 436f 6465 0073 6176  dGlobalsCode.sav
+00001420: 6547 6c6f 6261 6c73 436f 6465 0063 6861  eGlobalsCode.cha
+00001430: 7261 6374 6572 5661 7273 436f 6465 0073  racterVarsCode.s
+00001440: 7346 4744 6573 7472 6f79 436f 6465 0063  sFGDestroyCode.c
+00001450: 6f64 6500 7574 5465 7874 7572 6550 6167  ode.utTexturePag
+00001460: 6500 7465 7874 7572 6550 6167 6500 6134  e.texturePage.a4
+00001470: 5061 6765 3249 6d61 6765 0061 3450 6167  Page2Image.a4Pag
+00001480: 6549 6d61 6765 006d 7573 6963 4669 6c65  eImage.musicFile
+00001490: 0074 696c 6500 636f 6465 4e61 6d65 0073  .tile.codeName.s
+000014a0: 7072 6974 654e 616d 6500 6f72 6967 4e61  priteName.origNa
+000014b0: 6d65 006f 7269 6753 6f6e 674e 616d 6500  me.origSongName.
+000014c0: 6e65 7753 6f6e 674e 616d 6500 726f 6f6d  newSongName.room
+000014d0: 4e61 6d65 0070 6963 6b75 704e 616d 6500  Name.pickupName.
+000014e0: 4453 4d61 7043 6f6f 7264 526f 6f6d 6e61  DSMapCoordRoomna
+000014f0: 6d65 0070 6970 6500 7769 7364 6f6d 5365  me.pipe.wisdomSe
+00001500: 7074 6f67 6743 7265 6174 6500 6372 6561  ptoggCreate.crea
+00001510: 7465 0076 616c 7565 0062 6700 6f57 6973  te.value.bg.oWis
+00001520: 646f 6d53 6570 746f 6767 006c 6566 7446  domSeptogg.leftF
+00001530: 6163 696e 6700 726f 6f6d 4e61 6d65 4453  acing.roomNameDS
+00001540: 4d61 7053 7472 696e 6700 6973 5265 7365  MapString.isRese
+00001550: 6172 6368 4861 7463 6800 6d75 7369 6350  archHatch.musicP
+00001560: 6174 6800 7469 6c65 4465 7074 6800 726f  ath.tileDepth.ro
+00001570: 6f6d 4e61 6d65 4875 6444 7261 7747 7569  omNameHudDrawGui
+00001580: 006c 6162 426c 6f63 6b00 6172 6773 4c6f  .labBlock.argsLo
+00001590: 6361 6c00 7061 6765 4974 656d 0069 7465  cal.pageItem.ite
+000015a0: 6d00 6465 7074 6873 5069 7065 526f 6f6d  m.depthsPipeRoom
+000015b0: 0077 6174 6572 6661 6c6c 7350 6970 6552  .waterfallsPipeR
+000015c0: 6f6f 6d00 726f 6f6d 0064 6f6f 7253 616d  oom.room.doorSam
+000015d0: 7573 436f 6c6c 6973 696f 6e00 636f 6c6c  usCollision.coll
+000015e0: 6973 696f 6e00 7373 4647 4163 7469 6f6e  ision.ssFGAction
+000015f0: 0072 6f6f 6d48 7564 4163 7469 6f6e 0077  .roomHudAction.w
+00001600: 6973 646f 6d53 6570 746f 6767 4163 7469  isdomSeptoggActi
+00001610: 6f6e 006f 436f 6e74 726f 6c41 6374 696f  on.oControlActio
+00001620: 6e00 7661 7244 6f6f 7241 6374 696f 6e00  n.varDoorAction.
+00001630: 6163 7469 6f6e 0061 3541 6374 6976 6174  action.a5Activat
+00001640: 6543 6f6e 6469 7469 6f6e 0065 6d70 4261  eCondition.empBa
+00001650: 7474 6572 7943 656c 6c43 6f6e 6469 7469  tteryCellConditi
+00001660: 6f6e 0073 6372 444e 4153 7061 776e 0067  on.scrDNASpawn.g
+00001670: 6f00 726f 6f6d 4e61 6d65 4875 6453 7465  o.roomNameHudSte
+00001680: 7000 7769 7364 6f6d 5365 7074 6f67 6753  p.wisdomSeptoggS
+00001690: 7465 7000 7375 6273 6372 6565 6e4d 656e  tep.subscreenMen
+000016a0: 7553 7465 7000 7069 636b 7570 0064 734d  uStep.pickup.dsM
+000016b0: 6170 436f 7264 4275 696c 6465 7200 726f  apCordBuilder.ro
+000016c0: 6f6d 4e61 6d65 4453 4d61 7042 7569 6c64  omNameDSMapBuild
+000016d0: 6572 0074 696c 6573 6574 436f 756e 7465  er.tilesetCounte
+000016e0: 7200 6135 446f 6f72 0064 6f6f 7200 616c  r.a5Door.door.al
+000016f0: 7265 6164 7941 6464 6564 5042 6f6d 6273  readyAddedPBombs
+00001700: 0061 6c72 6561 6479 4164 6465 644d 6973  .alreadyAddedMis
+00001710: 7369 6c65 7300 6673 006c 6f63 616c 7300  siles.fs.locals.
+00001720: 6d73 0061 6c72 6561 6479 4164 6465 6453  ms.alreadyAddedS
+00001730: 7570 6572 7300 7365 6564 4f62 6a65 6374  upers.seedObject
+00001740: 0073 6f6c 6964 4f62 6a65 6374 0072 6f6f  .solidObject.roo
+00001750: 6d48 7564 4f62 6a65 6374 0067 616d 654f  mHudObject.gameO
+00001760: 626a 6563 7400 7761 7465 7254 7572 6269  bject.waterTurbi
+00001770: 6e65 4f62 6a65 6374 0070 6970 654f 626a  neObject.pipeObj
+00001780: 6563 7400 7265 7365 6172 6368 4861 7463  ect.researchHatc
+00001790: 684f 626a 6563 7400 676d 4f62 6a65 6374  hObject.gmObject
+000017a0: 0069 7347 6f74 6f4f 626a 6563 7400 646f  .isGotoObject.do
+000017b0: 6f72 4f62 6a65 6374 0065 6e65 6d79 4f62  orObject.enemyOb
+000017c0: 6a65 6374 0065 7461 6e6b 536e 6970 7065  ject.etankSnippe
+000017d0: 7400 7069 7065 4247 5469 6c65 7365 7400  t.pipeBGTileset.
+000017e0: 6465 7074 6873 456e 7472 616e 6365 5069  depthsEntrancePi
+000017f0: 7065 5469 6c65 7365 7400 7761 7465 7266  peTileset.waterf
+00001800: 616c 6c73 5069 7065 5469 6c65 7365 7400  allsPipeTileset.
+00001810: 6465 7074 6873 4578 6974 5069 7065 5469  depthsExitPipeTi
+00001820: 6c65 7365 7400 6869 6465 6f75 7450 6970  leset.hideoutPip
+00001830: 6554 696c 6573 6574 0064 6f6f 7254 696c  eTileset.doorTil
+00001840: 6573 6574 006d 6f76 696e 674f 6666 7365  eset.movingOffse
+00001850: 7400 7373 4647 4576 656e 7400 726f 6f6d  t.ssFGEvent.room
+00001860: 4875 6445 7665 6e74 0077 6973 646f 6d53  HudEvent.wisdomS
+00001870: 6570 746f 6767 4576 656e 7400 6f43 6f6e  eptoggEvent.oCon
+00001880: 7472 6f6c 4576 656e 7400 7042 6f6d 6243  trolEvent.pBombC
+00001890: 6861 7261 6374 6572 4576 656e 7400 7375  haracterEvent.su
+000018a0: 7065 724d 6973 7369 6c65 4368 6172 6163  perMissileCharac
+000018b0: 7465 7245 7665 6e74 006d 6973 7369 6c65  terEvent.missile
+000018c0: 4368 6172 6163 7465 7245 7665 6e74 0065  CharacterEvent.e
+000018d0: 5461 6e6b 4368 6172 6163 7465 7245 7665  TankCharacterEve
+000018e0: 6e74 0076 6172 446f 6f72 4576 656e 7400  nt.varDoorEvent.
+000018f0: 6974 656d 7353 7761 7053 6372 6970 7400  itemsSwapScript.
+00001900: 7363 7269 7074 0072 6f6f 6d4e 616d 6548  script.roomNameH
+00001910: 7564 526f 6f6d 5374 6172 7400 6c69 7374  udRoomStart.list
+00001920: 0063 6f64 6554 6578 7400 6e65 7744 6f6f  .codeText.newDoo
+00001930: 7252 6570 6c61 6365 6d65 6e74 5465 7874  rReplacementText
+00001940: 0073 7562 7363 7265 656e 4d69 7363 4461  .subscreenMiscDa
+00001950: 7700 7373 4472 6177 0073 7562 6372 6565  w.ssDraw.subcree
+00001960: 6e42 6f6f 7473 4472 6177 0073 7562 7363  nBootsDraw.subsc
+00001970: 7265 656e 5375 6974 4472 6177 0064 7261  reenSuitDraw.dra
+00001980: 7745 6e64 496e 6465 7800 646f 6f72 4576  wEndIndex.doorEv
+00001990: 656e 7449 6e64 6578 0064 7261 7753 7461  entIndex.drawSta
+000019a0: 7274 496e 6465 7800 6b65 7900 6173 7365  rtIndex.key.asse
+000019b0: 6d62 6c79 0072 6f6f 6d4e 616d 6548 7564  mbly.roomNameHud
+000019c0: 4465 7374 726f 7900 636f 6465 456e 7472  Destroy.codeEntr
+000019d0: 7900 7465 7874 7572 6545 6e74 7279 0064  y.textureEntry.d
+000019e0: 6f6f 7245 6e74 7279 006c 6f63 6b65 6450  oorEntry.lockedP
+000019f0: 426f 6d62 5175 616e 7469 7479 0070 426f  BombQuantity.pBo
+00001a00: 6d62 5175 616e 7469 7479 006c 6f63 6b65  mbQuantity.locke
+00001a10: 644d 6973 7369 6c65 5175 616e 7469 7479  dMissileQuantity
+00001a20: 006d 6973 7369 6c65 5175 616e 7469 7479  .missileQuantity
+00001a30: 0066 696e 616c 5175 616e 7469 7479 006c  .finalQuantity.l
+00001a40: 6f63 6b65 6453 7570 6572 5175 616e 7469  ockedSuperQuanti
+00001a50: 7479 0073 7570 6572 5175 616e 7469 7479  ty.superQuantity
+00001a60: 0071 7561 6e74 6974 7900 0000 0000 0000  .quantity.......
+00001a70: 0fd0 2988 b811 1342 878b 770e 8597 ac16  ..)....B..w.....
+00001a80: f862 513f c607 d311 9053 00c0 4fa3 02a1  .bQ?.....S..O...
+00001a90: 1b57 8a0e 2669 6e46 b4ad 8ab0 4611 f5fe  .W..&inF....F...
+00001aa0: bc74 2e93 a9db 7844 8d46 0f32 a7ba b3d3  .t....xD.F.2....
+00001ab0: 5605 11cc 91a0 384d 9fec 25ab 9a35 1a6a  V.....8M..%..5.j
+00001ac0: 05ec feb5 d08c 834a 96da 4662 84bb 4bd8  .......J..Fb..K.
+00001ad0: 0847 4d7e 6e09 5c4c aeda cb10 ba6a 740d  .GM~n.\L.....jt.
+00001ae0: 0004 686f 6d65 0672 756e 6e65 7204 776f  ..home.runner.wo
+00001af0: 726b 0459 414d 5308 5941 4d53 2d4c 4942  rk.YAMS.YAMS-LIB
+00001b00: 0d45 7863 6570 7469 6f6e 732e 6373 092f  .Exceptions.cs./
+00001b10: 0001 060d 1212 1720 2045 cf63 12b5 33a2  .......  E.c..3.
+00001b20: 5dfc 4dce b431 5040 06cb b9c4 4b95 8487  ].M..1P@....K...
+00001b30: 2f00 aa0c 69ad 7c7b 7913 4578 7465 6e73  /...i.|{y.Extens
+00001b40: 696f 6e4d 6574 686f 6473 2e63 7309 2f00  ionMethods.cs./.
+00001b50: 0106 0d12 1217 5920 8e60 29b7 ed9a 0b1a  ......Y .`).....
+00001b60: 1a46 f770 be95 760e ea0e 8ec0 45b2 e613  .F.p..v.....E...
+00001b70: b318 395a 43ae 57f7 0f4d 7573 6963 5368  ..9ZC.W..MusicSh
+00001b80: 7566 666c 652e 6373 0a2f 0001 060d 1212  uffle.cs./......
+00001b90: 1780 9820 3c0a 97ef 3aba 9a95 23f6 7f5c  ... <...:...#..\
+00001ba0: 7a9b 8254 fac4 f5de dc3e 0a75 a15d d33b  z..T.....>.u.].;
+00001bb0: dcc7 45e4 0b50 6167 6549 7465 6d2e 6373  ..E..PageItem.cs
+00001bc0: 0a2f 0001 060d 1212 1780 d420 b8f4 0c63  ./......... ...c
+00001bd0: e376 41df 859c 9e67 96f9 3ff7 c2ee f73b  .vA....g..?....;
+00001be0: bfa8 ba8e 5fa9 fa91 408f 2dda 0770 6174  ...._...@.-..pat
+00001bf0: 6368 6573 1141 6464 496e 4761 6d65 4869  ches.AddInGameHi
+00001c00: 6e74 732e 6373 0c2f 0001 060d 1212 1781  nts.cs./........
+00001c10: 0c81 1420 6e02 69a1 68e9 d66f e7cc 3811  ... n.i.h..o..8.
+00001c20: 95b7 b370 bf14 88e1 e2a0 5b53 5d2c f554  ...p......[S],.T
+00001c30: b77d acd2 1143 6f6c 6f72 6564 4c6f 6742  .}...ColoredLogB
+00001c40: 6f6f 6b2e 6373 0c2f 0001 060d 1212 1781  ook.cs./........
+00001c50: 0c81 5420 9976 41d2 e57a 9dd3 dd48 b469  ..T .vA..z...H.i
+00001c60: 44a7 eba7 d941 9e3a 7de0 5496 2332 a331  D....A.:}.T.#2.1
+00001c70: c4bb 0036 0e43 6f73 6d65 7469 6348 7564  ...6.CosmeticHud
+00001c80: 2e63 730c 2f00 0106 0d12 1217 810c 8194  .cs./...........
+00001c90: 2021 0e9e e208 512b df26 8fe7 4a3d 859d   !....Q+.&..J=..
+00001ca0: 6171 9813 5331 5cb5 3dfc e038 894d ca8a  aq..S1\.=..8.M..
+00001cb0: e010 446f 6f72 4c6f 636b 5261 6e64 6f2e  ..DoorLockRando.
+00001cc0: 6373 0c2f 0001 060d 1212 1781 0c81 d120  cs./........... 
+00001cd0: 780a 31fc a051 1956 556d a460 50ff 69df  x.1..Q.VUm.`P.i.
+00001ce0: ae84 d034 fa19 3e85 4760 de9d b997 cd22  ...4..>.G`....."
+00001cf0: 0d4d 756c 7469 776f 726c 642e 6373 0c2f  .Multiworld.cs./
+00001d00: 0001 060d 1212 1781 0c82 1020 5745 9d60  ........... WE.`
+00001d10: dc2f cf43 e910 20e3 47c7 28bd 073b 292c  ./.C.. .G.(..;),
+00001d20: 110a 5be0 f2cb 6078 ac1f 09de 0371 6f6c  ..[...`x.....qol
+00001d30: 1744 6973 706c 6179 526f 6f6d 4e61 6d65  .DisplayRoomName
+00001d40: 4f6e 4855 442e 6373 0e2f 0001 060d 1212  OnHUD.cs./......
+00001d50: 1781 0c82 4c82 5020 4d23 0e05 5638 4766  ....L.P M#..V8Gf
+00001d60: 9700 43bc 2d01 9dcb c8ef f918 c361 86d3  ..C.-........a..
+00001d70: f16f c89a 1bfb ec85 1844 6973 706c 6179  .o.......Display
+00001d80: 526f 6f6d 4e61 6d65 734f 6e4d 6170 2e63  RoomNamesOnMap.c
+00001d90: 730e 2f00 0106 0d12 1217 810c 824c 8298  s./..........L..
+00001da0: 2099 1928 51d6 abde 1669 e226 83bb 64d4   ..(Q....i.&..d.
+00001db0: 46ec 545d 2c37 82f1 3415 3b56 6cd5 e2b5  F.T],7..4.;Vl...
+00001dc0: 3d15 526f 6f6d 4665 6174 7572 654d 6170  =.RoomFeatureMap
+00001dd0: 5465 7874 2e63 730e 2f00 0106 0d12 1217  Text.cs./.......
+00001de0: 810c 824c 82e1 20c4 8253 0a0a 876a 5cfe  ...L.. ..S...j\.
+00001df0: 6919 2a2c 85e5 ccb9 d59e 17e1 94a1 d4dc  i.*,............
+00001e00: e7ab 234c 0ed7 c719 5368 6f77 4675 6c6c  ..#L....ShowFull
+00001e10: 7955 6e65 7870 6c6f 7265 644d 6170 2e63  yUnexploredMap.c
+00001e20: 730e 2f00 0106 0d12 1217 810c 824c 8327  s./..........L.'
+00001e30: 204b 3897 7778 2bb2 56ca 6138 17db bdb9   K8.wx+.V.a8....
+00001e40: b4ee cc3d 52c6 5a60 a4aa 48c2 7668 3ad2  ...=R.Z`..H.vh:.
+00001e50: af0a 5370 7269 7465 732e 6373 0c2f 0001  ..Sprites.cs./..
+00001e60: 060d 1212 1781 0c83 7120 6eff f914 7f50  ........q n....P
+00001e70: 5d94 82a7 92ec 1785 0187 33ff ee64 b40c  ].........3..d..
+00001e80: 3958 ca4f 1cfb fc3f fe46 0a50 726f 6772  9X.O...?.F.Progr
+00001e90: 616d 2e63 730a 2f00 0106 0d12 1217 83aa  am.cs./.........
+00001ea0: 2061 dcc5 0e5e ef7c 5ce0 0a24 a7f0 5afc   a...^.|\..$..Z.
+00001eb0: 1dba 3ce0 7d22 2e11 34ff 72f1 832d c0a1  ..<.}"..4.r..-..
+00001ec0: 700d 5365 6564 4f62 6a65 6374 2e63 730a  p.SeedObject.cs.
+00001ed0: 2f00 0106 0d12 1217 83e1 20f1 9a62 ab77  /......... ..b.w
+00001ee0: 8c2a 9e5e 4db8 c4b7 fdc8 9864 f43a c3f1  .*.^M......d.:..
+00001ef0: 547c d764 8efa 1db5 16cc 6003 6f62 6a07  T|.d......`.obj.
+00001f00: 5265 6c65 6173 6506 6e65 7436 2e30 1a59  Release.net6.0.Y
+00001f10: 414d 532d 4c49 422e 476c 6f62 616c 5573  AMS-LIB.GlobalUs
+00001f20: 696e 6773 2e67 2e63 7310 2f00 0106 0d12  ings.g.cs./.....
+00001f30: 1217 841b 841f 8427 842e 20ad db14 3f8c  .......'.. ...?.
+00001f40: 43b9 5f1b b73a 0cba 7c79 3281 935c 4ab8  C._..:..|y2..\J.
+00001f50: ccab bdf6 b04d 3e0f 809e 0e70 1f01 0000  .....M>....p....
+00001f60: d3d7 57b0 492c 2dc9 d74d 4fcd 4b2d 4a2c  ..W.I,-..MO.K-J,
+00001f70: 494d d1b7 e34a cfc9 4f4a cc51 282d cecc  IM...J..OJ.Q(-..
+00001f80: 4b57 8070 acac 822b 8b4b 5273 adf1 49ea  KW.p...+.KRs..I.
+00001f90: 39e7 e7e4 a426 9764 e6e7 15eb b983 0ccc  9....&.d........
+00001fa0: 4cc6 afc1 d31f bfbc 4f66 5e21 7e15 7ea9  L.......Of^!~.~.
+00001fb0: 257a 1e25 2505 f855 8564 14a5 26a6 0025  %z.%%..U.d..&..%
+00001fc0: 8854 a617 9258 9c5d 6ccd 0500 2e2e 4e45  .T...X.]l.....NE
+00001fd0: 5443 6f72 6541 7070 2c56 6572 7369 6f6e  TCoreApp,Version
+00001fe0: 3d76 362e 302e 4173 7365 6d62 6c79 4174  =v6.0.AssemblyAt
+00001ff0: 7472 6962 7574 6573 2e63 7310 2f00 0106  tributes.cs./...
+00002000: 0d12 1217 841b 841f 8427 84ec 2078 97e5  .........'.. x..
+00002010: 953c b5cd 5131 509b 3504 2186 34c2 4b9c  .<..Q1P.5.!.4.K.
+00002020: e7a6 8b98 4ffb 5a16 686e b5af 5c80 c900  ....O.Z.hn..\...
+00002030: 0000 002f 2f20 3c61 7574 6f67 656e 6572  ...// <autogener
+00002040: 6174 6564 202f 3e0d 0a75 7369 6e67 2053  ated />..using S
+00002050: 7973 7465 6d3b 0d0a 7573 696e 6720 5379  ystem;..using Sy
+00002060: 7374 656d 2e52 6566 6c65 6374 696f 6e3b  stem.Reflection;
+00002070: 0d0a 5b61 7373 656d 626c 793a 2067 6c6f  ..[assembly: glo
+00002080: 6261 6c3a 3a53 7973 7465 6d2e 5275 6e74  bal::System.Runt
+00002090: 696d 652e 5665 7273 696f 6e69 6e67 2e54  ime.Versioning.T
+000020a0: 6172 6765 7446 7261 6d65 776f 726b 4174  argetFrameworkAt
+000020b0: 7472 6962 7574 6528 222e 4e45 5443 6f72  tribute(".NETCor
+000020c0: 6541 7070 2c56 6572 7369 6f6e 3d76 362e  eApp,Version=v6.
+000020d0: 3022 2c20 4672 616d 6577 6f72 6b44 6973  0", FrameworkDis
+000020e0: 706c 6179 4e61 6d65 203d 2022 2e4e 4554  playName = ".NET
+000020f0: 2036 2e30 2229 5d0a 1859 414d 532d 4c49   6.0")]..YAMS-LI
+00002100: 422e 4173 7365 6d62 6c79 496e 666f 2e63  B.AssemblyInfo.c
+00002110: 7310 2f00 0106 0d12 1217 841b 841f 8427  s./............'
+00002120: 8618 203b efb2 b83d 0a79 26d8 9610 83de  .. ;...=.y&.....
+00002130: 4f4a 97d8 13ba e215 5ed7 a152 aeca 1b45  OJ......^..R...E
+00002140: 2057 0881 57d2 0300 00ad 93df 4bc3 3010   W..W.......K.0.
+00002150: c7df fb57 1c3e 29b2 3674 ed7e 3811 b6c1  ...W.>).6t.~8...
+00002160: 64e0 40b6 a188 f890 b697 3690 2692 a48e  d.@.......6.&...
+00002170: fef7 a6d3 8d8d a114 b67b cbdd e573 dfbb  .........{...s..
+00002180: 5c82 a073 51f3 8200 ee69 6555 2747 899a  \..sQ....ieU'G..
+00002190: 5acc 1e1a 5f63 eb82 1b48 5586 b0a1 06f6  Z..._c...HU.....
+000021a0: 7148 6aa0 6095 12be cbdc 254f 0b2a 7334  qHj.`.....%O.*s4
+000021b0: ce0f b6b9 c7b8 4028 690d 29ad 0c02 97a9  ......@(i.).....
+000021c0: d21a 530b 0916 f48b 2b0d 5466 b0e1 4238  ..S.....+.Tf..B8
+000021d0: 0f08 652c 70b6 83d9 027f 0a3b 90c6 7d65  ..e,p......;..}e
+000021e0: 7fab 3638 957b e199 7895 e132 8755 6d2c  ..68.{..x..2.Um,
+000021f0: 96a3 a393 bf44 265c 1b5c c991 e7bd 5363  .....D&\.\....Sc
+00002200: b04c 447d 771a f6c7 bfb1 a92a 3fa9 acc7  .LD}w......*?...
+00002210: d66a 9e54 16af afde c68b 55e7 693e b9ba  .j.T......U.i>..
+00002220: f968 8b90 8ce7 95eb d779 0f40 4b14 480d  .h.......y.@K.H.
+00002230: b6e6 ccdc a3bc a036 c794 d00f 7de2 93d6  .......6....}...
+00002240: 94b9 644a 975b 2d54 fc81 bb8d 49c8 623a  ..dJ.[-T....I.b:
+00002250: 24ac df4b 48c4 9228 2351 2fee 7687 8384  $..KH..(#Q/.v...
+00002260: 1112 a761 34a0 fd61 afbd f667 adb2 2ab5  ...a4..a...g..*.
+00002270: e78c 71cd adc0 7300 ffce ae59 cec7 c34f  ..q...s....Y...O
+00002280: d26c f162 35a9 b8c8 e055 738b 53b7 d233  .l.b5....Us.S..3
+00002290: 4df3 12a5 8554 b88a bee7 7d03 0110 8127  M....T....}....'
+000022a0: 7b22 646f 6375 6d65 6e74 7322 3a7b 222f  {"documents":{"/
+000022b0: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
+000022c0: 2f59 414d 532f 5941 4d53 2f2a 223a 2268  /YAMS/YAMS/*":"h
+000022d0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000022e0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+000022f0: 2f72 616e 646f 7661 6e69 612f 5941 4d53  /randovania/YAMS
+00002300: 2f35 3032 6635 6139 3066 3736 6230 3466  /502f5a90f76b04f
+00002310: 6234 6430 3436 3533 3339 3862 6630 3035  b4d04653398bf005
+00002320: 6332 3438 6137 3936 652f 2a22 2c22 2f68  c248a796e/*","/h
+00002330: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
+00002340: 5941 4d53 2f59 414d 532f 556e 6465 7274  YAMS/YAMS/Undert
+00002350: 616c 654d 6f64 546f 6f6c 2f2a 223a 2268  aleModTool/*":"h
+00002360: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00002370: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00002380: 2f6b 727a 7973 2d68 2f55 6e64 6572 7461  /krzys-h/Underta
+00002390: 6c65 4d6f 6454 6f6f 6c2f 3266 3065 3636  leModTool/2f0e66
+000023a0: 6530 3931 3034 3937 6435 3132 6331 3862  e0910497d512c18b
+000023b0: 3434 3966 3735 6634 3734 6133 3432 3566  449f75f474a3425f
+000023c0: 3037 2f2a 227d 7d82 2776 6572 7369 6f6e  07/*"}}.'version
+000023d0: 0032 0063 6f6d 7069 6c65 722d 7665 7273  .2.compiler-vers
+000023e0: 696f 6e00 342e 3130 2e30 2d33 2e32 3432  ion.4.10.0-3.242
+000023f0: 3136 2e31 322b 3361 6630 3038 3161 3665  16.12+3af0081a6e
+00002400: 3831 3162 3738 6433 3763 3632 6534 3739  811b78d37c62e479
+00002410: 3931 3466 3766 3463 6662 3064 3161 006c  914f7f4cfb0d1a.l
+00002420: 616e 6775 6167 6500 4323 0073 6f75 7263  anguage.C#.sourc
+00002430: 652d 6669 6c65 2d63 6f75 6e74 0031 3900  e-file-count.19.
+00002440: 6f75 7470 7574 2d6b 696e 6400 4479 6e61  output-kind.Dyna
+00002450: 6d69 6361 6c6c 794c 696e 6b65 644c 6962  micallyLinkedLib
+00002460: 7261 7279 006f 7074 696d 697a 6174 696f  rary.optimizatio
+00002470: 6e00 7265 6c65 6173 6500 706c 6174 666f  n.release.platfo
+00002480: 726d 0041 6e79 4370 7500 7275 6e74 696d  rm.AnyCpu.runtim
+00002490: 652d 7665 7273 696f 6e00 382e 302e 352b  e-version.8.0.5+
+000024a0: 3038 3765 3135 3332 3162 6237 3132 6566  087e15321bb712ef
+000024b0: 3666 6538 6230 6261 3666 3862 6431 3266  6fe8b0ba6f8bd12f
+000024c0: 6163 6639 3236 3239 006c 616e 6775 6167  acf92629.languag
+000024d0: 652d 7665 7273 696f 6e00 7072 6576 6965  e-version.previe
+000024e0: 7700 6e75 6c6c 6162 6c65 0045 6e61 626c  w.nullable.Enabl
+000024f0: 6500 6465 6669 6e65 0054 5241 4345 2c52  e.define.TRACE,R
+00002500: 454c 4541 5345 2c4e 4554 2c4e 4554 365f  ELEASE,NET,NET6_
+00002510: 302c 4e45 5443 4f52 4541 5050 2c4e 4554  0,NETCOREAPP,NET
+00002520: 355f 305f 4f52 5f47 5245 4154 4552 2c4e  5_0_OR_GREATER,N
+00002530: 4554 365f 305f 4f52 5f47 5245 4154 4552  ET6_0_OR_GREATER
+00002540: 2c4e 4554 434f 5245 4150 5031 5f30 5f4f  ,NETCOREAPP1_0_O
+00002550: 525f 4752 4541 5445 522c 4e45 5443 4f52  R_GREATER,NETCOR
+00002560: 4541 5050 315f 315f 4f52 5f47 5245 4154  EAPP1_1_OR_GREAT
+00002570: 4552 2c4e 4554 434f 5245 4150 5032 5f30  ER,NETCOREAPP2_0
+00002580: 5f4f 525f 4752 4541 5445 522c 4e45 5443  _OR_GREATER,NETC
+00002590: 4f52 4541 5050 325f 315f 4f52 5f47 5245  OREAPP2_1_OR_GRE
+000025a0: 4154 4552 2c4e 4554 434f 5245 4150 5032  ATER,NETCOREAPP2
+000025b0: 5f32 5f4f 525f 4752 4541 5445 522c 4e45  _2_OR_GREATER,NE
+000025c0: 5443 4f52 4541 5050 335f 305f 4f52 5f47  TCOREAPP3_0_OR_G
+000025d0: 5245 4154 4552 2c4e 4554 434f 5245 4150  REATER,NETCOREAP
+000025e0: 5033 5f31 5f4f 525f 4752 4541 5445 5200  P3_1_OR_GREATER.
+000025f0: a3ee 4943 5368 6172 7043 6f64 652e 5368  ..ICSharpCode.Sh
+00002600: 6172 705a 6970 4c69 622e 646c 6c00 0001  arpZipLib.dll...
+00002610: 6c99 0498 0080 0300 87d2 8216 a495 d14a  l..............J
+00002620: bd3f 1fc4 0213 b4ed 4d61 6372 6f73 732e  .?......Macross.
+00002630: 4a73 6f6e 2e45 7874 656e 7369 6f6e 732e  Json.Extensions.
+00002640: 646c 6c00 0001 55c4 78ba 0000 0100 b209  dll...U.x.......
+00002650: bad9 cad5 dc4e 93a4 2a22 b117 ec34 4d69  .....N..*"...4Mi
+00002660: 6372 6f73 6f66 742e 4353 6861 7270 2e64  crosoft.CSharp.d
+00002670: 6c6c 0000 01f5 8a16 a100 8000 004c 050a  ll...........L..
+00002680: b9c6 f798 43a1 b96e 5c83 3d2e 034d 6963  ....C..n\.=..Mic
+00002690: 726f 736f 6674 2e56 6973 7561 6c42 6173  rosoft.VisualBas
+000026a0: 6963 2e43 6f72 652e 646c 6c00 0001 e5ed  ic.Core.dll.....
+000026b0: c2c6 0020 0100 97df a5f1 a085 d443 ae46  ... .........C.F
+000026c0: 90c6 0c81 a93d 4d69 6372 6f73 6f66 742e  .....=Microsoft.
+000026d0: 5669 7375 616c 4261 7369 632e 646c 6c00  VisualBasic.dll.
+000026e0: 0001 326a 92aa 0080 0000 99ce 439c acc8  ..2j........C...
+000026f0: 3c49 81d3 8453 1c46 0cfd 4d69 6372 6f73  <I...S.F..Micros
+00002700: 6f66 742e 5769 6e33 322e 5072 696d 6974  oft.Win32.Primit
+00002710: 6976 6573 2e64 6c6c 0000 01e8 b368 9500  ives.dll.....h..
+00002720: 8000 0005 f586 f7bf c9a8 40a9 db13 19ad  ..........@.....
+00002730: ce55 be4d 6963 726f 736f 6674 2e57 696e  .U.Microsoft.Win
+00002740: 3332 2e52 6567 6973 7472 792e 646c 6c00  32.Registry.dll.
+00002750: 0001 4065 05c3 00a0 0000 dbaa 2478 8848  ..@e........$x.H
+00002760: e049 b500 9a18 92b8 ca79 6d73 636f 726c  .I.......ymscorl
+00002770: 6962 2e64 6c6c 0000 012c b231 dd00 2001  ib.dll...,.1.. .
+00002780: 00ec dbee 2c6d 5db8 4695 ca62 0154 ecc6  ....,m].F..b.T..
+00002790: be4e 6174 7572 616c 536f 7274 2e45 7874  .NaturalSort.Ext
+000027a0: 656e 7369 6f6e 2e64 6c6c 0000 01f8 cdb5  ension.dll......
+000027b0: 9e00 a000 005c dfe3 2353 f79a 4bb5 43e2  .....\..#S..K.C.
+000027c0: 52f8 16d1 b96e 6574 7374 616e 6461 7264  R....netstandard
+000027d0: 2e64 6c6c 0000 0132 ac6e bd00 c001 00ef  .dll...2.n......
+000027e0: 9c44 482e dc50 419b 9cf7 2b84 5ea3 c650  .DH..PA...+.^..P
+000027f0: 726f 7065 7274 7943 6861 6e67 6564 2e64  ropertyChanged.d
+00002800: 6c6c 0000 018b 5a97 8a00 8000 0031 74ff  ll....Z......1t.
+00002810: 35d3 a634 4c90 ea21 b0de 577f e053 6978  5..4L..!..W..Six
+00002820: 4c61 626f 7273 2e49 6d61 6765 5368 6172  Labors.ImageShar
+00002830: 702e 646c 6c00 0001 2e78 c49f 0040 2000  p.dll....x...@ .
+00002840: 1201 6d04 683c 5747 b755 9c23 1bf1 cf27  ..m.h<WG.U.#...'
+00002850: 5379 7374 656d 2e41 7070 436f 6e74 6578  System.AppContex
+00002860: 742e 646c 6c00 0001 012f a6c4 0080 0000  t.dll..../......
+00002870: 3de7 79b7 8341 594d ab86 ec35 05cf be16  =.y..AYM...5....
+00002880: 5379 7374 656d 2e42 7566 6665 7273 2e64  System.Buffers.d
+00002890: 6c6c 0000 0150 a14a ce00 8000 00f9 5baa  ll...P.J......[.
+000028a0: 3216 58d5 45b6 b6df 990d d224 4053 7973  2.X.E......$@Sys
+000028b0: 7465 6d2e 436f 6c6c 6563 7469 6f6e 732e  tem.Collections.
+000028c0: 436f 6e63 7572 7265 6e74 2e64 6c6c 0000  Concurrent.dll..
+000028d0: 0179 4ae8 c800 a000 00e8 4ff2 ad2b c27a  .yJ.......O..+.z
+000028e0: 43a5 fc08 2a2a dbd5 3653 7973 7465 6d2e  C...**..6System.
+000028f0: 436f 6c6c 6563 7469 6f6e 732e 646c 6c00  Collections.dll.
+00002900: 0001 6cfb 028a 0000 0100 fa3e a80d f10a  ..l........>....
+00002910: c543 ab6e 56c3 80da 0e32 5379 7374 656d  .C.nV....2System
+00002920: 2e43 6f6c 6c65 6374 696f 6e73 2e49 6d6d  .Collections.Imm
+00002930: 7574 6162 6c65 2e64 6c6c 0000 01b6 06ff  utable.dll......
+00002940: 9400 4001 000d 407b 7695 9b76 448e 7b32  ..@...@{v..vD.{2
+00002950: 18eb c14a 0553 7973 7465 6d2e 436f 6c6c  ...J.System.Coll
+00002960: 6563 7469 6f6e 732e 4e6f 6e47 656e 6572  ections.NonGener
+00002970: 6963 2e64 6c6c 0000 0119 cdd1 8c00 a000  ic.dll..........
+00002980: 008f 8b75 0ced d5b3 4c8e 049f d59b 9fd9  ...u....L.......
+00002990: f653 7973 7465 6d2e 436f 6c6c 6563 7469  .System.Collecti
+000029a0: 6f6e 732e 5370 6563 6961 6c69 7a65 642e  ons.Specialized.
+000029b0: 646c 6c00 0001 10b8 59fb 00a0 0000 db8e  dll.....Y.......
+000029c0: 8d5a 6336 414f 886b 1fa3 eca0 a665 5379  .Zc6AO.k.....eSy
+000029d0: 7374 656d 2e43 6f6d 706f 6e65 6e74 4d6f  stem.ComponentMo
+000029e0: 6465 6c2e 416e 6e6f 7461 7469 6f6e 732e  del.Annotations.
+000029f0: 646c 6c00 0001 0775 3cf2 00c0 0000 bbdc  dll....u<.......
+00002a00: ecb4 221d 884c a3fa 6032 d997 6bd3 5379  .."..L..`2..k.Sy
+00002a10: 7374 656d 2e43 6f6d 706f 6e65 6e74 4d6f  stem.ComponentMo
+00002a20: 6465 6c2e 4461 7461 416e 6e6f 7461 7469  del.DataAnnotati
+00002a30: 6f6e 732e 646c 6c00 0001 80f8 1cff 0080  ons.dll.........
+00002a40: 0000 a4a7 abc0 93ab cb4a a521 8f7c ba66  .........J.!.|.f
+00002a50: 575a 5379 7374 656d 2e43 6f6d 706f 6e65  WZSystem.Compone
+00002a60: 6e74 4d6f 6465 6c2e 646c 6c00 0001 65d3  ntModel.dll...e.
+00002a70: 80a2 0080 0000 d0de d495 2e65 f24f 85b1  ...........e.O..
+00002a80: 78e7 c30a b252 5379 7374 656d 2e43 6f6d  x....RSystem.Com
+00002a90: 706f 6e65 6e74 4d6f 6465 6c2e 4576 656e  ponentModel.Even
+00002aa0: 7442 6173 6564 4173 796e 632e 646c 6c00  tBasedAsync.dll.
+00002ab0: 0001 3666 f9e7 0080 0000 cf28 13ce 3a11  ..6f.......(..:.
+00002ac0: 5340 b695 7bc9 0b65 4c6b 5379 7374 656d  S@..{..eLkSystem
+00002ad0: 2e43 6f6d 706f 6e65 6e74 4d6f 6465 6c2e  .ComponentModel.
+00002ae0: 5072 696d 6974 6976 6573 2e64 6c6c 0000  Primitives.dll..
+00002af0: 01c8 619f e000 a000 00d9 39c5 0f6b 4705  ..a.......9..kG.
+00002b00: 4099 161e 3654 6a5f f553 7973 7465 6d2e  @...6Tj_.System.
+00002b10: 436f 6d70 6f6e 656e 744d 6f64 656c 2e54  ComponentModel.T
+00002b20: 7970 6543 6f6e 7665 7274 6572 2e64 6c6c  ypeConverter.dll
+00002b30: 0000 017a f0cc f000 c001 0067 3dc4 599f  ...z.......g=.Y.
+00002b40: 7473 4993 737d e603 a195 3153 7973 7465  tsI.s}....1Syste
+00002b50: 6d2e 436f 6e66 6967 7572 6174 696f 6e2e  m.Configuration.
+00002b60: 646c 6c00 0001 8477 6c89 0080 0000 2a37  dll....wl.....*7
+00002b70: 740d a6c9 2349 b47b f60e bba7 b9d3 5379  t...#I.{......Sy
+00002b80: 7374 656d 2e43 6f6e 736f 6c65 2e64 6c6c  stem.Console.dll
+00002b90: 0000 018b a486 9800 a000 0016 b621 ca3d  .............!.=
+00002ba0: f639 4f83 668c 306f 6bcd 3c53 7973 7465  .9O.f.0ok.<Syste
+00002bb0: 6d2e 436f 7265 2e64 6c6c 0000 01aa 8524  m.Core.dll.....$
+00002bc0: 9400 a000 0033 6636 4d17 6ea4 41ad fd4c  .....3f6M.n.A..L
+00002bd0: 86a8 d0b7 8653 7973 7465 6d2e 4461 7461  .....System.Data
+00002be0: 2e43 6f6d 6d6f 6e2e 646c 6c00 0001 a82a  .Common.dll....*
+00002bf0: 77b0 0080 0200 8a60 bb0f e365 d64d 94f8  w......`...e.M..
+00002c00: deeb 1784 90db 5379 7374 656d 2e44 6174  ......System.Dat
+00002c10: 612e 4461 7461 5365 7445 7874 656e 7369  a.DataSetExtensi
+00002c20: 6f6e 732e 646c 6c00 0001 1c91 b5e2 0080  ons.dll.........
+00002c30: 0000 0c90 d603 1d62 dd49 a0c1 84fd d75c  .......b.I.....\
+00002c40: 9ad8 5379 7374 656d 2e44 6174 612e 646c  ..System.Data.dl
+00002c50: 6c00 0001 3097 0efa 00a0 0000 f7ef 3242  l...0.........2B
+00002c60: a934 aa47 96a2 7a3d 82f6 f478 5379 7374  .4.G..z=...xSyst
+00002c70: 656d 2e44 6961 676e 6f73 7469 6373 2e43  em.Diagnostics.C
+00002c80: 6f6e 7472 6163 7473 2e64 6c6c 0000 013a  ontracts.dll...:
+00002c90: ad8c d200 8000 0031 99cf 5607 766b 45a4  .......1..V.vkE.
+00002ca0: 7c6e 6554 6879 b353 7973 7465 6d2e 4469  |neThy.System.Di
+00002cb0: 6167 6e6f 7374 6963 732e 4465 6275 672e  agnostics.Debug.
+00002cc0: 646c 6c00 0001 7807 7a9a 0080 0000 4b00  dll...x.z.....K.
+00002cd0: e205 da91 8842 bc46 3f89 36af 27e1 5379  .....B.F?.6.'.Sy
+00002ce0: 7374 656d 2e44 6961 676e 6f73 7469 6373  stem.Diagnostics
+00002cf0: 2e44 6961 676e 6f73 7469 6353 6f75 7263  .DiagnosticSourc
+00002d00: 652e 646c 6c00 0001 7ba2 dccc 00c0 0000  e.dll...{.......
+00002d10: 2237 dea9 883d db4f 8e86 1d63 a9ef a27d  "7...=.O...c...}
+00002d20: 5379 7374 656d 2e44 6961 676e 6f73 7469  System.Diagnosti
+00002d30: 6373 2e46 696c 6556 6572 7369 6f6e 496e  cs.FileVersionIn
+00002d40: 666f 2e64 6c6c 0000 01bb 1540 9b00 8000  fo.dll.....@....
+00002d50: 003e 0521 78b6 0bfd 45ad af10 0fe4 5c85  .>.!x...E.....\.
+00002d60: 9253 7973 7465 6d2e 4469 6167 6e6f 7374  .System.Diagnost
+00002d70: 6963 732e 5072 6f63 6573 732e 646c 6c00  ics.Process.dll.
+00002d80: 0001 9560 9c9e 00c0 0000 8f79 e50b b6d2  ...`.......y....
+00002d90: 3f48 a943 20e1 fabb 4fcc 5379 7374 656d  ?H.C ...O.System
+00002da0: 2e44 6961 676e 6f73 7469 6373 2e53 7461  .Diagnostics.Sta
+00002db0: 636b 5472 6163 652e 646c 6c00 0001 a7a5  ckTrace.dll.....
+00002dc0: b5f4 00a0 0000 94d5 63eb 7e25 eb49 a275  ........c.~%.I.u
+00002dd0: f1fb df8a aa48 5379 7374 656d 2e44 6961  .....HSystem.Dia
+00002de0: 676e 6f73 7469 6373 2e54 6578 7457 7269  gnostics.TextWri
+00002df0: 7465 7254 7261 6365 4c69 7374 656e 6572  terTraceListener
+00002e00: 2e64 6c6c 0000 0182 28ca e600 8000 00fc  .dll....(.......
+00002e10: 956f 58a0 0e44 4384 89b1 1dad acf3 7553  .oX..DC.......uS
+00002e20: 7973 7465 6d2e 4469 6167 6e6f 7374 6963  ystem.Diagnostic
+00002e30: 732e 546f 6f6c 732e 646c 6c00 0001 a33e  s.Tools.dll....>
+00002e40: 1898 0080 0000 92d0 37d0 6ed7 254a bcc8  ........7.n.%J..
+00002e50: f9e9 7b42 1ea1 5379 7374 656d 2e44 6961  ..{B..System.Dia
+00002e60: 676e 6f73 7469 6373 2e54 7261 6365 536f  gnostics.TraceSo
+00002e70: 7572 6365 2e64 6c6c 0000 01ab a0f9 8900  urce.dll........
+00002e80: a000 008c b05a 38a8 eb9f 4099 04ed 43db  .....Z8...@...C.
+00002e90: 2986 fc53 7973 7465 6d2e 4469 6167 6e6f  )..System.Diagno
+00002ea0: 7374 6963 732e 5472 6163 696e 672e 646c  stics.Tracing.dl
+00002eb0: 6c00 0001 16f7 63b4 00a0 0000 ba36 dd5a  l.....c......6.Z
+00002ec0: bbfc c64d b1d7 df66 293b e334 5379 7374  ...M...f);.4Syst
+00002ed0: 656d 2e64 6c6c 0000 017d b0da f200 0001  em.dll...}......
+00002ee0: 0044 a701 5d45 deda 48af a885 e1af 3d66  .D..]E..H.....=f
+00002ef0: 6653 7973 7465 6d2e 4472 6177 696e 672e  fSystem.Drawing.
+00002f00: 436f 6d6d 6f6e 2e64 6c6c 0000 0121 8d42  Common.dll...!.B
+00002f10: d500 2002 0008 43fe c06a 78bb 469f 62dc  .. ...C..jx.F.b.
+00002f20: 8ac5 b55a bc53 7973 7465 6d2e 4472 6177  ...Z.System.Draw
+00002f30: 696e 672e 646c 6c00 0001 3962 7c88 0080  ing.dll...9b|...
+00002f40: 0000 f33f efca 4bd3 b245 8671 6a6e fa11  ...?..K..E.qjn..
+00002f50: 129b 5379 7374 656d 2e44 7261 7769 6e67  ..System.Drawing
+00002f60: 2e50 7269 6d69 7469 7665 732e 646c 6c00  .Primitives.dll.
+00002f70: 0001 a73a bfb7 00c0 0000 917d e8b4 31cf  ...:.......}..1.
+00002f80: c942 97ea bc49 542b ed68 5379 7374 656d  .B...IT+.hSystem
+00002f90: 2e44 796e 616d 6963 2e52 756e 7469 6d65  .Dynamic.Runtime
+00002fa0: 2e64 6c6c 0000 01ea b87b 8900 8000 0093  .dll.....{......
+00002fb0: 1dae 6191 048b 4397 7868 4768 0df7 2753  ..a...C.xhGh..'S
+00002fc0: 7973 7465 6d2e 466f 726d 6174 732e 4173  ystem.Formats.As
+00002fd0: 6e31 2e64 6c6c 0000 01db ca80 b600 a000  n1.dll..........
+00002fe0: 0075 fc63 10ac 83d3 41b8 b25c 8b82 4ee5  .u.c....A..\..N.
+00002ff0: e653 7973 7465 6d2e 476c 6f62 616c 697a  .System.Globaliz
+00003000: 6174 696f 6e2e 4361 6c65 6e64 6172 732e  ation.Calendars.
+00003010: 646c 6c00 0001 f2a1 dc97 0080 0000 3de7  dll...........=.
+00003020: 19aa 09c6 a347 9e35 e562 9700 b75a 5379  .....G.5.b...ZSy
+00003030: 7374 656d 2e47 6c6f 6261 6c69 7a61 7469  stem.Globalizati
+00003040: 6f6e 2e64 6c6c 0000 0187 5ac5 fc00 8000  on.dll....Z.....
+00003050: 0026 1623 1619 e911 4192 d34e 652e 7e70  .&.#....A..Ne.~p
+00003060: 5553 7973 7465 6d2e 476c 6f62 616c 697a  USystem.Globaliz
+00003070: 6174 696f 6e2e 4578 7465 6e73 696f 6e73  ation.Extensions
+00003080: 2e64 6c6c 0000 01f7 efc1 cb00 8000 0070  .dll...........p
+00003090: 66ef 7540 15c8 469a ed43 79a4 c951 7853  f.u@..F..Cy..QxS
+000030a0: 7973 7465 6d2e 494f 2e43 6f6d 7072 6573  ystem.IO.Compres
+000030b0: 7369 6f6e 2e42 726f 746c 692e 646c 6c00  sion.Brotli.dll.
+000030c0: 0001 95e4 07a3 0080 0000 a98d 9062 8f83  .............b..
+000030d0: 9140 94df 94b5 25e8 2d97 5379 7374 656d  .@....%.-.System
+000030e0: 2e49 4f2e 436f 6d70 7265 7373 696f 6e2e  .IO.Compression.
+000030f0: 646c 6c00 0001 32ac 449d 00a0 0000 8310  dll...2.D.......
+00003100: b06b 0d1a 7c41 abae 90cb 9015 1c41 5379  .k..|A.......ASy
+00003110: 7374 656d 2e49 4f2e 436f 6d70 7265 7373  stem.IO.Compress
+00003120: 696f 6e2e 4669 6c65 5379 7374 656d 2e64  ion.FileSystem.d
+00003130: 6c6c 0000 012f 1845 b000 8000 009f 78d8  ll.../.E......x.
+00003140: 18b6 e186 42a1 ac20 85b7 0822 f453 7973  ....B.. ...".Sys
+00003150: 7465 6d2e 494f 2e43 6f6d 7072 6573 7369  tem.IO.Compressi
+00003160: 6f6e 2e5a 6970 4669 6c65 2e64 6c6c 0000  on.ZipFile.dll..
+00003170: 01a6 62fc a200 8000 0039 f5fe 0f65 deb7  ..b......9...e..
+00003180: 4595 f95c 66aa c92c 6453 7973 7465 6d2e  E..\f..,dSystem.
+00003190: 494f 2e64 6c6c 0000 0199 7640 b700 8000  IO.dll....v@....
+000031a0: 002d a4bb 8d9a e3f1 45bc 709e d2d3 c84f  .-......E.p....O
+000031b0: f753 7973 7465 6d2e 494f 2e46 696c 6553  .System.IO.FileS
+000031c0: 7973 7465 6d2e 4163 6365 7373 436f 6e74  ystem.AccessCont
+000031d0: 726f 6c2e 646c 6c00 0001 cd7e 1b8e 00a0  rol.dll....~....
+000031e0: 0000 00a1 0ba7 3795 0a47 9bb2 7724 2dc2  ......7..G..w$-.
+000031f0: bb58 5379 7374 656d 2e49 4f2e 4669 6c65  .XSystem.IO.File
+00003200: 5379 7374 656d 2e64 6c6c 0000 016c a373  System.dll...l.s
+00003210: c000 8000 00be 9a1a 63ee 1a30 4c86 dbfa  ........c..0L...
+00003220: 24d2 5a8b 6d53 7973 7465 6d2e 494f 2e46  $.Z.mSystem.IO.F
+00003230: 696c 6553 7973 7465 6d2e 4472 6976 6549  ileSystem.DriveI
+00003240: 6e66 6f2e 646c 6c00 0001 1873 c294 0080  nfo.dll....s....
+00003250: 0000 ee59 85af c71e 8d41 b192 1178 5fce  ...Y.....A...x_.
+00003260: df4e 5379 7374 656d 2e49 4f2e 4669 6c65  .NSystem.IO.File
+00003270: 5379 7374 656d 2e50 7269 6d69 7469 7665  System.Primitive
+00003280: 732e 646c 6c00 0001 fa99 dafb 0080 0000  s.dll...........
+00003290: a8e7 b99f b9fa 114c bb3f 306e 70bd ba3c  .......L.?0np..<
+000032a0: 5379 7374 656d 2e49 4f2e 4669 6c65 5379  System.IO.FileSy
+000032b0: 7374 656d 2e57 6174 6368 6572 2e64 6c6c  stem.Watcher.dll
+000032c0: 0000 010e 4c26 ab00 a000 0055 84cf f6da  ....L&.....U....
+000032d0: b75b 46b8 9383 c665 016f a753 7973 7465  .[F....e.o.Syste
+000032e0: 6d2e 494f 2e49 736f 6c61 7465 6453 746f  m.IO.IsolatedSto
+000032f0: 7261 6765 2e64 6c6c 0000 01ca d2fd f400  rage.dll........
+00003300: a000 000d 1344 3050 5c6f 458e 02cf 5a35  .....D0P\oE...Z5
+00003310: 2e71 2653 7973 7465 6d2e 494f 2e4d 656d  .q&System.IO.Mem
+00003320: 6f72 794d 6170 7065 6446 696c 6573 2e64  oryMappedFiles.d
+00003330: 6c6c 0000 0194 5445 fc00 8000 00dd aa07  ll....TE........
+00003340: 7a1d 63f9 489c 4fd7 f4cf 7f0f 2753 7973  z.c.H.O.....'Sys
+00003350: 7465 6d2e 494f 2e50 6970 6573 2e41 6363  tem.IO.Pipes.Acc
+00003360: 6573 7343 6f6e 7472 6f6c 2e64 6c6c 0000  essControl.dll..
+00003370: 0142 4813 b000 8000 00d7 d2fd 31a5 70af  .BH.........1.p.
+00003380: 47bd d5e8 9864 f39c 3f53 7973 7465 6d2e  G....d..?System.
+00003390: 494f 2e50 6970 6573 2e64 6c6c 0000 0183  IO.Pipes.dll....
+000033a0: 78f0 b600 a000 00ba ebc5 f8f2 793a 43bc  x...........y:C.
+000033b0: 7297 a8e6 a48c e253 7973 7465 6d2e 494f  r......System.IO
+000033c0: 2e55 6e6d 616e 6167 6564 4d65 6d6f 7279  .UnmanagedMemory
+000033d0: 5374 7265 616d 2e64 6c6c 0000 0134 3726  Stream.dll...47&
+000033e0: ad00 8000 000e 1a67 2d55 206d 4d85 8df2  .......g-U mM...
+000033f0: a1d5 641d aa53 7973 7465 6d2e 4c69 6e71  ..d..System.Linq
+00003400: 2e64 6c6c 0000 01f2 9154 d800 c000 000b  .dll.....T......
+00003410: e850 596a 0ff5 46aa 30f0 922e e3b6 b453  .PYj..F.0......S
+00003420: 7973 7465 6d2e 4c69 6e71 2e45 7870 7265  ystem.Linq.Expre
+00003430: 7373 696f 6e73 2e64 6c6c 0000 01b9 4d6b  ssions.dll....Mk
+00003440: a500 4001 00cf 39c4 14e4 b9da 4bbd 6346  ..@...9.....K.cF
+00003450: b90f 7141 a953 7973 7465 6d2e 4c69 6e71  ..qA.System.Linq
+00003460: 2e50 6172 616c 6c65 6c2e 646c 6c00 0001  .Parallel.dll...
+00003470: ef4a b6ee 00c0 0000 654e c0bf 8504 534b  .J......eN....SK
+00003480: 8e24 1e20 8515 85ee 5379 7374 656d 2e4c  .$. ....System.L
+00003490: 696e 712e 5175 6572 7961 626c 652e 646c  inq.Queryable.dl
+000034a0: 6c00 0001 0f58 cae6 00c0 0000 938e 9a77  l....X.........w
+000034b0: c57f 954c ab96 c063 fbe8 48e7 5379 7374  ...L...c..H.Syst
+000034c0: 656d 2e4d 656d 6f72 792e 646c 6c00 0001  em.Memory.dll...
+000034d0: 31cf 70e5 00e0 0000 a5af f55a 0e20 8540  1.p........Z. .@
+000034e0: 9652 4571 bfc2 ec2d 5379 7374 656d 2e4e  .REq...-System.N
+000034f0: 6574 2e64 6c6c 0000 01d1 85e8 9d00 8000  et.dll..........
+00003500: 008d afda 0db7 6f1c 4697 13bf b152 5fd6  ......o.F....R_.
+00003510: 9853 7973 7465 6d2e 4e65 742e 4874 7470  .System.Net.Http
+00003520: 2e64 6c6c 0000 01b9 81fa d100 2001 00d2  .dll........ ...
+00003530: 3604 f91b 07db 40b3 34ff bb5b 7b96 e253  6.....@.4..[{..S
+00003540: 7973 7465 6d2e 4e65 742e 4874 7470 2e4a  ystem.Net.Http.J
+00003550: 736f 6e2e 646c 6c00 0001 cb9b a0a4 0080  son.dll.........
+00003560: 0000 b825 9e1d fd05 b343 a6eb 805f 5d22  ...%.....C..._]"
+00003570: 9d3f 5379 7374 656d 2e4e 6574 2e48 7474  .?System.Net.Htt
+00003580: 704c 6973 7465 6e65 722e 646c 6c00 0001  pListener.dll...
+00003590: 55ab c5ce 00a0 0000 13ea 751a 1b38 1b4c  U.........u..8.L
+000035a0: 968b 7091 e824 734f 5379 7374 656d 2e4e  ..p..$sOSystem.N
+000035b0: 6574 2e4d 6169 6c2e 646c 6c00 0001 85dd  et.Mail.dll.....
+000035c0: c1ef 00c0 0000 3190 d068 eef2 214a 8e8c  ......1..h..!J..
+000035d0: 8ca0 5db0 11e9 5379 7374 656d 2e4e 6574  ..]...System.Net
+000035e0: 2e4e 616d 6552 6573 6f6c 7574 696f 6e2e  .NameResolution.
+000035f0: 646c 6c00 0001 27c8 bda9 0080 0000 a5e7  dll...'.........
+00003600: 2b76 309b 0440 9228 e679 76ed 8746 5379  +v0..@.(.yv..FSy
+00003610: 7374 656d 2e4e 6574 2e4e 6574 776f 726b  stem.Net.Network
+00003620: 496e 666f 726d 6174 696f 6e2e 646c 6c00  Information.dll.
+00003630: 0001 7b89 d1ac 00c0 0000 10ba 8d84 9236  ..{............6
+00003640: 5145 87eb 3f31 c42a 594e 5379 7374 656d  QE..?1.*YNSystem
+00003650: 2e4e 6574 2e50 696e 672e 646c 6c00 0001  .Net.Ping.dll...
+00003660: e018 c597 0080 0000 2495 b7a9 e1be 4346  ........$.....CF
+00003670: b048 bc27 0230 2207 5379 7374 656d 2e4e  .H.'.0".System.N
+00003680: 6574 2e50 7269 6d69 7469 7665 732e 646c  et.Primitives.dl
+00003690: 6c00 0001 ef0b 01b1 00c0 0000 f3b4 f496  l...............
+000036a0: c7f4 c94d b4e9 24d5 8630 3d8e 5379 7374  ...M..$..0=.Syst
+000036b0: 656d 2e4e 6574 2e52 6571 7565 7374 732e  em.Net.Requests.
+000036c0: 646c 6c00 0001 2035 a794 00e0 0000 9181  dll... 5........
+000036d0: 89dd 1300 a54f 8a9e d1df 5498 c824 5379  .....O....T..$Sy
+000036e0: 7374 656d 2e4e 6574 2e53 6563 7572 6974  stem.Net.Securit
+000036f0: 792e 646c 6c00 0001 c526 b6b4 0000 0100  y.dll....&......
+00003700: 77e6 f81b c452 e446 b35d abc2 bfa9 d795  w....R.F.]......
+00003710: 5379 7374 656d 2e4e 6574 2e53 6572 7669  System.Net.Servi
+00003720: 6365 506f 696e 742e 646c 6c00 0001 6184  cePoint.dll...a.
+00003730: b7c8 0080 0000 0663 f7b5 f5d7 dc4b 83bc  .......c.....K..
+00003740: 687f 5edc 6c93 5379 7374 656d 2e4e 6574  h.^.l.System.Net
+00003750: 2e53 6f63 6b65 7473 2e64 6c6c 0000 010d  .Sockets.dll....
+00003760: 738e 8600 0001 001b 2a1a bb38 e055 4ab1  s.......*..8.UJ.
+00003770: c71c ab87 a8fb 3c53 7973 7465 6d2e 4e65  ......<System.Ne
+00003780: 742e 5765 6243 6c69 656e 742e 646c 6c00  t.WebClient.dll.
+00003790: 0001 b668 5184 00a0 0000 e44a 3186 c5d3  ...hQ......J1...
+000037a0: 3040 ab1d 3e58 e7a7 becc 5379 7374 656d  0@..>X....System
+000037b0: 2e4e 6574 2e57 6562 4865 6164 6572 436f  .Net.WebHeaderCo
+000037c0: 6c6c 6563 7469 6f6e 2e64 6c6c 0000 0147  llection.dll...G
+000037d0: aba5 e700 8000 00cd ff0f b595 13bc 4b99  ..............K.
+000037e0: a433 5a70 08f4 7853 7973 7465 6d2e 4e65  .3Zp..xSystem.Ne
+000037f0: 742e 5765 6250 726f 7879 2e64 6c6c 0000  t.WebProxy.dll..
+00003800: 01fb 051b c500 8000 0043 8981 44e6 d7d8  .........C..D...
+00003810: 4aba 0057 626b 5fb1 7853 7973 7465 6d2e  J..Wbk_.xSystem.
+00003820: 4e65 742e 5765 6253 6f63 6b65 7473 2e43  Net.WebSockets.C
+00003830: 6c69 656e 742e 646c 6c00 0001 7051 a6bb  lient.dll...pQ..
+00003840: 0080 0000 6c80 cd49 1f2e 6e45 81ba 52b2  ....l..I..nE..R.
+00003850: bb3b ff22 5379 7374 656d 2e4e 6574 2e57  .;."System.Net.W
+00003860: 6562 536f 636b 6574 732e 646c 6c00 0001  ebSockets.dll...
+00003870: 59be 1fb9 00a0 0000 a4f3 f3f8 f7a0 3e45  Y.............>E
+00003880: 9ff2 d436 8e48 a7ce 5379 7374 656d 2e4e  ...6.H..System.N
+00003890: 756d 6572 6963 732e 646c 6c00 0001 6b8d  umerics.dll...k.
+000038a0: c3b5 0080 0000 2ba1 9510 ad96 d046 bae3  ......+......F..
+000038b0: d16b d822 b667 5379 7374 656d 2e4e 756d  .k.".gSystem.Num
+000038c0: 6572 6963 732e 5665 6374 6f72 732e 646c  erics.Vectors.dl
+000038d0: 6c00 0001 5719 57ed 00c0 0000 668e 4886  l...W.W.....f.H.
+000038e0: 0afc 4549 9af5 6dc9 6808 086a 5379 7374  ..EI..m.h..jSyst
+000038f0: 656d 2e4f 626a 6563 744d 6f64 656c 2e64  em.ObjectModel.d
+00003900: 6c6c 0000 013d c7f5 e300 c000 00c1 9e86  ll...=..........
+00003910: 0c1d 3631 4380 d133 1820 5466 a953 7973  ..61C..3. Tf.Sys
+00003920: 7465 6d2e 5265 666c 6563 7469 6f6e 2e44  tem.Reflection.D
+00003930: 6973 7061 7463 6850 726f 7879 2e64 6c6c  ispatchProxy.dll
+00003940: 0000 0173 16a4 9e00 8000 0063 861d c302  ...s.......c....
+00003950: 59cc 4c91 9312 1405 8cb9 0853 7973 7465  Y.L........Syste
+00003960: 6d2e 5265 666c 6563 7469 6f6e 2e64 6c6c  m.Reflection.dll
+00003970: 0000 0169 3e48 9600 8000 006d 250d 1279  ...i>H.....m%..y
+00003980: c961 46a5 f793 737f ceda 4753 7973 7465  .aF...s...GSyste
+00003990: 6d2e 5265 666c 6563 7469 6f6e 2e45 6d69  m.Reflection.Emi
+000039a0: 742e 646c 6c00 0001 70f9 e2e2 00e0 0000  t.dll...p.......
+000039b0: 1ead 64f4 c02e de4c 87e5 cc06 1805 8e6f  ..d....L.......o
+000039c0: 5379 7374 656d 2e52 6566 6c65 6374 696f  System.Reflectio
+000039d0: 6e2e 456d 6974 2e49 4c47 656e 6572 6174  n.Emit.ILGenerat
+000039e0: 696f 6e2e 646c 6c00 0001 624f 59eb 00a0  ion.dll...bOY...
+000039f0: 0000 8240 ee6a 2052 5f41 8a5f 9145 b12a  ...@.j R_A._.E.*
+00003a00: ffed 5379 7374 656d 2e52 6566 6c65 6374  ..System.Reflect
+00003a10: 696f 6e2e 456d 6974 2e4c 6967 6874 7765  ion.Emit.Lightwe
+00003a20: 6967 6874 2e64 6c6c 0000 010b 7b7f dc00  ight.dll....{...
+00003a30: 8000 008a ad54 1086 2fc5 47a0 0c64 97cb  .....T../.G..d..
+00003a40: 2edf 7d53 7973 7465 6d2e 5265 666c 6563  ..}System.Reflec
+00003a50: 7469 6f6e 2e45 7874 656e 7369 6f6e 732e  tion.Extensions.
+00003a60: 646c 6c00 0001 5267 c89f 0080 0000 6bba  dll...Rg......k.
+00003a70: d6e1 3421 4249 9460 741a d514 35e4 5379  ..4!BI.`t...5.Sy
+00003a80: 7374 656d 2e52 6566 6c65 6374 696f 6e2e  stem.Reflection.
+00003a90: 4d65 7461 6461 7461 2e64 6c6c 0000 0158  Metadata.dll...X
+00003aa0: 72da d000 2002 0063 015e 075c 1316 4a96  r... ..c.^.\..J.
+00003ab0: 830b af7a bb72 b553 7973 7465 6d2e 5265  ...z.r.System.Re
+00003ac0: 666c 6563 7469 6f6e 2e50 7269 6d69 7469  flection.Primiti
+00003ad0: 7665 732e 646c 6c00 0001 9b82 5cf3 00a0  ves.dll.....\...
+00003ae0: 0000 453c 9823 cbac 0442 a5c7 1565 a178  ..E<.#...B...e.x
+00003af0: d9e7 5379 7374 656d 2e52 6566 6c65 6374  ..System.Reflect
+00003b00: 696f 6e2e 5479 7065 4578 7465 6e73 696f  ion.TypeExtensio
+00003b10: 6e73 2e64 6c6c 0000 0113 8f33 b500 8000  ns.dll.....3....
+00003b20: 0001 face 0c93 ff10 429b 3fe3 da96 ea5d  ........B.?....]
+00003b30: f653 7973 7465 6d2e 5265 736f 7572 6365  .System.Resource
+00003b40: 732e 5265 6164 6572 2e64 6c6c 0000 0150  s.Reader.dll...P
+00003b50: ff13 9300 8000 0056 3f00 f661 53a4 418f  .......V?..aS.A.
+00003b60: 74d2 c8db 669f 5153 7973 7465 6d2e 5265  t...f.QSystem.Re
+00003b70: 736f 7572 6365 732e 5265 736f 7572 6365  sources.Resource
+00003b80: 4d61 6e61 6765 722e 646c 6c00 0001 958e  Manager.dll.....
+00003b90: 74ed 0080 0000 863e 7d61 cd3e 3043 8d06  t......>}a.>0C..
+00003ba0: d9e0 dfe8 87ee 5379 7374 656d 2e52 6573  ......System.Res
+00003bb0: 6f75 7263 6573 2e57 7269 7465 722e 646c  ources.Writer.dl
+00003bc0: 6c00 0001 6fd8 c080 0080 0000 caaf d5d3  l...o...........
+00003bd0: e70f 1645 b34c d5ce 83a6 eed5 5379 7374  ...E.L......Syst
+00003be0: 656d 2e52 756e 7469 6d65 2e43 6f6d 7069  em.Runtime.Compi
+00003bf0: 6c65 7253 6572 7669 6365 732e 556e 7361  lerServices.Unsa
+00003c00: 6665 2e64 6c6c 0000 0184 da7e 8e00 8000  fe.dll.....~....
+00003c10: 00b3 02b7 6f06 37e1 4194 8f8c 3c00 7913  ....o.7.A...<.y.
+00003c20: ba53 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
+00003c30: 436f 6d70 696c 6572 5365 7276 6963 6573  CompilerServices
+00003c40: 2e56 6973 7561 6c43 2e64 6c6c 0000 01c9  .VisualC.dll....
+00003c50: 1d7e cb00 8000 00fb 0819 0649 6523 47af  .~.........Ie#G.
+00003c60: f445 416a 3bf4 ec53 7973 7465 6d2e 5275  .EAj;..System.Ru
+00003c70: 6e74 696d 652e 646c 6c00 0001 d0f0 32ca  ntime.dll.....2.
+00003c80: 0080 0700 c5bb 4031 7d64 384b b4c1 4cc1  ......@1}d8K..L.
+00003c90: 0b2c 6009 5379 7374 656d 2e52 756e 7469  .,`.System.Runti
+00003ca0: 6d65 2e45 7874 656e 7369 6f6e 732e 646c  me.Extensions.dl
+00003cb0: 6c00 0001 b063 57b4 0080 0000 194e 58ff  l....cW......NX.
+00003cc0: 56d5 bd4e b98b 8e9f bc65 6e7f 5379 7374  V..N.....en.Syst
+00003cd0: 656d 2e52 756e 7469 6d65 2e48 616e 646c  em.Runtime.Handl
+00003ce0: 6573 2e64 6c6c 0000 01c6 8331 b200 8000  es.dll.....1....
+00003cf0: 0038 cd8d 0625 1670 4082 5e6a 52f8 e752  .8...%.p@.^jR..R
+00003d00: 4953 7973 7465 6d2e 5275 6e74 696d 652e  ISystem.Runtime.
+00003d10: 496e 7465 726f 7053 6572 7669 6365 732e  InteropServices.
+00003d20: 646c 6c00 0001 e188 1ea7 0040 0100 cdd4  dll........@....
+00003d30: 0b84 8fbf c248 925d 34bb 6520 f7a8 5379  .....H.]4.e ..Sy
+00003d40: 7374 656d 2e52 756e 7469 6d65 2e49 6e74  stem.Runtime.Int
+00003d50: 6572 6f70 5365 7276 6963 6573 2e52 756e  eropServices.Run
+00003d60: 7469 6d65 496e 666f 726d 6174 696f 6e2e  timeInformation.
+00003d70: 646c 6c00 0001 57d2 26cb 0080 0000 6bda  dll...W.&.....k.
+00003d80: b3af c348 fd4b 8931 291c cb9b 43f8 5379  ...H.K.1)...C.Sy
+00003d90: 7374 656d 2e52 756e 7469 6d65 2e49 6e74  stem.Runtime.Int
+00003da0: 7269 6e73 6963 732e 646c 6c00 0001 2efc  rinsics.dll.....
+00003db0: f6db 00c0 0200 bbda c48f b6a9 2e48 9758  .............H.X
+00003dc0: 34ea 8555 9572 5379 7374 656d 2e52 756e  4..U.rSystem.Run
+00003dd0: 7469 6d65 2e4c 6f61 6465 722e 646c 6c00  time.Loader.dll.
+00003de0: 0001 c1f5 0c83 0080 0000 025a 4b6e 37c8  ...........ZKn7.
+00003df0: ec49 95e0 8008 13f2 8d12 5379 7374 656d  .I........System
+00003e00: 2e52 756e 7469 6d65 2e4e 756d 6572 6963  .Runtime.Numeric
+00003e10: 732e 646c 6c00 0001 464c ecf6 00a0 0000  s.dll...FL......
+00003e20: 5a26 2d7b 254e 7544 a7c4 1831 9e4b a703  Z&-{%NuD...1.K..
+00003e30: 5379 7374 656d 2e52 756e 7469 6d65 2e53  System.Runtime.S
+00003e40: 6572 6961 6c69 7a61 7469 6f6e 2e64 6c6c  erialization.dll
+00003e50: 0000 010c bd27 e400 8000 00cf 81dc c8c8  .....'..........
+00003e60: 9dff 4b93 966d ee2a 422b 4f53 7973 7465  ..K..m.*B+OSyste
+00003e70: 6d2e 5275 6e74 696d 652e 5365 7269 616c  m.Runtime.Serial
+00003e80: 697a 6174 696f 6e2e 466f 726d 6174 7465  ization.Formatte
+00003e90: 7273 2e64 6c6c 0000 014c d670 8f00 a000  rs.dll...L.p....
+00003ea0: 0056 d998 3547 d1dc 40b5 0499 ba23 c7d2  .V..5G..@....#..
+00003eb0: fd53 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
+00003ec0: 5365 7269 616c 697a 6174 696f 6e2e 4a73  Serialization.Js
+00003ed0: 6f6e 2e64 6c6c 0000 0110 6feb e800 8000  on.dll....o.....
+00003ee0: 00fb 619b d76e 01b8 49ae 551f 99e0 157b  ..a..n..I.U....{
+00003ef0: 9553 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
+00003f00: 5365 7269 616c 697a 6174 696f 6e2e 5072  Serialization.Pr
+00003f10: 696d 6974 6976 6573 2e64 6c6c 0000 012f  imitives.dll.../
+00003f20: 8e69 c400 8000 005a 1d57 c6ec 550b 4da7  .i.....Z.W..U.M.
+00003f30: b741 ea01 d847 e253 7973 7465 6d2e 5275  .A...G.System.Ru
+00003f40: 6e74 696d 652e 5365 7269 616c 697a 6174  ntime.Serializat
+00003f50: 696f 6e2e 586d 6c2e 646c 6c00 0001 b82f  ion.Xml.dll..../
+00003f60: 84ba 00c0 0000 f3b6 6b60 8a89 1f43 8e48  ........k`...C.H
+00003f70: 1448 3769 a452 5379 7374 656d 2e53 6563  .H7i.RSystem.Sec
+00003f80: 7572 6974 792e 4163 6365 7373 436f 6e74  urity.AccessCont
+00003f90: 726f 6c2e 646c 6c00 0001 da30 abef 00e0  rol.dll....0....
+00003fa0: 0000 7998 fab8 c9f5 3043 b737 5afb 0032  ..y.....0C.7Z..2
+00003fb0: ee5b 5379 7374 656d 2e53 6563 7572 6974  .[System.Securit
+00003fc0: 792e 436c 6169 6d73 2e64 6c6c 0000 0113  y.Claims.dll....
+00003fd0: a29d fe00 c000 00e0 dd5f 805e a447 4a96  ........._.^.GJ.
+00003fe0: 7fd8 a50a 3cd2 9a53 7973 7465 6d2e 5365  ....<..System.Se
+00003ff0: 6375 7269 7479 2e43 7279 7074 6f67 7261  curity.Cryptogra
+00004000: 7068 792e 416c 676f 7269 7468 6d73 2e64  phy.Algorithms.d
+00004010: 6c6c 0000 01df 6342 9f00 0001 00ff 8627  ll....cB.......'
+00004020: 8abb 9a6c 4c84 c350 b9a0 eb91 4053 7973  ...lL..P....@Sys
+00004030: 7465 6d2e 5365 6375 7269 7479 2e43 7279  tem.Security.Cry
+00004040: 7074 6f67 7261 7068 792e 436e 672e 646c  ptography.Cng.dl
+00004050: 6c00 0001 df68 459c 00c0 0000 8918 c25c  l....hE........\
+00004060: 48ef ba45 84ee 5cbc a035 cbf6 5379 7374  H..E..\..5..Syst
+00004070: 656d 2e53 6563 7572 6974 792e 4372 7970  em.Security.Cryp
+00004080: 746f 6772 6170 6879 2e43 7370 2e64 6c6c  tography.Csp.dll
+00004090: 0000 0183 3ca2 d800 a000 0069 a9ac b258  ....<......i...X
+000040a0: 5f00 458d 92a5 0de5 e9e1 a753 7973 7465  _.E........Syste
+000040b0: 6d2e 5365 6375 7269 7479 2e43 7279 7074  m.Security.Crypt
+000040c0: 6f67 7261 7068 792e 456e 636f 6469 6e67  ography.Encoding
+000040d0: 2e64 6c6c 0000 0180 c6ef 9b00 a000 007f  .dll............
+000040e0: 6403 6712 05cf 418a 3565 e275 1ad5 be53  d.g...A.5e.u...S
+000040f0: 7973 7465 6d2e 5365 6375 7269 7479 2e43  ystem.Security.C
+00004100: 7279 7074 6f67 7261 7068 792e 4f70 656e  ryptography.Open
+00004110: 5373 6c2e 646c 6c00 0001 4099 b5a9 0080  Ssl.dll...@.....
+00004120: 0000 883e 78a3 02f7 9f46 b8c6 6359 b1f6  ...>x....F..cY..
+00004130: faf2 5379 7374 656d 2e53 6563 7572 6974  ..System.Securit
+00004140: 792e 4372 7970 746f 6772 6170 6879 2e50  y.Cryptography.P
+00004150: 7269 6d69 7469 7665 732e 646c 6c00 0001  rimitives.dll...
+00004160: dcfc 3e9a 00a0 0000 7b18 be31 15b9 a24f  ..>.....{..1...O
+00004170: 85c2 a058 a05c 0618 5379 7374 656d 2e53  ...X.\..System.S
+00004180: 6563 7572 6974 792e 4372 7970 746f 6772  ecurity.Cryptogr
+00004190: 6170 6879 2e58 3530 3943 6572 7469 6669  aphy.X509Certifi
+000041a0: 6361 7465 732e 646c 6c00 0001 f920 00a9  cates.dll.... ..
+000041b0: 00e0 0000 d92a 52fd fa1e 5344 b94b d71e  .....*R...SD.K..
+000041c0: a957 4b44 5379 7374 656d 2e53 6563 7572  .WKDSystem.Secur
+000041d0: 6974 792e 646c 6c00 0001 3db3 80d2 0080  ity.dll...=.....
+000041e0: 0000 ec19 139a d711 474b 9059 7e5f 6c59  ........GK.Y~_lY
+000041f0: 3a39 5379 7374 656d 2e53 6563 7572 6974  :9System.Securit
+00004200: 792e 5072 696e 6369 7061 6c2e 646c 6c00  y.Principal.dll.
+00004210: 0001 0898 0cf7 0080 0000 d774 4b1d 9a29  ...........tK..)
+00004220: c34e bc38 faac c15b dcf6 5379 7374 656d  .N.8...[..System
+00004230: 2e53 6563 7572 6974 792e 5072 696e 6369  .Security.Princi
+00004240: 7061 6c2e 5769 6e64 6f77 732e 646c 6c00  pal.Windows.dll.
+00004250: 0001 b625 43f1 00a0 0000 a157 35ba 62b4  ...%C......W5.b.
+00004260: dc4c 82ed 6dcc 383d f303 5379 7374 656d  .L..m.8=..System
+00004270: 2e53 6563 7572 6974 792e 5365 6375 7265  .Security.Secure
+00004280: 5374 7269 6e67 2e64 6c6c 0000 0108 f17e  String.dll.....~
+00004290: 8b00 8000 00f3 8efd 9a72 219b 438c 234a  .........r!.C.#J
+000042a0: ab8a 7f3e 4853 7973 7465 6d2e 5365 7276  ...>HSystem.Serv
+000042b0: 6963 654d 6f64 656c 2e57 6562 2e64 6c6c  iceModel.Web.dll
+000042c0: 0000 01cd d2e8 ee00 8000 0047 a11a a77e  ...........G...~
+000042d0: 2f78 42bf b92f 4578 f916 3353 7973 7465  /xB../Ex..3Syste
+000042e0: 6d2e 5365 7276 6963 6550 726f 6365 7373  m.ServiceProcess
+000042f0: 2e64 6c6c 0000 01b0 cb79 b900 8000 0098  .dll.....y......
+00004300: 589f a7cf 52a0 4b85 746f e33d 8827 8553  X...R.K.to.=.'.S
+00004310: 7973 7465 6d2e 5465 7874 2e45 6e63 6f64  ystem.Text.Encod
+00004320: 696e 672e 436f 6465 5061 6765 732e 646c  ing.CodePages.dl
+00004330: 6c00 0001 308b 6bab 0080 0000 94c1 4af1  l...0.k.......J.
+00004340: 661e 3548 940d c2ba 904f fcb5 5379 7374  f.5H.....O..Syst
+00004350: 656d 2e54 6578 742e 456e 636f 6469 6e67  em.Text.Encoding
+00004360: 2e64 6c6c 0000 016c 9f5b e200 8000 005e  .dll...l.[.....^
+00004370: 34d6 718d 2284 4bb4 7ca9 dc7a 652c 4853  4.q.".K.|..ze,HS
+00004380: 7973 7465 6d2e 5465 7874 2e45 6e63 6f64  ystem.Text.Encod
+00004390: 696e 672e 4578 7465 6e73 696f 6e73 2e64  ing.Extensions.d
+000043a0: 6c6c 0000 0196 16c3 8800 a000 00a6 106e  ll.............n
+000043b0: d0c9 26df 4185 0e70 cdf8 b442 7753 7973  ..&.A..p...BwSys
+000043c0: 7465 6d2e 5465 7874 2e45 6e63 6f64 696e  tem.Text.Encodin
+000043d0: 6773 2e57 6562 2e64 6c6c 0000 0170 222d  gs.Web.dll...p"-
+000043e0: f900 a000 0042 d6c8 960f fc0d 47bc a462  .....B......G..b
+000043f0: f0aa 2532 6f53 7973 7465 6d2e 5465 7874  ..%2oSystem.Text
+00004400: 2e4a 736f 6e2e 646c 6c00 0001 787d f7bc  .Json.dll...x}..
+00004410: 0020 0100 aaed da92 1e2b bc40 8ad2 9964  . .......+.@...d
+00004420: ebee d8f3 5379 7374 656d 2e54 6578 742e  ....System.Text.
+00004430: 5265 6775 6c61 7245 7870 7265 7373 696f  RegularExpressio
+00004440: 6e73 2e64 6c6c 0000 0148 34c9 fa00 c000  ns.dll...H4.....
+00004450: 0079 7712 2297 1c0b 4d83 c052 a421 04ba  .yw."...M..R.!..
+00004460: 9f53 7973 7465 6d2e 5468 7265 6164 696e  .System.Threadin
+00004470: 672e 4368 616e 6e65 6c73 2e64 6c6c 0000  g.Channels.dll..
+00004480: 0141 4ae2 e000 8000 0027 c55c 9fa6 09c8  .AJ......'.\....
+00004490: 46ad 8624 b0cf 766c ba53 7973 7465 6d2e  F..$..vl.System.
+000044a0: 5468 7265 6164 696e 672e 646c 6c00 0001  Threading.dll...
+000044b0: e269 1cf2 00c0 0000 cb91 22c1 4237 a340  .i........".B7.@
+000044c0: 822b 1ae7 8654 9cc4 5379 7374 656d 2e54  .+...T..System.T
+000044d0: 6872 6561 6469 6e67 2e4f 7665 726c 6170  hreading.Overlap
+000044e0: 7065 642e 646c 6c00 0001 d514 3bdb 0080  ped.dll.....;...
+000044f0: 0000 158a d0ce 3159 024c 954c a988 9d89  ......1Y.L.L....
+00004500: 65fd 5379 7374 656d 2e54 6872 6561 6469  e.System.Threadi
+00004510: 6e67 2e54 6173 6b73 2e44 6174 6166 6c6f  ng.Tasks.Dataflo
+00004520: 772e 646c 6c00 0001 62df 88b6 00c0 0000  w.dll...b.......
+00004530: c842 effc 55a8 e147 aca6 f351 fd9c ba60  .B..U..G...Q...`
+00004540: 5379 7374 656d 2e54 6872 6561 6469 6e67  System.Threading
+00004550: 2e54 6173 6b73 2e64 6c6c 0000 01fa b8fe  .Tasks.dll......
+00004560: 8f00 8000 0038 d58d 84fa b88f 4fbe 5013  .....8......O.P.
+00004570: b313 ca37 b553 7973 7465 6d2e 5468 7265  ...7.System.Thre
+00004580: 6164 696e 672e 5461 736b 732e 4578 7465  ading.Tasks.Exte
+00004590: 6e73 696f 6e73 2e64 6c6c 0000 01c2 6e88  nsions.dll....n.
+000045a0: 8d00 8000 00f3 6b4e aaf9 ea4c 459e 56f3  ......kN...LE.V.
+000045b0: 4cc8 d1e2 8f53 7973 7465 6d2e 5468 7265  L....System.Thre
+000045c0: 6164 696e 672e 5461 736b 732e 5061 7261  ading.Tasks.Para
+000045d0: 6c6c 656c 2e64 6c6c 0000 01ab ff61 da00  llel.dll.....a..
+000045e0: 8000 0045 a0bb 0378 c707 46ae 9a35 0f97  ...E...x..F..5..
+000045f0: a1ae fc53 7973 7465 6d2e 5468 7265 6164  ...System.Thread
+00004600: 696e 672e 5468 7265 6164 2e64 6c6c 0000  ing.Thread.dll..
+00004610: 012b 62c4 de00 a000 00ad 2b85 f853 a3ba  .+b.......+..S..
+00004620: 40b2 4a0c b399 d095 4953 7973 7465 6d2e  @.J.....ISystem.
+00004630: 5468 7265 6164 696e 672e 5468 7265 6164  Threading.Thread
+00004640: 506f 6f6c 2e64 6c6c 0000 010b fe86 b200  Pool.dll........
+00004650: 8000 0036 8cb1 a30e c08e 4489 9177 0c8a  ...6......D..w..
+00004660: e679 9853 7973 7465 6d2e 5468 7265 6164  .y.System.Thread
+00004670: 696e 672e 5469 6d65 722e 646c 6c00 0001  ing.Timer.dll...
+00004680: f90b 0cee 0080 0000 8639 6e21 0227 964f  .........9n!.'.O
+00004690: ba44 8def fc15 617e 5379 7374 656d 2e54  .D....a~System.T
+000046a0: 7261 6e73 6163 7469 6f6e 732e 646c 6c00  ransactions.dll.
+000046b0: 0001 3c50 75c0 0080 0000 d60a b6b2 8114  ..<Pu...........
+000046c0: 6b4c b27f a84f b569 0942 5379 7374 656d  kL...O.i.BSystem
+000046d0: 2e54 7261 6e73 6163 7469 6f6e 732e 4c6f  .Transactions.Lo
+000046e0: 6361 6c2e 646c 6c00 0001 ae1e b2b6 00a0  cal.dll.........
+000046f0: 0000 0576 b11e f388 6e46 8e94 47ab 44e6  ...v....nF..G.D.
+00004700: a328 5379 7374 656d 2e56 616c 7565 5475  .(System.ValueTu
+00004710: 706c 652e 646c 6c00 0001 1e4b 6f93 0080  ple.dll....Ko...
+00004720: 0000 9c40 de95 73f1 0948 9844 0e98 0df0  ...@..s..H.D....
+00004730: bfbb 5379 7374 656d 2e57 6562 2e64 6c6c  ..System.Web.dll
+00004740: 0000 01f9 3110 f300 8000 00d9 b835 a8d2  ....1........5..
+00004750: da62 418a 6cb3 c3c0 228a 0153 7973 7465  .bA.l..."..Syste
+00004760: 6d2e 5765 622e 4874 7470 5574 696c 6974  m.Web.HttpUtilit
+00004770: 792e 646c 6c00 0001 d03d a0e9 0080 0000  y.dll....=......
+00004780: 285a cfa7 71ce a441 9aa8 1074 4d35 f982  (Z..q..A...tM5..
+00004790: 5379 7374 656d 2e57 696e 646f 7773 2e64  System.Windows.d
+000047a0: 6c6c 0000 01f4 f355 ea00 8000 0003 0c6f  ll.....U.......o
+000047b0: 80aa e16d 4aa2 12db 01f2 f3d5 6e53 7973  ...mJ.......nSys
+000047c0: 7465 6d2e 586d 6c2e 646c 6c00 0001 ba5d  tem.Xml.dll....]
+000047d0: 1caa 00a0 0000 8136 cc16 9d75 d84e b607  .......6...u.N..
+000047e0: e0be 5db1 bdd9 5379 7374 656d 2e58 6d6c  ..]...System.Xml
+000047f0: 2e4c 696e 712e 646c 6c00 0001 fee3 49a9  .Linq.dll.....I.
+00004800: 0080 0000 2a48 96e8 d73d cb44 a347 62a6  ....*H...=.D.Gb.
+00004810: 808d 6ff8 5379 7374 656d 2e58 6d6c 2e52  ..o.System.Xml.R
+00004820: 6561 6465 7257 7269 7465 722e 646c 6c00  eaderWriter.dll.
+00004830: 0001 3d99 9790 0000 0200 7d35 a46b 1089  ..=.......}5.k..
+00004840: 4648 b366 390c 4bff 44ab 5379 7374 656d  FH.f9.K.D.System
+00004850: 2e58 6d6c 2e53 6572 6961 6c69 7a61 7469  .Xml.Serializati
+00004860: 6f6e 2e64 6c6c 0000 01f1 3147 9900 8000  on.dll....1G....
+00004870: 0089 1f2d dba9 6da4 4e93 32fb cf9d a06a  ...-..m.N.2....j
+00004880: fa53 7973 7465 6d2e 586d 6c2e 5844 6f63  .System.Xml.XDoc
+00004890: 756d 656e 742e 646c 6c00 0001 4427 67f5  ument.dll...D'g.
+000048a0: 00c0 0000 43cd 189d a6f8 364e 8323 4960  ....C.....6N.#I`
+000048b0: 3c94 fe65 5379 7374 656d 2e58 6d6c 2e58  <..eSystem.Xml.X
+000048c0: 6d6c 446f 6375 6d65 6e74 2e64 6c6c 0000  mlDocument.dll..
+000048d0: 01d6 7a88 c500 8000 007f a5d2 7747 c22c  ..z.........wG.,
+000048e0: 41a3 38b0 0218 2bda 5d53 7973 7465 6d2e  A.8...+.]System.
+000048f0: 586d 6c2e 586d 6c53 6572 6961 6c69 7a65  Xml.XmlSerialize
+00004900: 722e 646c 6c00 0001 66b2 94c4 0000 0100  r.dll...f.......
+00004910: b295 4f57 870c e14a ae8e ae4e ebd4 f99f  ..OW...J...N....
+00004920: 5379 7374 656d 2e58 6d6c 2e58 5061 7468  System.Xml.XPath
+00004930: 2e64 6c6c 0000 0141 e29a ac00 8000 0098  .dll...A........
+00004940: 3a4b 1af7 c2e1 43bc a1cb e160 3765 4653  :K....C....`7eFS
+00004950: 7973 7465 6d2e 586d 6c2e 5850 6174 682e  ystem.Xml.XPath.
+00004960: 5844 6f63 756d 656e 742e 646c 6c00 0001  XDocument.dll...
+00004970: 0f09 69a9 0080 0000 319c d289 0e3f 994f  ..i.....1....?.O
+00004980: 95fe 8ade 93fb 5a4c 556e 6465 7274 616c  ......ZLUndertal
+00004990: 654d 6f64 4c69 622e 646c 6c00 0001 6a1e  eModLib.dll...j.
+000049a0: 31e9 0020 0300 544f 2c86 b678 2d4a 8ea9  1.. ..TO,..x-J..
+000049b0: 6e66 a33f fa6f 5769 6e64 6f77 7342 6173  nf.?.oWindowsBas
+000049c0: 652e 646c 6c00 0001 ba38 59c1 0080 0000  e.dll....8Y.....
+000049d0: e191 23da 5768 464a b3a9 ef61 0ff5 003f  ..#.WhFJ...a...?
+000049e0: 0b00 0000 2405 0506 0001 0400 0653 7973  ....$........Sys
+000049f0: 7465 6d1a 5379 7374 656d 2e43 6f6c 6c65  tem.System.Colle
+00004a00: 6374 696f 6e73 2e47 656e 6572 6963 0953  ctions.Generic.S
+00004a10: 7973 7465 6d2e 494f 0b53 7973 7465 6d2e  ystem.IO.System.
+00004a20: 4c69 6e71 0f53 7973 7465 6d2e 4e65 742e  Linq.System.Net.
+00004a30: 4874 7470 1053 7973 7465 6d2e 5468 7265  Http.System.Thre
+00004a40: 6164 696e 6716 5379 7374 656d 2e54 6872  ading.System.Thr
+00004a50: 6561 6469 6e67 2e54 6173 6b73 1501 af0c  eading.Tasks....
+00004a60: 01af 1301 af2e 01af 3801 af44 01af 5401  ........8..D..T.
+00004a70: af65 0b00 0000 0d0a 0b07 0001 0475 0b00  .e...........u..
+00004a80: 0000 140f 0b08 0001 0475 1000 0000 1810  .........u......
+00004a90: 090a 002c 0200 0a00 0102 790f 556e 6465  ...,......y.Unde
+00004aa0: 7274 616c 654d 6f64 4c69 621a 556e 6465  rtaleModLib.Unde
+00004ab0: 7274 616c 654d 6f64 4c69 622e 4465 636f  rtaleModLib.Deco
+00004ac0: 6d70 696c 6572 1655 6e64 6572 7461 6c65  mpiler.Undertale
+00004ad0: 4d6f 644c 6962 2e4d 6f64 656c 7311 5379  ModLib.Models.Sy
+00004ae0: 7374 656d 2e52 6566 6c65 6374 696f 6e1c  stem.Reflection.
+00004af0: 5379 7374 656d 2e52 756e 7469 6d65 2e53  System.Runtime.S
+00004b00: 6572 6961 6c69 7a61 7469 6f6e 2401 af0c  erialization$...
+00004b10: 01af 1301 af2e 01af 3801 af44 01af 5401  ........8..D..T.
+00004b20: af65 01af bb01 afcb 01af e601 affd 01b0  .e..............
+00004b30: 0f06 0000 0034 1709 2901 0000 3c1c 090d  .....4..)...<...
+00004b40: 0026 0200 0900 1104 0803 0007 0208 0100  .&..............
+00004b50: 6a04 7955 003c 0479 0900 2202 000c 0001  j.yU.<.y..".....
+00004b60: 0279 1502 0000 3c2a 090d 002b 0200 0d00  .y....<*...+....
+00004b70: 2202 000c 0001 0279 1502 0000 3c31 090d  "......y....<1..
+00004b80: 002a 0200 0d00 2202 000c 0001 0279 0b00  .*...."......y..
+00004b90: 0000 2438 090c 0001 0279 0b03 0000 253d  ..$8.....y....%=
+00004ba0: 0934 0b04 0200 0b03 0000 244e 0934 0904  .4........$N.4..
+00004bb0: 0200 0904 0000 000d 0518 5e09 4705 0000  ..........^.G...
+00004bc0: 5f68 0927 001b 0200 1000 3704 0006 001d  _h.'......7.....
+00004bd0: 0200 0c00 4c02 0006 0038 0200 1b00 1402  ....L....8......
+00004be0: 0007 001d 0200 0c00 1a02 0007 001e 0200  ................
+00004bf0: 1000 2204 0007 005f 0200 2400 1b02 0010  .."...._..$.....
+00004c00: 0001 0279 8086 0600 0019 0909 0800 0702  ...y............
+00004c10: 0801 003c 0679 0700 6f06 0024 0059 0208  ...<.y..o..$.Y..
+00004c20: 1b00 6904 7924 0053 0208 1b00 1b06 2c0e  ..i.y$.S......,.
+00004c30: 0000 0200 0d00 5f03 002b 0277 1500 0004  ......_..+.w....
+00004c40: 0002 7f26 0600 0908 3207 0000 0200 2300  ...&....2.....#.
+00004c50: 331c 003b 0477 1900 5902 0824 0002 7b4a  3..;.w..Y..$..{J
+00004c60: 0b00 000e 001c 0e5b 0e00 0002 000d 005f  .......[......._
+00004c70: 0500 2b04 771c 001b 0200 0900 1b02 0809  ..+.w...........
+00004c80: 0000 0400 0279 1e06 0001 0c4b 1f53 7973  .....y.....K.Sys
+00004c90: 7465 6d2e 4469 6167 6e6f 7374 6963 732e  tem.Diagnostics.
+00004ca0: 436f 6465 416e 616c 7973 6973 1801 af0c  CodeAnalysis....
+00004cb0: 01af 1301 af2e 01af 3801 af44 01af 5401  ........8..D..T.
+00004cc0: af65 01b1 ac06 0000 0018 0805 1e53 7973  .e...........Sys
+00004cd0: 7465 6d2e 5465 7874 2e4a 736f 6e2e 5365  tem.Text.Json.Se
+00004ce0: 7269 616c 697a 6174 696f 6e18 01af 0c01  rialization.....
+00004cf0: af13 01af 2e01 af38 01af 4401 af54 01af  .......8..D..T..
+00004d00: 6501 b1ec 1507 0000 461b 0910 0015 0200  e.......F.......
+00004d10: 0300 0a00 2c06 003d 0455 1c53 7973 7465  ....,..=.U.Syste
+00004d20: 6d2e 436f 6d70 6f6e 656e 744d 6f64 656c  m.ComponentModel
+00004d30: 2e44 6573 6967 6e14 5379 7374 656d 2e47  .Design.System.G
+00004d40: 6c6f 6261 6c69 7a61 7469 6f6e 1053 7973  lobalization.Sys
+00004d50: 7465 6d2e 5465 7874 2e4a 736f 6e15 4e61  tem.Text.Json.Na
+00004d60: 7475 7261 6c53 6f72 742e 4578 7465 6e73  turalSort.Extens
+00004d70: 696f 6e14 5369 784c 6162 6f72 732e 496d  ion.SixLabors.Im
+00004d80: 6167 6553 6861 7270 2053 6978 4c61 626f  ageSharp SixLabo
+00004d90: 7273 2e49 6d61 6765 5368 6172 702e 466f  rs.ImageSharp.Fo
+00004da0: 726d 6174 732e 506e 6721 5369 784c 6162  rmats.Png!SixLab
+00004db0: 6f72 732e 496d 6167 6553 6861 7270 2e50  ors.ImageSharp.P
+00004dc0: 6978 656c 466f 726d 6174 731f 5369 784c  ixelFormats.SixL
+00004dd0: 6162 6f72 732e 496d 6167 6553 6861 7270  abors.ImageSharp
+00004de0: 2e50 726f 6365 7373 696e 6710 5941 4d53  .Processing.YAMS
+00004df0: 5f4c 4942 2e70 6174 6368 6573 1459 414d  _LIB.patches.YAM
+00004e00: 535f 4c49 422e 7061 7463 6865 732e 716f  S_LIB.patches.qo
+00004e10: 6c41 01af 0c01 af13 01af 2e01 af38 01af  lA...........8..
+00004e20: 4401 af54 01af 6501 b23a 01b2 5701 affd  D..T..e..:..W...
+00004e30: 01b2 6c01 b27d 01b2 9301 b2a8 01b2 c901  ..l..}..........
+00004e40: b2eb 01af bb01 afcb 01af e601 b30b 01b3  ................
+00004e50: 1c03 1c94 2e08 0000 0006 003a 2e09 0a00  ...........:....
+00004e60: 5c04 000d 001d 0e00 0a00 3104 0e0d 001e  \.........1.....
+00004e70: 047b 0f00 0102 7902 0000 0b00 0001 0025  .{....y........%
+00004e80: 0400 0a00 3d02 0010 0057 0600 1a00 4002  ....=....W....@.
+00004e90: 000c 004e 0080 820b 0034 06bf 7f10 0038  ...N.....4.....8
+00004ea0: 0400 1000 6806 0016 0080 8204 001f 0067  ....h..........g
+00004eb0: 0200 2505 0408 0044 0080 810c 0021 0055  ..%....D.....!.U
+00004ec0: 0200 0b00 2502 0010 0037 0200 0c00 5c02  ....%....7....\.
+00004ed0: 0007 0031 0200 0800 4f02 0007 0024 0200  ...1....O....$..
+00004ee0: 0800 3402 000e 0030 0200 0700 7d02 0022  ..4....0....}.."
+00004ef0: 0074 0200 0c00 2302 0011 0035 0200 0c00  .t....#....5....
+00004f00: 3c02 0007 002f 0200 0900 3502 0007 0024  <..../....5....$
+00004f10: 0200 0800 3402 000e 002e 0200 0700 2702  ....4.........'.
+00004f20: 0010 0058 0400 1700 5a06 0015 0056 0200  ...X....Z....V..
+00004f30: 1001 80d2 0200 2501 81ca 0800 2500 8087  ......%.....%...
+00004f40: 0800 1f00 5906 001f 0053 0600 1500 5e02  ....Y....S....^.
+00004f50: 000a 0058 0200 1f00 5506 001f 0080 8f06  ...X....U.......
+00004f60: 0025 0080 8802 0025 0280 a606 0025 0280  .%.....%.....%..
+00004f70: a60a 0025 0077 0a00 2500 8087 0400 2500  ...%.w..%.....%.
+00004f80: 809d 0600 2500 5c06 001f 005a 0200 1f00  ....%.\....Z....
+00004f90: 3b06 0010 0047 0600 1700 8089 0200 1200  ;....G..........
+00004fa0: 8081 0200 1200 8083 0200 1200 7e02 0012  ............~...
+00004fb0: 0060 0232 2a00 0002 000c 0061 0700 4704  .`.2*......a..G.
+00004fc0: 7722 0047 0200 2200 0006 0002 7b24 0801  w".G..".....{$..
+00004fd0: 809a 0e55 2500 6706 0025 0058 0600 1f00  ...U%.g..%.X....
+00004fe0: 8084 0200 2500 7306 001f 0073 0200 1f00  ....%.s....s....
+00004ff0: 7302 001f 006e 0200 1f00 7302 001f 004e  s....n....s....N
+00005000: 0638 1b00 0002 000f 005b 0700 3c04 771c  .8.......[..<.w.
+00005010: 0000 0600 027d 2a08 0080 a60c 4f1f 0e12  .....}*.....O...
+00005020: 0200 2501 8104 1e00 2511 1204 0025 002d  ..%.....%....%.-
+00005030: 2800 1200 6700 5c25 0180 da06 251f 0068  (...g.\%....%..h
+00005040: 0400 1f00 7606 0025 007d 0200 2500 7402  ....v..%.}..%.t.
+00005050: 0025 0080 9c06 001f 0080 9702 001f 0080  .%..............
+00005060: 9702 001f 005e 0600 2500 6002 0025 055d  .....^..%.`..%.]
+00005070: 0638 6600 0002 000f 005b 0700 330e 771c  .8f......[..3.w.
+00005080: 0000 0600 0273 2a08 0080 8f14 4f1f 0181  .....s*.....O...
+00005090: 1a06 0025 0380 e208 0025 0071 0e00 2500  ...%.....%.q..%.
+000050a0: 3702 0007 0056 0200 1c02 6c02 000c 0024  7....V....l....$
+000050b0: 0600 1100 4502 0020 0056 0200 0700 2a02  ....E.. .V....*.
+000050c0: 0009 0049 0200 0700 2002 000c 0028 0200  ...I.... ....(..
+000050d0: 0e00 2402 0007 0781 220c 0007 0180 f612  ..$.....".......
+000050e0: 382b 0000 0200 0f00 5b07 0053 0677 1f00  8+......[..S.w..
+000050f0: 0006 0002 7b2a 0800 6a0e 4f25 0029 0600  ....{*..j.O%.)..
+00005100: 0700 5d02 3017 0000 0200 0b00 6307 002e  ..].0.......c...
+00005110: 0477 0f00 3100 5e2f 0000 0600 027d 4508  .w..1.^/.....}E.
+00005120: 0480 900a 5731 0480 860a 0031 0025 0c00  ....W1.....1.%..
+00005130: 0700 1d02 301b 0000 0200 0b00 6307 002e  ....0.......c...
+00005140: 0477 0f00 2d00 5e2f 0000 0600 027d 4508  .w..-.^/.....}E.
+00005150: 0480 880a 5731 047e 0a00 3109 808a 1000  ....W1.~..1.....
+00005160: 1f00 5d16 0025 005d 0200 2500 6006 0025  ..]..%.]..%.`..%
+00005170: 0080 9d06 0025 004e 0600 1f00 5506 381b  .....%.N....U.8.
+00005180: 0000 0200 0f00 5b07 007b 0477 2200 0006  ......[..{.w"...
+00005190: 0002 7d2a 0800 808c 0c4f 2501 7406 0025  ..}*.....O%.t..%
+000051a0: 1780 9e08 0025 007a 3400 2200 7c02 0022  .....%.z4.".|.."
+000051b0: 0021 0200 1100 2202 0011 0906 0200 7809  .!....".......x.
+000051c0: 0614 007b 005c 1800 1f00 8080 0800 2200  ...{.\........".
+000051d0: 2402 0011 003a 0200 1500 808b 0200 3700  $....:........7.
+000051e0: 4706 0017 0048 0200 2d00 4802 002d 0048  G....H..-.H..-.H
+000051f0: 0200 2a00 4602 0029 0046 0200 2c00 4602  ..*.F..).F..,.F.
+00005200: 002c 0046 0200 2900 4402 0027 0046 0800  .,.F..).D..'.F..
+00005210: 1700 0b02 0a07 0000 0500 3304 7f07 0035  ..........3....5
+00005220: 0200 2800 1a02 0009 002b 0400 0700 4d02  ..(......+....M.
+00005230: 0049 0043 0200 1d00 1802 0011 0023 0200  .I.C.........#..
+00005240: 0d00 4f02 0007 0017 0200 0900 4302 0007  ..O.........C...
+00005250: 001b 0200 0e00 1c02 0007 002e 0400 0700  ................
+00005260: 5502 0049 001b 0200 1100 2602 000d 002f  U..I......&..../
+00005270: 0200 0700 1a02 0009 0029 0200 0700 1a02  .........)......
+00005280: 000c 001b 0200 0e00 1f02 0007 001b 0200  ................
+00005290: 1100 034b 3006 0008 006d 0c0e 5a3e 5d12  ...K0....m..Z>].
+000052a0: 004e 1e00 2500 4e02 0025 0030 0600 0700  .N..%.N..%.0....
+000052b0: 4802 001c 5d46 0200 0c00 1d80 bc00 1100  H...]F..........
+000052c0: 7102 0037 0181 7a06 0012 0181 7a04 0012  q..7..z.....z...
+000052d0: 0465 0830 3300 0002 000b 0063 0700 3b0c  .e.03......c..;.
+000052e0: 7722 0000 0600 0275 2208 0465 1406 3b00  w".....u"..e..;.
+000052f0: 0002 000b 0063 0700 290c 7714 0053 0200  .....c..).w..S..
+00005300: 1203 1a02 0013 0812 0e08 1200 0002 050a  ................
+00005310: 1800 0c00 0006 0002 4b1a 0800 474a 5717  ........K...GJW.
+00005320: 0042 0200 1200 5402 0012 0080 9202 0025  .B....T........%
+00005330: 0080 9202 0025 0168 0200 2500 5f04 0015  .....%.h..%._...
+00005340: 0071 0200 1100 6f02 0011 0080 8802 0011  .q....o.........
+00005350: 0180 9e02 0011 0080 8c04 0010 006d 0200  .............m..
+00005360: 2500 2106 0010 0041 0608 1500 5c02 0017  %.!....A....\...
+00005370: 005c 0200 1700 5a02 0017 005b 0200 1700  .\....Z....[....
+00005380: 4e02 0017 0048 0200 1700 5002 0017 005c  N....H....P....\
+00005390: 0200 2f00 5502 002f 0056 0200 3000 5502  ../.U../.V..0.U.
+000053a0: 002f 0055 0200 2f00 5602 0030 0056 0200  ./.U../.V..0.V..
+000053b0: 3000 5602 0030 0056 0200 2c00 5204 0029  0.V..0.V..,.R..)
+000053c0: 0049 0200 2900 5202 0029 007a 0400 2200  .I..).R..).z..".
+000053d0: 6502 000c 0021 0200 1100 7002 002a 0068  e....!....p..*.h
+000053e0: 0200 0f00 3e06 0015 0060 0200 2f00 5802  ....>....`../.X.
+000053f0: 002e 005a 0200 3000 5902 002f 005a 0200  ...Z..0.Y../.Z..
+00005400: 3000 5902 002f 005a 0200 3000 5a02 0030  0.Y../.Z..0.Z..0
+00005410: 004f 0600 2900 4602 0029 004f 0200 2900  .O..).F..).O..).
+00005420: 4504 0010 0077 0400 2200 6302 000c 001e  E....w..".c.....
+00005430: 0200 1100 6e02 002a 005d 0600 3000 4008  ....n..*.]..0.@.
+00005440: 0017 005d 0200 2d00 5602 002d 0057 0200  ...]..-.V..-.W..
+00005450: 2e00 5702 002d 0056 0200 2d00 5702 002e  ..W..-.V..-.W...
+00005460: 0057 0200 2e00 5802 002e 0057 0800 3800  .W....X....W..8.
+00005470: 5602 0038 005e 0200 3200 5004 0027 0047  V..8.^..2.P..'.G
+00005480: 0200 2700 5002 0027 0048 0400 1100 7904  ..'.P..'.H....y.
+00005490: 0022 0065 0200 0c00 2002 0011 0071 0200  .".e.... ....q..
+000054a0: 2800 4406 0017 0062 0200 3000 5a02 002f  (.D....b..0.Z../
+000054b0: 005c 0200 3100 5b02 0030 005c 0200 3100  .\..1.[..0.\..1.
+000054c0: 5b02 0030 005c 0200 3100 5c02 0031 005f  [..0.\..1.\..1._
+000054d0: 0800 3800 5f02 0038 005f 0200 3800 5f02  ..8._..8._..8._.
+000054e0: 0038 006f 0200 4300 5504 002a 004c 0200  .8.o..C.U..*.L..
+000054f0: 2a00 5502 002a 007d 0400 2200 6702 000c  *.U..*.}..".g...
+00005500: 0024 0200 1100 7902 002b 0049 0400 1100  .$....y..+.I....
+00005510: 8088 0800 2500 8088 0200 2501 8094 0400  ....%.....%.....
+00005520: 2500 8088 0600 2500 8088 0200 2500 8088  %.....%.....%...
+00005530: 0200 2500 8088 0200 2500 8088 0200 2500  ..%.....%.....%.
+00005540: 8086 0400 2500 8086 0200 2500 8086 0200  ....%.....%.....
+00005550: 2500 8088 0200 2501 8192 0879 2501 8192  %.....%....y%...
+00005560: 0400 2501 8192 0400 2501 8192 0400 2502  ..%.....%.....%.
+00005570: 8170 0800 1f00 3b0a 0015 0043 0200 0700  .p....;....C....
+00005580: 1002 0009 0010 0200 0900 1402 000c 0014  ................
+00005590: 0200 0c00 3302 0024 0041 0200 1c00 3102  ....3..$.A....1.
+000055a0: 0007 0056 0200 1c00 6e02 000c 001e 0200  ...V....n.......
+000055b0: 1100 2502 0009 0023 0200 0d0b 0602 0080  ..%....#........
+000055c0: 880b 0618 0080 8a00 7b1c 0025 0280 9806  ........{..%....
+000055d0: 004b 004a 0a00 1500 6302 0011 006f 0600  .K.J....c....o..
+000055e0: 1000 5b06 0025 005b 0200 2501 8094 0600  ..[..%.[..%.....
+000055f0: 2501 812a 0e00 0c00 6c0a 0012 0080 8002  %..*....l.......
+00005600: 0012 0054 0200 1200 6902 0012 004e 0200  ...T....i....N..
+00005610: 1200 6002 0012 0067 0200 1200 5106 0015  ..`....g....Q...
+00005620: 0281 5602 0010 004c 0600 1500 6802 0010  ..V....L....h...
+00005630: 0b12 0800 1208 4e18 0012 084e 1200 120a  ......N....N....
+00005640: 4e12 0012 0b12 1a00 1208 4e18 0012 084e  N.........N....N
+00005650: 1200 120a 4e12 0012 0a12 1a00 1208 4e16  ....N.........N.
+00005660: 0012 084e 1200 120a 4e12 0012 0052 1a00  ...N....N....R..
+00005670: 1500 8095 0200 1101 80b6 0200 1101 8124  ...............$
+00005680: 0800 1109 5a08 0011 0059 1400 1002 8128  ....Z....Y.....(
+00005690: 0e00 0c00 3b0a 000c 006a 0600 0c00 7f06  ....;....j......
+000056a0: 0024 0080 8302 002a 0181 2a06 000c 0180  .$.....*..*.....
+000056b0: cc08 000c 0064 0400 1708 6202 0012 0067  .....d....b....g
+000056c0: 1200 1200 6e04 0017 086c 0200 1200 7112  ....n....l....q.
+000056d0: 0012 0064 0400 1708 5e02 0012 0067 1200  ...d....^....g..
+000056e0: 1200 6504 0017 085e 0200 1200 6412 0012  ..e....^....d...
+000056f0: 004e 0600 0c01 8110 0200 2500 80a3 0400  .N........%.....
+00005700: 250f 809e 0200 2500 7d24 000c 0080 af02  %.....%.}$......
+00005710: 001f 0080 be02 0025 0037 0200 0d00 6104  .......%.7....a.
+00005720: 0812 0080 9302 002c 0080 9402 002c 0281  .......,.....,..
+00005730: 4a08 790c 1e5a 0a00 1201 8100 3e00 1200  J.y..Z......>...
+00005740: 7a08 0025 005a 0600 1700 4e02 0012 0059  z..%.Z....N....Y
+00005750: 0200 1700 4702 0012 0565 0430 4b00 0002  ....G....e.0K...
+00005760: 000b 0063 0700 4f0e 7722 0000 0600 0273  ...c..O.w".....s
+00005770: 2208 004f 1457 1b00 0c02 3e11 0000 0200  "..O.W....>.....
+00005780: 1200 5507 0060 0446 3200 0002 001b 0043  ..U..`.F2......C
+00005790: 0700 4c04 7715 0002 7d42 0b00 000b 0000  ..L.w...}B......
+000057a0: 0100 027d 670b 0000 0b00 0001 004b 1449  ...}g........K.I
+000057b0: 1200 5202 0012 004c 0600 1200 5302 0012  ..R....L....S...
+000057c0: 0180 da02 3e35 0000 0200 1200 5507 0040  ....>5......U..@
+000057d0: 0677 1000 027b 300b 0000 0b00 0001 004a  .w...{0........J
+000057e0: 0e49 1200 5102 0012 0075 0200 2500 5b06  .I..Q....u..%.[.
+000057f0: 0017 0049 0200 1200 4f02 0012 0280 9602  ...I....O.......
+00005800: 4035 0000 0200 1300 5307 003c 0877 1000  @5......S..<.w..
+00005810: 0279 320b 0000 0b00 0001 005a 1047 1700  .y2........Z.G..
+00005820: 4802 0012 004e 0200 1204 6502 3033 0000  H....N....e.03..
+00005830: 0200 0b00 6307 004f 0c77 2200 0006 0002  ....c..O.w".....
+00005840: 7522 0800 4c14 5712 0052 0200 1202 8096  u"..L.W..R......
+00005850: 0240 3500 0002 0013 0053 0700 4508 7710  .@5......S..E.w.
+00005860: 0002 7932 0b00 000b 0000 0100 4f10 4712  ..y2........O.G.
+00005870: 0055 0200 1201 80d6 0240 3500 0002 0013  .U.......@5.....
+00005880: 0053 0700 4806 7710 0002 7b32 0b00 000b  .S..H.w...{2....
+00005890: 0000 0100 4d10 4712 0054 0200 1207 6502  ....M.G..T....e.
+000058a0: 3080 9c00 0002 000b 0063 0700 5512 7722  0........c..U.w"
+000058b0: 0000 0600 026f 2208 004a 1c57 1200 5002  .....o"..J.W..P.
+000058c0: 0012 0665 0430 808a 0000 0200 0b00 6307  ...e.0........c.
+000058d0: 0051 1077 2200 0006 0002 7122 0800 5518  .Q.w".....q"..U.
+000058e0: 5717 0047 0200 1200 4f02 0012 0047 0600  W..G....O....G..
+000058f0: 1200 4f02 0012 0080 8c02 302b 0000 0200  ..O.......0+....
+00005900: 0b00 6307 0056 0477 2200 0006 0002 7d22  ..c..V.w".....}"
+00005910: 0800 470c 5712 004f 0200 1200 4706 0012  ..G.W..O....G...
+00005920: 004f 0200 1200 4706 0012 004f 0200 1208  .O....G....O....
+00005930: 5806 0012 085a 1200 1208 5a12 0012 125a  X....Z....Z....Z
+00005940: 1200 1208 5a28 0012 003e 1600 0c00 5702  ....Z(...>....W.
+00005950: 001f 0080 ac02 001f 0038 0600 0c02 8158  .........8.....X
+00005960: 0200 2500 390a 000c 0080 b802 001f 0080  ..%.9...........
+00005970: bd02 001f 1212 0200 2500 80a8 2a00 7e00  ........%...*.~.
+00005980: 6606 0025 0065 0200 1f00 5f02 001f 0065  f..%.e...._....e
+00005990: 0600 2500 8083 0400 1f00 3f06 000c 004e  ..%.......?....N
+000059a0: 0200 1504 80f6 0200 1010 80a6 0e00 1f00  ................
+000059b0: 6e22 0025 0780 a202 001f 2780 aa10 0025  n".%......'....%
+000059c0: 0780 a250 001f 0067 1000 1f08 8092 0200  ...P...g........
+000059d0: 1f01 80a6 1200 2500 3408 0007 0052 0200  ......%.4....R..
+000059e0: 1c30 4e02 000c 0021 6200 1100 7b02 0037  .0N....!b...{..7
+000059f0: 0034 0400 0700 5202 001c 3b4e 0200 0c00  .4....R...;N....
+00005a00: 2178 0011 007b 0200 3700 4304 0015 0080  !x...{..7.C.....
+00005a10: 8002 0011 002d 0200 1100 3702 0010 0043  .....-....7....C
+00005a20: 0400 1500 2d02 0011 0074 0200 1100 7102  ....-....t....q.
+00005a30: 0011 0d44 0200 1100 80a1 2000 7d04 6002  ...D...... .}.`.
+00005a40: 0010 0052 1000 1500 3402 0011 007b 0200  ...R....4....{..
+00005a50: 1000 6e04 302b 0000 0200 0b00 6307 003e  ..n.0+......c..>
+00005a60: 0477 2200 0006 0002 7d22 0800 400c 5724  .w".....}"..@.W$
+00005a70: 0044 0200 2400 8081 0600 4a00 809c 0200  .D..$.....J.....
+00005a80: 3c00 4206 000c 0064 0200 2508 1202 001f  <.B....d..%.....
+00005a90: 0022 1600 0300 2002 0003 0020 0200 0300  .".... .... ....
+00005aa0: 4802 000c 0018 0254 0d00 0005 001d 003f  H......T.......?
+00005ab0: 1c00 1d04 7704 000d 0200 0400 0080 c200  ....w...........
+00005ac0: 5806 103f 0180 e802 0080 8500 0604 0005  X..?............
+00005ad0: 0019 0600 0700 7c04 0017 0027 0408 0700  ......|....'....
+00005ae0: 7606 7917 0021 0080 ee07 0061 04bf 133f  v.y..!.....a...?
+00005af0: 001c 0200 0300 0602 0005 0017 0600 0700  ................
+00005b00: 8084 0400 1700 2504 0807 007e 0679 1700  ......%....~.y..
+00005b10: 1f00 80fe 0700 6304 bf03 3f00 1a02 0003  ......c...?.....
+00005b20: 0006 0200 0500 1708 0007 0076 0400 1700  ...........v....
+00005b30: 2500 80ee 0700 7004 bf13 1700 1f00 80e2  %.....p.........
+00005b40: 0700 5d04 bf1f 3f00 1a02 0003 0006 0200  ..]...?.........
+00005b50: 0500 0004 0023 0e0e 1c00 4702 7312 0006  .....#....G.s...
+00005b60: 0200 0500 5c06 003f 0006 0200 0500 6404  ....\..?......d.
+00005b70: 003f 0006 0200 0500 6604 003f 0006 0200  .?......f..?....
+00005b80: 0500 6204 003f 0006 0200 0500 5e04 003f  ..b..?......^..?
+00005b90: 0006 0200 0500 5c04 003f 0006 0200 0500  ......\..?......
+00005ba0: 6404 003f 0006 0200 0500 1204 0005 0054  d..?...........T
+00005bb0: 0026 1200 1204 5b08 005a 0026 1200 0604  .&....[..Z.&....
+00005bc0: 5b05 006a 0400 3f00 0602 0005 0068 0400  [..j..?......h..
+00005bd0: 3f00 0602 0005 0060 0400 3f00 0602 0005  ?......`..?.....
+00005be0: 0012 0400 0500 5200 2612 0012 045b 0800  ......R.&....[..
+00005bf0: 5600 2612 0006 045b 0500 5c0a 003f 0006  V.&....[..\..?..
+00005c00: 0200 0500 5c04 003f 0006 0200 0500 5c04  ....\..?......\.
+00005c10: 003f 0006 0200 0500 5c04 003f 0006 0200  .?......\..?....
+00005c20: 0500 5c04 003f 0006 0200 0500 5c04 003f  ..\..?......\..?
+00005c30: 0006 0200 0500 6a04 003f 0006 0200 0500  ......j..?......
+00005c40: 6b04 003f 0006 0200 0500 8081 0400 3300  k..?..........3.
+00005c50: 0602 0005 0055 0400 3300 0602 0002 0057  .....U..3......W
+00005c60: 0400 3300 0602 0002 0061 0400 3300 0602  ..3......a..3...
+00005c70: 0002 0028 0800 0600 6b04 7153 0002 bedd  ...(....k.qS....
+00005c80: 460e 0000 0e00 7581 2a33 4800 7106 001c  F.....u.*3H.q...
+00005c90: 005f 0408 1200 7406 791c 0061 0408 1200  ._....t.y..a....
+00005ca0: 6a06 791c 005b 0408 1200 7f08 793c 0079  j.y..[......y<.y
+00005cb0: 0200 3c08 8090 0600 2500 6112 0025 2d7e  ..<.....%.a..%-~
+00005cc0: 0400 1f00 5662 001f 017a 0200 2500 3a08  ....Vb...z..%.:.
+00005cd0: 0010 0066 0600 1f00 4a06 0019 0182 2e02  ...f....J.......
+00005ce0: 0080 a000 810f 0400 2a01 824a 0200 80a0  ........*..J....
+00005cf0: 0081 1e04 002a 0182 2002 0080 a000 8100  .....*.. .......
+00005d00: 0400 2a00 4902 0019 004f 0200 1900 5d02  ..*.I....O....].
+00005d10: 0019 0060 0200 1900 5d02 0019 0080 8f02  ...`....].......
+00005d20: 0019 1756 0200 1900 8089 3000 1900 6602  ...V......0...f.
+00005d30: 0019 0053 0200 1900 8174 0200 6817 5a02  ...S.....t..h.Z.
+00005d40: 0019 2b6c 3000 6800 5658 0019 0054 0200  ..+l0.h.VX...T..
+00005d50: 1900 5402 0019 0056 0200 1900 5602 0019  ..T....V....V...
+00005d60: 005a 0200 1900 80aa 0200 1900 80a8 0200  .Z..............
+00005d70: 1900 809d 0200 1900 80a9 0200 1900 8096  ................
+00005d80: 0200 1900 80d9 0200 1900 80d8 0200 1900  ................
+00005d90: 6a02 0019 0046 0200 1900 4202 0019 0045  j....F....B....E
+00005da0: 0200 1900 1806 6a0d 0000 0500 2800 291c  ......j.....(.).
+00005db0: 0046 0477 1400 4302 0023 0055 0200 1c00  .F.w..C..#.U....
+00005dc0: 6a04 0857 0044 0879 2301 813e 0200 80c4  j..W.D.y#..>....
+00005dd0: 0047 0600 2546 0402 0080 d700 0d04 360c  .G..%F........6.
+00005de0: 002b 020c 3e01 8088 027f 4800 3104 0c3e  .+..>.....H.1..>
+00005df0: 0180 9402 7f48 0026 0475 3e01 7e02 7f48  .....H.&.u>.~..H
+00005e00: 0026 0459 1600 2e00 540c 0047 0245 0c00  .&.Y....T..G.E..
+00005e10: 3502 080c 004b 0202 0c00 4c02 000c 0038  5....K....L....8
+00005e20: 0202 0c06 0602 750c 0037 0e08 0c00 3802  ......u..7....8.
+00005e30: 060c 0031 0275 0c00 3d04 630c 0606 0220  ...1.u..=.c.... 
+00005e40: 0c06 060e 100c 004c 0e6f 0c00 3302 7b0c  .......L.o..3.{.
+00005e50: 0034 0202 0c00 3602 040c 0036 0200 0c00  .4....6....6....
+00005e60: 3502 060c 0051 045d 3e00 4f04 003e 004c  5....Q.]>.O..>.L
+00005e70: 0400 3e00 5204 003e 004f 0400 3e00 4a04  ..>.R..>.O..>.J.
+00005e80: 003e 0049 0400 3e00 5502 383b 003c 026b  .>.I..>.U.8;.<.k
+00005e90: 0900 3702 1009 0035 0271 0900 1402 7f09  ..7....5.q......
+00005ea0: 0049 0263 2200 0004 0033 046f 0900 02bf  .I.c"....3.o....
+00005eb0: 555c 0e00 000e 0764 80b4 1d12 076e 1200  U\.....d.....n..
+00005ec0: 1207 6012 0012 0780 9016 0080 9900 4a16  ..`...........J.
+00005ed0: 000d 0044 0200 0d00 4902 000d 005b 0200  ...D....I....[..
+00005ee0: 0e13 6402 0080 a100 262c 000d 005d 004e  ..d.....&,...].N
+00005ef0: 1200 4d04 7335 0000 0200 1300 5307 0055  ..M.s5......S..U
+00005f00: 0477 0a00 027d 320b 0000 0b00 0001 000c  .w...}2.........
+00005f10: 0a04 1100 0002 0012 0055 0700 6004 4632  .........U..`.F2
+00005f20: 0000 0200 1b00 4307 0148 0477 1500 027d  ......C..H.w...}
+00005f30: 420b 0000 0b00 0001 0002 7d67 0b00 000b  B.........}g....
+00005f40: 0000 0101 5012 4925 0073 0600 2500 7302  ....P.I%.s..%.s.
+00005f50: 0025 0073 0200 2500 270a 000d 005f 0050  .%.s..%.'...._.P
+00005f60: 1204 5d06 6943 0000 0200 0f00 5b07 0076  ..].iC......[..v
+00005f70: 0c77 1c00 0006 0002 752a 0800 2c12 0623  .w......u*..,..#
+00005f80: 0000 0500 0f00 5b07 0066 0458 4200 0002  ......[..f.XB...
+00005f90: 0024 0031 0900 2404 7709 0050 0400 1700  .$.1..$.w..P....
+00005fa0: 0279 540b 0000 0b00 0001 0000 0600 027d  .yT............}
+00005fb0: 4f0b 000a 1659 0400 0002 007e 047f 4c00  O....Y.....~..L.
+00005fc0: 037d 2c06 0007 006f 0600 280c 5f0d 0050  .},....o..(._..P
+00005fd0: 0408 1202 3806 7925 002a 0a00 0d00 6600  ....8.y%.*....f.
+00005fe0: 5612 006f 087d 4500 0002 001c 0041 0700  V..o.}E......A..
+00005ff0: 4304 771a 0002 7d44 0b00 000b 0000 0129  C.w...}D.......)
+00006000: 8094 0a35 2500 3758 0015 004e 0262 3000  ...5%.7X...N.b0.
+00006010: 0002 0024 0031 0900 1706 770b 0364 0408  ...$.1....w..d..
+00006020: 1700 180e 790e 005e 0032 1100 0269 220b  ....y..^.2...i".
+00006030: 0000 0b00 0001 0068 2006 4500 0002 0024  .......h .E....$
+00006040: 0031 0900 2d04 7716 0142 0408 1700 0279  .1..-.w..B.....y
+00006050: 4c0b 0000 0b00 0001 0078 1406 4500 0002  L........x..E...
+00006060: 0024 0031 0701 4204 7715 0002 7d54 0b00  .$.1..B.w...}T..
+00006070: 000b 0000 0100 670e 0645 0000 0200 2400  ......g..E....$.
+00006080: 3109 002e 0477 1601 4204 0817 0002 794c  1....w..B.....yL
+00006090: 0b00 000b 0000 0100 6c16 0645 0000 0200  ........l..E....
+000060a0: 2400 3109 0017 0677 0b04 6404 0817 0018  $.1....w..d.....
+000060b0: 1079 0e00 5e00 3211 0002 6722 0b00 000b  .y..^.2...g"....
+000060c0: 0000 0100 808b 2225 1f00 4e06 381b 0000  ......"%..N.8...
+000060d0: 0200 0f00 5b07 0080 8604 7722 0000 0600  ....[.....w"....
+000060e0: 027d 2a08 0080 f80c 4f1f 0224 0600 2501  .}*.....O..$..%.
+000060f0: 2406 0025 0080 9e08 001f 0075 0600 1f00  $..%.......u....
+00006100: 2906 000d 0063 0054 1200 80a6 062d 1f00  )....c.T.....-..
+00006110: 4306 0010 0026 0600 0d00 5900 4e12 0180  C....&....Y.N...
+00006120: cc04 331f 0025 0800 0d00 5b00 4c12 0060  ..3..%....[.L..`
+00006130: 0635 1f00 4c04 000c 0b80 b204 001f 004e  .5..L..........N
+00006140: 1a00 0c00 4e04 000c 1b80 9804 001f 0052  ....N..........R
+00006150: 3a00 0c02 81f4 0400 1f02 81f4 0800 1f00  :...............
+00006160: 5c08 001f 0181 1604 001f 0e80 a206 0025  \..............%
+00006170: 0180 ba1e 0025 0028 0800 0d00 6100 5212  .....%.(....a.R.
+00006180: 1b80 9e04 2f25 0028 3c00 0d00 5f00 5212  ..../%.(<..._.R.
+00006190: 006e 062f 1f00 7606 0025 0080 8404 0025  .n./..v..%.....%
+000061a0: 0812 0600 1f00 4116 0010 0080 8f06 0052  ......A........R
+000061b0: 0680 9606 0080 b200 3212 000d 0075 0066  ........2....u.f
+000061c0: 1200 3b0a 1b10 1763 0e32 80c0 0000 0500  ..;....c.2......
+000061d0: 0c00 6107 0604 3277 4000 4a04 142a 004e  ..a...2w@.J..*.N
+000061e0: 0080 9c09 0018 022d 0900 2202 4909 0019  .......-..".I...
+000061f0: 026f 0700 0004 0080 9006 6f28 0000 0600  .o........o(....
+00006200: 023f 240b 0016 4a7f 0d00 0005 0008 0069  .?$...J........i
+00006210: 0900 0c04 3611 0000 0500 1300 5307 0010  ....6.......S...
+00006220: 0458 0c00 0005 0024 0031 0900 2604 7713  .X.....$.1..&.w.
+00006230: 0080 9004 0080 8600 0279 540e 0000 0b00  .........yT.....
+00006240: 0001 0002 7d57 0e00 000b 0000 0100 027d  ....}W.........}
+00006250: 630e 0000 0e00 421c 5d10 0033 0600 0f01  c.....B.]..3....
+00006260: 8108 0800 3500 3708 0010 0038 060e 0d00  ....5.7....8....
+00006270: 3104 7b27 0001 0279 0200 000b 0000 0100  1.{'...y........
+00006280: 0102 7905 0980 1a06 0005 0981 1a06 0005  ..y.............
+00006290: 0982 1a06 0005 0983 1a06 0005 0984 1a06  ................
+000062a0: 0005 0985 1a06 0005 0986 1a06 0006 0000  ................
+000062b0: 0035 1505 1a00 0000 5f1b 050b 0059 0800  .5......_....Y..
+000062c0: 0b00 5508 000b 0051 0800 0b00 5f10 0025  ..U....Q...._..%
+000062d0: 5379 7374 656d 2e43 6f6d 706f 6e65 6e74  System.Component
+000062e0: 4d6f 6465 6c2e 4461 7461 416e 6e6f 7461  Model.DataAnnota
+000062f0: 7469 6f6e 7323 01af 0c01 af13 01af 2e01  tions#..........
+00006300: af38 01af 4401 af54 01af 6501 c000 47ef  .8..D..T..e...G.
+00006310: 01b0 0f01 b26c 01b1 ec07 0000 0056 80da  .....l.......V..
+00006320: 050c 0000 002e 8110 0507 0021 4800 1b00  ...........!H...
+00006330: 0000 1d81 3b05 0b00 2408 000b 0028 0800  ....;...$....(..
+00006340: 0b00 2608 000b 001d 1200 0700 0000 2482  ..&...........$.
+00006350: 3405 0c00 0000 2682 3e05 0b00 3208 0011  4.....&.>...2...
+00006360: 0000 001f 8249 050b 001e 0800 0b00 3d08  .....I........=.
+00006370: 0007 0000 0018 8260 0523 0000 0069 0c09  .......`.#...i..
+00006380: 2100 80a8 0400 2100 80bc 0400 3100 808f  !.....!.....1...
+00006390: 0400 2100 8085 0600 2100 0102 791d 01af  ..!.....!...y...
+000063a0: 0c01 af13 01af 2e01 af38 01af 4401 af54  .........8..D..T
+000063b0: 01af 6501 afbb 01af cb03 1c80 a909 0000  ..e.............
+000063c0: 5f1c 0921 005f 0200 2114 1204 001b 0612  _..!._..!.......
+000063d0: 2c00 2107 1210 0021 0412 1200 2106 120c  ,.!....!....!...
+000063e0: 0021 1d12 0e00 2117 123e 0082 2800 4134  .!....!..>..(.A4
+000063f0: 0012 005b 0600 3400 6e02 001b 005c 0400  ...[..4.n....\..
+00006400: 3700 6f02 001b 005c 0400 3400 6f02 001b  7.o....\..4.o...
+00006410: 005c 0400 3700 6f02 001b 005b 0400 3400  .\..7.o....[..4.
+00006420: 6e02 001b 005c 0400 3700 6f02 001b 005c  n....\..7.o....\
+00006430: 0400 3700 6f02 001b 0080 870a 0021 0080  ..7.o........!..
+00006440: 8706 0021 0080 8706 0021 0080 8706 0021  ...!.....!.....!
+00006450: 0080 8706 0021 0080 8706 0021 0080 8706  .....!.....!....
+00006460: 0021 0001 0279 1100 0000 3780 be09 0800  .!...y....7.....
+00006470: 3e02 0008 0001 0279 2200 0080 df12 0a09  >......y".......
+00006480: 1519 1281 c200 1500 6e36 0021 0080 aa02  ........n6.!....
+00006490: 0021 006e 0200 2100 0102 791b 01af 0c01  .!.n..!...y.....
+000064a0: af13 01af 2e01 af38 01af 4401 af54 01af  .......8..D..T..
+000064b0: 6501 afbb 01af cb34 0a00 0000 1400 520e  e......4......R.
+000064c0: 0920 0080 8702 0012 002b 0400 0600 2902  . .......+....).
+000064d0: 000c 003b 0200 1b00 0102 7902 0000 0900  ...;......y.....
+000064e0: 0001 0000 0900 0001 0001 0000 2701 af0c  ............'...
+000064f0: 01af 1301 af2e 01af 3801 af44 01af 5401  ........8..D..T.
+00006500: af65 01b2 9301 b2a8 01b2 eb01 afbb 01af  .e..............
+00006510: cb01 afe6 6a0b 0000 2f1a 090d 002b 0476  ....j.../....+.v
+00006520: 1c00 0002 002a 0025 0700 5f04 7716 0002  .....*.%.._.w...
+00006530: 7d60 0a00 0009 0000 0100 300e 110d 0060  }`........0....`
+00006540: 0476 3700 0002 002a 0025 0700 6004 7716  .v7....*.%..`.w.
+00006550: 0002 7d60 0a00 0009 0000 0100 2d0e 110d  ..}`........-...
+00006560: 0080 8104 4e39 0000 0200 1600 4d09 0053  ....N9......M..S
+00006570: 0477 1700 027d 380b 0000 0e00 010a 3183  .w...}8.......1.
+00006580: 5f0c 0000 0006 004d 0d09 110e 1206 0010  _......M........
+00006590: 0050 1e02 2100 5002 0021 0032 067f 1200  .P..!.P..!.2....
+000065a0: 0c02 2a0c 0000 0200 0800 6906 0052 0420  ..*.......i..R. 
+000065b0: 3000 0002 0008 0069 0700 1f04 7706 0002  0......i....w...
+000065c0: 7d1c 0b00 000b 0000 0100 027d 790a 0000  }..........}y...
+000065d0: 0900 0001 0013 105d 0800 3306 0017 001e  .......]..3.....
+000065e0: 0238 1b00 0005 000f 005b 0700 2904 7710  .8.......[..).w.
+000065f0: 0504 0200 1e00 4e04 2431 0043 0200 3100  ......N.$1.C..1.
+00006600: 5c02 6f0b 0000 0200 1604 180c 0000 0200  \.o.............
+00006610: 0800 6909 0018 0477 0f00 027d 1c0b 0000  ..i....w...}....
+00006620: 0e00 1b0a 5d0e 0045 0408 3400 0002 001b  ....]..E..4.....
+00006630: 0402 0e00 4304 7f30 0000 0600 0259 220b  ....C..0.....Y".
+00006640: 0019 324f 0600 1402 480d 0000 0500 1700  ..2O....H.......
+00006650: 4b1c 0013 0477 0300 0c02 2a0c 0000 0500  K....w....*.....
+00006660: 0800 6908 0010 042c 0e00 0005 000e 005d  ..i....,.......]
+00006670: 0900 2004 770e 004c 0400 1d00 5002 001d  .. .w..L....P...
+00006680: 0026 0200 0d00 8090 0408 3801 2a06 7942  .&........8.*.yB
+00006690: 0055 0608 3800 2b06 7904 0011 0200 0700  .U..8.+.y.......
+000066a0: 1406 0804 003f 0200 1300 80ec 0200 5608  .....?........V.
+000066b0: 0404 005c 0004 0c16 0500 0502 7d03 0000  ...\........}...
+000066c0: 0600 1606 6f05 0009 0412 0300 0002 005a  ....o..........Z
+000066d0: 047f 1200 811e 0200 6700 037b 2806 0006  ........g..{(...
+000066e0: 0071 0800 80ed 1059 5300 1b02 000e 000d  .q.....YS.......
+000066f0: 0679 0300 1e02 000c 0073 0408 6a00 1602  .y.......s..j...
+00006700: 000d 0019 0200 0900 3606 7913 0044 0200  ........6.y..D..
+00006710: 1300 4202 0013 2804 0400 809d 0017 0436  ..B...(........6
+00006720: 0c00 3b02 0238 003b 020a 3800 3b02 7338  ..;..8.;..8.;.s8
+00006730: 002d 020a 0c00 2d02 790c 002d 027d 0c00  .-....-.y..-.}..
+00006740: 2d02 040c 002d 0200 0c00 2d02 7b0c 002d  -....-....-.{..-
+00006750: 0202 0c00 2d02 040c 002d 027f 0c00 2d02  ....-....-....-.
+00006760: 0e0c 002d 027d 0c00 2d02 040c 002d 0200  ...-.}..-....-..
+00006770: 0c00 2d02 7d0c 002d 0200 0c00 2d02 020c  ..-.}..-....-...
+00006780: 002d 027d 0c00 2d02 060c 002d 0273 0c00  .-.}..-....-.s..
+00006790: 2d02 000c 002d 0200 0c00 2d02 100c 002d  -....-....-....-
+000067a0: 0202 0c00 2d02 7f0c 002d 0204 0c00 2d02  ....-....-....-.
+000067b0: 7b0c 002d 020c 0c00 2d02 690c 0380 b202  {..-....-.i.....
+000067c0: 105f 005d 087f 4c00 5e02 4f52 0000 0400  ._.]..L.^.OR....
+000067d0: 6106 6f1c 002f 0408 0c00 3102 000c 000c  a.o../....1.....
+000067e0: 0200 0400 1204 0813 000d 0200 1000 2208  ..............".
+000067f0: 7919 0036 0200 1300 8086 0200 4600 6108  y..6........F.a.
+00006800: 7916 0014 0408 0e00 2404 0813 000d 0200  y.......$.......
+00006810: 1000 6108 711c 0022 0408 1900 1202 0013  ..a.q.."........
+00006820: 0022 0200 1000 8096 0200 5400 809e 0200  ."........T.....
+00006830: 3000 0d02 2a07 0000 0200 0800 6909 0018  0...*.......i...
+00006840: 0277 0f00 027f 1c0b 0000 0e00 6108 551c  .w..........a.U.
+00006850: 004a 0408 1300 2c02 0019 0012 0200 1300  .J....,.........
+00006860: 1702 000c 0062 0208 4000 0002 0020 0202  .....b..@.... ..
+00006870: 1500 6202 7f40 0031 0871 0b00 2c02 0809  ..b..@.1.q..,...
+00006880: 0000 0200 3202 020b 002b 027f 0900 0002  ....2....+......
+00006890: 0023 0400 0900 2c04 790e 0011 0200 0400  .#....,.y.......
+000068a0: 0602 0002 0002 bebf 280e 0000 0b00 0001  ........(.......
+000068b0: 000a 8148 5104 0006 0016 0200 02be b506  ...HQ...........
+000068c0: 0d00 0009 0000 0100 0b81 525d 0400 4302  ..........R]..C.
+000068d0: 0838 0002 bea7 320e 0000 0e00 0181 5e37  .8....2.......^7
+000068e0: 1753 7973 7465 6d2e 4e65 742e 4874 7470  .System.Net.Http
+000068f0: 2e48 6561 6465 7273 2501 af0c 01af 1301  .Headers%.......
+00006900: af2e 01af 3801 af44 01af 5401 af65 01c0  ....8..D..T..e..
+00006910: 004e 0001 afbb 01af cb01 afe6 031c 809a  .N..............
+00006920: 0d00 004d 0b09 1108 0a08 0015 270a 1400  ...M........'...
+00006930: 3004 0a54 000a 1f0a 0e00 1506 0a46 0021  0..T.........F.!
+00006940: 040a 1200 1b14 0a0e 0015 030a 2c00 1b15  ............,...
+00006950: 0a0c 001b 2954 3000 1b00 7758 001d 0037  ....)T0...wX...7
+00006960: 0200 0600 2b02 000c 004c 0200 0600 3802  ....+....L....8.
+00006970: 0017 0014 0200 0700 1d02 000c 0028 0200  .............(..
+00006980: 0700 1e02 000c 811c 0a02 0083 cf00 2982  ..............).
+00006990: 3a00 0c00 4c02 001c 003b 0200 0600 3002  :...L....;....0.
+000069a0: 0007 0034 0200 0700 2002 0009 002a 0200  ...4.... ....*..
+000069b0: 0d00 2902 0007 0001 0279 1e01 af0c 01af  ..)......y......
+000069c0: 1301 af2e 01af 3801 af44 01af 5401 af65  ......8..D..T..e
+000069d0: 01af bb01 afcb 01af e685 310e 0000 0008  ..........1.....
+000069e0: 0037 1109 0c00 4902 0006 0024 040e 0600  .7....I....$....
+000069f0: 7b04 7b1f 002f 0200 0c00 3102 000c 0029  {.{../....1....)
+00006a00: 0200 0c00 6002 0017 0001 0279 0200 0009  ....`......y....
+00006a10: 0000 0100 2b02 0011 0080 c204 0024 000c  ....+........$..
+00006a20: 022a 0700 0005 0008 0069 0900 4304 7707  .*.......i..C.w.
+00006a30: 001a 0200 0e00 1a02 000e 0052 0200 2600  ...........R..&.
+00006a40: 5602 0026 0025 0200 0800 2602 0012 0045  V..&.%....&....E
+00006a50: 0200 2400 026f 1c0e 0000 0e00 0007 0060  ..$..o.........`
+00006a60: 1c65 2700 4e02 0027 0080 8402 0019 0053  .e'.N..'.......S
+00006a70: 0200 2200 4a02 0022 0064 0200 1400 2402  ..".J..".d....$.
+00006a80: 0e07 0029 047b 0e00 3902 001d 0001 0279  ...).{..9......y
+00006a90: 0200 000b 0000 0100 6204 0027 0050 0200  ........b..'.P..
+00006aa0: 2700 8089 0200 1900 5502 0022 004c 0200  '.......U..".L..
+00006ab0: 2200 6802 0014 0024 020e 0700 2a04 7b0e  ".h....$....*.{.
+00006ac0: 003a 0200 1d00 0102 7902 0000 0b00 0001  .:......y.......
+00006ad0: 0072 2279 3b00 7802 003b 0078 0200 3b00  .r"y;.x..;.x..;.
+00006ae0: 7e02 003b 006b 0200 3b00 80a6 0200 5700  ~..;.k..;.....W.
+00006af0: 80a6 0200 5700 80a6 0200 5700 80a6 0200  ....W.....W.....
+00006b00: 5700 80a6 0200 5700 80a6 0200 5700 80a6  W.....W.....W...
+00006b10: 0200 5700 80b2 0400 5701 8136 0400 5701  ..W.....W..6..W.
+00006b20: 8122 0400 5701 8112 0400 5701 810e 0400  ."..W.....W.....
+00006b30: 5700 80a5 0800 4b00 80a7 0200 4b00 80a1  W.....K.....K...
+00006b40: 0200 4b00 80a3 0200 4b00 80a5 0200 4b00  ..K.....K.....K.
+00006b50: 809f 0200 4b00 80a8 0200 4b00 80aa 0200  ....K.....K.....
+00006b60: 4b00 80a4 0200 4b00 7506 0046 0078 0200  K.....K.u..F.x..
+00006b70: 4600 7602 0046 0076 0200 4600 7b02 0046  F.v..F.v..F.{..F
+00006b80: 0080 a206 004b 0080 a002 004b 0080 a202  .....K.....K....
+00006b90: 004b 0080 a202 004b 0080 9f02 004b 0080  .K.....K.....K..
+00006ba0: 9c02 004b 0080 9e02 004b 0080 9d02 004b  ...K.....K.....K
+00006bb0: 0080 a402 004b 0080 9e02 004b 0080 a002  .....K.....K....
+00006bc0: 004b 0080 a002 004b 0080 9e02 004b 0080  .K.....K.....K..
+00006bd0: 9e02 004b 0080 9f02 004b 0080 9d02 004b  ...K.....K.....K
+00006be0: 0080 a402 004b 0080 9d02 004b 0080 9d02  .....K.....K....
+00006bf0: 004b 0080 9d02 004b 0080 a602 004b 0080  .K.....K.....K..
+00006c00: a602 004b 0080 a502 004b 0080 ab02 004b  ...K.....K.....K
+00006c10: 0080 a802 004b 0080 aa02 004b 0080 9e02  .....K.....K....
+00006c20: 004b 0032 0600 2000 8099 0200 4b00 8099  .K.2.. .....K...
+00006c30: 0200 4b00 8099 0200 4b00 8099 0200 4b00  ..K.....K.....K.
+00006c40: 8099 0200 4b00 8099 0200 4b00 8099 0200  ....K.....K.....
+00006c50: 4b00 8099 0200 4b00 8099 0200 4b05 0616  K.....K.....K...
+00006c60: 0080 8004 060e 0072 0406 0c00 7204 060c  .......r....r...
+00006c70: 0072 0406 0c00 7204 060c 0072 0406 0c00  .r....r....r....
+00006c80: 7204 060a 0072 0406 0c00 7200 280c 000c  r....r....r.(...
+00006c90: 0023 0200 0c00 2802 000c 0506 0400 7204  .#....(.......r.
+00006ca0: 060e 0072 0406 0c00 7204 060c 0072 0506  ...r....r....r..
+00006cb0: 0c00 8080 0506 0e00 8080 0039 0e00 2000  ...........9.. .
+00006cc0: 6702 0027 0034 0600 1c00 3502 001d 0039  g..'.4....5....9
+00006cd0: 0400 2000 6702 0027 0080 9504 004b 0a06  .. .g..'.....K..
+00006ce0: 0400 8117 3706 1800 8a97 0406 7200 7204  ....7.......r.r.
+00006cf0: 060c 0072 0406 0c00 7204 060c 0072 002f  ...r....r....r./
+00006d00: 0c00 0c00 2f02 000c 0506 0600 8082 0023  ..../..........#
+00006d10: 1000 0d00 3404 4423 0000 0200 1100 5707  ....4.D#......W.
+00006d20: 003c 0477 1300 5502 002d 0000 0600 027b  .<.w..U..-.....{
+00006d30: 2e08 0406 1043 6d00 2312 000c 002d 0600  .....Cm.#....-..
+00006d40: 0c00 3202 000c 0032 0200 0c00 3602 000c  ..2....2....6...
+00006d50: 0033 0200 0c00 3402 000c 0033 0200 0c00  .3....4....3....
+00006d60: 3502 000c 0030 0200 0c00 3202 000c 0034  5....0....2....4
+00006d70: 0200 0c00 3102 000c 0032 0200 0c00 2a02  ....1....2....*.
+00006d80: 000c 002e 0200 0c00 3002 000c 0031 0200  ........0....1..
+00006d90: 0c00 3002 000c 0030 0200 0c00 2c02 000c  ..0....0....,...
+00006da0: 0030 0200 0c00 2e02 000c 002f 0200 0c00  .0........./....
+00006db0: 2f02 000c 002e 0200 0c00 3602 000c 002e  /.........6.....
+00006dc0: 0200 0c00 2f02 000c 0031 0200 0c00 3102  ..../....1....1.
+00006dd0: 000c 002e 0200 0c00 2d02 000c 002f 0200  ........-..../..
+00006de0: 0c00 2e02 000c 002b 0800 0c00 3102 000c  .......+....1...
+00006df0: 002e 0200 0c00 3002 000c 002c 0200 0c00  ......0....,....
+00006e00: 3102 000c 002e 0200 0c00 2e02 000c 002e  1...............
+00006e10: 0200 0c00 3302 000c 002f 0200 0c00 2f02  ....3..../..../.
+00006e20: 000c 002f 0200 0c00 2d02 000c 0030 0200  .../....-....0..
+00006e30: 0c00 2f02 000c 002f 0200 0c00 2f02 000c  ../..../..../...
+00006e40: 0037 0200 0c00 3502 000c 0031 0200 0c00  .7....5....1....
+00006e50: 3302 000c 0032 0200 0c00 3202 000c 002f  3....2....2..../
+00006e60: 0200 0c00 2c02 000c 002f 0800 0c00 3202  ....,..../....2.
+00006e70: 000c 002a 0200 0c00 2a02 000c 002f 0200  ...*....*..../..
+00006e80: 0c00 3002 000c 0030 0200 0c00 3402 000c  ..0....0....4...
+00006e90: 0030 0200 0c00 3402 000c 002e 0200 0c00  .0....4.........
+00006ea0: 3602 000c 0032 0200 0c00 3102 000c 002f  6....2....1..../
+00006eb0: 0200 0c00 2e02 000c 0031 0200 0c00 3802  .........1....8.
+00006ec0: 000c 0031 0200 0c00 2e02 000c 0032 0200  ...1.........2..
+00006ed0: 0c00 3902 000c 002e 0200 0c00 2d02 000c  ..9.........-...
+00006ee0: 0029 0800 0c00 2e08 000c 002c 0200 0c00  .).........,....
+00006ef0: 3102 000c 002d 0200 0c00 2c02 000c 002d  1....-....,....-
+00006f00: 0200 0c00 3008 000c 0001 0679 3001 af0c  ....0......y0...
+00006f10: 01af 1301 af2e 01af 3801 af44 01af 5401  ........8..D..T.
+00006f20: af65 01af fd01 b26c 01b2 7d01 b293 01b2  .e.....l..}.....
+00006f30: a801 b2eb 01af bb01 afcb 01af e637 0f00  .............7..
+00006f40: 0043 480d 0600 5d02 2e3b 0000 0200 0a00  .CH...]..;......
+00006f50: 6507 0019 0477 0900 6a00 342d 0002 7d6d  e....w..j.4-..}m
+00006f60: 0a00 0009 0000 0100 100a 5908 003e 0208  ..........Y..>..
+00006f70: 1100 0c04 790c 0000 0406 80a9 0d73 0001  ....y........s..
+00006f80: 0a79 8135 1000 0039 0c09 0600 1602 520d  .y.5...9......R.
+00006f90: 0000 0200 1c00 411c 0065 0277 5400 027f  ......A..e.wT...
+00006fa0: 440b 0000 0e00 3d04 3507 0071 0400 1d0d  D.....=.5..q....
+00006fb0: 0a02 004c 0077 1c00 1d00 5e02 000b 0075  ...L.w....^....u
+00006fc0: 0200 1e05 0a02 000c 0075 0c00 1e09 0a02  .........u......
+00006fd0: 000c 0071 1400 1e22 0a02 000c 001f 4600  ...q..."......F.
+00006fe0: 0c00 2402 000c 0024 0200 0d00 2602 000d  ..$....$....&...
+00006ff0: 0021 0200 0d00 8087 0600 3000 2602 000d  .!........0.&...
+00007000: 0080 9202 001b 0033 0400 0d00 3a02 0007  .......3....:...
+00007010: 0025 0200 0800 3302 0007 001e 0200 0800  .%....3.........
+00007020: 2802 000e 0027 0200 0700 2f04 000d 0036  (....'..../....6
+00007030: 0200 0700 2a02 0008 002f 0200 0700 1e02  ....*..../......
+00007040: 0008 0028 0200 0e00 2702 0007 002f 0400  ...(....'..../..
+00007050: 0d00 3602 0007 0027 0200 0900 2f02 0007  ..6....'..../...
+00007060: 001e 0200 0800 2802 000e 0027 0200 0700  ......(....'....
+00007070: 2f04 000d 0036 0200 0700 2c02 0009 002f  /....6....,..../
+00007080: 0200 0700 1e02 0008 0028 0200 0e00 2702  .........(....'.
+00007090: 0007 002f 0400 0d00 3602 0007 002a 0200  .../....6....*..
+000070a0: 0900 2f02 0007 001f 0200 0900 2802 000e  ../.........(...
+000070b0: 0027 0200 0700 0102 790b 5379 7374 656d  .'......y.System
+000070c0: 2e54 6578 7423 01af 0c01 af13 01af 2e01  .Text#..........
+000070d0: af38 01af 4401 af54 01af 6501 c000 55d9  .8..D..T..e...U.
+000070e0: 01af bb01 afcb 01af e67d 1100 005a 0c09  .........}...Z..
+000070f0: 0b00 1602 560d 0000 0500 1e00 3d18 0011  ....V.......=...
+00007100: 0430 0e00 0005 0010 0059 0900 8084 0477  .0.......Y.....w
+00007110: 808d 0002 7d2c 0e00 000e 0002 7d14 0e00  ....},......}...
+00007120: 000e 0038 0e31 0700 5602 0017 110a 0200  ...8.1..V.......
+00007130: 2100 6e24 001d 0048 0200 0b00 2102 000c  !.n$...H....!...
+00007140: 0046 0200 1c00 3702 0006 0024 0200 0700  .F....7....$....
+00007150: 3002 0007 001b 0200 0800 2202 000d 0021  0........."....!
+00007160: 0200 0700 0102 790c 0000 0080 a30a 0921  ......y........!
+00007170: 0001 0279 4b12 0000 4d0a 0912 005d 0600  ...yK...M....]..
+00007180: 2100 5f02 0021 002b 0600 0d00 5d04 0811  !._..!.+....]...
+00007190: 1412 0279 2107 1a2c 0021 0080 af12 0021  ...y!..,.!.....!
+000071a0: 0080 af02 0021 0080 8904 001b 0080 a304  .....!..........
+000071b0: 0021 2a0a 0400 1b0d 0a5a 001b 0001 1c79  .!*......Z.....y
+000071c0: 0600 0000 1a61 2307 0000 0018 82ea 3107  .....a#.......1.
+000071d0: 0000 0018 82fa 4907 0000 0017 82fb 4907  ......I.......I.
+000071e0: 0000 0017 82fc 3307 0000 0018 8316 5107  ......3.......Q.
+000071f0: 0000 0018 8317 5107 0000 0018 8318 5107  ......Q.......Q.
+00007200: 0000 0018 8319 5108 0000 0180 aa84 f13f  ......Q........?
+00007210: 0700 0002 6685 0040 0700 0002 6685 1740  ....f..@....f..@
+00007220: 0800 0001 80a6 8521 4007 0000 0035 88fc  .......!@....5..
+00007230: 4007 0000 0030 8922 7307 0000 0036 893f  @....0."s....6.?
+00007240: 6a07 0000 0030 8971 5707 0000 0030 8981  j....0.qW....0..
+00007250: 7107 1300 0040 898b 7107 0000 002f 8992  q....@..q..../..
+00007260: 7107 0000 0034 899d 7107 0000 0042 84e3  q....4..q....B..
+00007270: 5207 0000 0042 8903 5206 0000 006c 0f22  R....B..R....l."
+00007280: 0600 0000 3426 3f07 1400 0067 80d6 4406  ....4&?....g..D.
+00007290: 1500 0037 3535 0600 0000 2c36 3506 0000  ...755....,65...
+000072a0: 0001 4949 0600 0000 6a2f 2506 0000 004a  ..II....j/%....J
+000072b0: 3225 0600 0000 6e3b 2606 0000 004d 3e26  2%....n;&....M>&
```

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-2.2.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-2.2.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-2.2.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/am2r_yams/yams/sprites/texturepageiteminfo.json` & `am2r_yams-2.2.0/am2r_yams/yams/sprites/texturepageiteminfo.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7310661764705798%*

 * *Differences: {'100': "{'Name': 'sItemShinyHijump_2', 'Y': 435}",*

 * * '1000': "{'Name': 'sItemProgressiveSuitEchoes_15', 'Y': 690}",*

 * * '1001': "{'Name': 'sItemProgressiveSuitEchoes_11', 'Y': 690}",*

 * * '1002': "{'Name': 'sItemProgressiveSuitEchoes_7', 'Y': 690}",*

 * * '1003': "{'Name': 'sItemProgressiveSuitEchoes_8', 'Y': 690}",*

 * * '1004': "{'Name': 'sItemProgressiveSuitEchoes_16', 'Y': 690}",*

 * * '1005': "{'Name': 'sItemProgressiveSuitEchoes_4', 'Y': 690}",*

 * * '1006': "{'Name': 'sItemProgressiveSuitEchoes_10', 'Y': 690}",*

 * * '1007': "{'Nam […]*

```diff
@@ -1,7198 +1,7534 @@
 [
     {
+        "Height": 22,
+        "Name": "sAutoadP",
+        "Width": 33,
+        "X": 0,
+        "Y": 0
+    },
+    {
+        "Height": 21,
+        "Name": "sAutoadPClaw",
+        "Width": 12,
+        "X": 34,
+        "Y": 0
+    },
+    {
         "Height": 16,
-        "Name": "sItemMorphBall_3",
+        "Name": "sAutoadPFang",
+        "Width": 15,
+        "X": 47,
+        "Y": 0
+    },
+    {
+        "Height": 35,
+        "Name": "sWisdomSeptogg_2",
+        "Width": 47,
+        "X": 63,
+        "Y": 0
+    },
+    {
+        "Height": 35,
+        "Name": "sWisdomSeptogg_1",
+        "Width": 47,
+        "X": 111,
+        "Y": 0
+    },
+    {
+        "Height": 35,
+        "Name": "sWisdomSeptogg_3",
+        "Width": 47,
+        "X": 159,
+        "Y": 0
+    },
+    {
+        "Height": 35,
+        "Name": "sWisdomSeptogg_4",
+        "Width": 47,
+        "X": 207,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_3",
+        "Width": 8,
+        "X": 255,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_8",
+        "Width": 8,
+        "X": 264,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_9",
+        "Width": 8,
+        "X": 273,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_4",
+        "Width": 8,
+        "X": 282,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_2",
+        "Width": 8,
+        "X": 291,
+        "Y": 0
+    },
+    {
+        "Height": 4,
+        "Name": "sMapCornerUnexplored_0",
+        "Width": 8,
+        "X": 300,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_7",
+        "Width": 8,
+        "X": 309,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_6",
+        "Width": 8,
+        "X": 318,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapBlockUnexplored",
+        "Width": 8,
+        "X": 327,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_5",
+        "Width": 8,
+        "X": 336,
+        "Y": 0
+    },
+    {
+        "Height": 8,
+        "Name": "sMapCornerUnexplored_1",
+        "Width": 4,
+        "X": 345,
+        "Y": 0
+    },
+    {
+        "Height": 12,
+        "Name": "sGUISMissileSelected",
         "Width": 16,
-        "X": 0,
+        "X": 350,
+        "Y": 0
+    },
+    {
+        "Height": 12,
+        "Name": "sGUIPBombSelected",
+        "Width": 16,
+        "X": 367,
+        "Y": 0
+    },
+    {
+        "Height": 12,
+        "Name": "sGUISMissileNormalGreen",
+        "Width": 16,
+        "X": 384,
+        "Y": 0
+    },
+    {
+        "Height": 12,
+        "Name": "sGUIPBombNormal",
+        "Width": 16,
+        "X": 401,
+        "Y": 0
+    },
+    {
+        "Height": 12,
+        "Name": "sGUISMissileNormal",
+        "Width": 16,
+        "X": 418,
+        "Y": 0
+    },
+    {
+        "Height": 12,
+        "Name": "sGUIMissileSelected",
+        "Width": 16,
+        "X": 435,
+        "Y": 0
+    },
+    {
+        "Height": 12,
+        "Name": "sGUIMissileNormalGreen",
+        "Width": 16,
+        "X": 452,
         "Y": 0
     },
     {
+        "Height": 12,
+        "Name": "sGUIPBombNormalGreen",
+        "Width": 16,
+        "X": 469,
+        "Y": 0
+    },
+    {
+        "Height": 12,
+        "Name": "sGUIMissileNormal",
+        "Width": 16,
+        "X": 486,
+        "Y": 0
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogDNA",
+        "Width": 149,
+        "X": 503,
+        "Y": 0
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogDNA1",
+        "Width": 149,
+        "X": 653,
+        "Y": 0
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogDNA5",
+        "Width": 149,
+        "X": 803,
+        "Y": 0
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogDNA2",
+        "Width": 149,
+        "X": 0,
+        "Y": 137
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogDNA3",
+        "Width": 149,
+        "X": 150,
+        "Y": 137
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogDNA0",
+        "Width": 149,
+        "X": 300,
+        "Y": 137
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogIce",
+        "Width": 149,
+        "X": 450,
+        "Y": 137
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogDNA6",
+        "Width": 149,
+        "X": 600,
+        "Y": 137
+    },
+    {
+        "Height": 137,
+        "Name": "bgLogDNA4",
+        "Width": 149,
+        "X": 750,
+        "Y": 137
+    },
+    {
+        "Height": 96,
+        "Name": "tlWarpDepthsEntrance",
+        "Width": 64,
+        "X": 900,
+        "Y": 137
+    },
+    {
+        "Height": 14,
+        "Name": "bg_MapBottom2",
+        "Width": 320,
+        "X": 0,
+        "Y": 275
+    },
+    {
+        "Height": 8,
+        "Name": "sDisconnected",
+        "Width": 8,
+        "X": 321,
+        "Y": 275
+    },
+    {
+        "Height": 96,
+        "Name": "tlWarpHideout",
+        "Width": 64,
+        "X": 330,
+        "Y": 275
+    },
+    {
+        "Height": 160,
+        "Name": "tlDoorsExtended",
+        "Width": 224,
+        "X": 395,
+        "Y": 275
+    },
+    {
+        "Height": 96,
+        "Name": "tlWarpWaterfall",
+        "Width": 64,
+        "X": 620,
+        "Y": 275
+    },
+    {
+        "Height": 8,
+        "Name": "sMapHint",
+        "Width": 8,
+        "X": 685,
+        "Y": 275
+    },
+    {
+        "Height": 96,
+        "Name": "tlWarpDepthsExit",
+        "Width": 64,
+        "X": 694,
+        "Y": 275
+    },
+    {
+        "Height": 64,
+        "Name": "newA4Doors",
+        "Width": 48,
+        "X": 759,
+        "Y": 275
+    },
+    {
+        "Height": 24,
+        "Name": "bgGUIMetCountBG2ELM",
+        "Width": 17,
+        "X": 808,
+        "Y": 275
+    },
+    {
+        "Height": 24,
+        "Name": "bgGUIMetCountBG2",
+        "Width": 17,
+        "X": 826,
+        "Y": 275
+    },
+    {
+        "Height": 64,
+        "Name": "newA4Doors2",
+        "Width": 48,
+        "X": 844,
+        "Y": 275
+    },
+    {
         "Height": 16,
-        "Name": "sItemMorphBall_2",
+        "Name": "sItemSMissileLauncher_7",
+        "Width": 16,
+        "X": 893,
+        "Y": 275
+    },
+    {
+        "Height": 16,
+        "Name": "sItemSMissileLauncher_3",
+        "Width": 16,
+        "X": 910,
+        "Y": 275
+    },
+    {
+        "Height": 16,
+        "Name": "sItemSMissileLauncher_9",
+        "Width": 16,
+        "X": 927,
+        "Y": 275
+    },
+    {
+        "Height": 16,
+        "Name": "sItemSMissileLauncher_8",
+        "Width": 16,
+        "X": 944,
+        "Y": 275
+    },
+    {
+        "Height": 16,
+        "Name": "sItemSMissileLauncher_4",
+        "Width": 16,
+        "X": 961,
+        "Y": 275
+    },
+    {
+        "Height": 16,
+        "Name": "sItemSMissileLauncher_10",
+        "Width": 16,
+        "X": 978,
+        "Y": 275
+    },
+    {
+        "Height": 16,
+        "Name": "sItemSMissileLauncher_6",
+        "Width": 16,
+        "X": 995,
+        "Y": 275
+    },
+    {
+        "Height": 16,
+        "Name": "sItemSMissileLauncher_11",
+        "Width": 16,
+        "X": 0,
+        "Y": 435
+    },
+    {
+        "Height": 16,
+        "Name": "sItemSMissileLauncher_2",
         "Width": 16,
         "X": 17,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_12",
+        "Name": "sItemSMissileLauncher_12",
         "Width": 16,
         "X": 34,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_5",
+        "Name": "sItemSMissileLauncher_1",
         "Width": 16,
         "X": 51,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_9",
+        "Name": "sItemSMissileLauncher_5",
         "Width": 16,
         "X": 68,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_1",
+        "Name": "sItemIBJ_13",
         "Width": 16,
         "X": 85,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_14",
+        "Name": "sItemIBJ_14",
         "Width": 16,
         "X": 102,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_8",
+        "Name": "sItemIBJ_36",
         "Width": 16,
         "X": 119,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_16",
+        "Name": "sItemIBJ_25",
         "Width": 16,
         "X": 136,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_15",
+        "Name": "sItemIBJ_22",
         "Width": 16,
         "X": 153,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_6",
+        "Name": "sItemIBJ_17",
         "Width": 16,
         "X": 170,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_10",
+        "Name": "sItemIBJ_21",
         "Width": 16,
         "X": 187,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_11",
+        "Name": "sItemIBJ_1",
         "Width": 16,
         "X": 204,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_13",
+        "Name": "sItemIBJ_2",
         "Width": 16,
         "X": 221,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_4",
+        "Name": "sItemIBJ_37",
         "Width": 16,
         "X": 238,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBall_7",
+        "Name": "sItemIBJ_16",
         "Width": 16,
         "X": 255,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_13",
+        "Name": "sItemIBJ_3",
         "Width": 16,
         "X": 272,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_12",
+        "Name": "sItemIBJ_27",
         "Width": 16,
         "X": 289,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_2",
+        "Name": "sItemIBJ_4",
         "Width": 16,
         "X": 306,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_9",
+        "Name": "sItemIBJ_11",
         "Width": 16,
         "X": 323,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_18",
+        "Name": "sItemIBJ_28",
         "Width": 16,
         "X": 340,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_6",
+        "Name": "sItemIBJ_9",
         "Width": 16,
         "X": 357,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_16",
+        "Name": "sItemIBJ_10",
         "Width": 16,
         "X": 374,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_17",
+        "Name": "sItemIBJ_32",
         "Width": 16,
         "X": 391,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_7",
+        "Name": "sItemIBJ_35",
         "Width": 16,
         "X": 408,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_4",
+        "Name": "sItemIBJ_15",
         "Width": 16,
         "X": 425,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_5",
+        "Name": "sItemIBJ_33",
         "Width": 16,
         "X": 442,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_3",
+        "Name": "sItemIBJ_38",
         "Width": 16,
         "X": 459,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_15",
+        "Name": "sItemIBJ_18",
         "Width": 16,
         "X": 476,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_11",
+        "Name": "sItemIBJ_31",
         "Width": 16,
         "X": 493,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_10",
+        "Name": "sItemIBJ_7",
         "Width": 16,
         "X": 510,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_8",
+        "Name": "sItemIBJ_26",
         "Width": 16,
         "X": 527,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_14",
+        "Name": "sItemIBJ_30",
         "Width": 16,
         "X": 544,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttacker_1",
+        "Name": "sItemIBJ_19",
         "Width": 16,
         "X": 561,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMissileDrop_4",
+        "Name": "sItemIBJ_6",
         "Width": 16,
         "X": 578,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMissileDrop_3",
+        "Name": "sItemIBJ_0",
         "Width": 16,
         "X": 595,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMissileDrop_1",
+        "Name": "sItemIBJ_20",
         "Width": 16,
         "X": 612,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemMissileDrop_2",
+        "Name": "sItemIBJ_34",
         "Width": 16,
         "X": 629,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemShinyNothing_8",
+        "Name": "sItemIBJ_5",
         "Width": 16,
         "X": 646,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemShinyNothing_7",
+        "Name": "sItemIBJ_29",
         "Width": 16,
         "X": 663,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemShinyNothing_1",
+        "Name": "sItemIBJ_8",
         "Width": 16,
         "X": 680,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemShinyNothing_5",
+        "Name": "sItemIBJ_23",
         "Width": 16,
         "X": 697,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemShinyNothing_6",
+        "Name": "sItemIBJ_12",
         "Width": 16,
         "X": 714,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemShinyNothing_3",
+        "Name": "sItemIBJ_24",
         "Width": 16,
         "X": 731,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemShinyNothing_4",
+        "Name": "sItemShinyHijump_1",
         "Width": 16,
         "X": 748,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemShinyNothing_2",
+        "Name": "sItemShinyHijump_2",
         "Width": 16,
         "X": 765,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemPBombDrop_3",
+        "Name": "sItemShinyHijump_3",
         "Width": 16,
         "X": 782,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemPBombDrop_2",
+        "Name": "sItemShinyHijump_4",
         "Width": 16,
         "X": 799,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemPBombDrop_4",
+        "Name": "sItemSmallHealthDrop_3",
         "Width": 16,
         "X": 816,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemPBombDrop_1",
+        "Name": "sItemSmallHealthDrop_1",
         "Width": 16,
         "X": 833,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_5",
+        "Name": "sItemSmallHealthDrop_4",
         "Width": 16,
         "X": 850,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_1",
+        "Name": "sItemSmallHealthDrop_2",
         "Width": 16,
         "X": 867,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_8",
+        "Name": "sItemNothing_2",
         "Width": 16,
         "X": 884,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_3",
+        "Name": "sItemNothing_1",
         "Width": 16,
         "X": 901,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_4",
+        "Name": "sItemNothing_3",
         "Width": 16,
         "X": 918,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_6",
+        "Name": "sItemNothing_4",
         "Width": 16,
         "X": 935,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_2",
+        "Name": "sItemUnknown_4",
         "Width": 16,
         "X": 952,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_9",
+        "Name": "sItemUnknown_1",
         "Width": 16,
         "X": 969,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemDNA_7",
+        "Name": "sItemUnknown_2",
         "Width": 16,
         "X": 986,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgrade_3",
+        "Name": "sItemUnknown_3",
         "Width": 16,
         "X": 1003,
-        "Y": 0
+        "Y": 435
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgrade_1",
+        "Name": "sItemBigHealthDrop_3",
         "Width": 16,
         "X": 0,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgrade_4",
+        "Name": "sItemBigHealthDrop_4",
         "Width": 16,
         "X": 17,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgrade_7",
+        "Name": "sItemBigHealthDrop_1",
         "Width": 16,
         "X": 34,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgrade_2",
+        "Name": "sItemBigHealthDrop_2",
         "Width": 16,
         "X": 51,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgrade_5",
+        "Name": "sItemShinyIceBeam_2",
         "Width": 16,
         "X": 68,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgrade_8",
+        "Name": "sItemShinyIceBeam_3",
         "Width": 16,
         "X": 85,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgrade_6",
+        "Name": "sItemShinyIceBeam_1",
         "Width": 16,
         "X": 102,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuit_3",
+        "Name": "sItemShinyIceBeam_4",
         "Width": 16,
         "X": 119,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuit_1",
+        "Name": "sItemLongBeam_3",
         "Width": 16,
         "X": 136,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuit_2",
+        "Name": "sItemLongBeam_1",
         "Width": 16,
         "X": 153,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuit_4",
+        "Name": "sItemLongBeam_4",
         "Width": 16,
         "X": 170,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemShinyMissile_4",
+        "Name": "sItemLongBeam_2",
         "Width": 16,
         "X": 187,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemShinyMissile_1",
+        "Name": "sItemProgressiveJump_4",
         "Width": 16,
         "X": 204,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemShinyMissile_2",
+        "Name": "sItemProgressiveJump_2",
         "Width": 16,
         "X": 221,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemShinyMissile_3",
+        "Name": "sItemProgressiveJump_3",
         "Width": 16,
         "X": 238,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemUnknown_4",
+        "Name": "sItemProgressiveJump_1",
         "Width": 16,
         "X": 255,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemUnknown_2",
+        "Name": "sItemFlashlight_1",
         "Width": 16,
         "X": 272,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemUnknown_1",
+        "Name": "sItemFlashlight_2",
         "Width": 16,
         "X": 289,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemUnknown_3",
+        "Name": "sItemFlashlight_5",
         "Width": 16,
         "X": 306,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemBigHealthDrop_1",
+        "Name": "sItemFlashlight_9",
         "Width": 16,
         "X": 323,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemBigHealthDrop_2",
+        "Name": "sItemFlashlight_10",
         "Width": 16,
         "X": 340,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemBigHealthDrop_3",
+        "Name": "sItemFlashlight_3",
         "Width": 16,
         "X": 357,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemBigHealthDrop_4",
+        "Name": "sItemFlashlight_7",
         "Width": 16,
         "X": 374,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_2",
+        "Name": "sItemFlashlight_8",
         "Width": 16,
         "X": 391,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_1",
+        "Name": "sItemFlashlight_4",
         "Width": 16,
         "X": 408,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_9",
+        "Name": "sItemFlashlight_6",
         "Width": 16,
         "X": 425,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_5",
+        "Name": "sItemShinyMissile_4",
         "Width": 16,
         "X": 442,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_7",
+        "Name": "sItemShinyMissile_2",
         "Width": 16,
         "X": 459,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_6",
+        "Name": "sItemShinyMissile_1",
         "Width": 16,
         "X": 476,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_11",
+        "Name": "sItemShinyMissile_3",
         "Width": 16,
         "X": 493,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_12",
+        "Name": "sItemSMissileDrop_4",
         "Width": 16,
         "X": 510,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_4",
+        "Name": "sItemSMissileDrop_3",
         "Width": 16,
         "X": 527,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_8",
+        "Name": "sItemSMissileDrop_1",
         "Width": 16,
         "X": 544,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_10",
+        "Name": "sItemSMissileDrop_2",
         "Width": 16,
         "X": 561,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileLauncher_3",
+        "Name": "sItemMissileDrop_4",
         "Width": 16,
         "X": 578,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemShinyIceBeam_1",
+        "Name": "sItemMissileDrop_2",
         "Width": 16,
         "X": 595,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemShinyIceBeam_4",
+        "Name": "sItemMissileDrop_3",
         "Width": 16,
         "X": 612,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemShinyIceBeam_3",
+        "Name": "sItemMissileDrop_1",
         "Width": 16,
         "X": 629,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemShinyIceBeam_2",
+        "Name": "sItemScrewAttacker_6",
         "Width": 16,
         "X": 646,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPowergrip_2",
+        "Name": "sItemScrewAttacker_1",
         "Width": 16,
         "X": 663,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPowergrip_1",
+        "Name": "sItemScrewAttacker_14",
         "Width": 16,
         "X": 680,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPowergrip_4",
+        "Name": "sItemScrewAttacker_5",
         "Width": 16,
         "X": 697,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPowergrip_3",
+        "Name": "sItemScrewAttacker_9",
         "Width": 16,
         "X": 714,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileDrop_2",
+        "Name": "sItemScrewAttacker_4",
         "Width": 16,
         "X": 731,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileDrop_4",
+        "Name": "sItemScrewAttacker_7",
         "Width": 16,
         "X": 748,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileDrop_1",
+        "Name": "sItemScrewAttacker_15",
         "Width": 16,
         "X": 765,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemSMissileDrop_3",
+        "Name": "sItemScrewAttacker_11",
         "Width": 16,
         "X": 782,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemBlindfold_4",
+        "Name": "sItemScrewAttacker_3",
         "Width": 16,
         "X": 799,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemBlindfold_2",
+        "Name": "sItemScrewAttacker_18",
         "Width": 16,
         "X": 816,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemBlindfold_1",
+        "Name": "sItemScrewAttacker_12",
         "Width": 16,
         "X": 833,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemBlindfold_3",
+        "Name": "sItemScrewAttacker_8",
         "Width": 16,
         "X": 850,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_3",
+        "Name": "sItemScrewAttacker_10",
         "Width": 16,
         "X": 867,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_1",
+        "Name": "sItemScrewAttacker_2",
         "Width": 16,
         "X": 884,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_12",
+        "Name": "sItemScrewAttacker_16",
         "Width": 16,
         "X": 901,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_8",
+        "Name": "sItemScrewAttacker_17",
         "Width": 16,
         "X": 918,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_5",
+        "Name": "sItemScrewAttacker_13",
         "Width": 16,
         "X": 935,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_9",
+        "Name": "sItemPBombDrop_3",
         "Width": 16,
         "X": 952,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_4",
+        "Name": "sItemPBombDrop_2",
         "Width": 16,
         "X": 969,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_2",
+        "Name": "sItemPBombDrop_1",
         "Width": 16,
         "X": 986,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_11",
+        "Name": "sItemPBombDrop_4",
         "Width": 16,
         "X": 1003,
-        "Y": 16
+        "Y": 452
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_10",
+        "Name": "sItemProgressiveSuit_3",
         "Width": 16,
         "X": 0,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_6",
+        "Name": "sItemProgressiveSuit_1",
         "Width": 16,
         "X": 17,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemPBombLauncher_7",
+        "Name": "sItemProgressiveSuit_2",
         "Width": 16,
         "X": 34,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemSmallHealthDrop_2",
+        "Name": "sItemProgressiveSuit_4",
         "Width": 16,
         "X": 51,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemSmallHealthDrop_1",
+        "Name": "sItemDNA_9",
         "Width": 16,
         "X": 68,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemSmallHealthDrop_4",
+        "Name": "sItemDNA_4",
         "Width": 16,
         "X": 85,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemSmallHealthDrop_3",
+        "Name": "sItemDNA_5",
         "Width": 16,
         "X": 102,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemShinyHijump_2",
+        "Name": "sItemDNA_1",
         "Width": 16,
         "X": 119,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemShinyHijump_1",
+        "Name": "sItemDNA_8",
         "Width": 16,
         "X": 136,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemShinyHijump_3",
+        "Name": "sItemDNA_2",
         "Width": 16,
         "X": 153,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemShinyHijump_4",
+        "Name": "sItemDNA_3",
         "Width": 16,
         "X": 170,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_10",
+        "Name": "sItemDNA_6",
         "Width": 16,
         "X": 187,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_7",
+        "Name": "sItemDNA_7",
         "Width": 16,
         "X": 204,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_4",
+        "Name": "sItemShinyNothing_8",
         "Width": 16,
         "X": 221,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_6",
+        "Name": "sItemShinyNothing_7",
         "Width": 16,
         "X": 238,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_2",
+        "Name": "sItemShinyNothing_5",
         "Width": 16,
         "X": 255,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_1",
+        "Name": "sItemShinyNothing_4",
         "Width": 16,
         "X": 272,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_9",
+        "Name": "sItemShinyNothing_3",
         "Width": 16,
         "X": 289,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_5",
+        "Name": "sItemShinyNothing_6",
         "Width": 16,
         "X": 306,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_8",
+        "Name": "sItemShinyNothing_2",
         "Width": 16,
         "X": 323,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemFlashlight_3",
+        "Name": "sItemShinyNothing_1",
         "Width": 16,
         "X": 340,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveJump_2",
+        "Name": "sItemPBombLauncher_2",
         "Width": 16,
         "X": 357,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveJump_3",
+        "Name": "sItemPBombLauncher_8",
         "Width": 16,
         "X": 374,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveJump_1",
+        "Name": "sItemPBombLauncher_7",
         "Width": 16,
         "X": 391,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveJump_4",
+        "Name": "sItemPBombLauncher_5",
         "Width": 16,
         "X": 408,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_11",
+        "Name": "sItemPBombLauncher_4",
         "Width": 16,
         "X": 425,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_3",
+        "Name": "sItemPBombLauncher_11",
         "Width": 16,
         "X": 442,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_6",
+        "Name": "sItemPBombLauncher_3",
         "Width": 16,
         "X": 459,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_7",
+        "Name": "sItemPBombLauncher_10",
         "Width": 16,
         "X": 476,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_5",
+        "Name": "sItemPBombLauncher_12",
         "Width": 16,
         "X": 493,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_12",
+        "Name": "sItemPBombLauncher_6",
         "Width": 16,
         "X": 510,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_9",
+        "Name": "sItemPBombLauncher_1",
         "Width": 16,
         "X": 527,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_2",
+        "Name": "sItemPBombLauncher_9",
         "Width": 16,
         "X": 544,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_4",
+        "Name": "sItemBlindfold_1",
         "Width": 16,
         "X": 561,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_10",
+        "Name": "sItemBlindfold_4",
         "Width": 16,
         "X": 578,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_8",
+        "Name": "sItemBlindfold_2",
         "Width": 16,
         "X": 595,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncher_1",
+        "Name": "sItemBlindfold_3",
         "Width": 16,
         "X": 612,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemNothing_4",
+        "Name": "sItemPowergrip_1",
         "Width": 16,
         "X": 629,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemNothing_2",
+        "Name": "sItemPowergrip_4",
         "Width": 16,
         "X": 646,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemNothing_1",
+        "Name": "sItemPowergrip_3",
         "Width": 16,
         "X": 663,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sItemNothing_3",
+        "Name": "sItemPowergrip_2",
         "Width": 16,
         "X": 680,
-        "Y": 33
+        "Y": 469
     },
     {
-        "Height": 21,
-        "Name": "sAutoadPClaw",
-        "Width": 12,
+        "Height": 16,
+        "Name": "sItemSpeedBoosterUpgrade_2",
+        "Width": 16,
         "X": 697,
-        "Y": 33
+        "Y": 469
     },
     {
         "Height": 16,
-        "Name": "sAutoadPFang",
-        "Width": 15,
-        "X": 710,
-        "Y": 33
-    },
-    {
-        "Height": 22,
-        "Name": "sAutoadP",
-        "Width": 33,
-        "X": 726,
-        "Y": 33
-    },
-    {
-        "Height": 35,
-        "Name": "sWisdomSeptogg_2",
-        "Width": 47,
-        "X": 760,
-        "Y": 33
-    },
-    {
-        "Height": 35,
-        "Name": "sWisdomSeptogg_4",
-        "Width": 47,
-        "X": 808,
-        "Y": 33
+        "Name": "sItemSpeedBoosterUpgrade_6",
+        "Width": 16,
+        "X": 714,
+        "Y": 469
     },
     {
-        "Height": 35,
-        "Name": "sWisdomSeptogg_3",
-        "Width": 47,
-        "X": 856,
-        "Y": 33
+        "Height": 16,
+        "Name": "sItemSpeedBoosterUpgrade_8",
+        "Width": 16,
+        "X": 731,
+        "Y": 469
     },
     {
-        "Height": 35,
-        "Name": "sWisdomSeptogg_1",
-        "Width": 47,
-        "X": 904,
-        "Y": 33
+        "Height": 16,
+        "Name": "sItemSpeedBoosterUpgrade_4",
+        "Width": 16,
+        "X": 748,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUIMissileNormal",
+        "Height": 16,
+        "Name": "sItemSpeedBoosterUpgrade_7",
         "Width": 16,
-        "X": 952,
-        "Y": 33
+        "X": 765,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUIMissileSelected",
+        "Height": 16,
+        "Name": "sItemSpeedBoosterUpgrade_5",
         "Width": 16,
-        "X": 969,
-        "Y": 33
+        "X": 782,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUISMissileNormalGreen",
+        "Height": 16,
+        "Name": "sItemSpeedBoosterUpgrade_1",
         "Width": 16,
-        "X": 986,
-        "Y": 33
+        "X": 799,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUISMissileNormal",
+        "Height": 16,
+        "Name": "sItemSpeedBoosterUpgrade_3",
         "Width": 16,
-        "X": 1003,
-        "Y": 33
+        "X": 816,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUIMissileNormalGreen",
+        "Height": 16,
+        "Name": "sItemMissileLauncher_3",
         "Width": 16,
-        "X": 0,
-        "Y": 68
+        "X": 833,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUIPBombNormal",
+        "Height": 16,
+        "Name": "sItemMissileLauncher_7",
         "Width": 16,
-        "X": 17,
-        "Y": 68
+        "X": 850,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUIPBombSelected",
+        "Height": 16,
+        "Name": "sItemMissileLauncher_5",
         "Width": 16,
-        "X": 34,
-        "Y": 68
+        "X": 867,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUISMissileSelected",
+        "Height": 16,
+        "Name": "sItemMissileLauncher_10",
         "Width": 16,
-        "X": 51,
-        "Y": 68
+        "X": 884,
+        "Y": 469
     },
     {
-        "Height": 12,
-        "Name": "sGUIPBombNormalGreen",
+        "Height": 16,
+        "Name": "sItemMissileLauncher_1",
         "Width": 16,
-        "X": 68,
-        "Y": 68
+        "X": 901,
+        "Y": 469
     },
     {
-        "Height": 137,
-        "Name": "bgLogDNA2",
-        "Width": 149,
-        "X": 85,
-        "Y": 68
+        "Height": 16,
+        "Name": "sItemMissileLauncher_4",
+        "Width": 16,
+        "X": 918,
+        "Y": 469
     },
     {
-        "Height": 137,
-        "Name": "bgLogDNA3",
-        "Width": 149,
-        "X": 235,
-        "Y": 68
+        "Height": 16,
+        "Name": "sItemMissileLauncher_9",
+        "Width": 16,
+        "X": 935,
+        "Y": 469
     },
     {
-        "Height": 137,
-        "Name": "bgLogIce",
-        "Width": 149,
-        "X": 385,
-        "Y": 68
+        "Height": 16,
+        "Name": "sItemMissileLauncher_11",
+        "Width": 16,
+        "X": 952,
+        "Y": 469
     },
     {
-        "Height": 137,
-        "Name": "bgLogDNA5",
-        "Width": 149,
-        "X": 535,
-        "Y": 68
+        "Height": 16,
+        "Name": "sItemMissileLauncher_12",
+        "Width": 16,
+        "X": 969,
+        "Y": 469
     },
     {
-        "Height": 137,
-        "Name": "bgLogDNA4",
-        "Width": 149,
-        "X": 685,
-        "Y": 68
+        "Height": 16,
+        "Name": "sItemMissileLauncher_6",
+        "Width": 16,
+        "X": 986,
+        "Y": 469
     },
     {
-        "Height": 137,
-        "Name": "bgLogDNA6",
-        "Width": 149,
-        "X": 835,
-        "Y": 68
+        "Height": 16,
+        "Name": "sItemMissileLauncher_2",
+        "Width": 16,
+        "X": 1003,
+        "Y": 469
     },
     {
-        "Height": 137,
-        "Name": "bgLogDNA1",
-        "Width": 149,
+        "Height": 16,
+        "Name": "sItemMissileLauncher_8",
+        "Width": 16,
         "X": 0,
-        "Y": 205
-    },
-    {
-        "Height": 137,
-        "Name": "bgLogDNA",
-        "Width": 149,
-        "X": 150,
-        "Y": 205
-    },
-    {
-        "Height": 137,
-        "Name": "bgLogDNA0",
-        "Width": 149,
-        "X": 300,
-        "Y": 205
-    },
-    {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_7",
-        "Width": 8,
-        "X": 450,
-        "Y": 205
-    },
-    {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_2",
-        "Width": 8,
-        "X": 459,
-        "Y": 205
-    },
-    {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_1",
-        "Width": 4,
-        "X": 468,
-        "Y": 205
-    },
-    {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_6",
-        "Width": 8,
-        "X": 473,
-        "Y": 205
+        "Y": 486
     },
     {
-        "Height": 8,
-        "Name": "sMapBlockUnexplored",
-        "Width": 8,
-        "X": 482,
-        "Y": 205
-    },
-    {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_4",
-        "Width": 8,
-        "X": 491,
-        "Y": 205
-    },
-    {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_9",
-        "Width": 8,
-        "X": 500,
-        "Y": 205
-    },
-    {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_8",
-        "Width": 8,
-        "X": 509,
-        "Y": 205
+        "Height": 16,
+        "Name": "sItemMorphBall_13",
+        "Width": 16,
+        "X": 17,
+        "Y": 486
     },
     {
-        "Height": 4,
-        "Name": "sMapCornerUnexplored_0",
-        "Width": 8,
-        "X": 518,
-        "Y": 205
+        "Height": 16,
+        "Name": "sItemMorphBall_9",
+        "Width": 16,
+        "X": 34,
+        "Y": 486
     },
     {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_3",
-        "Width": 8,
-        "X": 527,
-        "Y": 205
+        "Height": 16,
+        "Name": "sItemMorphBall_3",
+        "Width": 16,
+        "X": 51,
+        "Y": 486
     },
     {
-        "Height": 8,
-        "Name": "sMapCornerUnexplored_5",
-        "Width": 8,
-        "X": 536,
-        "Y": 205
+        "Height": 16,
+        "Name": "sItemMorphBall_8",
+        "Width": 16,
+        "X": 68,
+        "Y": 486
     },
     {
-        "Height": 24,
-        "Name": "bgGUIMetCountBG2",
-        "Width": 17,
-        "X": 545,
-        "Y": 205
+        "Height": 16,
+        "Name": "sItemMorphBall_15",
+        "Width": 16,
+        "X": 85,
+        "Y": 486
     },
     {
-        "Height": 14,
-        "Name": "bg_MapBottom2",
-        "Width": 320,
-        "X": 563,
-        "Y": 205
+        "Height": 16,
+        "Name": "sItemMorphBall_10",
+        "Width": 16,
+        "X": 102,
+        "Y": 486
     },
     {
-        "Height": 96,
-        "Name": "tlWarpDepthsExit",
-        "Width": 64,
-        "X": 884,
-        "Y": 205
+        "Height": 16,
+        "Name": "sItemMorphBall_14",
+        "Width": 16,
+        "X": 119,
+        "Y": 486
     },
     {
-        "Height": 96,
-        "Name": "tlWarpWaterfall",
-        "Width": 64,
-        "X": 949,
-        "Y": 205
+        "Height": 16,
+        "Name": "sItemMorphBall_1",
+        "Width": 16,
+        "X": 136,
+        "Y": 486
     },
     {
-        "Height": 96,
-        "Name": "tlWarpDepthsEntrance",
-        "Width": 64,
-        "X": 0,
-        "Y": 343
+        "Height": 16,
+        "Name": "sItemMorphBall_7",
+        "Width": 16,
+        "X": 153,
+        "Y": 486
     },
     {
-        "Height": 24,
-        "Name": "bgGUIMetCountBG2ELM",
-        "Width": 17,
-        "X": 65,
-        "Y": 343
+        "Height": 16,
+        "Name": "sItemMorphBall_5",
+        "Width": 16,
+        "X": 170,
+        "Y": 486
     },
     {
-        "Height": 8,
-        "Name": "sDisconnected",
-        "Width": 8,
-        "X": 83,
-        "Y": 343
+        "Height": 16,
+        "Name": "sItemMorphBall_6",
+        "Width": 16,
+        "X": 187,
+        "Y": 486
     },
     {
-        "Height": 64,
-        "Name": "newA4Doors2",
-        "Width": 48,
-        "X": 92,
-        "Y": 343
+        "Height": 16,
+        "Name": "sItemMorphBall_11",
+        "Width": 16,
+        "X": 204,
+        "Y": 486
     },
     {
-        "Height": 8,
-        "Name": "sMapHint",
-        "Width": 8,
-        "X": 141,
-        "Y": 343
+        "Height": 16,
+        "Name": "sItemMorphBall_16",
+        "Width": 16,
+        "X": 221,
+        "Y": 486
     },
     {
-        "Height": 96,
-        "Name": "tlWarpHideout",
-        "Width": 64,
-        "X": 150,
-        "Y": 343
+        "Height": 16,
+        "Name": "sItemMorphBall_12",
+        "Width": 16,
+        "X": 238,
+        "Y": 486
     },
     {
-        "Height": 64,
-        "Name": "newA4Doors",
-        "Width": 48,
-        "X": 215,
-        "Y": 343
+        "Height": 16,
+        "Name": "sItemMorphBall_2",
+        "Width": 16,
+        "X": 255,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemETankDread_4",
+        "Name": "sItemMorphBall_4",
         "Width": 16,
-        "X": 264,
-        "Y": 343
+        "X": 272,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemETankDread_3",
+        "Name": "sItemWallJump_3",
         "Width": 16,
-        "X": 281,
-        "Y": 343
+        "X": 289,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemETankDread_1",
+        "Name": "sItemWallJump_0",
         "Width": 16,
-        "X": 298,
-        "Y": 343
+        "X": 306,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemETankDread_2",
+        "Name": "sItemWallJump_1",
         "Width": 16,
-        "X": 315,
-        "Y": 343
+        "X": 323,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_12",
+        "Name": "sItemWallJump_2",
         "Width": 16,
-        "X": 332,
-        "Y": 343
+        "X": 340,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_8",
+        "Name": "sItemPhaseDriftMSR_4",
         "Width": 16,
-        "X": 349,
-        "Y": 343
+        "X": 357,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_6",
+        "Name": "sItemPhaseDriftMSR_3",
         "Width": 16,
-        "X": 366,
-        "Y": 343
+        "X": 374,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_10",
+        "Name": "sItemPhaseDriftMSR_1",
         "Width": 16,
-        "X": 383,
-        "Y": 343
+        "X": 391,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_17",
+        "Name": "sItemPhaseDriftMSR_2",
         "Width": 16,
-        "X": 400,
-        "Y": 343
+        "X": 408,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_13",
+        "Name": "sItemBabyMetroidMSR_1",
         "Width": 16,
-        "X": 417,
-        "Y": 343
+        "X": 425,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_4",
+        "Name": "sItemBabyMetroidMSR_8",
         "Width": 16,
-        "X": 434,
-        "Y": 343
+        "X": 442,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_19",
+        "Name": "sItemBabyMetroidMSR_3",
         "Width": 16,
-        "X": 451,
-        "Y": 343
+        "X": 459,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_5",
+        "Name": "sItemBabyMetroidMSR_4",
         "Width": 16,
-        "X": 468,
-        "Y": 343
+        "X": 476,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_2",
+        "Name": "sItemBabyMetroidMSR_7",
         "Width": 16,
-        "X": 485,
-        "Y": 343
+        "X": 493,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_7",
+        "Name": "sItemBabyMetroidMSR_6",
         "Width": 16,
-        "X": 502,
-        "Y": 343
+        "X": 510,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_20",
+        "Name": "sItemBabyMetroidMSR_5",
         "Width": 16,
-        "X": 519,
-        "Y": 343
+        "X": 527,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_1",
+        "Name": "sItemBabyMetroidMSR_2",
         "Width": 16,
-        "X": 536,
-        "Y": 343
+        "X": 544,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_18",
+        "Name": "sItemLightningArmorMSR_2",
         "Width": 16,
-        "X": 553,
-        "Y": 343
+        "X": 561,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_16",
+        "Name": "sItemLightningArmorMSR_1",
         "Width": 16,
-        "X": 570,
-        "Y": 343
+        "X": 578,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_11",
+        "Name": "sItemLightningArmorMSR_4",
         "Width": 16,
-        "X": 587,
-        "Y": 343
+        "X": 595,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_15",
+        "Name": "sItemLightningArmorMSR_3",
         "Width": 16,
-        "X": 604,
-        "Y": 343
+        "X": 612,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_3",
+        "Name": "sItemBeamBurstMSR_2",
         "Width": 16,
-        "X": 621,
-        "Y": 343
+        "X": 629,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_14",
+        "Name": "sItemBeamBurstMSR_1",
         "Width": 16,
-        "X": 638,
-        "Y": 343
+        "X": 646,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderMagnetDread_9",
+        "Name": "sItemBeamBurstMSR_3",
         "Width": 16,
-        "X": 655,
-        "Y": 343
+        "X": 663,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemWideBeamDread_2",
+        "Name": "sItemBeamBurstMSR_4",
         "Width": 16,
-        "X": 672,
-        "Y": 343
+        "X": 680,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemWideBeamDread_1",
+        "Name": "sItemSpiderBallMSR_4",
         "Width": 16,
-        "X": 689,
-        "Y": 343
+        "X": 697,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemWideBeamDread_3",
+        "Name": "sItemSpiderBallMSR_2",
         "Width": 16,
-        "X": 706,
-        "Y": 343
+        "X": 714,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemWideBeamDread_0",
+        "Name": "sItemSpiderBallMSR_1",
         "Width": 16,
-        "X": 723,
-        "Y": 343
+        "X": 731,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_9",
+        "Name": "sItemSpiderBallMSR_3",
         "Width": 16,
-        "X": 740,
-        "Y": 343
+        "X": 748,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_1",
+        "Name": "sItemScanPulseMSR_3",
         "Width": 16,
-        "X": 757,
-        "Y": 343
+        "X": 765,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_7",
+        "Name": "sItemScanPulseMSR_2",
         "Width": 16,
-        "X": 774,
-        "Y": 343
+        "X": 782,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_14",
+        "Name": "sItemScanPulseMSR_1",
         "Width": 16,
-        "X": 791,
-        "Y": 343
+        "X": 799,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_6",
+        "Name": "sItemScanPulseMSR_4",
         "Width": 16,
-        "X": 808,
-        "Y": 343
+        "X": 816,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_4",
+        "Name": "sItemSpaceJumpDread_2",
         "Width": 16,
-        "X": 825,
-        "Y": 343
+        "X": 833,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_10",
+        "Name": "sItemSpaceJumpDread_1",
         "Width": 16,
-        "X": 842,
-        "Y": 343
+        "X": 850,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_8",
+        "Name": "sItemSpaceJumpDread_0",
         "Width": 16,
-        "X": 859,
-        "Y": 343
+        "X": 867,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_5",
+        "Name": "sItemSpaceJumpDread_3",
         "Width": 16,
-        "X": 876,
-        "Y": 343
+        "X": 884,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_11",
+        "Name": "sItemMorphBallDread_12",
         "Width": 16,
-        "X": 893,
-        "Y": 343
+        "X": 901,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_0",
+        "Name": "sItemMorphBallDread_6",
         "Width": 16,
-        "X": 910,
-        "Y": 343
+        "X": 918,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_3",
+        "Name": "sItemMorphBallDread_14",
         "Width": 16,
-        "X": 927,
-        "Y": 343
+        "X": 935,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_12",
+        "Name": "sItemMorphBallDread_10",
         "Width": 16,
-        "X": 944,
-        "Y": 343
+        "X": 952,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_13",
+        "Name": "sItemMorphBallDread_7",
         "Width": 16,
-        "X": 961,
-        "Y": 343
+        "X": 969,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_15",
+        "Name": "sItemMorphBallDread_13",
         "Width": 16,
-        "X": 978,
-        "Y": 343
+        "X": 986,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterUpgradeDread_2",
+        "Name": "sItemMorphBallDread_16",
         "Width": 16,
-        "X": 995,
-        "Y": 343
+        "X": 1003,
+        "Y": 486
     },
     {
         "Height": 16,
-        "Name": "sItemPulseRadarDread_0",
+        "Name": "sItemMorphBallDread_2",
         "Width": 16,
         "X": 0,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPulseRadarDread_2",
+        "Name": "sItemMorphBallDread_11",
         "Width": 16,
         "X": 17,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPulseRadarDread_3",
+        "Name": "sItemMorphBallDread_9",
         "Width": 16,
         "X": 34,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPulseRadarDread_7",
+        "Name": "sItemMorphBallDread_4",
         "Width": 16,
         "X": 51,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPulseRadarDread_5",
+        "Name": "sItemMorphBallDread_3",
         "Width": 16,
         "X": 68,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPulseRadarDread_6",
+        "Name": "sItemMorphBallDread_15",
         "Width": 16,
         "X": 85,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPulseRadarDread_1",
+        "Name": "sItemMorphBallDread_8",
         "Width": 16,
         "X": 102,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPulseRadarDread_4",
+        "Name": "sItemMorphBallDread_5",
         "Width": 16,
         "X": 119,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_1",
+        "Name": "sItemMorphBallDread_1",
         "Width": 16,
         "X": 136,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_3",
+        "Name": "sItemETankDread_2",
         "Width": 16,
         "X": 153,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_2",
+        "Name": "sItemETankDread_3",
         "Width": 16,
         "X": 170,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_5",
+        "Name": "sItemETankDread_1",
         "Width": 16,
         "X": 187,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_8",
+        "Name": "sItemETankDread_4",
         "Width": 16,
         "X": 204,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_0",
+        "Name": "sItemSuperMissileLauncherDread_6",
         "Width": 16,
         "X": 221,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_6",
+        "Name": "sItemSuperMissileLauncherDread_7",
         "Width": 16,
         "X": 238,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_7",
+        "Name": "sItemSuperMissileLauncherDread_5",
         "Width": 16,
         "X": 255,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitDread_4",
+        "Name": "sItemSuperMissileLauncherDread_8",
         "Width": 16,
         "X": 272,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankPlusDread_3",
+        "Name": "sItemSuperMissileLauncherDread_1",
         "Width": 16,
         "X": 289,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankPlusDread_2",
+        "Name": "sItemSuperMissileLauncherDread_3",
         "Width": 16,
         "X": 306,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankPlusDread_4",
+        "Name": "sItemSuperMissileLauncherDread_2",
         "Width": 16,
         "X": 323,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankPlusDread_1",
+        "Name": "sItemSuperMissileLauncherDread_4",
         "Width": 16,
         "X": 340,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankPlusDread_6",
+        "Name": "sItemStormMissilesDread_16",
         "Width": 16,
         "X": 357,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankPlusDread_0",
+        "Name": "sItemStormMissilesDread_5",
         "Width": 16,
         "X": 374,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankPlusDread_7",
+        "Name": "sItemStormMissilesDread_15",
         "Width": 16,
         "X": 391,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankPlusDread_5",
+        "Name": "sItemStormMissilesDread_2",
         "Width": 16,
         "X": 408,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileLauncherDread_6",
+        "Name": "sItemStormMissilesDread_12",
         "Width": 16,
         "X": 425,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileLauncherDread_8",
+        "Name": "sItemStormMissilesDread_8",
         "Width": 16,
         "X": 442,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileLauncherDread_1",
+        "Name": "sItemStormMissilesDread_3",
         "Width": 16,
         "X": 459,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileLauncherDread_4",
+        "Name": "sItemStormMissilesDread_13",
         "Width": 16,
         "X": 476,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileLauncherDread_7",
+        "Name": "sItemStormMissilesDread_14",
         "Width": 16,
         "X": 493,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileLauncherDread_3",
+        "Name": "sItemStormMissilesDread_1",
         "Width": 16,
         "X": 510,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileLauncherDread_5",
+        "Name": "sItemStormMissilesDread_6",
         "Width": 16,
         "X": 527,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileLauncherDread_2",
+        "Name": "sItemStormMissilesDread_9",
         "Width": 16,
         "X": 544,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_6",
+        "Name": "sItemStormMissilesDread_4",
         "Width": 16,
         "X": 561,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_5",
+        "Name": "sItemStormMissilesDread_11",
         "Width": 16,
         "X": 578,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_3",
+        "Name": "sItemStormMissilesDread_10",
         "Width": 16,
         "X": 595,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_11",
+        "Name": "sItemStormMissilesDread_7",
         "Width": 16,
         "X": 612,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_7",
+        "Name": "sItemSpinBoostDread_13",
         "Width": 16,
         "X": 629,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_12",
+        "Name": "sItemSpinBoostDread_3",
         "Width": 16,
         "X": 646,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_8",
+        "Name": "sItemSpinBoostDread_1",
         "Width": 16,
         "X": 663,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_4",
+        "Name": "sItemSpinBoostDread_16",
         "Width": 16,
         "X": 680,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_9",
+        "Name": "sItemSpinBoostDread_7",
         "Width": 16,
         "X": 697,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_2",
+        "Name": "sItemSpinBoostDread_12",
         "Width": 16,
         "X": 714,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_10",
+        "Name": "sItemSpinBoostDread_17",
         "Width": 16,
         "X": 731,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemCrossBombsDread_1",
+        "Name": "sItemSpinBoostDread_2",
         "Width": 16,
         "X": 748,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSpaceJumpDread_3",
+        "Name": "sItemSpinBoostDread_5",
         "Width": 16,
         "X": 765,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSpaceJumpDread_1",
+        "Name": "sItemSpinBoostDread_19",
         "Width": 16,
         "X": 782,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSpaceJumpDread_0",
+        "Name": "sItemSpinBoostDread_10",
         "Width": 16,
         "X": 799,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemSpaceJumpDread_2",
+        "Name": "sItemSpinBoostDread_9",
         "Width": 16,
         "X": 816,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemFlashShiftDread_3",
+        "Name": "sItemSpinBoostDread_11",
         "Width": 16,
         "X": 833,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemFlashShiftDread_5",
+        "Name": "sItemSpinBoostDread_4",
         "Width": 16,
         "X": 850,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemFlashShiftDread_4",
+        "Name": "sItemSpinBoostDread_20",
         "Width": 16,
         "X": 867,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemFlashShiftDread_7",
+        "Name": "sItemSpinBoostDread_15",
         "Width": 16,
         "X": 884,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemFlashShiftDread_6",
+        "Name": "sItemSpinBoostDread_18",
         "Width": 16,
         "X": 901,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemFlashShiftDread_1",
+        "Name": "sItemSpinBoostDread_8",
         "Width": 16,
         "X": 918,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemFlashShiftDread_0",
+        "Name": "sItemSpinBoostDread_14",
         "Width": 16,
         "X": 935,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemFlashShiftDread_2",
+        "Name": "sItemSpinBoostDread_6",
         "Width": 16,
         "X": 952,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombTankDread_2",
+        "Name": "sItemEPartDread_3",
         "Width": 16,
         "X": 969,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombTankDread_6",
+        "Name": "sItemEPartDread_2",
         "Width": 16,
         "X": 986,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombTankDread_4",
+        "Name": "sItemEPartDread_1",
         "Width": 16,
         "X": 1003,
-        "Y": 440
+        "Y": 503
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombTankDread_5",
+        "Name": "sItemEPartDread_4",
         "Width": 16,
         "X": 0,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombTankDread_3",
+        "Name": "sItemMissileTankPlusDread_6",
         "Width": 16,
         "X": 17,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombTankDread_1",
+        "Name": "sItemMissileTankPlusDread_1",
         "Width": 16,
         "X": 34,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombTankDread_0",
+        "Name": "sItemMissileTankPlusDread_4",
         "Width": 16,
         "X": 51,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombTankDread_7",
+        "Name": "sItemMissileTankPlusDread_7",
         "Width": 16,
         "X": 68,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_4",
+        "Name": "sItemMissileTankPlusDread_0",
         "Width": 16,
         "X": 85,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_7",
+        "Name": "sItemMissileTankPlusDread_5",
         "Width": 16,
         "X": 102,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_2",
+        "Name": "sItemMissileTankPlusDread_2",
         "Width": 16,
         "X": 119,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_13",
+        "Name": "sItemMissileTankPlusDread_3",
         "Width": 16,
         "X": 136,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_14",
+        "Name": "sItemVariaSuitDread_0",
         "Width": 16,
         "X": 153,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_3",
+        "Name": "sItemVariaSuitDread_1",
         "Width": 16,
         "X": 170,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_17",
+        "Name": "sItemVariaSuitDread_2",
         "Width": 16,
         "X": 187,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_8",
+        "Name": "sItemVariaSuitDread_3",
         "Width": 16,
         "X": 204,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_6",
+        "Name": "sItemVariaSuitDread_5",
         "Width": 16,
         "X": 221,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_1",
+        "Name": "sItemVariaSuitDread_6",
         "Width": 16,
         "X": 238,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_15",
+        "Name": "sItemVariaSuitDread_8",
         "Width": 16,
         "X": 255,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_9",
+        "Name": "sItemVariaSuitDread_4",
         "Width": 16,
         "X": 272,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_10",
+        "Name": "sItemVariaSuitDread_7",
         "Width": 16,
         "X": 289,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_16",
+        "Name": "sItemMissileTankDread_7",
         "Width": 16,
         "X": 306,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_11",
+        "Name": "sItemMissileTankDread_6",
         "Width": 16,
         "X": 323,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_18",
+        "Name": "sItemMissileTankDread_0",
         "Width": 16,
         "X": 340,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_12",
+        "Name": "sItemMissileTankDread_4",
         "Width": 16,
         "X": 357,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_19",
+        "Name": "sItemMissileTankDread_1",
         "Width": 16,
         "X": 374,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpeedBoosterDread_5",
+        "Name": "sItemMissileTankDread_2",
         "Width": 16,
         "X": 391,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankDread_0",
+        "Name": "sItemMissileTankDread_5",
         "Width": 16,
         "X": 408,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankDread_1",
+        "Name": "sItemMissileTankDread_3",
         "Width": 16,
         "X": 425,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankDread_7",
+        "Name": "sItemWideBeamDread_0",
         "Width": 16,
         "X": 442,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankDread_5",
+        "Name": "sItemWideBeamDread_2",
         "Width": 16,
         "X": 459,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankDread_6",
+        "Name": "sItemWideBeamDread_3",
         "Width": 16,
         "X": 476,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankDread_4",
+        "Name": "sItemWideBeamDread_1",
         "Width": 16,
         "X": 493,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankDread_3",
+        "Name": "sItemGrappleBeamDread_12",
         "Width": 16,
         "X": 510,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemMissileTankDread_2",
+        "Name": "sItemGrappleBeamDread_13",
         "Width": 16,
         "X": 527,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_3",
+        "Name": "sItemGrappleBeamDread_15",
         "Width": 16,
         "X": 544,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_12",
+        "Name": "sItemGrappleBeamDread_8",
         "Width": 16,
         "X": 561,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_6",
+        "Name": "sItemGrappleBeamDread_14",
         "Width": 16,
         "X": 578,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_16",
+        "Name": "sItemGrappleBeamDread_6",
         "Width": 16,
         "X": 595,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_13",
+        "Name": "sItemGrappleBeamDread_1",
         "Width": 16,
         "X": 612,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_20",
+        "Name": "sItemGrappleBeamDread_7",
         "Width": 16,
         "X": 629,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_5",
+        "Name": "sItemGrappleBeamDread_3",
         "Width": 16,
         "X": 646,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_2",
+        "Name": "sItemGrappleBeamDread_11",
         "Width": 16,
         "X": 663,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_17",
+        "Name": "sItemGrappleBeamDread_9",
         "Width": 16,
         "X": 680,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_8",
+        "Name": "sItemGrappleBeamDread_10",
         "Width": 16,
         "X": 697,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_9",
+        "Name": "sItemGrappleBeamDread_16",
         "Width": 16,
         "X": 714,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_15",
+        "Name": "sItemGrappleBeamDread_5",
         "Width": 16,
         "X": 731,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_7",
+        "Name": "sItemGrappleBeamDread_2",
         "Width": 16,
         "X": 748,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_1",
+        "Name": "sItemGrappleBeamDread_4",
         "Width": 16,
         "X": 765,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_4",
+        "Name": "sItemPulseRadarDread_3",
         "Width": 16,
         "X": 782,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_18",
+        "Name": "sItemPulseRadarDread_0",
         "Width": 16,
         "X": 799,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_14",
+        "Name": "sItemPulseRadarDread_4",
         "Width": 16,
         "X": 816,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_19",
+        "Name": "sItemPulseRadarDread_5",
         "Width": 16,
         "X": 833,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_11",
+        "Name": "sItemPulseRadarDread_2",
         "Width": 16,
         "X": 850,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemSpinBoostDread_10",
+        "Name": "sItemPulseRadarDread_7",
         "Width": 16,
         "X": 867,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPhantomCloakDread_3",
+        "Name": "sItemPulseRadarDread_6",
         "Width": 16,
         "X": 884,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPhantomCloakDread_4",
+        "Name": "sItemPulseRadarDread_1",
         "Width": 16,
         "X": 901,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPhantomCloakDread_0",
+        "Name": "sItemSpeedBoosterUpgradeDread_3",
         "Width": 16,
         "X": 918,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPhantomCloakDread_6",
+        "Name": "sItemSpeedBoosterUpgradeDread_4",
         "Width": 16,
         "X": 935,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPhantomCloakDread_1",
+        "Name": "sItemSpeedBoosterUpgradeDread_7",
         "Width": 16,
         "X": 952,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPhantomCloakDread_5",
+        "Name": "sItemSpeedBoosterUpgradeDread_2",
         "Width": 16,
         "X": 969,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPhantomCloakDread_7",
+        "Name": "sItemSpeedBoosterUpgradeDread_1",
         "Width": 16,
         "X": 986,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPhantomCloakDread_2",
+        "Name": "sItemSpeedBoosterUpgradeDread_10",
         "Width": 16,
         "X": 1003,
-        "Y": 457
+        "Y": 520
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_5",
+        "Name": "sItemSpeedBoosterUpgradeDread_11",
         "Width": 16,
         "X": 0,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_7",
+        "Name": "sItemSpeedBoosterUpgradeDread_0",
         "Width": 16,
         "X": 17,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_0",
+        "Name": "sItemSpeedBoosterUpgradeDread_14",
         "Width": 16,
         "X": 34,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_12",
+        "Name": "sItemSpeedBoosterUpgradeDread_12",
         "Width": 16,
         "X": 51,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_6",
+        "Name": "sItemSpeedBoosterUpgradeDread_5",
         "Width": 16,
         "X": 68,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_14",
+        "Name": "sItemSpeedBoosterUpgradeDread_13",
         "Width": 16,
         "X": 85,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_8",
+        "Name": "sItemSpeedBoosterUpgradeDread_15",
         "Width": 16,
         "X": 102,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_10",
+        "Name": "sItemSpeedBoosterUpgradeDread_8",
         "Width": 16,
         "X": 119,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_13",
+        "Name": "sItemSpeedBoosterUpgradeDread_6",
         "Width": 16,
         "X": 136,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_9",
+        "Name": "sItemSpeedBoosterUpgradeDread_9",
         "Width": 16,
         "X": 153,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_2",
+        "Name": "sItemSpeedBoosterDread_11",
         "Width": 16,
         "X": 170,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_4",
+        "Name": "sItemSpeedBoosterDread_8",
         "Width": 16,
         "X": 187,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_1",
+        "Name": "sItemSpeedBoosterDread_13",
         "Width": 16,
         "X": 204,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_15",
+        "Name": "sItemSpeedBoosterDread_12",
         "Width": 16,
         "X": 221,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_11",
+        "Name": "sItemSpeedBoosterDread_3",
         "Width": 16,
         "X": 238,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherDread_3",
+        "Name": "sItemSpeedBoosterDread_9",
         "Width": 16,
         "X": 255,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_12",
+        "Name": "sItemSpeedBoosterDread_5",
         "Width": 16,
         "X": 272,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_4",
+        "Name": "sItemSpeedBoosterDread_10",
         "Width": 16,
         "X": 289,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_5",
+        "Name": "sItemSpeedBoosterDread_2",
         "Width": 16,
         "X": 306,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_15",
+        "Name": "sItemSpeedBoosterDread_4",
         "Width": 16,
         "X": 323,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_9",
+        "Name": "sItemSpeedBoosterDread_1",
         "Width": 16,
         "X": 340,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_3",
+        "Name": "sItemSpeedBoosterDread_15",
         "Width": 16,
         "X": 357,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_11",
+        "Name": "sItemSpeedBoosterDread_14",
         "Width": 16,
         "X": 374,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_13",
+        "Name": "sItemSpeedBoosterDread_19",
         "Width": 16,
         "X": 391,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_8",
+        "Name": "sItemSpeedBoosterDread_17",
         "Width": 16,
         "X": 408,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_10",
+        "Name": "sItemSpeedBoosterDread_6",
         "Width": 16,
         "X": 425,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_1",
+        "Name": "sItemSpeedBoosterDread_18",
         "Width": 16,
         "X": 442,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_6",
+        "Name": "sItemSpeedBoosterDread_7",
         "Width": 16,
         "X": 459,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_16",
+        "Name": "sItemSpeedBoosterDread_16",
         "Width": 16,
         "X": 476,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_14",
+        "Name": "sItemCrossBombsDread_12",
         "Width": 16,
         "X": 493,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_2",
+        "Name": "sItemCrossBombsDread_7",
         "Width": 16,
         "X": 510,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamDread_7",
+        "Name": "sItemCrossBombsDread_9",
         "Width": 16,
         "X": 527,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemDiffusionBeamDread_1",
+        "Name": "sItemCrossBombsDread_1",
         "Width": 16,
         "X": 544,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemDiffusionBeamDread_2",
+        "Name": "sItemCrossBombsDread_6",
         "Width": 16,
         "X": 561,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemDiffusionBeamDread_4",
+        "Name": "sItemCrossBombsDread_11",
         "Width": 16,
         "X": 578,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemDiffusionBeamDread_3",
+        "Name": "sItemCrossBombsDread_2",
         "Width": 16,
         "X": 595,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_15",
+        "Name": "sItemCrossBombsDread_5",
         "Width": 16,
         "X": 612,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_1",
+        "Name": "sItemCrossBombsDread_8",
         "Width": 16,
         "X": 629,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_6",
+        "Name": "sItemCrossBombsDread_10",
         "Width": 16,
         "X": 646,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_12",
+        "Name": "sItemCrossBombsDread_4",
         "Width": 16,
         "X": 663,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_13",
+        "Name": "sItemCrossBombsDread_3",
         "Width": 16,
         "X": 680,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_14",
+        "Name": "sItemDiffusionBeamDread_2",
         "Width": 16,
         "X": 697,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_4",
+        "Name": "sItemDiffusionBeamDread_1",
         "Width": 16,
         "X": 714,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_8",
+        "Name": "sItemDiffusionBeamDread_3",
         "Width": 16,
         "X": 731,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_3",
+        "Name": "sItemDiffusionBeamDread_4",
         "Width": 16,
         "X": 748,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_10",
+        "Name": "sItemIceMissilesDread_6",
         "Width": 16,
         "X": 765,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_11",
+        "Name": "sItemIceMissilesDread_5",
         "Width": 16,
         "X": 782,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_7",
+        "Name": "sItemIceMissilesDread_8",
         "Width": 16,
         "X": 799,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_2",
+        "Name": "sItemIceMissilesDread_3",
         "Width": 16,
         "X": 816,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_9",
+        "Name": "sItemIceMissilesDread_1",
         "Width": 16,
         "X": 833,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_5",
+        "Name": "sItemIceMissilesDread_4",
         "Width": 16,
         "X": 850,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemStormMissilesDread_16",
+        "Name": "sItemIceMissilesDread_7",
         "Width": 16,
         "X": 867,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncherDread_3",
+        "Name": "sItemIceMissilesDread_2",
         "Width": 16,
         "X": 884,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncherDread_2",
+        "Name": "sItemSpiderMagnetDread_16",
         "Width": 16,
         "X": 901,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncherDread_7",
+        "Name": "sItemSpiderMagnetDread_2",
         "Width": 16,
         "X": 918,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncherDread_0",
+        "Name": "sItemSpiderMagnetDread_10",
         "Width": 16,
         "X": 935,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncherDread_4",
+        "Name": "sItemSpiderMagnetDread_3",
         "Width": 16,
         "X": 952,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncherDread_1",
+        "Name": "sItemSpiderMagnetDread_11",
         "Width": 16,
         "X": 969,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncherDread_6",
+        "Name": "sItemSpiderMagnetDread_1",
         "Width": 16,
         "X": 986,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemMissileLauncherDread_5",
+        "Name": "sItemSpiderMagnetDread_18",
         "Width": 16,
         "X": 1003,
-        "Y": 474
+        "Y": 537
     },
     {
         "Height": 16,
-        "Name": "sItemIceMissilesDread_5",
+        "Name": "sItemSpiderMagnetDread_12",
         "Width": 16,
         "X": 0,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemIceMissilesDread_4",
+        "Name": "sItemSpiderMagnetDread_6",
         "Width": 16,
         "X": 17,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemIceMissilesDread_3",
+        "Name": "sItemSpiderMagnetDread_9",
         "Width": 16,
         "X": 34,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemIceMissilesDread_8",
+        "Name": "sItemSpiderMagnetDread_8",
         "Width": 16,
         "X": 51,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemIceMissilesDread_2",
+        "Name": "sItemSpiderMagnetDread_14",
         "Width": 16,
         "X": 68,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemIceMissilesDread_7",
+        "Name": "sItemSpiderMagnetDread_7",
         "Width": 16,
         "X": 85,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemIceMissilesDread_6",
+        "Name": "sItemSpiderMagnetDread_19",
         "Width": 16,
         "X": 102,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemIceMissilesDread_1",
+        "Name": "sItemSpiderMagnetDread_20",
         "Width": 16,
         "X": 119,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_8",
+        "Name": "sItemSpiderMagnetDread_15",
         "Width": 16,
         "X": 136,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_2",
+        "Name": "sItemSpiderMagnetDread_17",
         "Width": 16,
         "X": 153,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_1",
+        "Name": "sItemSpiderMagnetDread_5",
         "Width": 16,
         "X": 170,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_13",
+        "Name": "sItemSpiderMagnetDread_4",
         "Width": 16,
         "X": 187,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_6",
+        "Name": "sItemSpiderMagnetDread_13",
         "Width": 16,
         "X": 204,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_15",
+        "Name": "sItemPowerBombLauncherDread_8",
         "Width": 16,
         "X": 221,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_16",
+        "Name": "sItemPowerBombLauncherDread_12",
         "Width": 16,
         "X": 238,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_3",
+        "Name": "sItemPowerBombLauncherDread_5",
         "Width": 16,
         "X": 255,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_11",
+        "Name": "sItemPowerBombLauncherDread_2",
         "Width": 16,
         "X": 272,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_9",
+        "Name": "sItemPowerBombLauncherDread_15",
         "Width": 16,
         "X": 289,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_4",
+        "Name": "sItemPowerBombLauncherDread_7",
         "Width": 16,
         "X": 306,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_7",
+        "Name": "sItemPowerBombLauncherDread_9",
         "Width": 16,
         "X": 323,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_14",
+        "Name": "sItemPowerBombLauncherDread_0",
         "Width": 16,
         "X": 340,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_5",
+        "Name": "sItemPowerBombLauncherDread_11",
         "Width": 16,
         "X": 357,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_12",
+        "Name": "sItemPowerBombLauncherDread_10",
         "Width": 16,
         "X": 374,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallDread_10",
+        "Name": "sItemPowerBombLauncherDread_13",
         "Width": 16,
         "X": 391,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemEPartDread_3",
+        "Name": "sItemPowerBombLauncherDread_14",
         "Width": 16,
         "X": 408,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemEPartDread_4",
+        "Name": "sItemPowerBombLauncherDread_1",
         "Width": 16,
         "X": 425,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemEPartDread_2",
+        "Name": "sItemPowerBombLauncherDread_3",
         "Width": 16,
         "X": 442,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemEPartDread_1",
+        "Name": "sItemPowerBombLauncherDread_4",
         "Width": 16,
         "X": 459,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemRDV_4",
+        "Name": "sItemPowerBombLauncherDread_6",
         "Width": 16,
         "X": 476,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemRDV_3",
+        "Name": "sItemMissileLauncherDread_0",
         "Width": 16,
         "X": 493,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemRDV_2",
+        "Name": "sItemMissileLauncherDread_4",
         "Width": 16,
         "X": 510,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemRDV_1",
+        "Name": "sItemMissileLauncherDread_1",
         "Width": 16,
         "X": 527,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemGenericCS_1",
+        "Name": "sItemMissileLauncherDread_2",
         "Width": 16,
         "X": 544,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemGenericCS_2",
+        "Name": "sItemMissileLauncherDread_5",
         "Width": 16,
         "X": 561,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemGenericCS_3",
+        "Name": "sItemMissileLauncherDread_7",
         "Width": 16,
         "X": 578,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemGenericCS_4",
+        "Name": "sItemMissileLauncherDread_3",
         "Width": 16,
         "X": 595,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemScanPulseMSR_2",
+        "Name": "sItemMissileLauncherDread_6",
         "Width": 16,
         "X": 612,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemScanPulseMSR_3",
+        "Name": "sItemPowerBombTankDread_0",
         "Width": 16,
         "X": 629,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemScanPulseMSR_4",
+        "Name": "sItemPowerBombTankDread_2",
         "Width": 16,
         "X": 646,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemScanPulseMSR_1",
+        "Name": "sItemPowerBombTankDread_5",
         "Width": 16,
         "X": 663,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemPhaseDriftMSR_3",
+        "Name": "sItemPowerBombTankDread_1",
         "Width": 16,
         "X": 680,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemPhaseDriftMSR_2",
+        "Name": "sItemPowerBombTankDread_4",
         "Width": 16,
         "X": 697,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemPhaseDriftMSR_4",
+        "Name": "sItemPowerBombTankDread_6",
         "Width": 16,
         "X": 714,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemPhaseDriftMSR_1",
+        "Name": "sItemPowerBombTankDread_7",
         "Width": 16,
         "X": 731,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBabyMetroidMSR_5",
+        "Name": "sItemPowerBombTankDread_3",
         "Width": 16,
         "X": 748,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBabyMetroidMSR_3",
+        "Name": "sItemFlashShiftDread_4",
         "Width": 16,
         "X": 765,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBabyMetroidMSR_4",
+        "Name": "sItemFlashShiftDread_3",
         "Width": 16,
         "X": 782,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBabyMetroidMSR_6",
+        "Name": "sItemFlashShiftDread_2",
         "Width": 16,
         "X": 799,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBabyMetroidMSR_1",
+        "Name": "sItemFlashShiftDread_0",
         "Width": 16,
         "X": 816,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBabyMetroidMSR_7",
+        "Name": "sItemFlashShiftDread_6",
         "Width": 16,
         "X": 833,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBabyMetroidMSR_8",
+        "Name": "sItemFlashShiftDread_7",
         "Width": 16,
         "X": 850,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBabyMetroidMSR_2",
+        "Name": "sItemFlashShiftDread_5",
         "Width": 16,
         "X": 867,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallMSR_4",
+        "Name": "sItemFlashShiftDread_1",
         "Width": 16,
         "X": 884,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallMSR_1",
+        "Name": "sItemPhantomCloakDread_4",
         "Width": 16,
         "X": 901,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallMSR_3",
+        "Name": "sItemPhantomCloakDread_3",
         "Width": 16,
         "X": 918,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallMSR_2",
+        "Name": "sItemPhantomCloakDread_1",
         "Width": 16,
         "X": 935,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBeamBurstMSR_1",
+        "Name": "sItemPhantomCloakDread_7",
         "Width": 16,
         "X": 952,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBeamBurstMSR_4",
+        "Name": "sItemPhantomCloakDread_2",
         "Width": 16,
         "X": 969,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBeamBurstMSR_2",
+        "Name": "sItemPhantomCloakDread_5",
         "Width": 16,
         "X": 986,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemBeamBurstMSR_3",
+        "Name": "sItemPhantomCloakDread_6",
         "Width": 16,
         "X": 1003,
-        "Y": 491
+        "Y": 554
     },
     {
         "Height": 16,
-        "Name": "sItemLightningArmorMSR_3",
+        "Name": "sItemPhantomCloakDread_0",
         "Width": 16,
         "X": 0,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemLightningArmorMSR_2",
+        "Name": "sItemGrappleBeamSuper_2",
         "Width": 16,
         "X": 17,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemLightningArmorMSR_4",
+        "Name": "sItemGrappleBeamSuper_3",
         "Width": 16,
         "X": 34,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemLightningArmorMSR_1",
+        "Name": "sItemGrappleBeamSuper_1",
         "Width": 16,
         "X": 51,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemAmberEchoes_5",
+        "Name": "sItemGrappleBeamSuper_4",
         "Width": 16,
         "X": 68,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemAmberEchoes_3",
+        "Name": "sItemGenericCS_3",
         "Width": 16,
         "X": 85,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemAmberEchoes_1",
+        "Name": "sItemGenericCS_1",
         "Width": 16,
         "X": 102,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemAmberEchoes_4",
+        "Name": "sItemGenericCS_4",
         "Width": 16,
         "X": 119,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemAmberEchoes_6",
+        "Name": "sItemGenericCS_2",
         "Width": 16,
         "X": 136,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemAmberEchoes_2",
+        "Name": "sItemMorphBallPrime_7",
         "Width": 16,
         "X": 153,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_6",
+        "Name": "sItemMorphBallPrime_8",
         "Width": 16,
         "X": 170,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_10",
+        "Name": "sItemMorphBallPrime_10",
         "Width": 16,
         "X": 187,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_11",
+        "Name": "sItemMorphBallPrime_9",
         "Width": 16,
         "X": 204,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_12",
+        "Name": "sItemMorphBallPrime_3",
         "Width": 16,
         "X": 221,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_0",
+        "Name": "sItemMorphBallPrime_2",
         "Width": 16,
         "X": 238,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_4",
+        "Name": "sItemMorphBallPrime_6",
         "Width": 16,
         "X": 255,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_5",
+        "Name": "sItemMorphBallPrime_4",
         "Width": 16,
         "X": 272,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_7",
+        "Name": "sItemMorphBallPrime_1",
         "Width": 16,
         "X": 289,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_9",
+        "Name": "sItemMorphBallPrime_5",
         "Width": 16,
         "X": 306,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_3",
+        "Name": "sItemPowerBeamPrime__2",
         "Width": 16,
         "X": 323,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_2",
+        "Name": "sItemPowerBeamPrime__6",
         "Width": 16,
         "X": 340,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_13",
+        "Name": "sItemPowerBeamPrime__1",
         "Width": 16,
         "X": 357,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_1",
+        "Name": "sItemPowerBeamPrime__3",
         "Width": 16,
         "X": 374,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSkyTempleKeyEchoes_8",
+        "Name": "sItemPowerBeamPrime__5",
         "Width": 16,
         "X": 391,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkBeamEchoes_4",
+        "Name": "sItemPowerBeamPrime__4",
         "Width": 16,
         "X": 408,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkBeamEchoes_2",
+        "Name": "sItemPowerBombLauncherPrime_6",
         "Width": 16,
         "X": 425,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkBeamEchoes_3",
+        "Name": "sItemPowerBombLauncherPrime_3",
         "Width": 16,
         "X": 442,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkBeamEchoes_1",
+        "Name": "sItemPowerBombLauncherPrime_7",
         "Width": 16,
         "X": 459,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemCobaltEchoes_1",
+        "Name": "sItemPowerBombLauncherPrime_5",
         "Width": 16,
         "X": 476,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemCobaltEchoes_6",
+        "Name": "sItemPowerBombLauncherPrime_4",
         "Width": 16,
         "X": 493,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemCobaltEchoes_3",
+        "Name": "sItemPowerBombLauncherPrime_1",
         "Width": 16,
         "X": 510,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemCobaltEchoes_5",
+        "Name": "sItemPowerBombLauncherPrime_2",
         "Width": 16,
         "X": 527,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemCobaltEchoes_2",
+        "Name": "sItemArtifactLifegiverPrime_1",
         "Width": 16,
         "X": 544,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemCobaltEchoes_4",
+        "Name": "sItemArtifactLifegiverPrime_3",
         "Width": 16,
         "X": 561,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_9",
+        "Name": "sItemArtifactLifegiverPrime_2",
         "Width": 16,
         "X": 578,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_3",
+        "Name": "sItemArtifactLifegiverPrime_4",
         "Width": 16,
         "X": 595,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_1",
+        "Name": "sItemArtifactLifegiverPrime_0",
         "Width": 16,
         "X": 612,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_4",
+        "Name": "sItemXrayVisorPrime_1",
         "Width": 16,
         "X": 629,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_12",
+        "Name": "sItemXrayVisorPrime_6",
         "Width": 16,
         "X": 646,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_6",
+        "Name": "sItemXrayVisorPrime_4",
         "Width": 16,
         "X": 663,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_11",
+        "Name": "sItemXrayVisorPrime_3",
         "Width": 16,
         "X": 680,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_10",
+        "Name": "sItemXrayVisorPrime_5",
         "Width": 16,
         "X": 697,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_2",
+        "Name": "sItemXrayVisorPrime_2",
         "Width": 16,
         "X": 714,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_5",
+        "Name": "sItemGrappleBeamPrime_4",
         "Width": 16,
         "X": 731,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_7",
+        "Name": "sItemGrappleBeamPrime_3",
         "Width": 16,
         "X": 748,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemSonicBoomEchoes_8",
+        "Name": "sItemGrappleBeamPrime_1",
         "Width": 16,
         "X": 765,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkVisorEchoes_3",
+        "Name": "sItemGrappleBeamPrime_2",
         "Width": 16,
         "X": 782,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkVisorEchoes_5",
+        "Name": "sItemWaveBeamPrime_5",
         "Width": 16,
         "X": 799,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkVisorEchoes_2",
+        "Name": "sItemWaveBeamPrime_3",
         "Width": 16,
         "X": 816,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkVisorEchoes_1",
+        "Name": "sItemWaveBeamPrime_1",
         "Width": 16,
         "X": 833,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkVisorEchoes_0",
+        "Name": "sItemWaveBeamPrime_2",
         "Width": 16,
         "X": 850,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemDarkVisorEchoes_4",
+        "Name": "sItemWaveBeamPrime_4",
         "Width": 16,
         "X": 867,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_0",
+        "Name": "sItemWaveBeamPrime_6",
         "Width": 16,
         "X": 884,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_10",
+        "Name": "sItemArtifactChozoPrime_4",
         "Width": 16,
         "X": 901,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_7",
+        "Name": "sItemArtifactChozoPrime_3",
         "Width": 16,
         "X": 918,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_11",
+        "Name": "sItemArtifactChozoPrime_2",
         "Width": 16,
         "X": 935,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_6",
+        "Name": "sItemArtifactChozoPrime_0",
         "Width": 16,
         "X": 952,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_13",
+        "Name": "sItemArtifactChozoPrime_1",
         "Width": 16,
         "X": 969,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_9",
+        "Name": "sItemArtifactElderPrime_1",
         "Width": 16,
         "X": 986,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_15",
+        "Name": "sItemArtifactElderPrime_2",
         "Width": 16,
         "X": 1003,
-        "Y": 508
+        "Y": 571
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_2",
+        "Name": "sItemArtifactElderPrime_0",
         "Width": 16,
         "X": 0,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_1",
+        "Name": "sItemArtifactElderPrime_4",
         "Width": 16,
         "X": 17,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_8",
+        "Name": "sItemArtifactElderPrime_3",
         "Width": 16,
         "X": 34,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_14",
+        "Name": "sItemArtifactPrime_2",
         "Width": 16,
         "X": 51,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_5",
+        "Name": "sItemArtifactPrime_3",
         "Width": 16,
         "X": 68,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_3",
+        "Name": "sItemArtifactPrime_1",
         "Width": 16,
         "X": 85,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_12",
+        "Name": "sItemArtifactPrime_0",
         "Width": 16,
         "X": 102,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_16",
+        "Name": "sItemArtifactPrime_4",
         "Width": 16,
         "X": 119,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_17",
+        "Name": "sItemArtifactStrengthPrime_0",
         "Width": 16,
         "X": 136,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemProgressiveSuitEchoes_4",
+        "Name": "sItemArtifactStrengthPrime_3",
         "Width": 16,
         "X": 153,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAmmoEchoes_4",
+        "Name": "sItemArtifactStrengthPrime_4",
         "Width": 16,
         "X": 170,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAmmoEchoes_3",
+        "Name": "sItemArtifactStrengthPrime_2",
         "Width": 16,
         "X": 187,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAmmoEchoes_2",
+        "Name": "sItemArtifactStrengthPrime_1",
         "Width": 16,
         "X": 204,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAmmoEchoes_1",
+        "Name": "sItemVariaSuitPrime_15",
         "Width": 16,
         "X": 221,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_8",
+        "Name": "sItemVariaSuitPrime_17",
         "Width": 16,
         "X": 238,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_13",
+        "Name": "sItemVariaSuitPrime_13",
         "Width": 16,
         "X": 255,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_11",
+        "Name": "sItemVariaSuitPrime_14",
         "Width": 16,
         "X": 272,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_3",
+        "Name": "sItemVariaSuitPrime_10",
         "Width": 16,
         "X": 289,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_1",
+        "Name": "sItemVariaSuitPrime_0",
         "Width": 16,
         "X": 306,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_7",
+        "Name": "sItemVariaSuitPrime_16",
         "Width": 16,
         "X": 323,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_12",
+        "Name": "sItemVariaSuitPrime_5",
         "Width": 16,
         "X": 340,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_0",
+        "Name": "sItemVariaSuitPrime_1",
         "Width": 16,
         "X": 357,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_6",
+        "Name": "sItemVariaSuitPrime_8",
         "Width": 16,
         "X": 374,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_5",
+        "Name": "sItemVariaSuitPrime_11",
         "Width": 16,
         "X": 391,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_10",
+        "Name": "sItemVariaSuitPrime_6",
         "Width": 16,
         "X": 408,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_4",
+        "Name": "sItemVariaSuitPrime_7",
         "Width": 16,
         "X": 425,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_2",
+        "Name": "sItemVariaSuitPrime_4",
         "Width": 16,
         "X": 442,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkTorvusKeyEchoes_9",
+        "Name": "sItemVariaSuitPrime_3",
         "Width": 16,
         "X": 459,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemVioletEchoes_6",
+        "Name": "sItemVariaSuitPrime_9",
         "Width": 16,
         "X": 476,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemVioletEchoes_4",
+        "Name": "sItemVariaSuitPrime_2",
         "Width": 16,
         "X": 493,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemVioletEchoes_3",
+        "Name": "sItemVariaSuitPrime_12",
         "Width": 16,
         "X": 510,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemVioletEchoes_2",
+        "Name": "sItemGravitySuitPrime_12",
         "Width": 16,
         "X": 527,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemVioletEchoes_1",
+        "Name": "sItemGravitySuitPrime_13",
         "Width": 16,
         "X": 544,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemVioletEchoes_5",
+        "Name": "sItemGravitySuitPrime_9",
         "Width": 16,
         "X": 561,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemSeekerMissileEchoes_3",
+        "Name": "sItemGravitySuitPrime_10",
         "Width": 16,
         "X": 578,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemSeekerMissileEchoes_4",
+        "Name": "sItemGravitySuitPrime_3",
         "Width": 16,
         "X": 595,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemSeekerMissileEchoes_1",
+        "Name": "sItemGravitySuitPrime_5",
         "Width": 16,
         "X": 612,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemSeekerMissileEchoes_2",
+        "Name": "sItemGravitySuitPrime_14",
         "Width": 16,
         "X": 629,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemLightBeamEchoes_3",
+        "Name": "sItemGravitySuitPrime_7",
         "Width": 16,
         "X": 646,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemLightBeamEchoes_2",
+        "Name": "sItemGravitySuitPrime_6",
         "Width": 16,
         "X": 663,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemLightBeamEchoes_4",
+        "Name": "sItemGravitySuitPrime_4",
         "Width": 16,
         "X": 680,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemLightBeamEchoes_1",
+        "Name": "sItemGravitySuitPrime_16",
         "Width": 16,
         "X": 697,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_4",
+        "Name": "sItemGravitySuitPrime_1",
         "Width": 16,
         "X": 714,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_2",
+        "Name": "sItemGravitySuitPrime_2",
         "Width": 16,
         "X": 731,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_3",
+        "Name": "sItemGravitySuitPrime_17",
         "Width": 16,
         "X": 748,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_7",
+        "Name": "sItemGravitySuitPrime_8",
         "Width": 16,
         "X": 765,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_11",
+        "Name": "sItemGravitySuitPrime_11",
         "Width": 16,
         "X": 782,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_5",
+        "Name": "sItemGravitySuitPrime_0",
         "Width": 16,
         "X": 799,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_10",
+        "Name": "sItemGravitySuitPrime_15",
         "Width": 16,
         "X": 816,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_0",
+        "Name": "sItemArtifactSunPrime_1",
         "Width": 16,
         "X": 833,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_12",
+        "Name": "sItemArtifactSunPrime_3",
         "Width": 16,
         "X": 850,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_17",
+        "Name": "sItemArtifactSunPrime_0",
         "Width": 16,
         "X": 867,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_1",
+        "Name": "sItemArtifactSunPrime_4",
         "Width": 16,
         "X": 884,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_16",
+        "Name": "sItemArtifactSunPrime_2",
         "Width": 16,
         "X": 901,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_15",
+        "Name": "sItemThermalVisorPrime__1",
         "Width": 16,
         "X": 918,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_8",
+        "Name": "sItemThermalVisorPrime__4",
         "Width": 16,
         "X": 935,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_9",
+        "Name": "sItemThermalVisorPrime__3",
         "Width": 16,
         "X": 952,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_14",
+        "Name": "sItemThermalVisorPrime__2",
         "Width": 16,
         "X": 969,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_13",
+        "Name": "sItemThermalVisorPrime__5",
         "Width": 16,
         "X": 986,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemDarkSuitEchoes_6",
+        "Name": "sItemThermalVisorPrime__6",
         "Width": 16,
         "X": 1003,
-        "Y": 525
+        "Y": 588
     },
     {
         "Height": 16,
-        "Name": "sItemEchoVisorEchoes_3",
+        "Name": "sItemFlamethrowerPrime_3",
         "Width": 16,
         "X": 0,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEchoVisorEchoes_0",
+        "Name": "sItemFlamethrowerPrime_2",
         "Width": 16,
         "X": 17,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEchoVisorEchoes_5",
+        "Name": "sItemFlamethrowerPrime_1",
         "Width": 16,
         "X": 34,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEchoVisorEchoes_1",
+        "Name": "sItemFlamethrowerPrime_4",
         "Width": 16,
         "X": 51,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEchoVisorEchoes_4",
+        "Name": "sItemSuperMissilePrime_2",
         "Width": 16,
         "X": 68,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEchoVisorEchoes_2",
+        "Name": "sItemSuperMissilePrime_3",
         "Width": 16,
         "X": 85,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightAmmoEchoes_4",
+        "Name": "sItemSuperMissilePrime_1",
         "Width": 16,
         "X": 102,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightAmmoEchoes_1",
+        "Name": "sItemSuperMissilePrime_4",
         "Width": 16,
         "X": 119,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightAmmoEchoes_2",
+        "Name": "sItemSpiderBallPrime_1",
         "Width": 16,
         "X": 136,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightAmmoEchoes_3",
+        "Name": "sItemSpiderBallPrime_9",
         "Width": 16,
         "X": 153,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEmeraldEchoes_4",
+        "Name": "sItemSpiderBallPrime_10",
         "Width": 16,
         "X": 170,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEmeraldEchoes_2",
+        "Name": "sItemSpiderBallPrime_13",
         "Width": 16,
         "X": 187,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEmeraldEchoes_1",
+        "Name": "sItemSpiderBallPrime_12",
         "Width": 16,
         "X": 204,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEmeraldEchoes_6",
+        "Name": "sItemSpiderBallPrime_5",
         "Width": 16,
         "X": 221,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEmeraldEchoes_5",
+        "Name": "sItemSpiderBallPrime_3",
         "Width": 16,
         "X": 238,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemEmeraldEchoes_3",
+        "Name": "sItemSpiderBallPrime_11",
         "Width": 16,
         "X": 255,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttackEchoes_1",
+        "Name": "sItemSpiderBallPrime_19",
         "Width": 16,
         "X": 272,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttackEchoes_2",
+        "Name": "sItemSpiderBallPrime_14",
         "Width": 16,
         "X": 289,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttackEchoes_4",
+        "Name": "sItemSpiderBallPrime_6",
         "Width": 16,
         "X": 306,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemScrewAttackEchoes_3",
+        "Name": "sItemSpiderBallPrime_16",
         "Width": 16,
         "X": 323,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_13",
+        "Name": "sItemSpiderBallPrime_7",
         "Width": 16,
         "X": 340,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_6",
+        "Name": "sItemSpiderBallPrime_17",
         "Width": 16,
         "X": 357,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_5",
+        "Name": "sItemSpiderBallPrime_15",
         "Width": 16,
         "X": 374,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_10",
+        "Name": "sItemSpiderBallPrime_2",
         "Width": 16,
         "X": 391,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_7",
+        "Name": "sItemSpiderBallPrime_4",
         "Width": 16,
         "X": 408,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_14",
+        "Name": "sItemSpiderBallPrime_18",
         "Width": 16,
         "X": 425,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_17",
+        "Name": "sItemSpiderBallPrime_8",
         "Width": 16,
         "X": 442,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_3",
+        "Name": "sItemSpiderBallPrime_20",
         "Width": 16,
         "X": 459,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_15",
+        "Name": "sItemWaveBusterPrime_4",
         "Width": 16,
         "X": 476,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_1",
+        "Name": "sItemWaveBusterPrime_2",
         "Width": 16,
         "X": 493,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_12",
+        "Name": "sItemWaveBusterPrime_1",
         "Width": 16,
         "X": 510,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_11",
+        "Name": "sItemWaveBusterPrime_3",
         "Width": 16,
         "X": 527,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_0",
+        "Name": "sItemPhazonSuitPrime_16",
         "Width": 16,
         "X": 544,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_16",
+        "Name": "sItemPhazonSuitPrime_10",
         "Width": 16,
         "X": 561,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_9",
+        "Name": "sItemPhazonSuitPrime_1",
         "Width": 16,
         "X": 578,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_2",
+        "Name": "sItemPhazonSuitPrime_12",
         "Width": 16,
         "X": 595,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_4",
+        "Name": "sItemPhazonSuitPrime_15",
         "Width": 16,
         "X": 612,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemLightSuitEchoes_8",
+        "Name": "sItemPhazonSuitPrime_5",
         "Width": 16,
         "X": 629,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileEchoes_0",
+        "Name": "sItemPhazonSuitPrime_8",
         "Width": 16,
         "X": 646,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileEchoes_2",
+        "Name": "sItemPhazonSuitPrime_17",
         "Width": 16,
         "X": 663,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileEchoes_3",
+        "Name": "sItemPhazonSuitPrime_11",
         "Width": 16,
         "X": 680,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissileEchoes_1",
+        "Name": "sItemPhazonSuitPrime_0",
         "Width": 16,
         "X": 697,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemAnnihilatorEchoes_0",
+        "Name": "sItemPhazonSuitPrime_7",
         "Width": 16,
         "X": 714,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemAnnihilatorEchoes_1",
+        "Name": "sItemPhazonSuitPrime_13",
         "Width": 16,
         "X": 731,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemAnnihilatorEchoes_2",
+        "Name": "sItemPhazonSuitPrime_6",
         "Width": 16,
         "X": 748,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemAnnihilatorEchoes_3",
+        "Name": "sItemPhazonSuitPrime_2",
         "Width": 16,
         "X": 765,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_2",
+        "Name": "sItemPhazonSuitPrime_3",
         "Width": 16,
         "X": 782,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_12",
+        "Name": "sItemPhazonSuitPrime_9",
         "Width": 16,
         "X": 799,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_0",
+        "Name": "sItemPhazonSuitPrime_14",
         "Width": 16,
         "X": 816,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_6",
+        "Name": "sItemPhazonSuitPrime_4",
         "Width": 16,
         "X": 833,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_9",
+        "Name": "sItemBombsPrime_1",
         "Width": 16,
         "X": 850,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_13",
+        "Name": "sItemBombsPrime_4",
         "Width": 16,
         "X": 867,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_11",
+        "Name": "sItemBombsPrime_6",
         "Width": 16,
         "X": 884,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_10",
+        "Name": "sItemBombsPrime_7",
         "Width": 16,
         "X": 901,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_1",
+        "Name": "sItemBombsPrime_2",
         "Width": 16,
         "X": 918,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_8",
+        "Name": "sItemBombsPrime_5",
         "Width": 16,
         "X": 935,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_7",
+        "Name": "sItemBombsPrime_3",
         "Width": 16,
         "X": 952,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_4",
+        "Name": "sItemScanVisorPrime__5",
         "Width": 16,
         "X": 969,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_3",
+        "Name": "sItemScanVisorPrime__6",
         "Width": 16,
         "X": 986,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemDarkAgonKeyEchoes_5",
+        "Name": "sItemScanVisorPrime__3",
         "Width": 16,
         "X": 1003,
-        "Y": 542
+        "Y": 605
     },
     {
         "Height": 16,
-        "Name": "sItemBeamAmmoEchoes_2",
+        "Name": "sItemScanVisorPrime__1",
         "Width": 16,
         "X": 0,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemBeamAmmoEchoes_3",
+        "Name": "sItemScanVisorPrime__2",
         "Width": 16,
         "X": 17,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemBeamAmmoEchoes_1",
+        "Name": "sItemScanVisorPrime__4",
         "Width": 16,
         "X": 34,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemBeamAmmoEchoes_4",
+        "Name": "sItemIceSpreaderPrime_3",
         "Width": 16,
         "X": 51,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_4",
+        "Name": "sItemIceSpreaderPrime_1",
         "Width": 16,
         "X": 68,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_11",
+        "Name": "sItemIceSpreaderPrime_2",
         "Width": 16,
         "X": 85,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_7",
+        "Name": "sItemIceSpreaderPrime_4",
         "Width": 16,
         "X": 102,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_5",
+        "Name": "sItemArtifactWildPrime_2",
         "Width": 16,
         "X": 119,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_9",
+        "Name": "sItemArtifactWildPrime_1",
         "Width": 16,
         "X": 136,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_2",
+        "Name": "sItemArtifactWildPrime_3",
         "Width": 16,
         "X": 153,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_8",
+        "Name": "sItemArtifactWildPrime_0",
         "Width": 16,
         "X": 170,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_3",
+        "Name": "sItemArtifactWildPrime_4",
         "Width": 16,
         "X": 187,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_6",
+        "Name": "sItemBoostBallPrime_10",
         "Width": 16,
         "X": 204,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_1",
+        "Name": "sItemBoostBallPrime_19",
         "Width": 16,
         "X": 221,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemCannonBallEchoes_10",
+        "Name": "sItemBoostBallPrime_9",
         "Width": 16,
         "X": 238,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_14",
+        "Name": "sItemBoostBallPrime_2",
         "Width": 16,
         "X": 255,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_11",
+        "Name": "sItemBoostBallPrime_22",
         "Width": 16,
         "X": 272,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_13",
+        "Name": "sItemBoostBallPrime_18",
         "Width": 16,
         "X": 289,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_3",
+        "Name": "sItemBoostBallPrime_6",
         "Width": 16,
         "X": 306,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_0",
+        "Name": "sItemBoostBallPrime_16",
         "Width": 16,
         "X": 323,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_17",
+        "Name": "sItemBoostBallPrime_21",
         "Width": 16,
         "X": 340,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_4",
+        "Name": "sItemBoostBallPrime_8",
         "Width": 16,
         "X": 357,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_21",
+        "Name": "sItemBoostBallPrime_12",
         "Width": 16,
         "X": 374,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_23",
+        "Name": "sItemBoostBallPrime_14",
         "Width": 16,
         "X": 391,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_22",
+        "Name": "sItemBoostBallPrime_1",
         "Width": 16,
         "X": 408,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_10",
+        "Name": "sItemBoostBallPrime_20",
         "Width": 16,
         "X": 425,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_19",
+        "Name": "sItemBoostBallPrime_11",
         "Width": 16,
         "X": 442,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_15",
+        "Name": "sItemBoostBallPrime_5",
         "Width": 16,
         "X": 459,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_9",
+        "Name": "sItemBoostBallPrime_7",
         "Width": 16,
         "X": 476,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_18",
+        "Name": "sItemBoostBallPrime_3",
         "Width": 16,
         "X": 493,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_1",
+        "Name": "sItemBoostBallPrime_4",
         "Width": 16,
         "X": 510,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_8",
+        "Name": "sItemBoostBallPrime_15",
         "Width": 16,
         "X": 527,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_7",
+        "Name": "sItemBoostBallPrime_23",
         "Width": 16,
         "X": 544,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_6",
+        "Name": "sItemBoostBallPrime_13",
         "Width": 16,
         "X": 561,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_12",
+        "Name": "sItemBoostBallPrime_17",
         "Width": 16,
         "X": 578,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_2",
+        "Name": "sItemArtifactTruthPrime_0",
         "Width": 16,
         "X": 595,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_16",
+        "Name": "sItemArtifactTruthPrime_1",
         "Width": 16,
         "X": 612,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_20",
+        "Name": "sItemArtifactTruthPrime_4",
         "Width": 16,
         "X": 629,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemDarkburstEchoes_5",
+        "Name": "sItemArtifactTruthPrime_3",
         "Width": 16,
         "X": 646,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherEchoes_1",
+        "Name": "sItemArtifactTruthPrime_2",
         "Width": 16,
         "X": 663,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherEchoes_4",
+        "Name": "sItemArtifactSpiritPrime_4",
         "Width": 16,
         "X": 680,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherEchoes_2",
+        "Name": "sItemArtifactSpiritPrime_3",
         "Width": 16,
         "X": 697,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherEchoes_3",
+        "Name": "sItemArtifactSpiritPrime_1",
         "Width": 16,
         "X": 714,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_8",
+        "Name": "sItemArtifactSpiritPrime_0",
         "Width": 16,
         "X": 731,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_4",
+        "Name": "sItemArtifactSpiritPrime_2",
         "Width": 16,
         "X": 748,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_7",
+        "Name": "sItemCombatVisorPrime_4",
         "Width": 16,
         "X": 765,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_5",
+        "Name": "sItemCombatVisorPrime_2",
         "Width": 16,
         "X": 782,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_2",
+        "Name": "sItemCombatVisorPrime_1",
         "Width": 16,
         "X": 799,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_0",
+        "Name": "sItemCombatVisorPrime_6",
         "Width": 16,
         "X": 816,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_6",
+        "Name": "sItemCombatVisorPrime_3",
         "Width": 16,
         "X": 833,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_10",
+        "Name": "sItemCombatVisorPrime_5",
         "Width": 16,
         "X": 850,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_12",
+        "Name": "sItemArtifactWorldPrime_1",
         "Width": 16,
         "X": 867,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_11",
+        "Name": "sItemArtifactWorldPrime_2",
         "Width": 16,
         "X": 884,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_9",
+        "Name": "sItemArtifactWorldPrime_0",
         "Width": 16,
         "X": 901,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_3",
+        "Name": "sItemArtifactWorldPrime_4",
         "Width": 16,
         "X": 918,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_13",
+        "Name": "sItemArtifactWorldPrime_3",
         "Width": 16,
         "X": 935,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemIngHiveKeyEchoes_1",
+        "Name": "sItemIceBeamPrime__5",
         "Width": 16,
         "X": 952,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactElderPrime_4",
+        "Name": "sItemIceBeamPrime__4",
         "Width": 16,
         "X": 969,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactElderPrime_0",
+        "Name": "sItemIceBeamPrime__3",
         "Width": 16,
         "X": 986,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactElderPrime_2",
+        "Name": "sItemIceBeamPrime__6",
         "Width": 16,
         "X": 1003,
-        "Y": 559
+        "Y": 622
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactElderPrime_1",
+        "Name": "sItemIceBeamPrime__1",
         "Width": 16,
         "X": 0,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactElderPrime_3",
+        "Name": "sItemIceBeamPrime__2",
         "Width": 16,
         "X": 17,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemScanVisorPrime__6",
+        "Name": "sItemPlasmaBeamPrime__3",
         "Width": 16,
         "X": 34,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemScanVisorPrime__5",
+        "Name": "sItemPlasmaBeamPrime__2",
         "Width": 16,
         "X": 51,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemScanVisorPrime__2",
+        "Name": "sItemPlasmaBeamPrime__1",
         "Width": 16,
         "X": 68,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemScanVisorPrime__1",
+        "Name": "sItemPlasmaBeamPrime__6",
         "Width": 16,
         "X": 85,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemScanVisorPrime__3",
+        "Name": "sItemPlasmaBeamPrime__4",
         "Width": 16,
         "X": 102,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemScanVisorPrime__4",
+        "Name": "sItemPlasmaBeamPrime__5",
         "Width": 16,
         "X": 119,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNaturePrime_4",
+        "Name": "sItemArtifactNewbornPrime_1",
         "Width": 16,
         "X": 136,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNaturePrime_3",
+        "Name": "sItemArtifactNewbornPrime_0",
         "Width": 16,
         "X": 153,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNaturePrime_2",
+        "Name": "sItemArtifactNewbornPrime_2",
         "Width": 16,
         "X": 170,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNaturePrime_1",
+        "Name": "sItemArtifactNewbornPrime_4",
         "Width": 16,
         "X": 187,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNaturePrime_0",
+        "Name": "sItemArtifactNewbornPrime_3",
         "Width": 16,
         "X": 204,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemPlasmaBeamPrime__4",
+        "Name": "sItemArtifactWarriorPrime_3",
         "Width": 16,
         "X": 221,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemPlasmaBeamPrime__6",
+        "Name": "sItemArtifactWarriorPrime_1",
         "Width": 16,
         "X": 238,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemPlasmaBeamPrime__5",
+        "Name": "sItemArtifactWarriorPrime_0",
         "Width": 16,
         "X": 255,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemPlasmaBeamPrime__3",
+        "Name": "sItemArtifactWarriorPrime_2",
         "Width": 16,
         "X": 272,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemPlasmaBeamPrime__1",
+        "Name": "sItemArtifactWarriorPrime_4",
         "Width": 16,
         "X": 289,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemPlasmaBeamPrime__2",
+        "Name": "sItemArtifactNaturePrime_2",
         "Width": 16,
         "X": 306,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_7",
+        "Name": "sItemArtifactNaturePrime_3",
         "Width": 16,
         "X": 323,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_3",
+        "Name": "sItemArtifactNaturePrime_1",
         "Width": 16,
         "X": 340,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_0",
+        "Name": "sItemArtifactNaturePrime_4",
         "Width": 16,
         "X": 357,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_4",
+        "Name": "sItemArtifactNaturePrime_0",
         "Width": 16,
         "X": 374,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_9",
+        "Name": "sItemSonicBoomEchoes_3",
         "Width": 16,
         "X": 391,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_15",
+        "Name": "sItemSonicBoomEchoes_2",
         "Width": 16,
         "X": 408,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_6",
+        "Name": "sItemSonicBoomEchoes_12",
         "Width": 16,
         "X": 425,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_1",
+        "Name": "sItemSonicBoomEchoes_8",
         "Width": 16,
         "X": 442,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_5",
+        "Name": "sItemSonicBoomEchoes_10",
         "Width": 16,
         "X": 459,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_11",
+        "Name": "sItemSonicBoomEchoes_6",
         "Width": 16,
         "X": 476,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_12",
+        "Name": "sItemSonicBoomEchoes_1",
         "Width": 16,
         "X": 493,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_16",
+        "Name": "sItemSonicBoomEchoes_5",
         "Width": 16,
         "X": 510,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_13",
+        "Name": "sItemSonicBoomEchoes_4",
         "Width": 16,
         "X": 527,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_17",
+        "Name": "sItemSonicBoomEchoes_7",
         "Width": 16,
         "X": 544,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_8",
+        "Name": "sItemSonicBoomEchoes_9",
         "Width": 16,
         "X": 561,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_14",
+        "Name": "sItemSonicBoomEchoes_11",
         "Width": 16,
         "X": 578,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_2",
+        "Name": "sItemCannonBallEchoes_5",
         "Width": 16,
         "X": 595,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGravitySuitPrime_10",
+        "Name": "sItemCannonBallEchoes_7",
         "Width": 16,
         "X": 612,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemIceSpreaderPrime_1",
+        "Name": "sItemCannonBallEchoes_2",
         "Width": 16,
         "X": 629,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemIceSpreaderPrime_2",
+        "Name": "sItemCannonBallEchoes_11",
         "Width": 16,
         "X": 646,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemIceSpreaderPrime_4",
+        "Name": "sItemCannonBallEchoes_10",
         "Width": 16,
         "X": 663,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemIceSpreaderPrime_3",
+        "Name": "sItemCannonBallEchoes_9",
         "Width": 16,
         "X": 680,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_12",
+        "Name": "sItemCannonBallEchoes_4",
         "Width": 16,
         "X": 697,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_16",
+        "Name": "sItemCannonBallEchoes_8",
         "Width": 16,
         "X": 714,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_14",
+        "Name": "sItemCannonBallEchoes_6",
         "Width": 16,
         "X": 731,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_1",
+        "Name": "sItemCannonBallEchoes_3",
         "Width": 16,
         "X": 748,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_15",
+        "Name": "sItemCannonBallEchoes_1",
         "Width": 16,
         "X": 765,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_7",
+        "Name": "sItemDarkburstEchoes_0",
         "Width": 16,
         "X": 782,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_2",
+        "Name": "sItemDarkburstEchoes_15",
         "Width": 16,
         "X": 799,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_9",
+        "Name": "sItemDarkburstEchoes_21",
         "Width": 16,
         "X": 816,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_10",
+        "Name": "sItemDarkburstEchoes_14",
         "Width": 16,
         "X": 833,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_4",
+        "Name": "sItemDarkburstEchoes_11",
         "Width": 16,
         "X": 850,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_6",
+        "Name": "sItemDarkburstEchoes_4",
         "Width": 16,
         "X": 867,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_3",
+        "Name": "sItemDarkburstEchoes_19",
         "Width": 16,
         "X": 884,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_17",
+        "Name": "sItemDarkburstEchoes_18",
         "Width": 16,
         "X": 901,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_13",
+        "Name": "sItemDarkburstEchoes_17",
         "Width": 16,
         "X": 918,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_11",
+        "Name": "sItemDarkburstEchoes_6",
         "Width": 16,
         "X": 935,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_8",
+        "Name": "sItemDarkburstEchoes_16",
         "Width": 16,
         "X": 952,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_0",
+        "Name": "sItemDarkburstEchoes_22",
         "Width": 16,
         "X": 969,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemVariaSuitPrime_5",
+        "Name": "sItemDarkburstEchoes_5",
         "Width": 16,
         "X": 986,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamPrime_3",
+        "Name": "sItemDarkburstEchoes_13",
         "Width": 16,
         "X": 1003,
-        "Y": 576
+        "Y": 639
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamPrime_1",
+        "Name": "sItemDarkburstEchoes_1",
         "Width": 16,
         "X": 0,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamPrime_4",
+        "Name": "sItemDarkburstEchoes_9",
         "Width": 16,
         "X": 17,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamPrime_2",
+        "Name": "sItemDarkburstEchoes_8",
         "Width": 16,
         "X": 34,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemIceBeamPrime__5",
+        "Name": "sItemDarkburstEchoes_7",
         "Width": 16,
         "X": 51,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemIceBeamPrime__3",
+        "Name": "sItemDarkburstEchoes_3",
         "Width": 16,
         "X": 68,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemIceBeamPrime__4",
+        "Name": "sItemDarkburstEchoes_10",
         "Width": 16,
         "X": 85,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemIceBeamPrime__6",
+        "Name": "sItemDarkburstEchoes_23",
         "Width": 16,
         "X": 102,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemIceBeamPrime__1",
+        "Name": "sItemDarkburstEchoes_2",
         "Width": 16,
         "X": 119,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemIceBeamPrime__2",
+        "Name": "sItemDarkburstEchoes_20",
         "Width": 16,
         "X": 136,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_15",
+        "Name": "sItemDarkburstEchoes_12",
         "Width": 16,
         "X": 153,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_3",
+        "Name": "sItemPowerBombLauncherEchoes_2",
         "Width": 16,
         "X": 170,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_0",
+        "Name": "sItemPowerBombLauncherEchoes_4",
         "Width": 16,
         "X": 187,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_5",
+        "Name": "sItemPowerBombLauncherEchoes_1",
         "Width": 16,
         "X": 204,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_7",
+        "Name": "sItemPowerBombLauncherEchoes_3",
         "Width": 16,
         "X": 221,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_13",
+        "Name": "sItemDarkSuitEchoes_6",
         "Width": 16,
         "X": 238,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_9",
+        "Name": "sItemDarkSuitEchoes_12",
         "Width": 16,
         "X": 255,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_11",
+        "Name": "sItemDarkSuitEchoes_2",
         "Width": 16,
         "X": 272,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_6",
+        "Name": "sItemDarkSuitEchoes_16",
         "Width": 16,
         "X": 289,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_14",
+        "Name": "sItemDarkSuitEchoes_15",
         "Width": 16,
         "X": 306,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_1",
+        "Name": "sItemDarkSuitEchoes_3",
         "Width": 16,
         "X": 323,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_4",
+        "Name": "sItemDarkSuitEchoes_13",
         "Width": 16,
         "X": 340,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_8",
+        "Name": "sItemDarkSuitEchoes_0",
         "Width": 16,
         "X": 357,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_10",
+        "Name": "sItemDarkSuitEchoes_5",
         "Width": 16,
         "X": 374,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_17",
+        "Name": "sItemDarkSuitEchoes_1",
         "Width": 16,
         "X": 391,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_16",
+        "Name": "sItemDarkSuitEchoes_7",
         "Width": 16,
         "X": 408,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_2",
+        "Name": "sItemDarkSuitEchoes_11",
         "Width": 16,
         "X": 425,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemPhazonSuitPrime_12",
+        "Name": "sItemDarkSuitEchoes_14",
         "Width": 16,
         "X": 442,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactLifegiverPrime_3",
+        "Name": "sItemDarkSuitEchoes_17",
         "Width": 16,
         "X": 459,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactLifegiverPrime_4",
+        "Name": "sItemDarkSuitEchoes_8",
         "Width": 16,
         "X": 476,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactLifegiverPrime_1",
+        "Name": "sItemDarkSuitEchoes_9",
         "Width": 16,
         "X": 493,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactLifegiverPrime_0",
+        "Name": "sItemDarkSuitEchoes_4",
         "Width": 16,
         "X": 510,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactLifegiverPrime_2",
+        "Name": "sItemDarkSuitEchoes_10",
         "Width": 16,
         "X": 527,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemCombatVisorPrime_1",
+        "Name": "sItemDarkBeamEchoes_1",
         "Width": 16,
         "X": 544,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemCombatVisorPrime_5",
+        "Name": "sItemDarkBeamEchoes_3",
         "Width": 16,
         "X": 561,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemCombatVisorPrime_2",
+        "Name": "sItemDarkBeamEchoes_2",
         "Width": 16,
         "X": 578,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemCombatVisorPrime_6",
+        "Name": "sItemDarkBeamEchoes_4",
         "Width": 16,
         "X": 595,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemCombatVisorPrime_4",
+        "Name": "sItemLightAmmoEchoes_3",
         "Width": 16,
         "X": 612,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemCombatVisorPrime_3",
+        "Name": "sItemLightAmmoEchoes_4",
         "Width": 16,
         "X": 629,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNewbornPrime_0",
+        "Name": "sItemLightAmmoEchoes_1",
         "Width": 16,
         "X": 646,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNewbornPrime_4",
+        "Name": "sItemLightAmmoEchoes_2",
         "Width": 16,
         "X": 663,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNewbornPrime_1",
+        "Name": "sItemAnnihilatorEchoes_1",
         "Width": 16,
         "X": 680,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNewbornPrime_3",
+        "Name": "sItemAnnihilatorEchoes_2",
         "Width": 16,
         "X": 697,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactNewbornPrime_2",
+        "Name": "sItemAnnihilatorEchoes_0",
         "Width": 16,
         "X": 714,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSunPrime_1",
+        "Name": "sItemAnnihilatorEchoes_3",
         "Width": 16,
         "X": 731,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSunPrime_0",
+        "Name": "sItemDarkAmmoEchoes_1",
         "Width": 16,
         "X": 748,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSunPrime_3",
+        "Name": "sItemDarkAmmoEchoes_4",
         "Width": 16,
         "X": 765,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSunPrime_4",
+        "Name": "sItemDarkAmmoEchoes_3",
         "Width": 16,
         "X": 782,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSunPrime_2",
+        "Name": "sItemDarkAmmoEchoes_2",
         "Width": 16,
         "X": 799,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactTruthPrime_3",
+        "Name": "sItemSkyTempleKeyEchoes_12",
         "Width": 16,
         "X": 816,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactTruthPrime_2",
+        "Name": "sItemSkyTempleKeyEchoes_11",
         "Width": 16,
         "X": 833,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactTruthPrime_1",
+        "Name": "sItemSkyTempleKeyEchoes_10",
         "Width": 16,
         "X": 850,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactTruthPrime_0",
+        "Name": "sItemSkyTempleKeyEchoes_13",
         "Width": 16,
         "X": 867,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactTruthPrime_4",
+        "Name": "sItemSkyTempleKeyEchoes_1",
         "Width": 16,
         "X": 884,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemFlamethrowerPrime_2",
+        "Name": "sItemSkyTempleKeyEchoes_9",
         "Width": 16,
         "X": 901,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemFlamethrowerPrime_3",
+        "Name": "sItemSkyTempleKeyEchoes_8",
         "Width": 16,
         "X": 918,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemFlamethrowerPrime_1",
+        "Name": "sItemSkyTempleKeyEchoes_5",
         "Width": 16,
         "X": 935,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemFlamethrowerPrime_4",
+        "Name": "sItemSkyTempleKeyEchoes_0",
         "Width": 16,
         "X": 952,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_14",
+        "Name": "sItemSkyTempleKeyEchoes_4",
         "Width": 16,
         "X": 969,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_1",
+        "Name": "sItemSkyTempleKeyEchoes_2",
         "Width": 16,
         "X": 986,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_15",
+        "Name": "sItemSkyTempleKeyEchoes_6",
         "Width": 16,
         "X": 1003,
-        "Y": 593
+        "Y": 656
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_11",
+        "Name": "sItemSkyTempleKeyEchoes_7",
         "Width": 16,
         "X": 0,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_7",
+        "Name": "sItemSkyTempleKeyEchoes_3",
         "Width": 16,
         "X": 17,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_12",
+        "Name": "sItemCobaltEchoes_6",
         "Width": 16,
         "X": 34,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_19",
+        "Name": "sItemCobaltEchoes_4",
         "Width": 16,
         "X": 51,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_5",
+        "Name": "sItemCobaltEchoes_2",
         "Width": 16,
         "X": 68,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_20",
+        "Name": "sItemCobaltEchoes_1",
         "Width": 16,
         "X": 85,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_13",
+        "Name": "sItemCobaltEchoes_5",
         "Width": 16,
         "X": 102,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_9",
+        "Name": "sItemCobaltEchoes_3",
         "Width": 16,
         "X": 119,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_18",
+        "Name": "sItemLightBeamEchoes_3",
         "Width": 16,
         "X": 136,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_17",
+        "Name": "sItemLightBeamEchoes_1",
         "Width": 16,
         "X": 153,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_3",
+        "Name": "sItemLightBeamEchoes_2",
         "Width": 16,
         "X": 170,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_16",
+        "Name": "sItemLightBeamEchoes_4",
         "Width": 16,
         "X": 187,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_8",
+        "Name": "sItemEmeraldEchoes_6",
         "Width": 16,
         "X": 204,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_10",
+        "Name": "sItemEmeraldEchoes_3",
         "Width": 16,
         "X": 221,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_4",
+        "Name": "sItemEmeraldEchoes_2",
         "Width": 16,
         "X": 238,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_6",
+        "Name": "sItemEmeraldEchoes_1",
         "Width": 16,
         "X": 255,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSpiderBallPrime_2",
+        "Name": "sItemEmeraldEchoes_4",
         "Width": 16,
         "X": 272,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWarriorPrime_4",
+        "Name": "sItemEmeraldEchoes_5",
         "Width": 16,
         "X": 289,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWarriorPrime_3",
+        "Name": "sItemSuperMissileEchoes_0",
         "Width": 16,
         "X": 306,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWarriorPrime_2",
+        "Name": "sItemSuperMissileEchoes_1",
         "Width": 16,
         "X": 323,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWarriorPrime_1",
+        "Name": "sItemSuperMissileEchoes_2",
         "Width": 16,
         "X": 340,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWarriorPrime_0",
+        "Name": "sItemSuperMissileEchoes_3",
         "Width": 16,
         "X": 357,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSpiritPrime_1",
+        "Name": "sItemVioletEchoes_2",
         "Width": 16,
         "X": 374,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSpiritPrime_0",
+        "Name": "sItemVioletEchoes_3",
         "Width": 16,
         "X": 391,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSpiritPrime_2",
+        "Name": "sItemVioletEchoes_1",
         "Width": 16,
         "X": 408,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSpiritPrime_4",
+        "Name": "sItemVioletEchoes_5",
         "Width": 16,
         "X": 425,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactSpiritPrime_3",
+        "Name": "sItemVioletEchoes_4",
         "Width": 16,
         "X": 442,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactPrime_1",
+        "Name": "sItemVioletEchoes_6",
         "Width": 16,
         "X": 459,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactPrime_0",
+        "Name": "sItemEchoVisorEchoes_0",
         "Width": 16,
         "X": 476,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactPrime_4",
+        "Name": "sItemEchoVisorEchoes_3",
         "Width": 16,
         "X": 493,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactPrime_2",
+        "Name": "sItemEchoVisorEchoes_2",
         "Width": 16,
         "X": 510,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactPrime_3",
+        "Name": "sItemEchoVisorEchoes_1",
         "Width": 16,
         "X": 527,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissilePrime_3",
+        "Name": "sItemEchoVisorEchoes_4",
         "Width": 16,
         "X": 544,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissilePrime_4",
+        "Name": "sItemEchoVisorEchoes_5",
         "Width": 16,
         "X": 561,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissilePrime_2",
+        "Name": "sItemAmberEchoes_1",
         "Width": 16,
         "X": 578,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemSuperMissilePrime_1",
+        "Name": "sItemAmberEchoes_4",
         "Width": 16,
         "X": 595,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBeamPrime_5",
+        "Name": "sItemAmberEchoes_6",
         "Width": 16,
         "X": 612,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBeamPrime_4",
+        "Name": "sItemAmberEchoes_5",
         "Width": 16,
         "X": 629,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBeamPrime_1",
+        "Name": "sItemAmberEchoes_3",
         "Width": 16,
         "X": 646,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBeamPrime_3",
+        "Name": "sItemAmberEchoes_2",
         "Width": 16,
         "X": 663,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBeamPrime_2",
+        "Name": "sItemScrewAttackEchoes_4",
         "Width": 16,
         "X": 680,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBeamPrime_6",
+        "Name": "sItemScrewAttackEchoes_1",
         "Width": 16,
         "X": 697,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBeamPrime__1",
+        "Name": "sItemScrewAttackEchoes_3",
         "Width": 16,
         "X": 714,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBeamPrime__4",
+        "Name": "sItemScrewAttackEchoes_2",
         "Width": 16,
         "X": 731,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBeamPrime__5",
+        "Name": "sItemIngHiveKeyEchoes_9",
         "Width": 16,
         "X": 748,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBeamPrime__2",
+        "Name": "sItemIngHiveKeyEchoes_4",
         "Width": 16,
         "X": 765,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBeamPrime__3",
+        "Name": "sItemIngHiveKeyEchoes_6",
         "Width": 16,
         "X": 782,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBeamPrime__6",
+        "Name": "sItemIngHiveKeyEchoes_7",
         "Width": 16,
         "X": 799,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemThermalVisorPrime__6",
+        "Name": "sItemIngHiveKeyEchoes_1",
         "Width": 16,
         "X": 816,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemThermalVisorPrime__2",
+        "Name": "sItemIngHiveKeyEchoes_2",
         "Width": 16,
         "X": 833,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemThermalVisorPrime__3",
+        "Name": "sItemIngHiveKeyEchoes_13",
         "Width": 16,
         "X": 850,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemThermalVisorPrime__5",
+        "Name": "sItemIngHiveKeyEchoes_8",
         "Width": 16,
         "X": 867,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemThermalVisorPrime__4",
+        "Name": "sItemIngHiveKeyEchoes_12",
         "Width": 16,
         "X": 884,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemThermalVisorPrime__1",
+        "Name": "sItemIngHiveKeyEchoes_11",
         "Width": 16,
         "X": 901,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactStrengthPrime_2",
+        "Name": "sItemIngHiveKeyEchoes_5",
         "Width": 16,
         "X": 918,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactStrengthPrime_1",
+        "Name": "sItemIngHiveKeyEchoes_3",
         "Width": 16,
         "X": 935,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactStrengthPrime_4",
+        "Name": "sItemIngHiveKeyEchoes_10",
         "Width": 16,
         "X": 952,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactStrengthPrime_0",
+        "Name": "sItemIngHiveKeyEchoes_0",
         "Width": 16,
         "X": 969,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactStrengthPrime_3",
+        "Name": "sItemBeamAmmoEchoes_1",
         "Width": 16,
         "X": 986,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWildPrime_2",
+        "Name": "sItemBeamAmmoEchoes_3",
         "Width": 16,
         "X": 1003,
-        "Y": 610
+        "Y": 673
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWildPrime_1",
+        "Name": "sItemBeamAmmoEchoes_2",
         "Width": 16,
         "X": 0,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWildPrime_4",
+        "Name": "sItemBeamAmmoEchoes_4",
         "Width": 16,
         "X": 17,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWildPrime_0",
+        "Name": "sItemDarkVisorEchoes_0",
         "Width": 16,
         "X": 34,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWildPrime_3",
+        "Name": "sItemDarkVisorEchoes_1",
         "Width": 16,
         "X": 51,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemXrayVisorPrime_5",
+        "Name": "sItemDarkVisorEchoes_4",
         "Width": 16,
         "X": 68,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemXrayVisorPrime_4",
+        "Name": "sItemDarkVisorEchoes_5",
         "Width": 16,
         "X": 85,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemXrayVisorPrime_6",
+        "Name": "sItemDarkVisorEchoes_3",
         "Width": 16,
         "X": 102,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemXrayVisorPrime_3",
+        "Name": "sItemDarkVisorEchoes_2",
         "Width": 16,
         "X": 119,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemXrayVisorPrime_2",
+        "Name": "sItemDarkAgonKeyEchoes_0",
         "Width": 16,
         "X": 136,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemXrayVisorPrime_1",
+        "Name": "sItemDarkAgonKeyEchoes_10",
         "Width": 16,
         "X": 153,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_11",
+        "Name": "sItemDarkAgonKeyEchoes_8",
         "Width": 16,
         "X": 170,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_6",
+        "Name": "sItemDarkAgonKeyEchoes_13",
         "Width": 16,
         "X": 187,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_9",
+        "Name": "sItemDarkAgonKeyEchoes_11",
         "Width": 16,
         "X": 204,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_19",
+        "Name": "sItemDarkAgonKeyEchoes_6",
         "Width": 16,
         "X": 221,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_8",
+        "Name": "sItemDarkAgonKeyEchoes_1",
         "Width": 16,
         "X": 238,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_15",
+        "Name": "sItemDarkAgonKeyEchoes_7",
         "Width": 16,
         "X": 255,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_21",
+        "Name": "sItemDarkAgonKeyEchoes_4",
         "Width": 16,
         "X": 272,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_10",
+        "Name": "sItemDarkAgonKeyEchoes_12",
         "Width": 16,
         "X": 289,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_4",
+        "Name": "sItemDarkAgonKeyEchoes_3",
         "Width": 16,
         "X": 306,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_22",
+        "Name": "sItemDarkAgonKeyEchoes_2",
         "Width": 16,
         "X": 323,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_14",
+        "Name": "sItemDarkAgonKeyEchoes_5",
         "Width": 16,
         "X": 340,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_5",
+        "Name": "sItemDarkAgonKeyEchoes_9",
         "Width": 16,
         "X": 357,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_18",
+        "Name": "sItemDarkTorvusKeyEchoes_13",
         "Width": 16,
         "X": 374,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_2",
+        "Name": "sItemDarkTorvusKeyEchoes_6",
         "Width": 16,
         "X": 391,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_16",
+        "Name": "sItemDarkTorvusKeyEchoes_5",
         "Width": 16,
         "X": 408,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_3",
+        "Name": "sItemDarkTorvusKeyEchoes_0",
         "Width": 16,
         "X": 425,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_17",
+        "Name": "sItemDarkTorvusKeyEchoes_12",
         "Width": 16,
         "X": 442,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_7",
+        "Name": "sItemDarkTorvusKeyEchoes_10",
         "Width": 16,
         "X": 459,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_12",
+        "Name": "sItemDarkTorvusKeyEchoes_1",
         "Width": 16,
         "X": 476,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_13",
+        "Name": "sItemDarkTorvusKeyEchoes_2",
         "Width": 16,
         "X": 493,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_23",
+        "Name": "sItemDarkTorvusKeyEchoes_8",
         "Width": 16,
         "X": 510,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_20",
+        "Name": "sItemDarkTorvusKeyEchoes_7",
         "Width": 16,
         "X": 527,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBoostBallPrime_1",
+        "Name": "sItemDarkTorvusKeyEchoes_9",
         "Width": 16,
         "X": 544,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherPrime_6",
+        "Name": "sItemDarkTorvusKeyEchoes_4",
         "Width": 16,
         "X": 561,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherPrime_1",
+        "Name": "sItemDarkTorvusKeyEchoes_11",
         "Width": 16,
         "X": 578,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherPrime_5",
+        "Name": "sItemDarkTorvusKeyEchoes_3",
         "Width": 16,
         "X": 595,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherPrime_4",
+        "Name": "sItemSeekerMissileEchoes_1",
         "Width": 16,
         "X": 612,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherPrime_7",
+        "Name": "sItemSeekerMissileEchoes_3",
         "Width": 16,
         "X": 629,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherPrime_2",
+        "Name": "sItemSeekerMissileEchoes_4",
         "Width": 16,
         "X": 646,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemPowerBombLauncherPrime_3",
+        "Name": "sItemSeekerMissileEchoes_2",
         "Width": 16,
         "X": 663,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBombsPrime_6",
+        "Name": "sItemProgressiveSuitEchoes_9",
         "Width": 16,
         "X": 680,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBombsPrime_3",
+        "Name": "sItemProgressiveSuitEchoes_13",
         "Width": 16,
         "X": 697,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBombsPrime_1",
+        "Name": "sItemProgressiveSuitEchoes_12",
         "Width": 16,
         "X": 714,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBombsPrime_4",
+        "Name": "sItemProgressiveSuitEchoes_1",
         "Width": 16,
         "X": 731,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBombsPrime_5",
+        "Name": "sItemProgressiveSuitEchoes_0",
         "Width": 16,
         "X": 748,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBombsPrime_2",
+        "Name": "sItemProgressiveSuitEchoes_15",
         "Width": 16,
         "X": 765,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemBombsPrime_7",
+        "Name": "sItemProgressiveSuitEchoes_11",
         "Width": 16,
         "X": 782,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBusterPrime_3",
+        "Name": "sItemProgressiveSuitEchoes_7",
         "Width": 16,
         "X": 799,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBusterPrime_2",
+        "Name": "sItemProgressiveSuitEchoes_8",
         "Width": 16,
         "X": 816,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBusterPrime_1",
+        "Name": "sItemProgressiveSuitEchoes_16",
         "Width": 16,
         "X": 833,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemWaveBusterPrime_4",
+        "Name": "sItemProgressiveSuitEchoes_4",
         "Width": 16,
         "X": 850,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_9",
+        "Name": "sItemProgressiveSuitEchoes_10",
         "Width": 16,
         "X": 867,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_1",
+        "Name": "sItemProgressiveSuitEchoes_6",
         "Width": 16,
         "X": 884,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_8",
+        "Name": "sItemProgressiveSuitEchoes_5",
         "Width": 16,
         "X": 901,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_10",
+        "Name": "sItemProgressiveSuitEchoes_3",
         "Width": 16,
         "X": 918,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_4",
+        "Name": "sItemProgressiveSuitEchoes_2",
         "Width": 16,
         "X": 935,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_3",
+        "Name": "sItemProgressiveSuitEchoes_14",
         "Width": 16,
         "X": 952,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_6",
+        "Name": "sItemProgressiveSuitEchoes_17",
         "Width": 16,
         "X": 969,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_5",
+        "Name": "sItemLightSuitEchoes_14",
         "Width": 16,
         "X": 986,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_7",
+        "Name": "sItemLightSuitEchoes_3",
         "Width": 16,
         "X": 1003,
-        "Y": 627
+        "Y": 690
     },
     {
         "Height": 16,
-        "Name": "sItemMorphBallPrime_2",
+        "Name": "sItemLightSuitEchoes_2",
         "Width": 16,
         "X": 0,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactChozoPrime_0",
+        "Name": "sItemLightSuitEchoes_0",
         "Width": 16,
         "X": 17,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactChozoPrime_2",
+        "Name": "sItemLightSuitEchoes_5",
         "Width": 16,
         "X": 34,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactChozoPrime_1",
+        "Name": "sItemLightSuitEchoes_11",
         "Width": 16,
         "X": 51,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactChozoPrime_4",
+        "Name": "sItemLightSuitEchoes_4",
         "Width": 16,
         "X": 68,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactChozoPrime_3",
+        "Name": "sItemLightSuitEchoes_9",
         "Width": 16,
         "X": 85,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWorldPrime_1",
+        "Name": "sItemLightSuitEchoes_17",
         "Width": 16,
         "X": 102,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWorldPrime_4",
+        "Name": "sItemLightSuitEchoes_15",
         "Width": 16,
         "X": 119,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWorldPrime_3",
+        "Name": "sItemLightSuitEchoes_16",
         "Width": 16,
         "X": 136,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWorldPrime_2",
+        "Name": "sItemLightSuitEchoes_10",
         "Width": 16,
         "X": 153,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemArtifactWorldPrime_0",
+        "Name": "sItemLightSuitEchoes_12",
         "Width": 16,
         "X": 170,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamSuper_1",
+        "Name": "sItemLightSuitEchoes_1",
         "Width": 16,
         "X": 187,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamSuper_3",
+        "Name": "sItemLightSuitEchoes_13",
         "Width": 16,
         "X": 204,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamSuper_4",
+        "Name": "sItemLightSuitEchoes_8",
         "Width": 16,
         "X": 221,
-        "Y": 644
+        "Y": 707
     },
     {
         "Height": 16,
-        "Name": "sItemGrappleBeamSuper_2",
+        "Name": "sItemLightSuitEchoes_6",
         "Width": 16,
         "X": 238,
-        "Y": 644
+        "Y": 707
+    },
+    {
+        "Height": 16,
+        "Name": "sItemLightSuitEchoes_7",
+        "Width": 16,
+        "X": 255,
+        "Y": 707
+    },
+    {
+        "Height": 16,
+        "Name": "sItemRDV_2",
+        "Width": 16,
+        "X": 272,
+        "Y": 707
+    },
+    {
+        "Height": 16,
+        "Name": "sItemRDV_1",
+        "Width": 16,
+        "X": 289,
+        "Y": 707
+    },
+    {
+        "Height": 16,
+        "Name": "sItemRDV_3",
+        "Width": 16,
+        "X": 306,
+        "Y": 707
+    },
+    {
+        "Height": 16,
+        "Name": "sItemRDV_4",
+        "Width": 16,
+        "X": 323,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorAnim_6",
+        "Name": "sDoorSerris",
         "Width": 10,
-        "X": 255,
-        "Y": 644
+        "X": 340,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorA5EMPRightExterior",
+        "Name": "sDoorAnim_9",
         "Width": 10,
-        "X": 266,
-        "Y": 644
+        "X": 351,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorTester",
+        "Name": "sDoorA5EMPNearPipeHub",
         "Width": 10,
-        "X": 277,
-        "Y": 644
+        "X": 362,
+        "Y": 707
     },
     {
         "Height": 64,
         "Name": "sDoorWaveBeam",
         "Width": 10,
-        "X": 288,
-        "Y": 644
+        "X": 373,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorAnim_5",
+        "Name": "sDoorSuper",
         "Width": 10,
-        "X": 299,
-        "Y": 644
+        "X": 384,
+        "Y": 707
     },
     {
         "Height": 64,
         "Name": "sDoorSpazerBeam",
         "Width": 10,
-        "X": 310,
-        "Y": 644
+        "X": 395,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorGuardian",
+        "Name": "sDoorTempLocked",
         "Width": 10,
-        "X": 321,
-        "Y": 644
+        "X": 406,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorTorizo",
+        "Name": "sDoorAnim_4",
         "Width": 10,
-        "X": 332,
-        "Y": 644
+        "X": 417,
+        "Y": 707
     },
     {
         "Height": 64,
         "Name": "sDoorGenesis",
         "Width": 10,
-        "X": 343,
-        "Y": 644
+        "X": 428,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorLocked",
+        "Name": "sDoorAnim_6",
         "Width": 10,
-        "X": 354,
-        "Y": 644
+        "X": 439,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorAnim_9",
+        "Name": "sDoorSpider",
         "Width": 10,
-        "X": 365,
-        "Y": 644
+        "X": 450,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorMissile",
+        "Name": "sDoorAnim_5",
         "Width": 10,
-        "X": 376,
-        "Y": 644
+        "X": 461,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorEMPA3",
+        "Name": "sDoorTester",
         "Width": 10,
-        "X": 387,
-        "Y": 644
+        "X": 472,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorSuper",
+        "Name": "sDoorAnim_1",
         "Width": 10,
-        "X": 398,
-        "Y": 644
+        "X": 483,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorAnim_3",
+        "Name": "sDoorEMPA1",
         "Width": 10,
-        "X": 409,
-        "Y": 644
+        "X": 494,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorAnim_8",
+        "Name": "sDoorEMPActivated",
         "Width": 10,
-        "X": 420,
-        "Y": 644
+        "X": 505,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorTempLocked",
+        "Name": "sDoorTorizo",
         "Width": 10,
-        "X": 431,
-        "Y": 644
+        "X": 516,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorA5EMPRobotHome",
+        "Name": "sDoorChargeBeam",
         "Width": 10,
-        "X": 442,
-        "Y": 644
+        "X": 527,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorA5EMPNearTotem",
+        "Name": "sDoorArachnus",
         "Width": 10,
-        "X": 453,
-        "Y": 644
+        "X": 538,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorAnim_2",
+        "Name": "sDoorEMPA3",
         "Width": 10,
-        "X": 464,
-        "Y": 644
+        "X": 549,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorPlasmaBeam",
+        "Name": "sDoorIceBeam",
         "Width": 10,
-        "X": 475,
-        "Y": 644
+        "X": 560,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorBlue",
+        "Name": "sDoorAnim_2",
         "Width": 10,
-        "X": 486,
-        "Y": 644
+        "X": 571,
+        "Y": 707
     },
     {
         "Height": 64,
         "Name": "sDoorAnim_7",
         "Width": 10,
-        "X": 497,
-        "Y": 644
+        "X": 582,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorChargeBeam",
+        "Name": "sDoorTowerEnabled",
         "Width": 10,
-        "X": 508,
-        "Y": 644
+        "X": 593,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorScrew",
+        "Name": "sDoorA5EMPRobotHome",
         "Width": 10,
-        "X": 519,
-        "Y": 644
+        "X": 604,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorA5EMPNearSave",
+        "Name": "sDoorA5EMPRightExterior",
         "Width": 10,
-        "X": 530,
-        "Y": 644
+        "X": 615,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorTowerEnabled",
+        "Name": "sDoorAnim_3",
         "Width": 10,
-        "X": 541,
-        "Y": 644
+        "X": 626,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorEMPA2",
+        "Name": "sDoorPBomb",
         "Width": 10,
-        "X": 552,
-        "Y": 644
+        "X": 637,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorA5EMPNearPipeHub",
+        "Name": "sDoorScrew",
         "Width": 10,
-        "X": 563,
-        "Y": 644
+        "X": 648,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorAnim_1",
+        "Name": "sDoorAnim_8",
         "Width": 10,
-        "X": 574,
-        "Y": 644
+        "X": 659,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorBomb",
+        "Name": "sDoorBlue",
         "Width": 10,
-        "X": 585,
-        "Y": 644
+        "X": 670,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorPBomb",
+        "Name": "sDoorPlasmaBeam",
         "Width": 10,
-        "X": 596,
-        "Y": 644
+        "X": 681,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorSpider",
+        "Name": "sDoorEMPA2",
         "Width": 10,
-        "X": 607,
-        "Y": 644
+        "X": 692,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorArachnus",
+        "Name": "sDoorQueen",
         "Width": 10,
-        "X": 618,
-        "Y": 644
+        "X": 703,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorEMPActivated",
+        "Name": "sDoorA5EMPNearBulletHell",
         "Width": 10,
-        "X": 629,
-        "Y": 644
+        "X": 714,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorSerris",
+        "Name": "sDoorA5EMPNearSave",
         "Width": 10,
-        "X": 640,
-        "Y": 644
+        "X": 725,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorAnim_4",
+        "Name": "sDoorA5EMPNearTotem",
         "Width": 10,
-        "X": 651,
-        "Y": 644
+        "X": 736,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorQueen",
+        "Name": "sDoorLocked",
         "Width": 10,
-        "X": 662,
-        "Y": 644
+        "X": 747,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorA5EMPNearBulletHell",
+        "Name": "sDoorMissile",
         "Width": 10,
-        "X": 673,
-        "Y": 644
+        "X": 758,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorEMPA1",
+        "Name": "sDoorBomb",
         "Width": 10,
-        "X": 684,
-        "Y": 644
+        "X": 769,
+        "Y": 707
     },
     {
         "Height": 64,
-        "Name": "sDoorIceBeam",
+        "Name": "sDoorGuardian",
         "Width": 10,
-        "X": 695,
-        "Y": 644
+        "X": 780,
+        "Y": 707
     }
 ]
```

### Comparing `am2r_yams-2.1.2/am2r_yams.egg-info/PKG-INFO` & `am2r_yams-2.2.0/am2r_yams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 2.1.2
+Version: 2.2.0
 Summary: An open source randomizer patcher for AM2R.
 Author: Miepee
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `am2r_yams-2.1.2/am2r_yams.egg-info/SOURCES.txt` & `am2r_yams-2.2.0/am2r_yams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.1.2/pyproject.toml` & `am2r_yams-2.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "am2r_yams"
-version = "2.1.2"
+version = "2.2.0"
 authors = [
     {name = "Miepee"},
 ]
 description = "An open source randomizer patcher for AM2R."
 readme = "README.md"
 license = {file = "LICENSE-CODE"}
 requires-python = ">=3.11"
```

