# Comparing `tmp/instagrapi-2.1.1.tar.gz` & `tmp/instagrapi-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagrapi-2.1.1.tar", last modified: Mon Mar 18 21:19:05 2024, max compression
+gzip compressed data, was "instagrapi-2.1.2.tar", last modified: Sun May 19 12:10:44 2024, max compression
```

## Comparing `instagrapi-2.1.1.tar` & `instagrapi-2.1.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-03-18 21:19:05.771116 instagrapi-2.1.1/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1056 2023-09-03 19:01:30.000000 instagrapi-2.1.1/LICENSE
--rw-r--r--   0 adw0rd     (501) staff       (20)     1899 2024-03-18 21:19:05.770979 instagrapi-2.1.1/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)    10968 2024-01-13 13:28:26.000000 instagrapi-2.1.1/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-03-18 21:19:05.756436 instagrapi-2.1.1/instagrapi/
--rw-r--r--   0 adw0rd     (501) staff       (20)     3967 2023-03-30 17:33:04.000000 instagrapi-2.1.1/instagrapi/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2772 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/config.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     5592 2023-08-25 23:24:16.000000 instagrapi-2.1.1/instagrapi/exceptions.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    17214 2024-03-01 14:13:16.000000 instagrapi-2.1.1/instagrapi/extractors.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    11793 2023-12-25 12:53:25.000000 instagrapi-2.1.1/instagrapi/image_util.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-03-18 21:19:05.770376 instagrapi-2.1.1/instagrapi/mixins/
--rw-r--r--   0 adw0rd     (501) staff       (20)        0 2022-09-12 21:50:02.000000 instagrapi-2.1.1/instagrapi/mixins/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     9780 2024-01-13 13:28:26.000000 instagrapi-2.1.1/instagrapi/mixins/account.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10108 2024-01-20 18:35:22.000000 instagrapi-2.1.1/instagrapi/mixins/album.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    29424 2023-08-25 23:24:16.000000 instagrapi-2.1.1/instagrapi/mixins/auth.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     1530 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/mixins/bloks.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    22270 2023-12-25 12:56:13.000000 instagrapi-2.1.1/instagrapi/mixins/challenge.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    13965 2023-06-22 12:45:22.000000 instagrapi-2.1.1/instagrapi/mixins/clip.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     7365 2024-02-27 17:05:48.000000 instagrapi-2.1.1/instagrapi/mixins/collection.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     9428 2023-04-01 21:26:16.000000 instagrapi-2.1.1/instagrapi/mixins/comment.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    36460 2023-12-25 12:53:25.000000 instagrapi-2.1.1/instagrapi/mixins/direct.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     1254 2023-03-30 17:34:05.000000 instagrapi-2.1.1/instagrapi/mixins/explore.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3742 2023-12-25 12:53:25.000000 instagrapi-2.1.1/instagrapi/mixins/fbsearch.py
--rw-r--r--   0 adw0rd     (501) staff       (20)      455 2023-08-16 09:12:55.000000 instagrapi-2.1.1/instagrapi/mixins/fundraiser.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    15291 2023-12-25 12:53:25.000000 instagrapi-2.1.1/instagrapi/mixins/hashtag.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8465 2023-08-16 09:12:55.000000 instagrapi-2.1.1/instagrapi/mixins/highlight.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10860 2023-03-30 17:33:04.000000 instagrapi-2.1.1/instagrapi/mixins/igtv.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     6324 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/mixins/insights.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    16311 2023-12-25 12:53:25.000000 instagrapi-2.1.1/instagrapi/mixins/location.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    34637 2023-12-16 22:25:29.000000 instagrapi-2.1.1/instagrapi/mixins/media.py
--rw-r--r--   0 adw0rd     (501) staff       (20)      472 2023-08-16 09:12:55.000000 instagrapi-2.1.1/instagrapi/mixins/multiple_accounts.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2211 2023-08-11 11:28:38.000000 instagrapi-2.1.1/instagrapi/mixins/note.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    16206 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/mixins/notification.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     1625 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/mixins/password.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    24224 2024-02-27 17:05:48.000000 instagrapi-2.1.1/instagrapi/mixins/photo.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    20728 2023-12-25 12:53:25.000000 instagrapi-2.1.1/instagrapi/mixins/private.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    11162 2024-01-13 13:28:26.000000 instagrapi-2.1.1/instagrapi/mixins/public.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     1428 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/mixins/share.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    11932 2024-01-13 13:28:26.000000 instagrapi-2.1.1/instagrapi/mixins/story.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3086 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/mixins/timeline.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3997 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/mixins/totp.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3181 2024-01-13 13:28:26.000000 instagrapi-2.1.1/instagrapi/mixins/track.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    38229 2024-01-13 13:28:26.000000 instagrapi-2.1.1/instagrapi/mixins/user.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    34439 2024-01-13 13:28:26.000000 instagrapi-2.1.1/instagrapi/mixins/video.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8476 2023-12-21 12:06:08.000000 instagrapi-2.1.1/instagrapi/story.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    14439 2024-03-01 14:12:49.000000 instagrapi-2.1.1/instagrapi/types.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2938 2023-02-15 13:28:06.000000 instagrapi-2.1.1/instagrapi/utils.py
--rw-r--r--   0 adw0rd     (501) staff       (20)      311 2022-09-12 21:50:02.000000 instagrapi-2.1.1/instagrapi/zones.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-03-18 21:19:05.757139 instagrapi-2.1.1/instagrapi.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1899 2024-03-18 21:19:05.000000 instagrapi-2.1.1/instagrapi.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)     1346 2024-03-18 21:19:05.000000 instagrapi-2.1.1/instagrapi.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2024-03-18 21:19:05.000000 instagrapi-2.1.1/instagrapi.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       75 2024-03-18 21:19:05.000000 instagrapi-2.1.1/instagrapi.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       11 2024-03-18 21:19:05.000000 instagrapi-2.1.1/instagrapi.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2024-03-18 21:19:05.771163 instagrapi-2.1.1/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     2664 2024-03-18 21:18:29.000000 instagrapi-2.1.1/setup.py
+drwxr-xr-x   0 colinfrl   (501) staff       (20)        0 2024-05-19 12:10:44.061775 instagrapi-2.1.2/
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1056 2023-09-03 19:01:30.000000 instagrapi-2.1.2/LICENSE
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2034 2024-05-19 12:10:44.061581 instagrapi-2.1.2/PKG-INFO
+-rw-r--r--   0 colinfrl   (501) staff       (20)    11083 2024-04-13 15:39:07.000000 instagrapi-2.1.2/README.md
+drwxr-xr-x   0 colinfrl   (501) staff       (20)        0 2024-05-19 12:10:44.055553 instagrapi-2.1.2/instagrapi/
+-rw-r--r--   0 colinfrl   (501) staff       (20)     4033 2024-04-13 15:40:06.000000 instagrapi-2.1.2/instagrapi/__init__.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2772 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/config.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     5592 2023-08-25 23:24:16.000000 instagrapi-2.1.2/instagrapi/exceptions.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    17214 2024-04-13 15:40:18.000000 instagrapi-2.1.2/instagrapi/extractors.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    11793 2023-12-25 12:53:25.000000 instagrapi-2.1.2/instagrapi/image_util.py
+drwxr-xr-x   0 colinfrl   (501) staff       (20)        0 2024-05-19 12:10:44.061118 instagrapi-2.1.2/instagrapi/mixins/
+-rw-r--r--   0 colinfrl   (501) staff       (20)        0 2022-09-12 21:50:02.000000 instagrapi-2.1.2/instagrapi/mixins/__init__.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     9942 2024-04-13 16:18:43.000000 instagrapi-2.1.2/instagrapi/mixins/account.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    10108 2024-01-20 18:35:22.000000 instagrapi-2.1.2/instagrapi/mixins/album.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    29424 2023-08-25 23:24:16.000000 instagrapi-2.1.2/instagrapi/mixins/auth.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1530 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/mixins/bloks.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    22270 2023-12-25 12:56:13.000000 instagrapi-2.1.2/instagrapi/mixins/challenge.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    13965 2023-06-22 12:45:22.000000 instagrapi-2.1.2/instagrapi/mixins/clip.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     7365 2024-02-27 17:05:48.000000 instagrapi-2.1.2/instagrapi/mixins/collection.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     9428 2023-04-01 21:26:16.000000 instagrapi-2.1.2/instagrapi/mixins/comment.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    36414 2024-04-13 15:39:07.000000 instagrapi-2.1.2/instagrapi/mixins/direct.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1254 2023-03-30 17:34:05.000000 instagrapi-2.1.2/instagrapi/mixins/explore.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     3742 2023-12-25 12:53:25.000000 instagrapi-2.1.2/instagrapi/mixins/fbsearch.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)      455 2023-08-16 09:12:55.000000 instagrapi-2.1.2/instagrapi/mixins/fundraiser.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    15291 2023-12-25 12:53:25.000000 instagrapi-2.1.2/instagrapi/mixins/hashtag.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     8465 2023-08-16 09:12:55.000000 instagrapi-2.1.2/instagrapi/mixins/highlight.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    10860 2023-03-30 17:33:04.000000 instagrapi-2.1.2/instagrapi/mixins/igtv.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     6324 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/mixins/insights.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    16311 2023-12-25 12:53:25.000000 instagrapi-2.1.2/instagrapi/mixins/location.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    34637 2023-12-16 22:25:29.000000 instagrapi-2.1.2/instagrapi/mixins/media.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)      472 2023-08-16 09:12:55.000000 instagrapi-2.1.2/instagrapi/mixins/multiple_accounts.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2211 2023-08-11 11:28:38.000000 instagrapi-2.1.2/instagrapi/mixins/note.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    16206 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/mixins/notification.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1625 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/mixins/password.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    24224 2024-02-27 17:05:48.000000 instagrapi-2.1.2/instagrapi/mixins/photo.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    20728 2023-12-25 12:53:25.000000 instagrapi-2.1.2/instagrapi/mixins/private.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    11381 2024-04-13 15:39:28.000000 instagrapi-2.1.2/instagrapi/mixins/public.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1428 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/mixins/share.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     7261 2024-04-13 15:40:18.000000 instagrapi-2.1.2/instagrapi/mixins/signup.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    11961 2024-04-13 15:41:02.000000 instagrapi-2.1.2/instagrapi/mixins/story.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     3086 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/mixins/timeline.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     3997 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/mixins/totp.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     3181 2024-01-13 13:28:26.000000 instagrapi-2.1.2/instagrapi/mixins/track.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    38229 2024-01-13 13:28:26.000000 instagrapi-2.1.2/instagrapi/mixins/user.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    34439 2024-01-13 13:28:26.000000 instagrapi-2.1.2/instagrapi/mixins/video.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     8476 2024-04-13 15:39:28.000000 instagrapi-2.1.2/instagrapi/story.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)    14449 2024-05-19 12:10:02.000000 instagrapi-2.1.2/instagrapi/types.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2938 2023-02-15 13:28:06.000000 instagrapi-2.1.2/instagrapi/utils.py
+-rw-r--r--   0 colinfrl   (501) staff       (20)      311 2022-09-12 21:50:02.000000 instagrapi-2.1.2/instagrapi/zones.py
+drwxr-xr-x   0 colinfrl   (501) staff       (20)        0 2024-05-19 12:10:44.061284 instagrapi-2.1.2/instagrapi.egg-info/
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2034 2024-05-19 12:10:44.000000 instagrapi-2.1.2/instagrapi.egg-info/PKG-INFO
+-rw-r--r--   0 colinfrl   (501) staff       (20)     1374 2024-05-19 12:10:44.000000 instagrapi-2.1.2/instagrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 colinfrl   (501) staff       (20)        1 2024-05-19 12:10:44.000000 instagrapi-2.1.2/instagrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 colinfrl   (501) staff       (20)       75 2024-05-19 12:10:44.000000 instagrapi-2.1.2/instagrapi.egg-info/requires.txt
+-rw-r--r--   0 colinfrl   (501) staff       (20)       11 2024-05-19 12:10:44.000000 instagrapi-2.1.2/instagrapi.egg-info/top_level.txt
+-rw-r--r--   0 colinfrl   (501) staff       (20)       38 2024-05-19 12:10:44.061812 instagrapi-2.1.2/setup.cfg
+-rw-r--r--   0 colinfrl   (501) staff       (20)     2664 2024-05-19 12:10:11.000000 instagrapi-2.1.2/setup.py
```

### Comparing `instagrapi-2.1.1/LICENSE` & `instagrapi-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/PKG-INFO` & `instagrapi-2.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagrapi
-Version: 2.1.1
+Version: 2.1.2
 Summary: Fast and effective Instagram Private API wrapper
 Home-page: https://github.com/subzeroid/instagrapi
 Author: Mark Subzeroid
 Author-email: 143403577+subzeroid@users.noreply.github.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader,instagram-note
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests<3.0,>=2.25.1
+Requires-Dist: PySocks==1.7.1
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pycryptodomex==3.20.0
 
 
 Fast and effective Instagram Private API wrapper (public+private requests and challenge resolver).
 
 Use the most recent version of the API from Instagram.
 
 Features:
```

### Comparing `instagrapi-2.1.1/README.md` & `instagrapi-2.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 However, you won't need to spend weeks or even months setting it up.
 The best service available today is [HikerAPI](https://hikerapi.com/p/bkXQlaVe), which handles 4–5 million daily requests, provides support around-the-clock, and offers partners a special rate.
 In many instances, our clients tried to save money and preferred instagrapi, but in our experience, they ultimately returned to [HikerAPI](https://hikerapi.com/p/bkXQlaVe) after spending much more time and money.
 It will be difficult to find good accounts, good proxies, or resolve challenges, and IG will ban your accounts.
 
 The instagrapi more suits for testing or research than a working business!
 
+✨ [aiograpi - Asynchronous Python library for Instagram Private API](https://github.com/subzeroid/aiograpi) ✨
+
 ### We recommend using our services:
 
 * [LamaTok](https://lamatok.com/p/B9ScEYIQ) for TikTok API 🔥
 * [HikerAPI](https://hikerapi.com/p/bkXQlaVe) for Instagram API ⚡⚡⚡
 * [DataLikers](https://datalikers.com/p/S9Lv5vBy) for Instagram Datasets 🚀
 
 [![Package](https://github.com/subzeroid/instagrapi/actions/workflows/python-package.yml/badge.svg?branch=master&1)](https://github.com/subzeroid/instagrapi/actions/workflows/python-package.yml)
```

### Comparing `instagrapi-2.1.1/instagrapi/__init__.py` & `instagrapi-2.1.2/instagrapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from instagrapi.mixins.private import PrivateRequestMixin
 from instagrapi.mixins.public import (
     ProfilePublicMixin,
     PublicRequestMixin,
     TopSearchesPublicMixin,
 )
 from instagrapi.mixins.share import ShareMixin
+from instagrapi.mixins.signup import SignUpMixin
 from instagrapi.mixins.story import StoryMixin
 from instagrapi.mixins.timeline import ReelsMixin
 from instagrapi.mixins.totp import TOTPMixin
 from instagrapi.mixins.track import TrackMixin
 from instagrapi.mixins.user import UserMixin
 from instagrapi.mixins.video import DownloadVideoMixin, UploadVideoMixin
 
@@ -74,14 +75,15 @@
     AccountMixin,
     DirectMixin,
     LocationMixin,
     HashtagMixin,
     CommentMixin,
     StoryMixin,
     PasswordMixin,
+    SignUpMixin,
     DownloadClipMixin,
     UploadClipMixin,
     ReelsMixin,
     ExploreMixin,
     BloksMixin,
     TOTPMixin,
     MultipleAccountsMixin,
```

### Comparing `instagrapi-2.1.1/instagrapi/config.py` & `instagrapi-2.1.2/instagrapi/config.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/exceptions.py` & `instagrapi-2.1.2/instagrapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/extractors.py` & `instagrapi-2.1.2/instagrapi/extractors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import datetime
 import html
 import json
 import re
-import datetime
 from copy import deepcopy
 
 from .types import (
     Account,
     Collection,
     Comment,
     DirectMedia,
@@ -19,17 +19,17 @@
     Location,
     Media,
     MediaOembed,
     MediaXma,
     ReplyMessage,
     Resource,
     Story,
+    StoryHashtag,
     StoryLink,
     StoryLocation,
-    StoryHashtag,
     StoryMedia,
     StoryMention,
     Track,
     User,
     UserShort,
     Usertag,
 )
```

### Comparing `instagrapi-2.1.1/instagrapi/image_util.py` & `instagrapi-2.1.2/instagrapi/image_util.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/account.py` & `instagrapi-2.1.2/instagrapi/mixins/account.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 
 import requests
 
 from instagrapi.exceptions import ClientError, ClientLoginRequired
 from instagrapi.extractors import extract_account, extract_user_short
 from instagrapi.types import Account, UserShort
-from instagrapi.utils import dumps, gen_token
+from instagrapi.utils import dumps, gen_token, generate_signature
 
 
 class AccountMixin:
     """
     Helper class to manage your account
     """
 
@@ -30,15 +30,19 @@
             headers={
                 "x-requested-with": "XMLHttpRequest",
                 "x-csrftoken": gen_token(),
                 "Connection": "Keep-Alive",
                 "Accept": "*/*",
                 "Accept-Encoding": "gzip,deflate",
                 "Accept-Language": "en-US",
-                "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/11.1.2 Safari/605.1.15",
+                "User-Agent": (
+                    "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) "
+                    "AppleWebKit/605.1.15 (KHTML, like Gecko) "
+                    "Version/11.1.2 Safari/605.1.15"
+                ),
             },
             proxies=self.public.proxies,
             timeout=self.request_timeout,
         )
         try:
             return response.json()
         except JSONDecodeError as e:
@@ -53,15 +57,15 @@
         Returns
         -------
         Account
             An object of Account class
         """
         result = self.private_request("accounts/current_user/?edit=true")
         return extract_account(result["user"])
-    
+
     def change_password(
         self,
         old_password: str,
         new_password: str,
     ) -> bool:
         """
         Change password
@@ -92,23 +96,34 @@
                     "_uuid": self.uuid,
                     "_csrftoken": self.token,
                 }
             )
             result = self.private_request("accounts/change_password/", data=data)
             return result
         except Exception as e:
+            self.logger.exception(e)
             return False
+
     def set_external_url(self, external_url) -> dict:
         """
         Set new biography
         """
-
-        signed_body = f"signed_body=SIGNATURE.%7B%22updated_links%22%3A%22%5B%7B%5C%22url%5C%22%3A%5C%22{external_url}%5C%22%2C%5C%22title%5C%22%3A%5C%22%5C%22%2C%5C%22link_type%5C%22%3A%5C%22external%5C%22%7D%5D%22%2C%22_uid%22%3A%22{self.user_id}%22%2C%22_uuid%22%3A%22{self.uuid}%22%7D"
+        data = dumps(
+            {
+                "updated_links": dumps(
+                    [{"url": external_url, "title": "", "link_type": "external"}]
+                ),
+                "_uid": self.user_id,
+                "_uuid": self.uuid,
+            }
+        )
         return self.private_request(
-            "accounts/update_bio_links/", data=signed_body, with_signature=False
+            "accounts/update_bio_links/",
+            data=generate_signature(data),
+            with_signature=False,
         )
 
     def account_set_private(self) -> bool:
         """
         Sets your account private
 
         Returns
```

### Comparing `instagrapi-2.1.1/instagrapi/mixins/album.py` & `instagrapi-2.1.2/instagrapi/mixins/album.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/auth.py` & `instagrapi-2.1.2/instagrapi/mixins/auth.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/bloks.py` & `instagrapi-2.1.2/instagrapi/mixins/bloks.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/challenge.py` & `instagrapi-2.1.2/instagrapi/mixins/challenge.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/clip.py` & `instagrapi-2.1.2/instagrapi/mixins/clip.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/collection.py` & `instagrapi-2.1.2/instagrapi/mixins/collection.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/comment.py` & `instagrapi-2.1.2/instagrapi/mixins/comment.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/direct.py` & `instagrapi-2.1.2/instagrapi/mixins/direct.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,14 @@
         assert self.user_id, "Login required"
         params = {
             "visual_message_return_type": "unseen",
             "thread_message_limit": "10",
             "persistentBadging": "true",
             "limit": "20",
             "is_prefetching": "false",
-            "fetch_reason": "manual_refresh",
         }
         if selected_filter:
             assert (
                 selected_filter in SELECTED_FILTERS
             ), f'Unsupported selected_filter="{selected_filter}" {SELECTED_FILTERS}'
             params.update({"selected_filter": selected_filter})
         if box:
```

### Comparing `instagrapi-2.1.1/instagrapi/mixins/explore.py` & `instagrapi-2.1.2/instagrapi/mixins/explore.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/fbsearch.py` & `instagrapi-2.1.2/instagrapi/mixins/fbsearch.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/hashtag.py` & `instagrapi-2.1.2/instagrapi/mixins/hashtag.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/highlight.py` & `instagrapi-2.1.2/instagrapi/mixins/highlight.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/igtv.py` & `instagrapi-2.1.2/instagrapi/mixins/igtv.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/insights.py` & `instagrapi-2.1.2/instagrapi/mixins/insights.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/location.py` & `instagrapi-2.1.2/instagrapi/mixins/location.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/media.py` & `instagrapi-2.1.2/instagrapi/mixins/media.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/note.py` & `instagrapi-2.1.2/instagrapi/mixins/note.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/notification.py` & `instagrapi-2.1.2/instagrapi/mixins/notification.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/password.py` & `instagrapi-2.1.2/instagrapi/mixins/password.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/photo.py` & `instagrapi-2.1.2/instagrapi/mixins/photo.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/private.py` & `instagrapi-2.1.2/instagrapi/mixins/private.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/public.py` & `instagrapi-2.1.2/instagrapi/mixins/public.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,31 +119,46 @@
                 if retries_count > iteration + 1:
                     time.sleep(retries_timeout)
                 else:
                     raise e
                 continue
 
     def _send_public_request(
-        self, url, data=None, params=None, headers=None, return_json=False, stream=None, timeout=None
+        self,
+        url,
+        data=None,
+        params=None,
+        headers=None,
+        return_json=False,
+        stream=None,
+        timeout=None,
     ):
         self.public_requests_count += 1
         if headers:
             self.public.headers.update(headers)
         if self.last_response_ts and (time.time() - self.last_response_ts) < 1.0:
             time.sleep(1.0)
         if self.request_timeout:
             time.sleep(self.request_timeout)
         try:
             if data is not None:  # POST
                 response = self.public.data(
-                    url, data=data, params=params, proxies=self.public.proxies, timeout=timeout
+                    url,
+                    data=data,
+                    params=params,
+                    proxies=self.public.proxies,
+                    timeout=timeout,
                 )
             else:  # GET
                 response = self.public.get(
-                    url, params=params, proxies=self.public.proxies, stream=stream, timeout=timeout
+                    url,
+                    params=params,
+                    proxies=self.public.proxies,
+                    stream=stream,
+                    timeout=timeout,
                 )
 
             if stream:
                 return response
 
             expected_length = int(response.headers.get("Content-Length") or 0)
             actual_length = response.raw.tell()
```

### Comparing `instagrapi-2.1.1/instagrapi/mixins/share.py` & `instagrapi-2.1.2/instagrapi/mixins/share.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/story.py` & `instagrapi-2.1.2/instagrapi/mixins/story.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
 import shutil
 from copy import deepcopy
 from pathlib import Path
 from typing import List
 from urllib.parse import urlparse
 
-import requests
-
 from instagrapi import config
 from instagrapi.exceptions import ClientNotFoundError, StoryNotFound, UserNotFound
 from instagrapi.extractors import (
     extract_story_gql,
     extract_story_v1,
     extract_user_short,
 )
@@ -128,15 +126,16 @@
         assert isinstance(user_ids, list), "user_ids should be a list of user_id"
         self.inject_sessionid_to_public()
 
         def _userid_chunks():
             assert user_ids is not None
             user_ids_per_query = 50
             for i in range(0, len(user_ids), user_ids_per_query):
-                yield user_ids[i : i + user_ids_per_query]
+                end = i + user_ids_per_query
+                yield user_ids[i:end]
 
         stories_un = {}
         for userid_chunk in _userid_chunks():
             res = self.public_graphql_request(
                 query_hash="303a4ae99711322310f25250d988f3b7",
                 variables={"reel_ids": userid_chunk, "precomposed_overlay": False},
             )
@@ -292,15 +291,17 @@
         assert fname, (
             """The URL must contain the path to the file (mp4 or jpg).\n"""
             """Read the documentation https://subzeroid.github.io/instagrapi/usage-guide/story.html"""
         )
         filename = "%s.%s" % (filename, fname.rsplit(".", 1)[1]) if filename else fname
         path = Path(folder) / filename
 
-        response = self._send_public_request(url, stream=True, timeout=self.request_timeout)
+        response = self._send_public_request(
+            url, stream=True, timeout=self.request_timeout
+        )
         response.raise_for_status()
 
         with open(path, "wb") as f:
             response.raw.decode_content = True
             shutil.copyfileobj(response.raw, f)
         return path.resolve()
```

### Comparing `instagrapi-2.1.1/instagrapi/mixins/timeline.py` & `instagrapi-2.1.2/instagrapi/mixins/timeline.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/totp.py` & `instagrapi-2.1.2/instagrapi/mixins/totp.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/track.py` & `instagrapi-2.1.2/instagrapi/mixins/track.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/user.py` & `instagrapi-2.1.2/instagrapi/mixins/user.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/mixins/video.py` & `instagrapi-2.1.2/instagrapi/mixins/video.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/story.py` & `instagrapi-2.1.2/instagrapi/story.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi/types.py` & `instagrapi-2.1.2/instagrapi/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,18 +95,20 @@
 
     _external_url = validator("external_url", allow_reuse=True)(validate_external_url)
 
 
 class UserShort(TypesBaseModel):
     def __hash__(self):
         return hash(self.pk)
+
     def __eq__(self, other):
         if isinstance(other, UserShort):
             return self.pk == other.pk
         return NotImplemented
+
     pk: str
     username: Optional[str] = None
     full_name: Optional[str] = ""
     profile_pic_url: Optional[HttpUrl] = None
     profile_pic_url_hd: Optional[HttpUrl] = None
     is_private: Optional[bool] = None
     # is_verified: bool  # not found in hashtag_medias_v1
@@ -317,15 +319,15 @@
     media_type: int
     product_type: Optional[str] = ""
     thumbnail_url: Optional[HttpUrl] = None
     user: UserShort
     video_url: Optional[HttpUrl] = None  # for Video and IGTV
     video_duration: Optional[float] = 0.0  # for Video and IGTV
     sponsor_tags: List[UserShort]
-    is_paid_partnership: Optional[bool]
+    is_paid_partnership: Optional[bool] = False
     mentions: List[StoryMention]
     links: List[StoryLink]
     hashtags: List[StoryHashtag]
     locations: List[StoryLocation]
     stickers: List[StorySticker]
     medias: List[StoryMedia] = []
```

### Comparing `instagrapi-2.1.1/instagrapi/utils.py` & `instagrapi-2.1.2/instagrapi/utils.py`

 * *Files identical despite different names*

### Comparing `instagrapi-2.1.1/instagrapi.egg-info/PKG-INFO` & `instagrapi-2.1.2/instagrapi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagrapi
-Version: 2.1.1
+Version: 2.1.2
 Summary: Fast and effective Instagram Private API wrapper
 Home-page: https://github.com/subzeroid/instagrapi
 Author: Mark Subzeroid
 Author-email: 143403577+subzeroid@users.noreply.github.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader,instagram-note
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests<3.0,>=2.25.1
+Requires-Dist: PySocks==1.7.1
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pycryptodomex==3.20.0
 
 
 Fast and effective Instagram Private API wrapper (public+private requests and challenge resolver).
 
 Use the most recent version of the API from Instagram.
 
 Features:
```

### Comparing `instagrapi-2.1.1/instagrapi.egg-info/SOURCES.txt` & `instagrapi-2.1.2/instagrapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,14 @@
 instagrapi/mixins/note.py
 instagrapi/mixins/notification.py
 instagrapi/mixins/password.py
 instagrapi/mixins/photo.py
 instagrapi/mixins/private.py
 instagrapi/mixins/public.py
 instagrapi/mixins/share.py
+instagrapi/mixins/signup.py
 instagrapi/mixins/story.py
 instagrapi/mixins/timeline.py
 instagrapi/mixins/totp.py
 instagrapi/mixins/track.py
 instagrapi/mixins/user.py
 instagrapi/mixins/video.py
```

### Comparing `instagrapi-2.1.1/setup.py` & `instagrapi-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 7. Build stories with custom background, font animation, swipe up link and mention users
 8. In the next release, account registration and captcha passing will appear
 """
 
 requirements = [
     "requests<3.0,>=2.25.1",
     "PySocks==1.7.1",
-    "pydantic==2.6.4",
+    "pydantic==2.7.1",
     "pycryptodomex==3.20.0",
 ]
 # requirements = [
 #     line.strip()
 #     for line in open('requirements.txt').readlines()
 # ]
 
 setup(
     name="instagrapi",
-    version="2.1.1",
+    version="2.1.2",
     author="Mark Subzeroid",
     author_email="143403577+subzeroid@users.noreply.github.com",
     license="MIT",
     url="https://github.com/subzeroid/instagrapi",
     install_requires=requirements,
     keywords=[
         "instagram private api",
```

