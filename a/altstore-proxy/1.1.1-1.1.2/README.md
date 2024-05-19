# Comparing `tmp/altstore_proxy-1.1.1.tar.gz` & `tmp/altstore_proxy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.1.1.tar", last modified: Sat May 18 18:52:55 2024, max compression
+gzip compressed data, was "altstore_proxy-1.1.2.tar", last modified: Sat May 18 19:05:37 2024, max compression
```

## Comparing `altstore_proxy-1.1.1.tar` & `altstore_proxy-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/setup.py
```

### Comparing `altstore_proxy-1.1.1/PKG-INFO` & `altstore_proxy-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore_proxy
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/docker-altstore-proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.1.1/README.md` & `altstore_proxy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.1.1/altstore_proxy/proxy.py` & `altstore_proxy-1.1.2/altstore_proxy/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,16 +201,16 @@
                     button:hover {{
                         background-color: #45a049;
                     }}
                 </style>
             </head>
             <body>
                 <h1>AltStore-Proxy</h1>
-                <a href="/apps.json">View apps.json</a><br>
-                <a href="altstore://source?url={shared_state.values["baseurl"]}">
+                <a href="/apps.json">Source for use in AltStore</a><br>
+                <a href="altstore://source?url={shared_state.values["baseurl"]}/apps.json">
                     <button>Add this source to AltStore to receive app updates</button>
                 </a>
                 <h2>Source Repositories</h2>
                 <ul>
                     {repos_html}
                 </ul>
             </body>
```

### Comparing `altstore_proxy-1.1.1/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.1.2/altstore_proxy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore-proxy
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/docker-altstore-proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.1.1/setup.py` & `altstore_proxy-1.1.2/setup.py`

 * *Files identical despite different names*

