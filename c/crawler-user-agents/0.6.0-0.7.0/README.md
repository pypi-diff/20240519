# Comparing `tmp/crawler_user_agents-0.6.0-py3-none-any.whl.zip` & `tmp/crawler_user_agents-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 51073 bytes, number of entries: 12
--rw-r--r--  2.0 unx      472 b- defN 24-May-18 09:59 crawleruseragents/__init__.py
--rw-r--r--  2.0 unx      705 b- defN 24-May-18 09:59 crawleruseragents/composer.json
--rw-r--r--  2.0 unx   171732 b- defN 24-May-18 09:59 crawleruseragents/crawler-user-agents.json
--rw-r--r--  2.0 unx    63625 b- defN 24-May-18 09:59 crawleruseragents/package-lock.json
--rw-r--r--  2.0 unx      683 b- defN 24-May-18 09:59 crawleruseragents/package.json
--rw-r--r--  2.0 unx     7226 b- defN 24-May-18 09:59 crawleruseragents/test_validation.py
--rw-r--r--  2.0 unx     4134 b- defN 24-May-18 09:59 crawleruseragents/validate.py
--rw-r--r--  2.0 unx     1083 b- defN 24-May-18 09:59 crawler_user_agents-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3650 b- defN 24-May-18 09:59 crawler_user_agents-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-18 09:59 crawler_user_agents-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-May-18 09:59 crawler_user_agents-0.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1077 b- defN 24-May-18 09:59 crawler_user_agents-0.6.0.dist-info/RECORD
-12 files, 254497 bytes uncompressed, 49237 bytes compressed:  80.7%
+Zip file size: 51164 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      662 b- defN 24-May-19 13:55 crawleruseragents/__init__.py
+-rw-r--r--  2.0 unx      705 b- defN 24-May-19 13:55 crawleruseragents/composer.json
+-rw-r--r--  2.0 unx   171873 b- defN 24-May-19 13:55 crawleruseragents/crawler-user-agents.json
+-rw-r--r--  2.0 unx    63625 b- defN 24-May-19 13:55 crawleruseragents/package-lock.json
+-rw-r--r--  2.0 unx      683 b- defN 24-May-19 13:55 crawleruseragents/package.json
+-rw-r--r--  2.0 unx     7226 b- defN 24-May-19 13:55 crawleruseragents/test_validation.py
+-rw-r--r--  2.0 unx     4134 b- defN 24-May-19 13:55 crawleruseragents/validate.py
+-rw-r--r--  2.0 unx     1083 b- defN 24-May-19 13:56 crawler_user_agents-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3650 b- defN 24-May-19 13:56 crawler_user_agents-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-19 13:56 crawler_user_agents-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-19 13:56 crawler_user_agents-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1077 b- defN 24-May-19 13:56 crawler_user_agents-0.7.0.dist-info/RECORD
+12 files, 254828 bytes uncompressed, 49328 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: crawleruseragents/test_validation.py
 Comment: 
 
 Filename: crawleruseragents/validate.py
 Comment: 
 
-Filename: crawler_user_agents-0.6.0.dist-info/LICENSE
+Filename: crawler_user_agents-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: crawler_user_agents-0.6.0.dist-info/METADATA
+Filename: crawler_user_agents-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: crawler_user_agents-0.6.0.dist-info/WHEEL
+Filename: crawler_user_agents-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: crawler_user_agents-0.6.0.dist-info/top_level.txt
+Filename: crawler_user_agents-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: crawler_user_agents-0.6.0.dist-info/RECORD
+Filename: crawler_user_agents-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## crawleruseragents/__init__.py

```diff
@@ -1,22 +1,25 @@
-import crawleruseragents
 import re
 import json
-from importlib import resources 
-    
+from pathlib import Path
+
+
 def load_json():
-  return json.loads(resources.read_text(crawleruseragents,"crawler-user-agents.json"))
+    cwd = Path(__file__).parent
+    user_agents_file_path = cwd / "crawler-user-agents.json"
+    with user_agents_file_path.open() as patterns_file:
+        return json.load(patterns_file)
 
-DATA = load_json()
 
-def is_crawler(s):
-  # print(s)
-  for i in DATA:
-    test=re.search(i["pattern"],s,re.IGNORECASE)
-    if test:
-      return True
-  return False
+CRAWLER_USER_AGENTS_DATA = load_json()
 
-def is_crawler2(s):
-  regexp = re.compile("|".join([i["pattern"] for i in DATA]))
-  return regexp.search(s) != None
 
+def is_crawler(user_agent: str) -> bool:
+    for crawler_user_agent in CRAWLER_USER_AGENTS_DATA:
+        if re.search(crawler_user_agent["pattern"], user_agent, re.IGNORECASE):
+            return True
+    return False
+
+
+def is_crawler2(s):
+    regexp = re.compile("|".join([i["pattern"] for i in CRAWLER_USER_AGENTS_DATA]))
+    return regexp.search(s) is not None
```

## crawleruseragents/crawler-user-agents.json

### Pretty-printed

 * *Similarity: 0.9982547993019197%*

 * *Differences: {'insert': "[(572, OrderedDict([('pattern', 'GroupMeBot'), ('addition_date', '2024/05/19'), "*

 * *           "('instances', ['GroupMeBot/1.0']), ('url', 'https://groupme.com/')]))]"}*

```diff
@@ -4909,9 +4909,17 @@
     {
         "addition_date": "2024/05/14",
         "instances": [
             "Mozilla/5.0 (compatible; Monsidobot/2.2; +http://monsido.com/bot.html; info@monsido.com)"
         ],
         "pattern": "Monsidobot",
         "url": "http://monsido.com/bot.html"
+    },
+    {
+        "addition_date": "2024/05/19",
+        "instances": [
+            "GroupMeBot/1.0"
+        ],
+        "pattern": "GroupMeBot",
+        "url": "https://groupme.com/"
     }
 ]
```

## Comparing `crawler_user_agents-0.6.0.dist-info/LICENSE` & `crawler_user_agents-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `crawler_user_agents-0.6.0.dist-info/METADATA` & `crawler_user_agents-0.7.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawler-user-agents
-Version: 0.6.0
+Version: 0.7.0
 Author-email: Martin Monperrus <martin.monperrus@gnieh.org>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # crawler-user-agents
 
 This repository contains a list of of HTTP user-agents used by robots, crawlers, and spiders as in single JSON file.
```

## Comparing `crawler_user_agents-0.6.0.dist-info/RECORD` & `crawler_user_agents-0.7.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-crawleruseragents/__init__.py,sha256=qBqDODmZnMaC4vg2j76af1AnYN7OMozwRfagUxE7SHc,472
+crawleruseragents/__init__.py,sha256=8pOnhMLGw0daBvgxCST7wtBZbnE60wSc0b5qUF3RSss,662
 crawleruseragents/composer.json,sha256=1szuZqSrf27uxY3mH1m1ZgdtMcOEemVGHG2Fe1vG96I,705
-crawleruseragents/crawler-user-agents.json,sha256=7RUQpbDvmKrjvR0BVJHDRZYpGUTc7MXqtt4ZYrBGcmA,171732
+crawleruseragents/crawler-user-agents.json,sha256=d0V5f9Qz8xw9r8Pp_qO4z53Y0Kb-nyyAPuZ48Q92-n0,171873
 crawleruseragents/package-lock.json,sha256=sBCgJOX_U7ePhdxRZgDqxNWlzmOKleehK8JiJ_kPDk4,63625
 crawleruseragents/package.json,sha256=7qBY5cBrUVDsndax5o84Kng4W7MzUfSpagXPkBMW1QM,683
 crawleruseragents/test_validation.py,sha256=RzNHFxIsB44m8bxmXZcfl7HTvxXo1OrS6qxiFTn50iA,7226
 crawleruseragents/validate.py,sha256=-PRv133IbMRRf4L-KFLSRt8ohT7UITElpaoZKt79YnA,4134
-crawler_user_agents-0.6.0.dist-info/LICENSE,sha256=vR1UJ4wpoSwcMAklmWWmIMWTY7jX9XQNmNP8OPMZ16U,1083
-crawler_user_agents-0.6.0.dist-info/METADATA,sha256=fjj-HY9swyKNU3oGxgoGBHu5XujjqAgqyWGClGO9fG4,3650
-crawler_user_agents-0.6.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-crawler_user_agents-0.6.0.dist-info/top_level.txt,sha256=zWVNLMFuT-LyqADstPhEDHIxeAkHrT2ZOAJ58UQllMo,18
-crawler_user_agents-0.6.0.dist-info/RECORD,,
+crawler_user_agents-0.7.0.dist-info/LICENSE,sha256=vR1UJ4wpoSwcMAklmWWmIMWTY7jX9XQNmNP8OPMZ16U,1083
+crawler_user_agents-0.7.0.dist-info/METADATA,sha256=8XV5w1Os3VaxYyN3ftjVffIv_9Z06ENy6N4kRC4J_wQ,3650
+crawler_user_agents-0.7.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+crawler_user_agents-0.7.0.dist-info/top_level.txt,sha256=zWVNLMFuT-LyqADstPhEDHIxeAkHrT2ZOAJ58UQllMo,18
+crawler_user_agents-0.7.0.dist-info/RECORD,,
```

