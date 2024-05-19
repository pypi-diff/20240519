# Comparing `tmp/tdrpa.tdworker-1.1.4.12-py39-none-win_amd64.whl.zip` & `tmp/tdrpa.tdworker-1.1.4.13-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 426586 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  1207808 b- defN 24-May-17 05:44 tdrpa/tdworker.cp39-win_amd64.pyd
+Zip file size: 426755 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat  1208320 b- defN 24-May-19 08:05 tdrpa/tdworker.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      167 b- defN 24-May-16 02:23 tdrpa/tdworker/__init__.pyi
 -rw-rw-rw-  2.0 fat     4254 b- defN 24-May-16 02:23 tdrpa/tdworker/_w.pyi
 -rw-rw-rw-  2.0 fat    17361 b- defN 24-May-16 02:23 tdrpa/tdworker/_winE.pyi
 -rw-rw-rw-  2.0 fat     5395 b- defN 24-May-16 02:23 tdrpa/tdworker/_winK.pyi
 -rw-rw-rw-  2.0 fat     7908 b- defN 24-May-16 02:23 tdrpa/tdworker/_winM.pyi
--rw-rw-rw-  2.0 fat      668 b- defN 24-May-17 05:44 tdrpa.tdworker-1.1.4.12.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-17 05:44 tdrpa.tdworker-1.1.4.12.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-17 05:44 tdrpa.tdworker-1.1.4.12.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      834 b- defN 24-May-17 05:44 tdrpa.tdworker-1.1.4.12.dist-info/RECORD
-10 files, 1244493 bytes uncompressed, 425162 bytes compressed:  65.8%
+-rw-rw-rw-  2.0 fat      677 b- defN 24-May-19 08:05 tdrpa.tdworker-1.1.4.13.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-19 08:05 tdrpa.tdworker-1.1.4.13.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-19 08:05 tdrpa.tdworker-1.1.4.13.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      834 b- defN 24-May-19 08:05 tdrpa.tdworker-1.1.4.13.dist-info/RECORD
+10 files, 1245014 bytes uncompressed, 425331 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: tdrpa/tdworker/_winK.pyi
 Comment: 
 
 Filename: tdrpa/tdworker/_winM.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.12.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.4.13.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.12.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.4.13.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.12.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.4.13.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.12.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.4.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tdrpa.tdworker-1.1.4.12.dist-info/METADATA` & `tdrpa.tdworker-1.1.4.13.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.4.12
+Version: 1.1.4.13
 Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: vx:RPA_CREATOR
 Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Dist: tdrpa.tdcore
+Requires-Dist: tdrpa.tdcore >=1.1.34
 Requires-Dist: pyperclip
 Requires-Dist: WMI
 Requires-Dist: pycryptodome
 
 tdworker for tdrpa developers. supports python3.8+, windows x64
```

## Comparing `tdrpa.tdworker-1.1.4.12.dist-info/RECORD` & `tdrpa.tdworker-1.1.4.13.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tdrpa/tdworker.cp39-win_amd64.pyd,sha256=fdyW0BUJaJL2wXfV6_FSMs77Ki41XYfRtXzb2dDaMn8,1207808
+tdrpa/tdworker.cp39-win_amd64.pyd,sha256=hqHTgtZG_elKjwEqlCud2tFe6jYG2_ummqO-2PODSq8,1208320
 tdrpa/tdworker/__init__.pyi,sha256=sGWR5Le0SWyHPKV5mYz_zRxr8X7zIQSF9cqOB8YUcnE,167
 tdrpa/tdworker/_w.pyi,sha256=ZXgV35kxk0kjX2mHu2vL_TnB3_5bGkacQJbnglNsRtE,4254
 tdrpa/tdworker/_winE.pyi,sha256=a2zzqjlm1HoOrZa-plIsaCKaVujz0QuC2F8H-dbv-i4,17361
 tdrpa/tdworker/_winK.pyi,sha256=22vDxBqR9ZdiUFjbtW-SZVZA2h44cOfbOZ3oX9SrDjk,5395
 tdrpa/tdworker/_winM.pyi,sha256=ifh5EvOjNCsOzsfIYvRbpyAWA1FU5lzlEPkGPbfuQgE,7908
-tdrpa.tdworker-1.1.4.12.dist-info/METADATA,sha256=WlKd-qN48JfzuMzfHfWPEUSZ40Wo3sCb2a6Ac23ASdc,668
-tdrpa.tdworker-1.1.4.12.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdworker-1.1.4.12.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdworker-1.1.4.12.dist-info/RECORD,,
+tdrpa.tdworker-1.1.4.13.dist-info/METADATA,sha256=lAaVJkzUh6bVAI3YPPBtPX3wn5WQ2tVKoVXP4u35d1k,677
+tdrpa.tdworker-1.1.4.13.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdworker-1.1.4.13.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdworker-1.1.4.13.dist-info/RECORD,,
```

