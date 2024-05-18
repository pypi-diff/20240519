# Comparing `tmp/pypki3-2023.353.243.tar.gz` & `tmp/pypki3-2024.139.1394.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypki3-2023.353.243.tar", max compression
+gzip compressed data, was "pypki3-2024.139.1394.tar", max compression
```

## Comparing `pypki3-2023.353.243.tar` & `pypki3-2024.139.1394.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1110 2023-12-19 04:03:18.868021 pypki3-2023.353.243/LICENSE
--rw-r--r--   0        0        0     4188 2023-12-19 04:03:18.868021 pypki3-2023.353.243/README.md
--rw-r--r--   0        0        0      110 2023-12-19 04:03:18.868021 pypki3-2023.353.243/pypki3/README.md
--rw-r--r--   0        0        0      343 2023-12-19 04:03:18.868021 pypki3-2023.353.243/pypki3/__init__.py
--rw-r--r--   0        0        0    13858 2023-12-19 04:03:18.868021 pypki3-2023.353.243/pypki3/config.py
--rw-r--r--   0        0        0       43 2023-12-19 04:03:18.868021 pypki3-2023.353.243/pypki3/exceptions.py
--rw-r--r--   0        0        0      428 2023-12-19 04:03:18.868021 pypki3-2023.353.243/pypki3/utils.py
--rw-r--r--   0        0        0      834 2023-12-19 04:03:35.344017 pypki3-2023.353.243/pyproject.toml
--rw-r--r--   0        0        0     5012 1970-01-01 00:00:00.000000 pypki3-2023.353.243/PKG-INFO
+-rw-r--r--   0        0        0     1110 2024-05-18 23:14:43.652812 pypki3-2024.139.1394/LICENSE
+-rw-r--r--   0        0        0     4188 2024-05-18 23:14:43.652812 pypki3-2024.139.1394/README.md
+-rw-r--r--   0        0        0      110 2024-05-18 23:14:43.652812 pypki3-2024.139.1394/pypki3/README.md
+-rw-r--r--   0        0        0      343 2024-05-18 23:14:43.652812 pypki3-2024.139.1394/pypki3/__init__.py
+-rw-r--r--   0        0        0    14323 2024-05-18 23:14:43.652812 pypki3-2024.139.1394/pypki3/config.py
+-rw-r--r--   0        0        0       43 2024-05-18 23:14:43.652812 pypki3-2024.139.1394/pypki3/exceptions.py
+-rw-r--r--   0        0        0      428 2024-05-18 23:14:43.652812 pypki3-2024.139.1394/pypki3/utils.py
+-rw-r--r--   0        0        0      835 2024-05-18 23:14:53.284719 pypki3-2024.139.1394/pyproject.toml
+-rw-r--r--   0        0        0     5013 1970-01-01 00:00:00.000000 pypki3-2024.139.1394/PKG-INFO
```

### Comparing `pypki3-2023.353.243/LICENSE` & `pypki3-2024.139.1394/LICENSE`

 * *Files identical despite different names*

### Comparing `pypki3-2023.353.243/README.md` & `pypki3-2024.139.1394/README.md`

 * *Files identical despite different names*

### Comparing `pypki3-2023.353.243/pypki3/config.py` & `pypki3-2024.139.1394/pypki3/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from cryptography.hazmat.primitives.serialization.pkcs12 import load_key_and_certificates
 from cryptography.hazmat.primitives.serialization import Encoding, PrivateFormat, NoEncryption
 from cryptography.hazmat.primitives.serialization import load_pem_private_key
 
 from cryptography import x509
 
-from pem import parse as parse_pem
+from pem import parse as parse_pem, PrivateKey, Certificate
 
 from temppath import TemporaryPath, TemporaryPathContext
 
 from .exceptions import Pypki3Exception
 from .utils import in_ipython, in_nbgallery
 
 class ConfigType(Enum):
@@ -189,20 +189,34 @@
 
 def loaded_encoded_pem(key_obj: Any, cert_obj: Any) -> LoadedPKIBytes:
     key_bytes = key_obj.private_bytes(Encoding.PEM, PrivateFormat.PKCS8, NoEncryption())
     cert_bytes = cert_obj.public_bytes(Encoding.PEM)
     return LoadedPKIBytes(key_bytes, cert_bytes)
 
 def separate_pem(pem_data: bytes) -> Tuple[bytes, List[bytes]]:
-    certs = parse_pem(pem_data)
+    pem_objs = parse_pem(pem_data)
+    key = None
+    certs = list()
+    
+    for pem_obj in reversed(pem_objs):
+        if isinstance(pem_obj, PrivateKey):
+            key = pem_obj
+        elif isinstance(pem_obj, Certificate):
+            certs.append(pem_obj)
+
+    if not key and not certs:
+        raise Pypki3Exception('PEM missing key and certificate(s)')
 
-    if len(certs) < 2:
-        raise Pypki3Exception('PEM must contain the key then certificate(s)')
+    if key and not certs:
+        raise Pypki3Exception('PEM contains key but is missing certificate(s)')
 
-    return certs[0].as_bytes(), [x.as_bytes() for x in certs[1:]]
+    if certs and not key:
+        raise Pypki3Exception('PEM contains certificate(s) but is missing key')
+
+    return key.as_bytes(), [cert.as_bytes() for cert in certs]
 
 def find_matching_cert(key_obj: Any, certs_data: List[bytes]) -> Any:
     key_public_num = key_obj.public_key().public_numbers()
 
     for cert_data in certs_data:
         cert_obj = x509.load_pem_x509_certificate(cert_data)
         cert_public_num = cert_obj.public_key().public_numbers()
```

### Comparing `pypki3-2023.353.243/pyproject.toml` & `pypki3-2024.139.1394/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry]
 authors = ["Bill Allen <billallen256@gmail.com>"]
 description = "More user-friendly way to access PKI-enabled services."
 homepage = "http://github.com/nbgallery/pypki3"
 license = "MIT"
 name = "pypki3"
 readme = "README.md"
-version = "2023.353.243"
+version = "2024.139.1394"
 
 [tool.poetry.dependencies]
 python = ">=3.6"
 cryptography = "*"
 pem = "*"
 temppath = "*"
```

### Comparing `pypki3-2023.353.243/PKG-INFO` & `pypki3-2024.139.1394/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypki3
-Version: 2023.353.243
+Version: 2024.139.1394
 Summary: More user-friendly way to access PKI-enabled services.
 Home-page: http://github.com/nbgallery/pypki3
 License: MIT
 Author: Bill Allen
 Author-email: billallen256@gmail.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
```

