# Comparing `tmp/haondt_charon-1.0.4.tar.gz` & `tmp/haondt_charon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haondt_charon-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "haondt_charon-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `haondt_charon-1.0.4.tar` & `haondt_charon-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0       39 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/.gitignore
--rw-r--r--   0        0        0      169 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/.gitlab-ci.yml
--rw-r--r--   0        0        0      206 2024-05-03 22:30:54.865617 haondt_charon-1.0.4/Dockerfile
--rw-r--r--   0        0        0     1081 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/LICENSE
--rw-r--r--   0        0        0     5755 2024-05-03 22:30:54.865617 haondt_charon-1.0.4/README.md
--rw-r--r--   0        0        0     1054 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon.yml
--rw-r--r--   0        0        0        0 2024-05-03 22:30:54.933617 haondt_charon-1.0.4/charon/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/__main__.py
--rw-r--r--   0        0        0       45 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/destinations/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/destinations/gcp_bucket.py
--rw-r--r--   0        0        0     1164 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/destinations/local.py
--rw-r--r--   0        0        0       50 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/requirements.txt
--rw-r--r--   0        0        0     2532 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/scheduling.py
--rw-r--r--   0        0        0     2369 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/shared.py
--rw-r--r--   0        0        0      107 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/sources/__init__.py
--rw-r--r--   0        0        0     2145 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/sources/http.py
--rw-r--r--   0        0        0     2010 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/sources/lib.py
--rw-r--r--   0        0        0     1350 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/sources/local.py
--rw-r--r--   0        0        0     1312 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/styx.py
--rw-r--r--   0        0        0      314 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/docker-compose.yml
--rw-r--r--   0        0        0      468 2024-05-03 22:30:54.865617 haondt_charon-1.0.4/pipeline.yml
--rw-r--r--   0        0        0      742 2024-05-03 22:30:55.501625 haondt_charon-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      493 2024-04-29 01:45:23.306231 haondt_charon-1.0.4/tests/charon.test.yml
--rwxr-xr-x   0        0        0      561 2024-04-29 01:45:23.306231 haondt_charon-1.0.4/tests/test.sh
--rwxr-xr-x   0        0        0      787 2024-04-29 01:45:23.310231 haondt_charon-1.0.4/tests/test2.sh
--rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 haondt_charon-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/.gitignore
+-rw-r--r--   0        0        0      169 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      206 2024-05-03 22:30:54.865617 haondt_charon-1.1.0/Dockerfile
+-rw-r--r--   0        0        0     1081 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5755 2024-05-03 22:30:54.865617 haondt_charon-1.1.0/README.md
+-rw-r--r--   0        0        0     1054 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon.yml
+-rw-r--r--   0        0        0        0 2024-05-19 15:19:09.352337 haondt_charon-1.1.0/charon/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/__main__.py
+-rw-r--r--   0        0        0       45 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/destinations/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/destinations/gcp_bucket.py
+-rw-r--r--   0        0        0     1164 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/destinations/local.py
+-rw-r--r--   0        0        0       50 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/requirements.txt
+-rw-r--r--   0        0        0     2532 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/scheduling.py
+-rw-r--r--   0        0        0     2434 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/shared.py
+-rw-r--r--   0        0        0      138 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/__init__.py
+-rw-r--r--   0        0        0     1901 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/http.py
+-rw-r--r--   0        0        0     2431 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/lib.py
+-rw-r--r--   0        0        0     1024 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/local.py
+-rw-r--r--   0        0        0     1378 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/sqlite.py
+-rw-r--r--   0        0        0     1312 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/styx.py
+-rw-r--r--   0        0        0      314 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/docker-compose.yml
+-rw-r--r--   0        0        0      468 2024-05-03 22:30:54.865617 haondt_charon-1.1.0/pipeline.yml
+-rw-r--r--   0        0        0      742 2024-05-19 15:19:10.156346 haondt_charon-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      788 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/tests/charon.test.yml
+-rwxr-xr-x   0        0        0      682 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/tests/test.sh
+-rwxr-xr-x   0        0        0      923 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/tests/test2.sh
+-rwxr-xr-x   0        0        0      948 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/tests/test3.sh
+-rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 haondt_charon-1.1.0/PKG-INFO
```

### Comparing `haondt_charon-1.0.4/LICENSE` & `haondt_charon-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.4/README.md` & `haondt_charon-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.4/charon.yml` & `haondt_charon-1.1.0/charon.yml`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.4/charon/__main__.py` & `haondt_charon-1.1.0/charon/__main__.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.4/charon/destinations/gcp_bucket.py` & `haondt_charon-1.1.0/charon/destinations/gcp_bucket.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.4/charon/destinations/local.py` & `haondt_charon-1.1.0/charon/destinations/local.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.4/charon/scheduling.py` & `haondt_charon-1.1.0/charon/scheduling.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.4/charon/shared.py` & `haondt_charon-1.1.0/charon/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     destinations.gcp_bucket.configure(config.get('gcp_buckets', {}))
 
 def source_factory(source_type):
     if (source_type == 'local'):
         return  sources.local
     if (source_type == 'http'):
         return  sources.http
+    if (source_type == 'sqlite'):
+        return  sources.sqlite
     raise KeyError(f'unknown source type: {source_type}')
 
 def destination_factory(destination_type):
     if (destination_type == 'local'):
         return destinations.local
     if (destination_type == 'gcp_bucket'):
         return destinations.gcp_bucket
```

### Comparing `haondt_charon-1.0.4/charon/sources/http.py` & `haondt_charon-1.1.0/charon/sources/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import tempfile
 import os
 import requests
 from requests.models import HTTPError
-from .lib import _validate_and_decode_encryption_key, _tar, _untar, _encrypt, _decrypt, _get_file_extension
-
-
+from .lib import _validate_and_decode_encryption_key, _untar, _decrypt, _get_file_extension, _export_data
 
 def task_factory(name, config):
     url = config['url']
     encryption_key = config.get('encrypt')
-    encrypt = encryption_key is not None
-    if encrypt:
+    if encryption_key is not None:
         _validate_and_decode_encryption_key(encryption_key)
 
     headers = {}
     auth = config.get('auth')
     if auth is not None:
         if 'bearer' in auth:
             headers['Authorization'] = f'Bearer {auth["bearer"]}'
@@ -25,34 +22,27 @@
         method = method.upper(),
         url = url,
         headers = headers
     ).prepare()
 
     def task(output_file: str):
         nonlocal encryption_key
-        nonlocal encrypt
         nonlocal name
         nonlocal request
         nonlocal extension
 
         response = requests.Session().send(request, allow_redirects=False, timeout=30)
         if response.status_code != 200:
             raise HTTPError(f"received status code {response.status_code}")
 
         with tempfile.TemporaryDirectory() as td:
             initial_file_path = os.path.join(td, f'{name}.{extension}')
             with open(initial_file_path, 'w') as f:
                 f.write(response.text)
-
-            if encrypt:
-                tar_file = os.path.join(td, f'{name}.tar.gz')
-                _tar(initial_file_path, tar_file)
-                _encrypt(encryption_key, tar_file, output_file)
-            else:
-                _tar(initial_file_path, output_file)
+            _export_data(name, initial_file_path, output_file, encryption_key)
 
     return task, _get_file_extension(config)
 
 def revert(config, input_file, output_dir='.'):
     encryption_key = config.get('encrypt')
     encrypt = encryption_key is not None
     if encrypt:
```

### Comparing `haondt_charon-1.0.4/charon/sources/lib.py` & `haondt_charon-1.1.0/charon/sources/lib.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import os, tarfile
+import os, tarfile, tempfile
 from cryptography.fernet import Fernet
 from base64 import urlsafe_b64encode
 
 def _get_file_extension(config):
     if 'encrypt' in config:
         return 'enc'
     return 'tar.gz'
 
-def _validate_and_decode_encryption_key(encryption_key):
+def _validate_and_decode_encryption_key(encryption_key) -> bytes:
     encryption_bytes = bytes.fromhex(encryption_key)
     if len(encryption_bytes) != 32:
         raise ValueError("encryption key must be 32 bytes long")
     return encryption_bytes
 
 def _encrypt(encryption_key, input_file, output_file):
     encryption_bytes = _validate_and_decode_encryption_key(encryption_key)
-    fernet = Fernet(urlsafe_b64encode(encryption_bytes).decode())
+    fernet = Fernet(urlsafe_b64encode(encryption_bytes))
     with open(input_file, 'rb') as f:
         original = f.read()
     encrypted  = fernet.encrypt(original)
 
     with open(output_file, 'wb') as f:
         f.write(encrypted)
 
 def _decrypt(encryption_key, input_file, output_file):
     encryption_bytes = _validate_and_decode_encryption_key(encryption_key)
-    fernet = Fernet(urlsafe_b64encode(encryption_bytes).decode())
+    fernet = Fernet(urlsafe_b64encode(encryption_bytes))
     with open(input_file, 'rb') as f:
         encrypted = f.read()
     original  = fernet.decrypt(encrypted)
 
     with open(output_file, 'wb') as f:
         f.write(original)
 
@@ -54,7 +54,17 @@
         os.chdir(current_dir)
 
 def _untar(input_file, output_dir):
     if not os.path.exists(input_file):
         raise FileNotFoundError(input_file)
     with tarfile.open(input_file, "r:gz") as tar:
         tar.extractall(output_dir)
+
+def _export_data(name, input_path, output_file, encryption_key: str | None=None):
+    if encryption_key is not None:
+        with tempfile.TemporaryDirectory() as td:
+            tar_file = f'{name}.tar.gz'
+            tar_file_path = os.path.join(td, tar_file)
+            _tar(input_path, tar_file_path)
+            _encrypt(encryption_key, tar_file_path, output_file)
+    else:
+        _tar(input_path, output_file)
```

### Comparing `haondt_charon-1.0.4/charon/styx.py` & `haondt_charon-1.1.0/charon/styx.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.4/pyproject.toml` & `haondt_charon-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "flit_core >=3.2,<4",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "haondt_charon"
 classifiers = [ "License :: OSI Approved :: MIT License",]
 description = "charon is a utility for backing up data from one location to another at regular intervals."
-version = "1.0.4"
+version = "1.1.0"
 readme = "README.md"
 keywords = [ "backup", "recovery",]
 dependencies = [ "croniter>=2.0.5", "PyYAML>=6.0.1", "cryptography>=42.0.5", "google-cloud-storage>=2.16.0",]
 [[project.authors]]
 name = "haondt"
 
 [project.license]
```

### Comparing `haondt_charon-1.0.4/tests/test2.sh` & `haondt_charon-1.1.0/tests/test.sh`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #!/bin/bash
 
-mkdir -p input_directory/nested_directory
-echo "this is the foo file" > input_directory/file1.txt
-echo "this is the baz file" > input_directory/nested_directory/file2.txt
-python3 ../charon.py -f charon.test.yml styx apply test_2
+# tests individual files + encryption
+
+export PYTHONPATH="../"
+echo "this is some testing text" > first_file.txt
+python3 -m charon -f charon.test.yml styx apply test_1
 mkdir revert_output
-python3 ../charon.py -f charon.test.yml styx revert test_2 revert_output
-tree revert_output
-cat revert_output/file1.txt
-cat revert_output/nested_directory/file2.txt
-rm -r revert_output apply_archive.tar.gz input_directory
-
-# expected output:
-# -----------------
-# applying job: test_2
-# reverting job: test_2 into /home/noah/projects/charon/tests/revert_output
-# revert_output
-# ├── file1.txt
-# └── nested_directory
-#     └── file2.txt
-#
-# 1 directory, 2 files
-# this is the foo file
-# this is the baz file
+python3 -m charon -f charon.test.yml styx revert test_1 revert_output
+
+
+expected_output="revert_output
+└── first_file.txt
+
+0 directories, 1 file
+this is some testing text"
+
+real_output="$(tree revert_output)
+$(cat revert_output/first_file.txt)"
+
+if [ "$real_output" == "$expected_output" ]; then
+    echo "test passed!"
+else
+    echo "test failed!"
+    diff -y <(echo "$expected_output") <(echo "$real_output")
+fi
+
+rm -r revert_output apply_output first_file.txt 2>/dev/null
```

### Comparing `haondt_charon-1.0.4/PKG-INFO` & `haondt_charon-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haondt_charon
-Version: 1.0.4
+Version: 1.1.0
 Summary: charon is a utility for backing up data from one location to another at regular intervals.
 Keywords: backup,recovery
 Author: haondt
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: croniter>=2.0.5
 Requires-Dist: PyYAML>=6.0.1
```

