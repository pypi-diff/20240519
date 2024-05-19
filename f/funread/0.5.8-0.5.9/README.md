# Comparing `tmp/funread-0.5.8-py3-none-any.whl.zip` & `tmp/funread-0.5.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 13867 bytes, number of entries: 18
+Zip file size: 13891 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        0 b- defN 23-Nov-20 06:55 funread/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Nov-20 06:55 funread/legado/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Feb-13 14:35 funread/legado/manage/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Feb-13 14:42 funread/legado/manage/book/__init__.py
 -rw-rw-r--  2.0 unx     3312 b- defN 24-Feb-13 14:47 funread/legado/manage/book/format.py
 -rw-rw-r--  2.0 unx      126 b- defN 24-Mar-03 12:03 funread/legado/manage/download/__init__.py
 -rw-rw-r--  2.0 unx     5913 b- defN 24-Mar-10 09:55 funread/legado/manage/download/base.py
--rw-rw-r--  2.0 unx     3868 b- defN 24-Mar-10 10:05 funread/legado/manage/download/book.py
+-rw-rw-r--  2.0 unx     4006 b- defN 24-Mar-10 10:14 funread/legado/manage/download/book.py
 -rw-rw-r--  2.0 unx     6640 b- defN 24-Mar-06 17:22 funread/legado/manage/download/generate.py
 -rw-rw-r--  2.0 unx       33 b- defN 24-Feb-13 14:52 funread/legado/manage/utils/__init__.py
 -rw-rw-r--  2.0 unx       95 b- defN 24-Feb-13 14:52 funread/legado/manage/utils/core.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Nov-20 07:41 funread/scripts/__init__.py
 -rw-rw-r--  2.0 unx     1465 b- defN 24-Mar-03 13:02 funread/scripts/command.py
--rw-rw-r--  2.0 unx    10935 b- defN 24-Mar-10 10:05 funread-0.5.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx      489 b- defN 24-Mar-10 10:05 funread-0.5.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-10 10:05 funread-0.5.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Mar-10 10:05 funread-0.5.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1545 b- defN 24-Mar-10 10:05 funread-0.5.8.dist-info/RECORD
-18 files, 34521 bytes uncompressed, 11281 bytes compressed:  67.3%
+-rw-rw-r--  2.0 unx    10935 b- defN 24-Mar-10 10:14 funread-0.5.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      489 b- defN 24-Mar-10 10:14 funread-0.5.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Mar-10 10:14 funread-0.5.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Mar-10 10:14 funread-0.5.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1545 b- defN 24-Mar-10 10:14 funread-0.5.9.dist-info/RECORD
+18 files, 34659 bytes uncompressed, 11305 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: funread/scripts/__init__.py
 Comment: 
 
 Filename: funread/scripts/command.py
 Comment: 
 
-Filename: funread-0.5.8.dist-info/LICENSE
+Filename: funread-0.5.9.dist-info/LICENSE
 Comment: 
 
-Filename: funread-0.5.8.dist-info/METADATA
+Filename: funread-0.5.9.dist-info/METADATA
 Comment: 
 
-Filename: funread-0.5.8.dist-info/WHEEL
+Filename: funread-0.5.9.dist-info/WHEEL
 Comment: 
 
-Filename: funread-0.5.8.dist-info/top_level.txt
+Filename: funread-0.5.9.dist-info/top_level.txt
 Comment: 
 
-Filename: funread-0.5.8.dist-info/RECORD
+Filename: funread-0.5.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funread/legado/manage/download/book.py

```diff
@@ -21,14 +21,18 @@
 
     def run(self):
         self.format_book_info()
         self.format_content()
         self.format_search()
         self.format_explore()
         self.format_toc()
+        keys = [key for key in self.source.keys() if not self.source[key]]
+        for key in keys:
+                del self.source[key]
+
         for key in ['customOrder','respondTime','lastUpdateTime']:
             del self.source[key]
 
         for key in ['searchUrl','exploreUrl']:
             if key in self.source.keys():
                 self.source[key]=self.source[key].replace(self.source['bookSourceUrl'],'')
         return self.source
```

## Comparing `funread-0.5.8.dist-info/LICENSE` & `funread-0.5.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funread-0.5.8.dist-info/RECORD` & `funread-0.5.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 funread/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funread/legado/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funread/legado/manage/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funread/legado/manage/book/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funread/legado/manage/book/format.py,sha256=TiWEn1G-0aI_gTJlr625JVm-mLuLBFwxnfkAQWdjF7w,3312
 funread/legado/manage/download/__init__.py,sha256=8He1zPalMr8Hfaw6H65Ijax3nCODdUkAb-PahB6x5XE,126
 funread/legado/manage/download/base.py,sha256=FYy54ljl6pZ8eRlrnw11Qg6dXezGjcaBP9m_cxdkHos,5913
-funread/legado/manage/download/book.py,sha256=Pq8a9eYL1Us3DKn4Giq9XoFIfmxyF5tWxjtfYM1FEV0,3868
+funread/legado/manage/download/book.py,sha256=y-Fu8glGjB3uEGOqk_Did25jpZUmpQ6KVR_bUiDhIes,4006
 funread/legado/manage/download/generate.py,sha256=RUQBIEBrx7s07NXTZbhG6V2-0FL0loQetfkjJVHfGOc,6640
 funread/legado/manage/utils/__init__.py,sha256=dkQ6vmfYf8v7sRMCf9qzIgJrziT2gEXnorDv0pe5MIM,33
 funread/legado/manage/utils/core.py,sha256=Di4mu-EKQyH0IyAjNTDfSvtwwV6I38NMaR7_yqlhwdM,95
 funread/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funread/scripts/command.py,sha256=esSunklLRuswW4zOpi7tlhlSjdeFXOSu5LK2hc58Sbw,1465
-funread-0.5.8.dist-info/LICENSE,sha256=TP1Pk9L9nW9ihYD-jbpzwlG8XC5_V310d4XWebqsi8g,10935
-funread-0.5.8.dist-info/METADATA,sha256=vPD_ShjAZPwl2lLqGQSE9PSuU-lQEygYtPlkL4cm9q4,489
-funread-0.5.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-funread-0.5.8.dist-info/top_level.txt,sha256=KCVb7k7sr1o_a07nxGyuoX1WRcm-kt0Smn5RIZbjEUY,8
-funread-0.5.8.dist-info/RECORD,,
+funread-0.5.9.dist-info/LICENSE,sha256=TP1Pk9L9nW9ihYD-jbpzwlG8XC5_V310d4XWebqsi8g,10935
+funread-0.5.9.dist-info/METADATA,sha256=pH7xcQ7zFdB8tT21Tz-WhiYGyBnkOrTUmaDP_eKQqFk,489
+funread-0.5.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+funread-0.5.9.dist-info/top_level.txt,sha256=KCVb7k7sr1o_a07nxGyuoX1WRcm-kt0Smn5RIZbjEUY,8
+funread-0.5.9.dist-info/RECORD,,
```

