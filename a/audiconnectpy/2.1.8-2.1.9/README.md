# Comparing `tmp/audiconnectpy-2.1.8.tar.gz` & `tmp/audiconnectpy-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.1.8.tar", last modified: Sun May 19 13:58:19 2024, max compression
+gzip compressed data, was "audiconnectpy-2.1.9.tar", last modified: Sun May 19 16:57:54 2024, max compression
```

## Comparing `audiconnectpy-2.1.8.tar` & `audiconnectpy-2.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.623786 audiconnectpy-2.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.623786 audiconnectpy-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.623786 audiconnectpy-2.1.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26001 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:57:54.113718 audiconnectpy-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:57:54.105718 audiconnectpy-2.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:57:54.105718 audiconnectpy-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:57:54.105718 audiconnectpy-2.1.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 16:57:54.113718 audiconnectpy-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:57:54.109718 audiconnectpy-2.1.9/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26067 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:57:54.113718 audiconnectpy-2.1.9/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 16:57:54.000000 audiconnectpy-2.1.9/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 16:57:54.000000 audiconnectpy-2.1.9/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 16:57:54.000000 audiconnectpy-2.1.9/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 16:57:53.000000 audiconnectpy-2.1.9/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 16:57:54.000000 audiconnectpy-2.1.9/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 16:57:54.000000 audiconnectpy-2.1.9/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 16:57:54.113718 audiconnectpy-2.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:57:54.109718 audiconnectpy-2.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:57:54.109718 audiconnectpy-2.1.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-19 16:57:43.000000 audiconnectpy-2.1.9/tests/test_home.py
```

### Comparing `audiconnectpy-2.1.8/.github/dependabot.yml` & `audiconnectpy-2.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/.github/workflows/auto-approve.yml` & `audiconnectpy-2.1.9/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.1.9/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.1.9/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/.github/workflows/release.yml` & `audiconnectpy-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/.gitignore` & `audiconnectpy-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/.pre-commit-config.yaml` & `audiconnectpy-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/LICENSE` & `audiconnectpy-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/PKG-INFO` & `audiconnectpy-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.1.8
+Version: 2.1.9
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.1.8/README.md` & `audiconnectpy-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/audiconnectpy/api.py` & `audiconnectpy-2.1.9/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/audiconnectpy/auth.py` & `audiconnectpy-2.1.9/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/audiconnectpy/const.py` & `audiconnectpy-2.1.9/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/audiconnectpy/helpers.py` & `audiconnectpy-2.1.9/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/audiconnectpy/model.py` & `audiconnectpy-2.1.9/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/audiconnectpy/vehicle.py` & `audiconnectpy-2.1.9/audiconnectpy/vehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     """Vehicle class."""
 
     vin: str
     csid: str
     nickname: str | None = None
     last_access: datetime | None = None
     uris: dict[str, str] = field(init=False)
-    spin: str = field(init=False)
     auth: Any = field(init=False)
+    spin: str | None = field(init=False, default=None)
     infos: Information | None = field(
         metadata=field_options(alias="vehicle"), default=None
     )
     capabilities: list[str] | None = field(init=False, default=None)
     position: Position | None = field(init=False, default=None)
     location: Location | None = field(init=False, default=None)
 
@@ -633,15 +633,17 @@
                 break
 
         if stauts_good is False:
             raise TimeoutExceededError(("Cannot %s, operation timed out", action))
 
     async def _async_get_security_token(self, action: str) -> str:
         """Get security token."""
-        self.spin = "" if self.spin is None else self.spin
+        if self.spin is None:
+            logging.error("Security PIN not found")
+            return ""
 
         # Challenge
         headers = await self.auth.async_get_headers(token_type="mbb", okhttp=True)
         rsp = await self.auth.request(
             "GET",
             f"{self.uris['url_setter']}/rolesrights/authorization/v2/vehicles/{self.vin}/services/{action}/security-pin-auth-requested",
             headers=headers,
```

### Comparing `audiconnectpy-2.1.8/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.1.9/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.1.8
+Version: 2.1.9
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.1.8/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.1.9/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/pyproject.toml` & `audiconnectpy-2.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/tests/conftest.py` & `audiconnectpy-2.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/tests/fixtures/audi0.json` & `audiconnectpy-2.1.9/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/tests/fixtures/audi1.json` & `audiconnectpy-2.1.9/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/tests/fixtures/audi2.json` & `audiconnectpy-2.1.9/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.1.9/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/tests/fixtures/location.json` & `audiconnectpy-2.1.9/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.8/tests/test_home.py` & `audiconnectpy-2.1.9/tests/test_home.py`

 * *Files identical despite different names*

