# Comparing `tmp/almgroad-0.1.4-py3-none-any.whl.zip` & `tmp/almgroad-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 26375 bytes, number of entries: 13
--rw-rw----  2.0 unx      248 b- defN 24-May-18 06:30 almgroad/__init__.py
+Zip file size: 27177 bytes, number of entries: 14
+-rw-rw----  2.0 unx      295 b- defN 24-May-19 12:26 almgroad/__init__.py
 -rw-rw----  2.0 unx      182 b- defN 24-May-15 18:03 almgroad/chat.py
 -rw-rw----  2.0 unx     1331 b- defN 24-May-16 06:55 almgroad/info_tik.py
 -rw-rw----  2.0 unx     1071 b- defN 24-May-15 04:51 almgroad/infoinsta.py
 -rw-rw----  2.0 unx     1517 b- defN 24-May-17 08:57 almgroad/insta.py
 -rw-rw----  2.0 unx    84898 b- defN 24-May-15 18:03 almgroad/ktkt.py
 -rw-rw----  2.0 unx      460 b- defN 24-May-16 19:19 almgroad/pryer.py
+-rw-rw----  2.0 unx      969 b- defN 24-May-19 12:26 almgroad/search_pinterset.py
 -rw-rw----  2.0 unx      346 b- defN 24-May-18 06:34 almgroad/send_te_message.py
 -rw-rw----  2.0 unx      880 b- defN 24-May-15 18:02 almgroad/tik_tok.py
--rw-rw----  2.0 unx     1499 b- defN 24-May-18 06:34 almgroad-0.1.4.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-18 06:34 almgroad-0.1.4.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-18 06:34 almgroad-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      983 b- defN 24-May-18 06:34 almgroad-0.1.4.dist-info/RECORD
-13 files, 93516 bytes uncompressed, 24755 bytes compressed:  73.5%
+-rw-rw----  2.0 unx     1499 b- defN 24-May-19 12:27 almgroad-0.1.5.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-19 12:27 almgroad-0.1.5.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-19 12:27 almgroad-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1067 b- defN 24-May-19 12:27 almgroad-0.1.5.dist-info/RECORD
+14 files, 94616 bytes uncompressed, 25425 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -15,26 +15,29 @@
 
 Filename: almgroad/ktkt.py
 Comment: 
 
 Filename: almgroad/pryer.py
 Comment: 
 
+Filename: almgroad/search_pinterset.py
+Comment: 
+
 Filename: almgroad/send_te_message.py
 Comment: 
 
 Filename: almgroad/tik_tok.py
 Comment: 
 
-Filename: almgroad-0.1.4.dist-info/METADATA
+Filename: almgroad-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.1.4.dist-info/WHEEL
+Filename: almgroad-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.1.4.dist-info/top_level.txt
+Filename: almgroad-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.1.4.dist-info/RECORD
+Filename: almgroad-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/__init__.py

```diff
@@ -1,8 +1,9 @@
 from .infoinsta import Info_Insta
 from .chat import GPT
 from .ktkt import kt
 from .tik_tok import Tik_Tok
 from .info_tik import Info_Tik
 from .pryer import prayer_times
 from .insta import instagram
-from .send_te_message import Send_telegram_message
+from .send_te_message import Send_telegram_message
+from .search_pinterset import Search_Pinterest
```

## Comparing `almgroad-0.1.4.dist-info/METADATA` & `almgroad-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.1.4
+Version: 0.1.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `almgroad-0.1.4.dist-info/RECORD` & `almgroad-0.1.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-almgroad/__init__.py,sha256=2DbRi10J33IeqJhA8R5ReIOjCgY2RvFRTqNamoOVxng,248
+almgroad/__init__.py,sha256=E0hxPWeV-m_3aQiv8PxdFPe8LoqNeLmxbWL1Dgd0Frg,295
 almgroad/chat.py,sha256=QOkrkf2gUrcjSstul9hqhPWkTREsasSilv5nMvp_sq4,182
 almgroad/info_tik.py,sha256=dURJKszAIWQPeuHpgVHADcNTz4sTpFWbkxqvwH0RAo4,1331
 almgroad/infoinsta.py,sha256=DzqhmwPWbeBrSXoSZp9DsZQiVC6Nlx8PnZn9wM8sNrM,1071
 almgroad/insta.py,sha256=MKOPtEn7YRFm79pluSNKP1-d_-HYiKkVlpAx_9qz4GM,1517
 almgroad/ktkt.py,sha256=CoUbwbOAd18fMb2fTVPr3BHt81DR43hnSvNuKywcSlU,84898
 almgroad/pryer.py,sha256=jM3M_7DThca_-FvYOMuOnSelTUR49MnDxHYlS9k-6S4,460
+almgroad/search_pinterset.py,sha256=5fsKZ3O4Zz2Ewr-U8JDct_NI_vvhwUEfcsdGLV1X_2Y,969
 almgroad/send_te_message.py,sha256=sdzXHjZ9U4g9wms2zzdoj_A-nISUh0qWBFIgMPadmOw,346
 almgroad/tik_tok.py,sha256=22laOxfsGV1NhHq7YCQqxl3ZDxIBoGQtP9FSNffgEpI,880
-almgroad-0.1.4.dist-info/METADATA,sha256=xfIc75PnKeyfHFO1mcICIlqLQ-sxp7VGaYVv-v02z0I,1499
-almgroad-0.1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-almgroad-0.1.4.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
-almgroad-0.1.4.dist-info/RECORD,,
+almgroad-0.1.5.dist-info/METADATA,sha256=-0NdHzjmQfQ4Ymt8DTSyO1L1Hp9LUuJTi5hc2XtqhCs,1499
+almgroad-0.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+almgroad-0.1.5.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
+almgroad-0.1.5.dist-info/RECORD,,
```

