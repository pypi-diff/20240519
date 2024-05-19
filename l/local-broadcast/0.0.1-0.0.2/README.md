# Comparing `tmp/local_broadcast-0.0.1.tar.gz` & `tmp/local_broadcast-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_broadcast-0.0.1.tar", last modified: Wed May 15 15:31:32 2024, max compression
+gzip compressed data, was "local_broadcast-0.0.2.tar", last modified: Sun May 19 18:09:31 2024, max compression
```

## Comparing `local_broadcast-0.0.1.tar` & `local_broadcast-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 15:31:32.867555 local_broadcast-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1064 2024-05-15 15:23:05.000000 local_broadcast-0.0.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      791 2024-05-15 15:31:32.867555 local_broadcast-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      162 2024-05-15 15:28:57.000000 local_broadcast-0.0.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      609 2024-05-15 15:31:26.000000 local_broadcast-0.0.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-15 15:31:32.867555 local_broadcast-0.0.1/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 15:31:32.863555 local_broadcast-0.0.1/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 15:31:32.863555 local_broadcast-0.0.1/src/local_broadcast/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-15 15:25:31.000000 local_broadcast-0.0.1/src/local_broadcast/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 15:31:32.867555 local_broadcast-0.0.1/src/local_broadcast.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      791 2024-05-15 15:31:32.000000 local_broadcast-0.0.1/src/local_broadcast.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      278 2024-05-15 15:31:32.000000 local_broadcast-0.0.1/src/local_broadcast.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 15:31:32.000000 local_broadcast-0.0.1/src/local_broadcast.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2024-05-15 15:31:32.000000 local_broadcast-0.0.1/src/local_broadcast.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       16 2024-05-15 15:31:32.000000 local_broadcast-0.0.1/src/local_broadcast.egg-info/top_level.txt
+drwxrwxr-x   0 gambuzzi  (1001) gambuzzi  (1001)        0 2024-05-19 18:09:31.223220 local_broadcast-0.0.2/
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)     1064 2024-05-19 17:42:12.000000 local_broadcast-0.0.2/LICENSE
+-rw-r--r--   0 gambuzzi  (1001) gambuzzi  (1001)     1140 2024-05-19 18:09:31.223220 local_broadcast-0.0.2/PKG-INFO
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)      511 2024-05-19 18:09:04.000000 local_broadcast-0.0.2/README.md
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)      609 2024-05-19 18:04:54.000000 local_broadcast-0.0.2/pyproject.toml
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)       38 2024-05-19 18:09:31.223220 local_broadcast-0.0.2/setup.cfg
+drwxrwxr-x   0 gambuzzi  (1001) gambuzzi  (1001)        0 2024-05-19 18:09:31.215219 local_broadcast-0.0.2/src/
+drwxrwxr-x   0 gambuzzi  (1001) gambuzzi  (1001)        0 2024-05-19 18:09:31.219220 local_broadcast-0.0.2/src/example/
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)     2913 2024-05-19 17:54:58.000000 local_broadcast-0.0.2/src/example/chat_async.py
+drwxrwxr-x   0 gambuzzi  (1001) gambuzzi  (1001)        0 2024-05-19 18:09:31.219220 local_broadcast-0.0.2/src/local_broadcast/
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)     3982 2024-05-19 17:55:11.000000 local_broadcast-0.0.2/src/local_broadcast/__init__.py
+drwxrwxr-x   0 gambuzzi  (1001) gambuzzi  (1001)        0 2024-05-19 18:09:31.223220 local_broadcast-0.0.2/src/local_broadcast.egg-info/
+-rw-r--r--   0 gambuzzi  (1001) gambuzzi  (1001)     1140 2024-05-19 18:09:31.000000 local_broadcast-0.0.2/src/local_broadcast.egg-info/PKG-INFO
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)      304 2024-05-19 18:09:31.000000 local_broadcast-0.0.2/src/local_broadcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)        1 2024-05-19 18:09:31.000000 local_broadcast-0.0.2/src/local_broadcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)       13 2024-05-19 18:09:31.000000 local_broadcast-0.0.2/src/local_broadcast.egg-info/requires.txt
+-rw-rw-r--   0 gambuzzi  (1001) gambuzzi  (1001)       24 2024-05-19 18:09:31.000000 local_broadcast-0.0.2/src/local_broadcast.egg-info/top_level.txt
```

### Comparing `local_broadcast-0.0.1/LICENSE` & `local_broadcast-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `local_broadcast-0.0.1/pyproject.toml` & `local_broadcast-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "local_broadcast"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Roberto Gambuzzi", email="gambuzzi@gmail.com" },
 ]
 description = "A python library to send message to all instances of the current running program on local LAN"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

