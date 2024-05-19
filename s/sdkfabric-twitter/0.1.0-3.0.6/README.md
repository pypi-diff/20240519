# Comparing `tmp/sdkfabric_twitter-0.1.0.tar.gz` & `tmp/sdkfabric_twitter-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_twitter-0.1.0.tar", last modified: Sun May 19 07:30:38 2024, max compression
+gzip compressed data, was "sdkfabric_twitter-3.0.6.tar", last modified: Sun May 19 17:45:07 2024, max compression
```

## Comparing `sdkfabric_twitter-0.1.0.tar` & `sdkfabric_twitter-3.0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:30:38.044434 sdkfabric_twitter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 07:30:38.044434 sdkfabric_twitter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:30:38.044434 sdkfabric_twitter-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:30:38.036435 sdkfabric_twitter-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:30:38.044434 sdkfabric_twitter-0.1.0/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/bookmark_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/hide_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/hide_reply_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/like.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/like_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/quote_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/search_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/single_tweet.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/trend.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/trend_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/trends_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_media.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/tweet_usage_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/usage_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-19 07:30:34.000000 sdkfabric_twitter-0.1.0/src/sdk/user_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:30:38.044434 sdkfabric_twitter-0.1.0/src/sdkfabric_twitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 07:30:38.000000 sdkfabric_twitter-0.1.0/src/sdkfabric_twitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-19 07:30:38.000000 sdkfabric_twitter-0.1.0/src/sdkfabric_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:30:38.000000 sdkfabric_twitter-0.1.0/src/sdkfabric_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 07:30:38.000000 sdkfabric_twitter-0.1.0/src/sdkfabric_twitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 07:30:38.000000 sdkfabric_twitter-0.1.0/src/sdkfabric_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:07.970399 sdkfabric_twitter-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 17:45:07.970399 sdkfabric_twitter-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:45:07.970399 sdkfabric_twitter-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:07.962399 sdkfabric_twitter-3.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:07.966399 sdkfabric_twitter-3.0.6/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/bookmark_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/hide_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/hide_reply_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/like.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/like_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/quote_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/search_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/single_tweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/trend_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/trends_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/tweet_usage_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/usage_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-19 17:45:04.000000 sdkfabric_twitter-3.0.6/src/sdk/user_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:07.970399 sdkfabric_twitter-3.0.6/src/sdkfabric_twitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 17:45:07.000000 sdkfabric_twitter-3.0.6/src/sdkfabric_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-19 17:45:07.000000 sdkfabric_twitter-3.0.6/src/sdkfabric_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:45:07.000000 sdkfabric_twitter-3.0.6/src/sdkfabric_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 17:45:07.000000 sdkfabric_twitter-3.0.6/src/sdkfabric_twitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 17:45:07.000000 sdkfabric_twitter-3.0.6/src/sdkfabric_twitter.egg-info/top_level.txt
```

### Comparing `sdkfabric_twitter-0.1.0/LICENSE` & `sdkfabric_twitter-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/PKG-INFO` & `sdkfabric_twitter-3.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-twitter
-Version: 0.1.0
+Version: 3.0.6
 Summary: Twitter Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/twitter-python
 Project-URL: Issues, https://github.com/sdk-fabric/twitter-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_twitter-0.1.0/README.md` & `sdkfabric_twitter-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/pyproject.toml` & `sdkfabric_twitter-3.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-twitter"
-version = "0.1.0"
+version = "3.0.6"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Twitter Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/bookmark_tag.py` & `sdkfabric_twitter-3.0.6/src/sdk/bookmark_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/client.py` & `sdkfabric_twitter-3.0.6/src/sdk/client.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/fields.py` & `sdkfabric_twitter-3.0.6/src/sdk/fields.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/pagination.py` & `sdkfabric_twitter-3.0.6/src/sdk/pagination.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/quote_tag.py` & `sdkfabric_twitter-3.0.6/src/sdk/quote_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/search_tag.py` & `sdkfabric_twitter-3.0.6/src/sdk/search_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/trends_tag.py` & `sdkfabric_twitter-3.0.6/src/sdk/trends_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/tweet.py` & `sdkfabric_twitter-3.0.6/src/sdk/tweet.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,10 @@
     geo: Optional[TweetGeo] = Field(default=None, alias="geo")
     media: Optional[TweetMedia] = Field(default=None, alias="media")
     poll: Optional[TweetPoll] = Field(default=None, alias="poll")
     quote_tweet_id: Optional[str] = Field(default=None, alias="quote_tweet_id")
     reply: Optional[TweetReply] = Field(default=None, alias="reply")
     reply_settings: Optional[str] = Field(default=None, alias="reply_settings")
     text: Optional[str] = Field(default=None, alias="text")
+    possibly_sensitive: Optional[bool] = Field(default=None, alias="possibly_sensitive")
+    lang: Optional[str] = Field(default=None, alias="lang")
     pass
```

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/tweet_details.py` & `sdkfabric_twitter-3.0.6/src/sdk/tweet_details.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/tweet_reply.py` & `sdkfabric_twitter-3.0.6/src/sdk/tweet_reply.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/tweet_tag.py` & `sdkfabric_twitter-3.0.6/src/sdk/tweet_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/tweet_usage.py` & `sdkfabric_twitter-3.0.6/src/sdk/tweet_usage.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/usage_tag.py` & `sdkfabric_twitter-3.0.6/src/sdk/usage_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/user.py` & `sdkfabric_twitter-3.0.6/src/sdk/user.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-0.1.0/src/sdk/user_tag.py` & `sdkfabric_twitter-3.0.6/src/sdk/user_tag.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,21 +9,80 @@
 from typing import List
 
 from .fields import Fields
 from .like_response import LikeResponse
 from .pagination import Pagination
 from .single_tweet import SingleTweet
 from .tweet_collection import TweetCollection
+from .user import User
 from .user_collection import UserCollection
 
 class UserTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
+    def get_all(self, ids: str, expansions: str, fields: Fields) -> UserCollection:
+        """
+        Returns a variety of information about one or more users specified by the requested IDs.
+        """
+        try:
+            path_params = {}
+
+            query_params = {}
+            query_params["ids"] = ids
+            query_params["expansions"] = expansions
+            query_params["fields"] = fields
+
+            query_struct_names = []
+            query_struct_names.append('fields')
+
+            url = self.parser.url("/2/users", path_params)
+
+            headers = {}
+
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+
+            if response.status_code >= 200 and response.status_code < 300:
+                return UserCollection.model_validate_json(json_data=response.content)
+
+
+            raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
+        except RequestException as e:
+            raise sdkgen.ClientException("An unknown error occurred: " + str(e))
+
+    def get(self, user_id: str, expansions: str, fields: Fields) -> User:
+        """
+        Returns a variety of information about a single user specified by the requested ID.
+        """
+        try:
+            path_params = {}
+            path_params["user_id"] = user_id
+
+            query_params = {}
+            query_params["expansions"] = expansions
+            query_params["fields"] = fields
+
+            query_struct_names = []
+            query_struct_names.append('fields')
+
+            url = self.parser.url("/2/users/:user_id", path_params)
+
+            headers = {}
+
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+
+            if response.status_code >= 200 and response.status_code < 300:
+                return User.model_validate_json(json_data=response.content)
+
+
+            raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
+        except RequestException as e:
+            raise sdkgen.ClientException("An unknown error occurred: " + str(e))
+
     def get_timeline(self, user_id: str, exclude: str, expansions: str, pagination: Pagination, fields: Fields) -> TweetCollection:
         """
         Allows you to retrieve a collection of the most recent Tweets and Retweets posted by you and users you follow. This endpoint can return every Tweet created on a timeline over the last 7 days as well as the most recent 800 regardless of creation date.
         """
         try:
             path_params = {}
             path_params["user_id"] = user_id
```

### Comparing `sdkfabric_twitter-0.1.0/src/sdkfabric_twitter.egg-info/PKG-INFO` & `sdkfabric_twitter-3.0.6/src/sdkfabric_twitter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-twitter
-Version: 0.1.0
+Version: 3.0.6
 Summary: Twitter Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/twitter-python
 Project-URL: Issues, https://github.com/sdk-fabric/twitter-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_twitter-0.1.0/src/sdkfabric_twitter.egg-info/SOURCES.txt` & `sdkfabric_twitter-3.0.6/src/sdkfabric_twitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

