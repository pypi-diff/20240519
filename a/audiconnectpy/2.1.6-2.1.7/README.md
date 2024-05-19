# Comparing `tmp/audiconnectpy-2.1.6.tar.gz` & `tmp/audiconnectpy-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.1.6.tar", last modified: Sat May 18 17:26:12 2024, max compression
+gzip compressed data, was "audiconnectpy-2.1.7.tar", last modified: Sun May 19 11:26:52 2024, max compression
```

## Comparing `audiconnectpy-2.1.6.tar` & `audiconnectpy-2.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:26:12.509027 audiconnectpy-2.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:26:12.505027 audiconnectpy-2.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:26:12.505027 audiconnectpy-2.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:26:12.505027 audiconnectpy-2.1.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 17:26:12.509027 audiconnectpy-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:26:12.505027 audiconnectpy-2.1.6/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26001 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:26:12.509027 audiconnectpy-2.1.6/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 17:26:12.000000 audiconnectpy-2.1.6/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-18 17:26:12.000000 audiconnectpy-2.1.6/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:26:12.000000 audiconnectpy-2.1.6/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:26:12.000000 audiconnectpy-2.1.6/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 17:26:12.000000 audiconnectpy-2.1.6/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 17:26:12.000000 audiconnectpy-2.1.6/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 17:26:12.509027 audiconnectpy-2.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:26:12.509027 audiconnectpy-2.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:26:12.509027 audiconnectpy-2.1.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-18 17:25:56.000000 audiconnectpy-2.1.6/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.202625 audiconnectpy-2.1.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.202625 audiconnectpy-2.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.202625 audiconnectpy-2.1.7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.202625 audiconnectpy-2.1.7/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26001 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:26:51.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/test_home.py
```

### Comparing `audiconnectpy-2.1.6/.github/dependabot.yml` & `audiconnectpy-2.1.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/.github/workflows/auto-approve.yml` & `audiconnectpy-2.1.7/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.1.7/.github/workflows/pythonpackage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 jobs:
   build:
     runs-on: ubuntu-latest
     name: Check the code
     strategy:
       max-parallel: 4
       matrix:
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.10", "3.11", "3.12"]
 
     steps:
       - name: 📥 Checkout the repository
         uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
```

### Comparing `audiconnectpy-2.1.6/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.1.7/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/.github/workflows/release.yml` & `audiconnectpy-2.1.7/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           tag_name: ${{ github.ref }}
           release_name: ${{ github.ref }}
           body: ${{ steps.changelog.outputs.changelog }}
           draft: false
-          prerelease: false
+          prerelease: ${{ contains(github.ref_name,'-') }}
```

### Comparing `audiconnectpy-2.1.6/.gitignore` & `audiconnectpy-2.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/.pre-commit-config.yaml` & `audiconnectpy-2.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/LICENSE` & `audiconnectpy-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/PKG-INFO` & `audiconnectpy-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.1.6
+Version: 2.1.7
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.1.6/README.md` & `audiconnectpy-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/audiconnectpy/api.py` & `audiconnectpy-2.1.7/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/audiconnectpy/auth.py` & `audiconnectpy-2.1.7/audiconnectpy/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         # IDK token
         self._idk_token = await self._async_get_idk_token(
             code=authcode_strings["code"][0], code_verifier=code_verifier
         )
 
         # Audi token
         self._audi_token = await self._async_get_azs_token(
-            id_token=self._idk_token["id_token"]
+            id_token=self._idk_token["access_token"]
         )
 
         # mbboauth client register
         self._x_client_id = await self._async_register_idk()
 
         # MBB token
         self._mbb_token = await self._async_get_mbb_token(
@@ -306,15 +306,15 @@
                 # IDK Token
                 self._idk_token = await self._async_get_idk_token(
                     refresh_token=self._idk_token["refresh_token"]
                 )
 
                 # Audi token
                 self._audi_token = await self._async_get_azs_token(
-                    id_token=self._idk_token["id_token"]
+                    id_token=self._idk_token["access_token"]
                 )
 
                 # Here token
                 self._here_token = await self._async_get_here_token(
                     id_token=self._idk_token["id_token"]
                 )
```

### Comparing `audiconnectpy-2.1.6/audiconnectpy/const.py` & `audiconnectpy-2.1.7/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/audiconnectpy/helpers.py` & `audiconnectpy-2.1.7/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/audiconnectpy/model.py` & `audiconnectpy-2.1.7/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/audiconnectpy/vehicle.py` & `audiconnectpy-2.1.7/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.1.7/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.1.6
+Version: 2.1.7
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.1.6/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.1.7/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/example.py` & `audiconnectpy-2.1.7/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/pyproject.toml` & `audiconnectpy-2.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/tests/conftest.py` & `audiconnectpy-2.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/tests/fixtures/audi0.json` & `audiconnectpy-2.1.7/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.1.7/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/tests/fixtures/location.json` & `audiconnectpy-2.1.7/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.6/tests/test_home.py` & `audiconnectpy-2.1.7/tests/test_home.py`

 * *Files identical despite different names*

