# Comparing `tmp/tdrpa.tdcore-1.1.34-py39-none-win_amd64.whl.zip` & `tmp/tdrpa.tdcore-1.1.35-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 507556 bytes, number of entries: 22
--rw-rw-rw-  2.0 fat   640512 b- defN 24-May-19 02:13 tdrpa/bot.exe
--rw-rw-rw-  2.0 fat   614400 b- defN 24-May-19 02:14 tdrpa/tdcore.cp39-win_amd64.pyd
+Zip file size: 507331 bytes, number of entries: 22
+-rw-rw-rw-  2.0 fat   640512 b- defN 24-May-19 08:38 tdrpa/bot.exe
+-rw-rw-rw-  2.0 fat   612864 b- defN 24-May-19 08:39 tdrpa/tdcore.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      340 b- defN 24-May-19 01:03 tdrpa/tdcore/__init__.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-19 00:55 tdrpa/tdcore/locator/__init__.pyi
 -rw-rw-rw-  2.0 fat      265 b- defN 24-May-19 00:59 tdrpa/tdcore/locator/locatorWindows.pyi
 -rw-rw-rw-  2.0 fat      264 b- defN 24-May-19 00:59 tdrpa/tdcore/locator/tdObject.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-19 00:55 tdrpa/tdcore/log/__init__.pyi
 -rw-rw-rw-  2.0 fat      130 b- defN 24-May-19 00:55 tdrpa/tdcore/log/log.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-19 00:55 tdrpa/tdcore/util/__init__.pyi
@@ -13,12 +13,12 @@
 -rw-rw-rw-  2.0 fat     1473 b- defN 23-Sep-05 03:08 tdrpa/tdcore-license/infi.systray/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1548 b- defN 23-Sep-05 03:10 tdrpa/tdcore-license/psutil/LICENSE.txt
 -rw-rw-rw-  2.0 fat     7656 b- defN 24-May-18 00:04 tdrpa/tdcore-license/pynput/COPYING.LGPL
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-30 09:52 tdrpa/tdcore-license/pywin32/none
 -rw-rw-rw-  2.0 fat    10142 b- defN 23-Sep-05 03:11 tdrpa/tdcore-license/requests/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1060 b- defN 23-Sep-05 03:12 tdrpa/tdcore-license/tzlocal/LICENSE.txt
 -rw-rw-rw-  2.0 fat    11336 b- defN 23-Sep-05 03:13 tdrpa/tdcore-license/uiautomation/LICENSE.txt
--rw-rw-rw-  2.0 fat      636 b- defN 24-May-19 02:14 tdrpa.tdcore-1.1.34.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-19 02:14 tdrpa.tdcore-1.1.34.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-19 02:14 tdrpa.tdcore-1.1.34.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1931 b- defN 24-May-19 02:14 tdrpa.tdcore-1.1.34.dist-info/RECORD
-22 files, 1303212 bytes uncompressed, 504366 bytes compressed:  61.3%
+-rw-rw-rw-  2.0 fat      636 b- defN 24-May-19 08:39 tdrpa.tdcore-1.1.35.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-19 08:39 tdrpa.tdcore-1.1.35.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-19 08:39 tdrpa.tdcore-1.1.35.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1931 b- defN 24-May-19 08:39 tdrpa.tdcore-1.1.35.dist-info/RECORD
+22 files, 1301676 bytes uncompressed, 504141 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: tdrpa/tdcore-license/tzlocal/LICENSE.txt
 Comment: 
 
 Filename: tdrpa/tdcore-license/uiautomation/LICENSE.txt
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.34.dist-info/METADATA
+Filename: tdrpa.tdcore-1.1.35.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.34.dist-info/WHEEL
+Filename: tdrpa.tdcore-1.1.35.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.34.dist-info/top_level.txt
+Filename: tdrpa.tdcore-1.1.35.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.34.dist-info/RECORD
+Filename: tdrpa.tdcore-1.1.35.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdrpa/bot.exe

### objdump

```diff
@@ -6,15 +6,15 @@
 Characteristics 0x22e
 	executable
 	line numbers stripped
 	symbols stripped
 	large address aware
 	debugging information removed
 
-Time/Date		Sun May 19 02:13:53 2024
+Time/Date		Sun May 19 08:38:56 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	41
 SizeOfCode		0000000000078e00
 SizeOfInitializedData	000000000009c200
 SizeOfUninitializedData	0000000000003400
 AddressOfEntryPoint	00000000000010f6
@@ -27,15 +27,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		000a7000
 SizeOfHeaders		00000400
-CheckSum		0009dc7b
+CheckSum		000936bb
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000968000
 SizeOfStackCommit	0000000000001000
```

## Comparing `tdrpa.tdcore-1.1.34.dist-info/METADATA` & `tdrpa.tdcore-1.1.35.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdcore
-Version: 1.1.34
+Version: 1.1.35
 Summary: RPA SDK for software developers. Supports Python3.7+, Windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: tdrpa
 Author-email: armstrong.wang@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,uiautomation,uia
 Platform: Windows Only
```

## Comparing `tdrpa.tdcore-1.1.34.dist-info/RECORD` & `tdrpa.tdcore-1.1.35.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tdrpa/bot.exe,sha256=Nm6K6MuQTgvIoTEGM75vCSJSvncI4QRg83QB3ZWadOg,640512
-tdrpa/tdcore.cp39-win_amd64.pyd,sha256=jZDwJXZ6_UzWcWqrXbSlCnHs9X9ocwDvfXZtEg3bkZE,614400
+tdrpa/bot.exe,sha256=njcDbnT-Y1wSl5Y_VtWRsc_A8Ay1OjKHxin9Fvn3IxM,640512
+tdrpa/tdcore.cp39-win_amd64.pyd,sha256=9uXnT5cQode98_sZt6w26JQrITeHur9ahv1PBeHl_KU,612864
 tdrpa/tdcore/__init__.pyi,sha256=JnzaTk_abcvIjVEP12Z8YnpcpcpSvp_4ip1xXNsfadA,340
 tdrpa/tdcore/locator/__init__.pyi,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tdrpa/tdcore/locator/locatorWindows.pyi,sha256=4doiswkToDtOV5MKbkuX8gC-H6jOtLeUnraQLCaaBrA,265
 tdrpa/tdcore/locator/tdObject.pyi,sha256=bL4-DFpaE17uuCuN9ksd02DzNykVceBJsPSyw3wtSpI,264
 tdrpa/tdcore/log/__init__.pyi,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tdrpa/tdcore/log/log.pyi,sha256=0Ykq8rzUvpHtC9Hx9_BLZy_bARD9weAH_bbXacEEknQ,130
 tdrpa/tdcore/util/__init__.pyi,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -12,11 +12,11 @@
 tdrpa/tdcore-license/infi.systray/LICENSE.txt,sha256=-9Uy-R2R7bZjSp8m31SUjOX8_6Og1laqYUB8npdzUHI,1473
 tdrpa/tdcore-license/psutil/LICENSE.txt,sha256=uJwGOzeG4o4MCjjxkx22H-015p3SopZvvs_-4PRsjRA,1548
 tdrpa/tdcore-license/pynput/COPYING.LGPL,sha256=eInlwsfJhthC1m5_bBVCQ1Mmf5nTUtL8MpjKfZxi0LU,7656
 tdrpa/tdcore-license/pywin32/none,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tdrpa/tdcore-license/requests/LICENSE.txt,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
 tdrpa/tdcore-license/tzlocal/LICENSE.txt,sha256=2ZqyCa6xaq0sJckP_YPBqYHikP__dqQgoqsD4D8EG4w,1060
 tdrpa/tdcore-license/uiautomation/LICENSE.txt,sha256=dbcOQowi1H0PtxOlQxoO0HxUwqrfphk-OGwrkfn_Sys,11336
-tdrpa.tdcore-1.1.34.dist-info/METADATA,sha256=SzQugd7skxHA5qPDYZhf-Fxd6R-EaeUFRUfCzji1MbY,636
-tdrpa.tdcore-1.1.34.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdcore-1.1.34.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdcore-1.1.34.dist-info/RECORD,,
+tdrpa.tdcore-1.1.35.dist-info/METADATA,sha256=XFF2YX1XIUaspsMBWlCI1HuJdLj_0amyhgpla84Zppc,636
+tdrpa.tdcore-1.1.35.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdcore-1.1.35.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdcore-1.1.35.dist-info/RECORD,,
```

