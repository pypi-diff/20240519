# Comparing `tmp/ddge-0.2.137.2.tar.gz` & `tmp/ddge-0.2.137.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddge-0.2.137.2.tar", last modified: Fri Sep 22 09:04:47 2023, max compression
+gzip compressed data, was "ddge-0.2.137.3.tar", last modified: Sun May 19 09:20:19 2024, max compression
```

## Comparing `ddge-0.2.137.2.tar` & `ddge-0.2.137.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:04:47.141348 ddge-0.2.137.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-22 09:04:41.000000 ddge-0.2.137.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-09-22 09:04:47.141348 ddge-0.2.137.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-09-22 09:04:41.000000 ddge-0.2.137.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:04:47.137348 ddge-0.2.137.2/ddge/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-22 09:04:41.000000 ddge-0.2.137.2/ddge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-22 09:04:41.000000 ddge-0.2.137.2/ddge/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2023-09-22 09:04:41.000000 ddge-0.2.137.2/ddge/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2023-09-22 09:04:41.000000 ddge-0.2.137.2/ddge/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2023-09-22 09:04:41.000000 ddge-0.2.137.2/ddge/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:04:47.141348 ddge-0.2.137.2/ddge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-09-22 09:04:47.000000 ddge-0.2.137.2/ddge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-09-22 09:04:47.000000 ddge-0.2.137.2/ddge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 09:04:47.000000 ddge-0.2.137.2/ddge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-22 09:04:47.000000 ddge-0.2.137.2/ddge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-22 09:04:47.000000 ddge-0.2.137.2/ddge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-09-22 09:04:47.000000 ddge-0.2.137.2/ddge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-09-22 09:04:41.000000 ddge-0.2.137.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 09:04:47.141348 ddge-0.2.137.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-09-22 09:04:41.000000 ddge-0.2.137.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:20:19.589541 ddge-0.2.137.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 09:20:11.000000 ddge-0.2.137.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-19 09:20:19.589541 ddge-0.2.137.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-19 09:20:11.000000 ddge-0.2.137.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:20:19.589541 ddge-0.2.137.3/ddge/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 09:20:11.000000 ddge-0.2.137.3/ddge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 09:20:11.000000 ddge-0.2.137.3/ddge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-19 09:20:11.000000 ddge-0.2.137.3/ddge/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-19 09:20:11.000000 ddge-0.2.137.3/ddge/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-19 09:20:11.000000 ddge-0.2.137.3/ddge/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:20:19.589541 ddge-0.2.137.3/ddge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-19 09:20:19.000000 ddge-0.2.137.3/ddge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 09:20:19.000000 ddge-0.2.137.3/ddge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:20:19.000000 ddge-0.2.137.3/ddge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 09:20:19.000000 ddge-0.2.137.3/ddge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 09:20:19.000000 ddge-0.2.137.3/ddge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-19 09:20:19.000000 ddge-0.2.137.3/ddge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-19 09:20:11.000000 ddge-0.2.137.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 09:20:19.589541 ddge-0.2.137.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-19 09:20:11.000000 ddge-0.2.137.3/setup.py
```

### Comparing `ddge-0.2.137.2/LICENSE` & `ddge-0.2.137.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ddge-0.2.137.2/README.md` & `ddge-0.2.137.3/README.md`

 * *Files identical despite different names*

### Comparing `ddge-0.2.137.2/ddge/api.py` & `ddge-0.2.137.3/ddge/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         return d
 
     def full_login(self, otp: str, username: str | None = None):
         token = self.login(otp, username)
         self.token = token
         res = self.dashboard()
         self.access_token = res['user']['access_token']
-        self.real_email = res['user']['eamil']
+        self.real_email = res['user']['email']
         self.generated_addresses = res['stats']['addresses_generated']
         self.logged_in = True
         return True
 
     def generate_alias(self) -> str:
         headers = {**self.headers, "Authorization": f"Bearer {self.access_token}"}
         req = self.session.post(f"{API_BASE}{GEN_EMAIL}", headers=headers)
```

### Comparing `ddge-0.2.137.2/ddge/cli.py` & `ddge-0.2.137.3/ddge/cli.py`

 * *Files identical despite different names*

### Comparing `ddge-0.2.137.2/ddge/storage.py` & `ddge-0.2.137.3/ddge/storage.py`

 * *Files identical despite different names*

### Comparing `ddge-0.2.137.2/setup.py` & `ddge-0.2.137.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open(path) as fp:
         dependencies = (d.strip() for d in fp.read().split("\n") if d.strip())
         return [d for d in dependencies if not d.startswith("#")]
 
 
 setuptools.setup(
     name="ddge",
-    version='0.2.137.2',
+    version='0.2.137.3',
     description="DuckDuckGo Email Protection CLI",
     long_description=long_description(),
     long_description_content_type="text/markdown",
     author="Zoey !",
     maintainer_email="cb98uzhd@duck.com",
     license='GNU General Public License v3.0',
     url="https://github.com/lzgirlcat/ddge",
```

