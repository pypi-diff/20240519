# Comparing `tmp/skrutable-1.3.0.dev4.tar.gz` & `tmp/skrutable-1.3.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skrutable-1.3.0.dev4.tar", last modified: Tue May  7 00:42:27 2024, max compression
+gzip compressed data, was "skrutable-1.3.0.dev5.tar", last modified: Sun May 19 19:29:05 2024, max compression
```

## Comparing `skrutable-1.3.0.dev4.tar` & `skrutable-1.3.0.dev5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:42:27.483466 skrutable-1.3.0.dev4/
--rw-r--r--   0 tyler      (501) staff       (20)      165 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/LICENSE.md
--rw-r--r--   0 tyler      (501) staff       (20)     1280 2024-05-07 00:42:27.483411 skrutable-1.3.0.dev4/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      824 2024-05-06 02:59:42.000000 skrutable-1.3.0.dev4/README.md
--rw-r--r--   0 tyler      (501) staff       (20)      106 2024-05-07 00:42:27.483655 skrutable-1.3.0.dev4/setup.cfg
--rw-r--r--   0 tyler      (501) staff       (20)     1296 2024-05-07 00:37:20.000000 skrutable-1.3.0.dev4/setup.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:42:27.477600 skrutable-1.3.0.dev4/src/
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:42:27.482135 skrutable-1.3.0.dev4/src/skrutable/
--rw-r--r--   0 tyler      (501) staff       (20)       26 2024-05-07 00:42:22.000000 skrutable-1.3.0.dev4/src/skrutable/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     1115 2024-05-06 03:32:29.000000 skrutable-1.3.0.dev4/src/skrutable/config.json
--rw-r--r--   0 tyler      (501) staff       (20)      281 2024-05-06 12:26:54.000000 skrutable-1.3.0.dev4/src/skrutable/config.py
--rw-r--r--   0 tyler      (501) staff       (20)    16697 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/manual.md
--rw-r--r--   0 tyler      (501) staff       (20)    27225 2024-05-07 00:13:55.000000 skrutable-1.3.0.dev4/src/skrutable/meter_identification.py
--rw-r--r--   0 tyler      (501) staff       (20)    12348 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/meter_patterns.py
--rw-r--r--   0 tyler      (501) staff       (20)     4957 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/phonemes.py
--rw-r--r--   0 tyler      (501) staff       (20)    10736 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/scansion.py
--rw-r--r--   0 tyler      (501) staff       (20)     1339 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/scheme_detection.py
--rw-r--r--   0 tyler      (501) staff       (20)    17766 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/scheme_maps.py
--rw-r--r--   0 tyler      (501) staff       (20)   212298 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/scheme_vectors_mbh.py
--rw-r--r--   0 tyler      (501) staff       (20)     2933 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/skrutable_one.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:42:27.482832 skrutable-1.3.0.dev4/src/skrutable/splitter/
--rw-r--r--   0 tyler      (501) staff       (20)     7878 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/splitter/wrapper.py
--rw-r--r--   0 tyler      (501) staff       (20)     5532 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/transliteration.py
--rw-r--r--   0 tyler      (501) staff       (20)     1435 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev4/src/skrutable/virAma_avoidance.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-07 00:42:27.483175 skrutable-1.3.0.dev4/src/skrutable.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)     1280 2024-05-07 00:42:27.000000 skrutable-1.3.0.dev4/src/skrutable.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      676 2024-05-07 00:42:27.000000 skrutable-1.3.0.dev4/src/skrutable.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2024-05-07 00:42:27.000000 skrutable-1.3.0.dev4/src/skrutable.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)       15 2024-05-07 00:42:27.000000 skrutable-1.3.0.dev4/src/skrutable.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)       10 2024-05-07 00:42:27.000000 skrutable-1.3.0.dev4/src/skrutable.egg-info/top_level.txt
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-19 19:29:05.933323 skrutable-1.3.0.dev5/
+-rw-r--r--   0 tyler      (501) staff       (20)      165 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/LICENSE.md
+-rw-r--r--   0 tyler      (501) staff       (20)     1346 2024-05-19 19:29:05.933261 skrutable-1.3.0.dev5/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      824 2024-05-06 02:59:42.000000 skrutable-1.3.0.dev5/README.md
+-rw-r--r--   0 tyler      (501) staff       (20)      106 2024-05-19 19:29:05.933552 skrutable-1.3.0.dev5/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)     1366 2024-05-19 19:08:15.000000 skrutable-1.3.0.dev5/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-19 19:29:05.926533 skrutable-1.3.0.dev5/src/
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-19 19:29:05.931775 skrutable-1.3.0.dev5/src/skrutable/
+-rw-r--r--   0 tyler      (501) staff       (20)       26 2024-05-19 19:28:30.000000 skrutable-1.3.0.dev5/src/skrutable/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1115 2024-05-06 03:32:29.000000 skrutable-1.3.0.dev5/src/skrutable/config.json
+-rw-r--r--   0 tyler      (501) staff       (20)      281 2024-05-19 19:23:05.000000 skrutable-1.3.0.dev5/src/skrutable/config.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16697 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/manual.md
+-rw-r--r--   0 tyler      (501) staff       (20)    27240 2024-05-19 19:27:39.000000 skrutable-1.3.0.dev5/src/skrutable/meter_identification.py
+-rw-r--r--   0 tyler      (501) staff       (20)    12348 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/meter_patterns.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4957 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/phonemes.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10736 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/scansion.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1339 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/scheme_detection.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17766 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/scheme_maps.py
+-rw-r--r--   0 tyler      (501) staff       (20)   212298 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/scheme_vectors_mbh.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2933 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/skrutable_one.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-19 19:29:05.932619 skrutable-1.3.0.dev5/src/skrutable/splitter/
+-rw-r--r--   0 tyler      (501) staff       (20)     7878 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/splitter/wrapper.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5532 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/transliteration.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1435 2024-05-05 19:38:35.000000 skrutable-1.3.0.dev5/src/skrutable/virAma_avoidance.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-19 19:29:05.932909 skrutable-1.3.0.dev5/src/skrutable.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)     1346 2024-05-19 19:29:05.000000 skrutable-1.3.0.dev5/src/skrutable.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      676 2024-05-19 19:29:05.000000 skrutable-1.3.0.dev5/src/skrutable.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2024-05-19 19:29:05.000000 skrutable-1.3.0.dev5/src/skrutable.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       33 2024-05-19 19:29:05.000000 skrutable-1.3.0.dev5/src/skrutable.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       10 2024-05-19 19:29:05.000000 skrutable-1.3.0.dev5/src/skrutable.egg-info/top_level.txt
```

### Comparing `skrutable-1.3.0.dev4/PKG-INFO` & `skrutable-1.3.0.dev5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: skrutable
-Version: 1.3.0.dev4
+Version: 1.3.0.dev5
 Summary: skrutable library for working with Sanskrit text
 Home-page: https://github.com/tylergneill/skrutable
 Author: Tyler Neill
 Author-email: tyler.g.neill@gmail.com
 License: CC BY-SA 4.0
 Keywords: Sanskrit text transliteration scansion meter identification sandhi compound splitting
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: requests
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
 
 # skrutable
 
 A toolkit and online workbench providing 
 transliteration, scansion, and meter identification for Sanskrit text,
 as well access to powerful sandhi and compound splitting.
```

### Comparing `skrutable-1.3.0.dev4/README.md` & `skrutable-1.3.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/setup.py` & `skrutable-1.3.0.dev5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,12 +31,16 @@
     package_data={'': [
 		'config.json',
 		'manual.md'
 	]},
     url='https://github.com/tylergneill/skrutable',
     keywords='Sanskrit text transliteration scansion meter identification sandhi compound splitting',
     install_requires=[
-          'numpy',
-          'requests',
-      ],
-
+      'numpy',
+      'requests',
+    ],
+    extras_require={
+        "testing": [
+            "pytest",
+        ]
+    },
 )
```

### Comparing `skrutable-1.3.0.dev4/src/skrutable/config.json` & `skrutable-1.3.0.dev5/src/skrutable/config.json`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/manual.md` & `skrutable-1.3.0.dev5/src/skrutable/manual.md`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/meter_identification.py` & `skrutable-1.3.0.dev5/src/skrutable/meter_identification.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,21 +369,21 @@
 			return False
 
 	def test_as_samavftta_etc(self, Vrs):
 
 		wbp = Vrs.syllable_weights.split('\n') # weights by pāda
 		wbp_lens = [ len(line) for line in wbp ]
 
-		# make sure full four pādas
-		try: wbp[3]
-		except IndexError:
-			if self.resplit_option == "single_pAda" and len(wbp) == 1:
-				pass
-			else:
-				return 0
+		# make sure either full four pādas or one and single-pāda mode
+		if 	len(wbp) >= 4 or (
+			len(wbp) == 1 and self.resplit_option == "single_pAda"
+		):
+			pass
+		else:
+			return 0
 
 		self.count_pAdasamatva(Vrs) # [0,2,3,4]
 
 		# test in following order to prioritize left-right presentation of ties
 		# ties managed in self.combine_results()
 
 		# test perfect samavṛtta
@@ -402,15 +402,14 @@
 			# will give id_score == 8
 			self.evaluate_ardhasamavftta(Vrs)
 			# max score not necessarily yet reached, don't return
 
 		# test perfect single pāda of samavṛtta
 		if ( self.pAdasamatva_count == 0 and self.resplit_option == "single_pAda"):
 			self.evaluate_samavftta(Vrs)
-			#....
 
 		# test perfect viṣamavṛtta
 		if self.pAdasamatva_count == 0 and self.is_vizamavftta(Vrs):
 			# will give id_score == 9
 			# label and score already set in is_vizamavftta if test was successful
 			return 1 # max score already reached
```

### Comparing `skrutable-1.3.0.dev4/src/skrutable/meter_patterns.py` & `skrutable-1.3.0.dev5/src/skrutable/meter_patterns.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/phonemes.py` & `skrutable-1.3.0.dev5/src/skrutable/phonemes.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/scansion.py` & `skrutable-1.3.0.dev5/src/skrutable/scansion.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/scheme_detection.py` & `skrutable-1.3.0.dev5/src/skrutable/scheme_detection.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/scheme_maps.py` & `skrutable-1.3.0.dev5/src/skrutable/scheme_maps.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/scheme_vectors_mbh.py` & `skrutable-1.3.0.dev5/src/skrutable/scheme_vectors_mbh.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/skrutable_one.py` & `skrutable-1.3.0.dev5/src/skrutable/skrutable_one.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/splitter/wrapper.py` & `skrutable-1.3.0.dev5/src/skrutable/splitter/wrapper.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/transliteration.py` & `skrutable-1.3.0.dev5/src/skrutable/transliteration.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable/virAma_avoidance.py` & `skrutable-1.3.0.dev5/src/skrutable/virAma_avoidance.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.3.0.dev4/src/skrutable.egg-info/PKG-INFO` & `skrutable-1.3.0.dev5/src/skrutable.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: skrutable
-Version: 1.3.0.dev4
+Version: 1.3.0.dev5
 Summary: skrutable library for working with Sanskrit text
 Home-page: https://github.com/tylergneill/skrutable
 Author: Tyler Neill
 Author-email: tyler.g.neill@gmail.com
 License: CC BY-SA 4.0
 Keywords: Sanskrit text transliteration scansion meter identification sandhi compound splitting
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: requests
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
 
 # skrutable
 
 A toolkit and online workbench providing 
 transliteration, scansion, and meter identification for Sanskrit text,
 as well access to powerful sandhi and compound splitting.
```

### Comparing `skrutable-1.3.0.dev4/src/skrutable.egg-info/SOURCES.txt` & `skrutable-1.3.0.dev5/src/skrutable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

