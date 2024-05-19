# Comparing `tmp/sdkfabric_discord-0.1.0.tar.gz` & `tmp/sdkfabric_discord-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_discord-0.1.0.tar", last modified: Sat May 18 16:06:33 2024, max compression
+gzip compressed data, was "sdkfabric_discord-0.2.3.tar", last modified: Sun May 19 18:50:22 2024, max compression
```

## Comparing `sdkfabric_discord-0.1.0.tar` & `sdkfabric_discord-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:06:33.780642 sdkfabric_discord-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-18 16:06:33.780642 sdkfabric_discord-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:06:33.780642 sdkfabric_discord-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:06:33.776642 sdkfabric_discord-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:06:33.776642 sdkfabric_discord-0.1.0/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/src/sdk/channel_message_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/src/sdk/channel_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/src/sdk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/src/sdk/message_allowed_mentions.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/src/sdk/message_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-18 16:06:30.000000 sdkfabric_discord-0.1.0/src/sdk/message_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:06:33.780642 sdkfabric_discord-0.1.0/src/sdkfabric_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-18 16:06:33.000000 sdkfabric_discord-0.1.0/src/sdkfabric_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-18 16:06:33.000000 sdkfabric_discord-0.1.0/src/sdkfabric_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:06:33.000000 sdkfabric_discord-0.1.0/src/sdkfabric_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 16:06:33.000000 sdkfabric_discord-0.1.0/src/sdkfabric_discord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 16:06:33.000000 sdkfabric_discord-0.1.0/src/sdkfabric_discord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:50:22.474665 sdkfabric_discord-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 18:50:22.474665 sdkfabric_discord-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:50:22.474665 sdkfabric_discord-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:50:22.470666 sdkfabric_discord-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:50:22.474665 sdkfabric_discord-0.2.3/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/src/sdk/channel_message_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/src/sdk/channel_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/src/sdk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/src/sdk/message_allowed_mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/src/sdk/message_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-19 18:50:15.000000 sdkfabric_discord-0.2.3/src/sdk/message_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:50:22.474665 sdkfabric_discord-0.2.3/src/sdkfabric_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 18:50:22.000000 sdkfabric_discord-0.2.3/src/sdkfabric_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-19 18:50:22.000000 sdkfabric_discord-0.2.3/src/sdkfabric_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:50:22.000000 sdkfabric_discord-0.2.3/src/sdkfabric_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 18:50:22.000000 sdkfabric_discord-0.2.3/src/sdkfabric_discord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 18:50:22.000000 sdkfabric_discord-0.2.3/src/sdkfabric_discord.egg-info/top_level.txt
```

### Comparing `sdkfabric_discord-0.1.0/LICENSE` & `sdkfabric_discord-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.1.0/PKG-INFO` & `sdkfabric_discord-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-discord
-Version: 0.1.0
+Version: 0.2.3
 Summary: Discord Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/discord-python
 Project-URL: Issues, https://github.com/sdk-fabric/discord-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,19 @@
 please register at the [TypeHub](https://typehub.cloud/) platform and create
 a pull request at the [Discord](https://app.typehub.cloud/d/sdkfabric/discord)
 specification. The system will then automatically create a GIT commit and update
 the code.
 
 ## Usage
 
-The following example shows how you can use the client:
+The following example shows how you initialize the client:
 
 ```python
-const credentials = new HttpBearer('[access_token]');
-const client = Client::build(credentials);
+from sdk.client import Client
+
+client = Client.build("[access_token]")
 
 // @TODO use the client
 ```
+
+You can find all available operations and types at:
+https://app.typehub.cloud/d/sdkfabric/discord
```

### Comparing `sdkfabric_discord-0.1.0/README.md` & `sdkfabric_discord-0.2.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 please register at the [TypeHub](https://typehub.cloud/) platform and create
 a pull request at the [Discord](https://app.typehub.cloud/d/sdkfabric/discord)
 specification. The system will then automatically create a GIT commit and update
 the code.
 
 ## Usage
 
-The following example shows how you can use the client:
+The following example shows how you initialize the client:
 
 ```python
-const credentials = new HttpBearer('[access_token]');
-const client = Client::build(credentials);
+from sdk.client import Client
+
+client = Client.build("[access_token]")
 
 // @TODO use the client
 ```
+
+You can find all available operations and types at:
+https://app.typehub.cloud/d/sdkfabric/discord
```

### Comparing `sdkfabric_discord-0.1.0/pyproject.toml` & `sdkfabric_discord-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-discord"
-version = "0.1.0"
+version = "0.2.3"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Discord Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_discord-0.1.0/src/sdk/channel_message_tag.py` & `sdkfabric_discord-0.2.3/src/sdk/channel_message_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.1.0/src/sdk/client.py` & `sdkfabric_discord-0.2.3/src/sdk/client.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.1.0/src/sdk/message.py` & `sdkfabric_discord-0.2.3/src/sdk/message.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.1.0/src/sdk/message_allowed_mentions.py` & `sdkfabric_discord-0.2.3/src/sdk/message_allowed_mentions.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.1.0/src/sdk/message_embed.py` & `sdkfabric_discord-0.2.3/src/sdk/message_embed.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.1.0/src/sdk/message_reference.py` & `sdkfabric_discord-0.2.3/src/sdk/message_reference.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.1.0/src/sdkfabric_discord.egg-info/PKG-INFO` & `sdkfabric_discord-0.2.3/src/sdkfabric_discord.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-discord
-Version: 0.1.0
+Version: 0.2.3
 Summary: Discord Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/discord-python
 Project-URL: Issues, https://github.com/sdk-fabric/discord-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,19 @@
 please register at the [TypeHub](https://typehub.cloud/) platform and create
 a pull request at the [Discord](https://app.typehub.cloud/d/sdkfabric/discord)
 specification. The system will then automatically create a GIT commit and update
 the code.
 
 ## Usage
 
-The following example shows how you can use the client:
+The following example shows how you initialize the client:
 
 ```python
-const credentials = new HttpBearer('[access_token]');
-const client = Client::build(credentials);
+from sdk.client import Client
+
+client = Client.build("[access_token]")
 
 // @TODO use the client
 ```
+
+You can find all available operations and types at:
+https://app.typehub.cloud/d/sdkfabric/discord
```

