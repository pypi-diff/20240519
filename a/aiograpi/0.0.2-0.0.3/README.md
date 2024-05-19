# Comparing `tmp/aiograpi-0.0.2.tar.gz` & `tmp/aiograpi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiograpi-0.0.2.tar", last modified: Sat Apr 13 15:16:39 2024, max compression
+gzip compressed data, was "aiograpi-0.0.3.tar", last modified: Sun May 19 12:08:40 2024, max compression
```

## Comparing `aiograpi-0.0.2.tar` & `aiograpi-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-04-13 15:16:39.682994 aiograpi-0.0.2/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1056 2024-03-02 23:24:00.000000 aiograpi-0.0.2/LICENSE
--rw-r--r--   0 adw0rd     (501) staff       (20)     1729 2024-04-13 15:16:39.682699 aiograpi-0.0.2/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)    10756 2024-03-04 10:06:34.000000 aiograpi-0.0.2/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-04-13 15:16:39.669865 aiograpi-0.0.2/aiograpi/
--rw-r--r--   0 adw0rd     (501) staff       (20)     3541 2024-03-03 00:22:37.000000 aiograpi-0.0.2/aiograpi/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2772 2024-02-27 14:43:44.000000 aiograpi-0.0.2/aiograpi/config.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     6839 2024-03-03 00:20:42.000000 aiograpi-0.0.2/aiograpi/exceptions.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    19241 2024-03-03 01:00:05.000000 aiograpi-0.0.2/aiograpi/extractors.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-04-13 15:16:39.682034 aiograpi-0.0.2/aiograpi/mixins/
--rw-r--r--   0 adw0rd     (501) staff       (20)        0 2023-11-08 14:15:14.000000 aiograpi-0.0.2/aiograpi/mixins/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     7375 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/account.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10509 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/album.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    27252 2024-03-03 01:43:10.000000 aiograpi-0.0.2/aiograpi/mixins/auth.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     1572 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/bloks.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    23109 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/challenge.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10767 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/clip.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     6441 2024-03-03 00:01:17.000000 aiograpi-0.0.2/aiograpi/mixins/collection.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    18105 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/comment.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    22459 2024-03-02 23:18:03.000000 aiograpi-0.0.2/aiograpi/mixins/direct.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3310 2024-02-27 14:43:44.000000 aiograpi-0.0.2/aiograpi/mixins/fbsearch.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8142 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/graphql.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    15880 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/hashtag.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8652 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/highlight.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10812 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/igtv.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     6430 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/insights.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    16761 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/location.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    37772 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/media.py
--rw-r--r--   0 adw0rd     (501) staff       (20)      496 2024-03-03 00:24:12.000000 aiograpi-0.0.2/aiograpi/mixins/multiple_accounts.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2257 2024-03-03 01:57:36.000000 aiograpi-0.0.2/aiograpi/mixins/note.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    16438 2024-03-02 22:36:16.000000 aiograpi-0.0.2/aiograpi/mixins/notification.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2665 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/password.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    22899 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/photo.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    24114 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/private.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10183 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/public.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     1611 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/share.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    12525 2024-03-02 22:25:43.000000 aiograpi-0.0.2/aiograpi/mixins/signup.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    11639 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/story.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3132 2024-02-27 14:43:45.000000 aiograpi-0.0.2/aiograpi/mixins/timeline.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4039 2023-11-28 11:31:19.000000 aiograpi-0.0.2/aiograpi/mixins/totp.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2896 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/track.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    36854 2024-03-03 00:59:58.000000 aiograpi-0.0.2/aiograpi/mixins/user.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    33721 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/video.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4148 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/reqwests.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8476 2023-10-10 17:45:34.000000 aiograpi-0.0.2/aiograpi/story.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    15233 2024-03-03 01:41:07.000000 aiograpi-0.0.2/aiograpi/types.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2992 2024-02-27 14:43:45.000000 aiograpi-0.0.2/aiograpi/utils.py
--rw-r--r--   0 adw0rd     (501) staff       (20)      311 2023-11-22 18:01:30.000000 aiograpi-0.0.2/aiograpi/zones.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-04-13 15:16:39.670833 aiograpi-0.0.2/aiograpi.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1729 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)     1246 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)      100 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        9 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2024-04-13 15:16:39.683049 aiograpi-0.0.2/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     2436 2024-04-13 15:15:48.000000 aiograpi-0.0.2/setup.py
+drwxr-xr-x   0 colinfrl   (501) staff       (20)        0 2024-05-19 12:08:40.463545 aiograpi-0.0.3/
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1056 2024-03-02 23:24:00.000000 aiograpi-0.0.3/LICENSE
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1919 2024-05-19 12:08:40.463338 aiograpi-0.0.3/PKG-INFO
+-rw-r--r--   0 colinfrl   (501) staff       (20)    10756 2024-03-04 10:06:34.000000 aiograpi-0.0.3/README.md
+drwxr-xr-x   0 colinfrl   (501) staff       (20)        0 2024-05-19 12:08:40.458248 aiograpi-0.0.3/aiograpi/
+-rw-r--r--   0 colinfrl   (501) staff       (20)     3541 2024-03-03 00:22:37.000000 aiograpi-0.0.3/aiograpi/__init__.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2772 2024-02-27 14:43:44.000000 aiograpi-0.0.3/aiograpi/config.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     6839 2024-03-03 00:20:42.000000 aiograpi-0.0.3/aiograpi/exceptions.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    19323 2024-05-19 12:07:03.000000 aiograpi-0.0.3/aiograpi/extractors.py
+drwxr-xr-x   0 colinfrl   (501) staff       (20)        0 2024-05-19 12:08:40.462898 aiograpi-0.0.3/aiograpi/mixins/
+-rw-r--r--   0 colinfrl   (501) staff       (20)        0 2023-11-08 14:15:14.000000 aiograpi-0.0.3/aiograpi/mixins/__init__.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     7375 2024-02-27 14:33:28.000000 aiograpi-0.0.3/aiograpi/mixins/account.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    10509 2024-04-13 15:14:01.000000 aiograpi-0.0.3/aiograpi/mixins/album.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    27252 2024-03-03 01:43:10.000000 aiograpi-0.0.3/aiograpi/mixins/auth.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1572 2024-02-27 14:33:28.000000 aiograpi-0.0.3/aiograpi/mixins/bloks.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    23109 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/challenge.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    10767 2024-04-13 15:14:01.000000 aiograpi-0.0.3/aiograpi/mixins/clip.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     6441 2024-03-03 00:01:17.000000 aiograpi-0.0.3/aiograpi/mixins/collection.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    18105 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/comment.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    22459 2024-03-02 23:18:03.000000 aiograpi-0.0.3/aiograpi/mixins/direct.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     3310 2024-02-27 14:43:44.000000 aiograpi-0.0.3/aiograpi/mixins/fbsearch.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     8142 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/graphql.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    15880 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/hashtag.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     8652 2024-02-27 14:33:28.000000 aiograpi-0.0.3/aiograpi/mixins/highlight.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    10812 2024-04-13 15:14:01.000000 aiograpi-0.0.3/aiograpi/mixins/igtv.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     6430 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/insights.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    16761 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/location.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    37772 2024-04-13 15:14:01.000000 aiograpi-0.0.3/aiograpi/mixins/media.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)      496 2024-03-03 00:24:12.000000 aiograpi-0.0.3/aiograpi/mixins/multiple_accounts.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2257 2024-03-03 01:57:36.000000 aiograpi-0.0.3/aiograpi/mixins/note.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    16438 2024-03-02 22:36:16.000000 aiograpi-0.0.3/aiograpi/mixins/notification.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2665 2024-02-27 14:33:28.000000 aiograpi-0.0.3/aiograpi/mixins/password.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    22899 2024-04-13 15:14:01.000000 aiograpi-0.0.3/aiograpi/mixins/photo.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    24114 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/private.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    10183 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/public.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1611 2024-02-27 14:33:28.000000 aiograpi-0.0.3/aiograpi/mixins/share.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    12525 2024-03-02 22:25:43.000000 aiograpi-0.0.3/aiograpi/mixins/signup.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    11639 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/story.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     3132 2024-02-27 14:43:45.000000 aiograpi-0.0.3/aiograpi/mixins/timeline.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     4039 2023-11-28 11:31:19.000000 aiograpi-0.0.3/aiograpi/mixins/totp.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2896 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/mixins/track.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    36854 2024-03-03 00:59:58.000000 aiograpi-0.0.3/aiograpi/mixins/user.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    33721 2024-04-13 15:14:01.000000 aiograpi-0.0.3/aiograpi/mixins/video.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     4148 2024-03-02 23:19:15.000000 aiograpi-0.0.3/aiograpi/reqwests.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     8476 2023-10-10 17:45:34.000000 aiograpi-0.0.3/aiograpi/story.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    15233 2024-03-03 01:41:07.000000 aiograpi-0.0.3/aiograpi/types.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2992 2024-02-27 14:43:45.000000 aiograpi-0.0.3/aiograpi/utils.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)      311 2023-11-22 18:01:30.000000 aiograpi-0.0.3/aiograpi/zones.py
+drwxr-xr-x   0 colinfrl   (501) staff       (20)        0 2024-05-19 12:08:40.463062 aiograpi-0.0.3/aiograpi.egg-info/
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1919 2024-05-19 12:08:40.000000 aiograpi-0.0.3/aiograpi.egg-info/PKG-INFO
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1246 2024-05-19 12:08:40.000000 aiograpi-0.0.3/aiograpi.egg-info/SOURCES.txt
+-rw-r--r--   0 colinfrl   (501) staff       (20)        1 2024-05-19 12:08:40.000000 aiograpi-0.0.3/aiograpi.egg-info/dependency_links.txt
+-rw-r--r--   0 colinfrl   (501) staff       (20)      100 2024-05-19 12:08:40.000000 aiograpi-0.0.3/aiograpi.egg-info/requires.txt
+-rw-r--r--   0 colinfrl   (501) staff       (20)        9 2024-05-19 12:08:40.000000 aiograpi-0.0.3/aiograpi.egg-info/top_level.txt
+-rw-r--r--   0 colinfrl   (501) staff       (20)       38 2024-05-19 12:08:40.463586 aiograpi-0.0.3/setup.cfg
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2436 2024-05-19 12:07:10.000000 aiograpi-0.0.3/setup.py
```

### Comparing `aiograpi-0.0.2/LICENSE` & `aiograpi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/PKG-INFO` & `aiograpi-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiograpi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous Instagram Private API wrapper
 Home-page: https://github.com/subzeroid/aiograpi
 Author: Mr.Robot
 Author-email: mr.robot@example.org
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader,instagram-note
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx==0.27.0
+Requires-Dist: orjson==3.10.3
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: moviepy==1.0.3
+Requires-Dist: pycryptodomex==3.20.0
+Requires-Dist: zstandard==0.22.0
 
 
 Asynchronous Instagram Private API wrapper.
 
 Use the most recent version of the API from Instagram.
 
 Features:
```

### Comparing `aiograpi-0.0.2/README.md` & `aiograpi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/__init__.py` & `aiograpi-0.0.3/aiograpi/__init__.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/config.py` & `aiograpi-0.0.3/aiograpi/config.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/exceptions.py` & `aiograpi-0.0.3/aiograpi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/extractors.py` & `aiograpi-0.0.3/aiograpi/extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,17 @@
     for item in data["items"]:
         item["thread_id"] = data["id"]
         data["messages"].append(extract_direct_message(item))
     data["users"] = [extract_user_short(u) for u in data["users"]]
     if "inviter" in data:
         data["inviter"] = extract_user_short(data["inviter"])
     data["left_users"] = data.get("left_users", [])
+
+    data["last_activity_at"] = datetime.datetime.fromtimestamp(data["last_activity_at"] / 1_000_000)
+
     return DirectThread(**data)
 
 
 def extract_direct_short_thread(data):
     data["users"] = [extract_user_short(u) for u in data["users"]]
     data["id"] = data.get("thread_id")
     return DirectShortThread(**data)
@@ -369,15 +372,15 @@
     clip = data.get("clip", {})
     if clip:
         if "clip" in clip:
             # Instagram ¯\_(ツ)_/¯
             clip = clip.get("clip")
         data["clip"] = extract_media_v1(clip)
 
-    data["timestamp"] = datetime.datetime.fromtimestamp(data["timestamp"] // 1_000_000)
+    data["timestamp"] = datetime.datetime.fromtimestamp(data["timestamp"] / 1_000_000)
     data["user_id"] = str(data["user_id"])
 
     return ReplyMessage(**data)
 
 
 def extract_direct_message(data):
     data["id"] = data.get("item_id")
@@ -399,17 +402,15 @@
             # Instagram ¯\_(ツ)_/¯
             clip = clip.get("clip")
         data["clip"] = extract_media_v1(clip)
     xma_media_share = data.get("xma_media_share", {})
     if xma_media_share:
         data["xma_share"] = extract_media_v1_xma(xma_media_share[0])
 
-    data["timestamp"] = datetime.datetime.fromtimestamp(
-        int(data["timestamp"]) // 1_000_000
-    )
+    data["timestamp"] = datetime.datetime.fromtimestamp(data["timestamp"] / 1_000_000)
     data["user_id"] = str(data.get("user_id", ""))
 
     return DirectMessage(**data)
 
 
 def extract_direct_media(media):
     # media = deepcopy(data)
```

### Comparing `aiograpi-0.0.2/aiograpi/mixins/account.py` & `aiograpi-0.0.3/aiograpi/mixins/account.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/album.py` & `aiograpi-0.0.3/aiograpi/mixins/album.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/auth.py` & `aiograpi-0.0.3/aiograpi/mixins/auth.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/bloks.py` & `aiograpi-0.0.3/aiograpi/mixins/bloks.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/challenge.py` & `aiograpi-0.0.3/aiograpi/mixins/challenge.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/clip.py` & `aiograpi-0.0.3/aiograpi/mixins/clip.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/collection.py` & `aiograpi-0.0.3/aiograpi/mixins/collection.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/comment.py` & `aiograpi-0.0.3/aiograpi/mixins/comment.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/direct.py` & `aiograpi-0.0.3/aiograpi/mixins/direct.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/fbsearch.py` & `aiograpi-0.0.3/aiograpi/mixins/fbsearch.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/graphql.py` & `aiograpi-0.0.3/aiograpi/mixins/graphql.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/hashtag.py` & `aiograpi-0.0.3/aiograpi/mixins/hashtag.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/highlight.py` & `aiograpi-0.0.3/aiograpi/mixins/highlight.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/igtv.py` & `aiograpi-0.0.3/aiograpi/mixins/igtv.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/insights.py` & `aiograpi-0.0.3/aiograpi/mixins/insights.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/location.py` & `aiograpi-0.0.3/aiograpi/mixins/location.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/media.py` & `aiograpi-0.0.3/aiograpi/mixins/media.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/note.py` & `aiograpi-0.0.3/aiograpi/mixins/note.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/notification.py` & `aiograpi-0.0.3/aiograpi/mixins/notification.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/password.py` & `aiograpi-0.0.3/aiograpi/mixins/password.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/photo.py` & `aiograpi-0.0.3/aiograpi/mixins/photo.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/private.py` & `aiograpi-0.0.3/aiograpi/mixins/private.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/public.py` & `aiograpi-0.0.3/aiograpi/mixins/public.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/share.py` & `aiograpi-0.0.3/aiograpi/mixins/share.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/signup.py` & `aiograpi-0.0.3/aiograpi/mixins/signup.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/story.py` & `aiograpi-0.0.3/aiograpi/mixins/story.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/timeline.py` & `aiograpi-0.0.3/aiograpi/mixins/timeline.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/totp.py` & `aiograpi-0.0.3/aiograpi/mixins/totp.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/track.py` & `aiograpi-0.0.3/aiograpi/mixins/track.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/user.py` & `aiograpi-0.0.3/aiograpi/mixins/user.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/mixins/video.py` & `aiograpi-0.0.3/aiograpi/mixins/video.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/reqwests.py` & `aiograpi-0.0.3/aiograpi/reqwests.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/story.py` & `aiograpi-0.0.3/aiograpi/story.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/types.py` & `aiograpi-0.0.3/aiograpi/types.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi/utils.py` & `aiograpi-0.0.3/aiograpi/utils.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/aiograpi.egg-info/PKG-INFO` & `aiograpi-0.0.3/aiograpi.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiograpi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous Instagram Private API wrapper
 Home-page: https://github.com/subzeroid/aiograpi
 Author: Mr.Robot
 Author-email: mr.robot@example.org
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader,instagram-note
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx==0.27.0
+Requires-Dist: orjson==3.10.3
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: moviepy==1.0.3
+Requires-Dist: pycryptodomex==3.20.0
+Requires-Dist: zstandard==0.22.0
 
 
 Asynchronous Instagram Private API wrapper.
 
 Use the most recent version of the API from Instagram.
 
 Features:
```

### Comparing `aiograpi-0.0.2/aiograpi.egg-info/SOURCES.txt` & `aiograpi-0.0.3/aiograpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.2/setup.py` & `aiograpi-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 5. Like, Follow, Edit account (Bio) and much more else
 6. Insights by account, posts and stories
 7. Build stories with custom background, font animation, swipe up link and mention users
 """
 
 requirements = [
     "httpx==0.27.0",
-    "orjson==3.10.0",
-    "pydantic==2.7.0",
+    "orjson==3.10.3",
+    "pydantic==2.7.1",
     "moviepy==1.0.3",
     "pycryptodomex==3.20.0",
     "zstandard==0.22.0",
 ]
 
 setup(
     name="aiograpi",
-    version="0.0.2",
+    version="0.0.3",
     author="Mr.Robot",
     author_email="mr.robot@example.org",
     license="MIT",
     url="https://github.com/subzeroid/aiograpi",
     install_requires=requirements,
     keywords=[
         "instagram private api",
```

