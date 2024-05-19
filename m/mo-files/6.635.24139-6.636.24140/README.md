# Comparing `tmp/mo_files-6.635.24139.tar.gz` & `tmp/mo_files-6.636.24140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_files-6.635.24139.tar", last modified: Sat May 18 23:01:40 2024, max compression
+gzip compressed data, was "mo_files-6.636.24140.tar", last modified: Sun May 19 15:30:26 2024, max compression
```

## Comparing `mo_files-6.635.24139.tar` & `mo_files-6.636.24140.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 23:01:40.627528 mo_files-6.635.24139/
--rw-rw-rw-   0        0        0    16725 2019-09-12 21:03:36.000000 mo_files-6.635.24139/LICENSE
--rw-rw-rw-   0        0        0     2204 2024-05-18 23:01:40.626349 mo_files-6.635.24139/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-03-15 11:56:17.000000 mo_files-6.635.24139/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 23:01:40.613495 mo_files-6.635.24139/mo_files/
--rw-rw-rw-   0        0        0    19265 2024-03-02 21:33:58.000000 mo_files-6.635.24139/mo_files/__init__.py
--rw-rw-rw-   0        0        0      431 2024-01-28 14:54:30.000000 mo_files-6.635.24139/mo_files/mimetype.py
--rw-rw-rw-   0        0        0    11596 2024-03-10 19:21:39.000000 mo_files-6.635.24139/mo_files/url.py
-drwxrwxrwx   0        0        0        0 2024-05-18 23:01:40.625229 mo_files-6.635.24139/mo_files.egg-info/
--rw-rw-rw-   0        0        0     2204 2024-05-18 23:01:40.000000 mo_files-6.635.24139/mo_files.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-18 23:01:40.000000 mo_files-6.635.24139/mo_files.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 23:01:40.000000 mo_files-6.635.24139/mo_files.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:35:58.000000 mo_files-6.635.24139/mo_files.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      141 2024-05-18 23:01:40.000000 mo_files-6.635.24139/mo_files.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 23:01:40.000000 mo_files-6.635.24139/mo_files.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 23:01:40.627528 mo_files-6.635.24139/setup.cfg
--rw-rw-rw-   0        0        0     2237 2024-05-18 23:01:35.000000 mo_files-6.635.24139/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:30:26.073794 mo_files-6.636.24140/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 21:03:36.000000 mo_files-6.636.24140/LICENSE
+-rw-rw-rw-   0        0        0     2204 2024-05-19 15:30:26.072794 mo_files-6.636.24140/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-03-15 11:56:17.000000 mo_files-6.636.24140/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 15:30:26.062458 mo_files-6.636.24140/mo_files/
+-rw-rw-rw-   0        0        0    19210 2024-05-19 15:30:17.000000 mo_files-6.636.24140/mo_files/__init__.py
+-rw-rw-rw-   0        0        0      431 2024-01-28 14:54:30.000000 mo_files-6.636.24140/mo_files/mimetype.py
+-rw-rw-rw-   0        0        0    11596 2024-03-10 19:21:39.000000 mo_files-6.636.24140/mo_files/url.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:30:26.071785 mo_files-6.636.24140/mo_files.egg-info/
+-rw-rw-rw-   0        0        0     2204 2024-05-19 15:30:26.000000 mo_files-6.636.24140/mo_files.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-19 15:30:26.000000 mo_files-6.636.24140/mo_files.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 15:30:26.000000 mo_files-6.636.24140/mo_files.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:35:58.000000 mo_files-6.636.24140/mo_files.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      141 2024-05-19 15:30:26.000000 mo_files-6.636.24140/mo_files.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 15:30:26.000000 mo_files-6.636.24140/mo_files.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 15:30:26.073794 mo_files-6.636.24140/setup.cfg
+-rw-rw-rw-   0        0        0     2237 2024-05-19 15:30:21.000000 mo_files-6.636.24140/setup.py
```

### Comparing `mo_files-6.635.24139/LICENSE` & `mo_files-6.636.24140/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_files-6.635.24139/PKG-INFO` & `mo_files-6.636.24140/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-files
-Version: 6.635.24139
+Version: 6.636.24140
 Summary: More Files! Steamlined for UTF8 and JSON.
 Home-page: https://github.com/klahnakoski/mo-files
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -19,15 +19,15 @@
 License-File: LICENSE
 Requires-Dist: mo-dots==10.632.24139
 Requires-Dist: mo-future==7.584.24095
 Requires-Dist: mo-json==6.634.24139
 Requires-Dist: mo-logs==8.632.24139
 Requires-Dist: mo-math==7.632.24139
 Provides-Extra: tests
-Requires-Dist: mo-testing>=8.623.24125; extra == "tests"
+Requires-Dist: mo-testing>=8.633.24139; extra == "tests"
 
 # More Files!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-files.svg)](https://pypi.org/project/mo-files/)
 [![Build Status](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-files/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-files?branch=dev)
 [![Downloads](https://pepy.tech/badge/mo-files/month)](https://pepy.tech/project/mo-files)
```

### Comparing `mo_files-6.635.24139/README.md` & `mo_files-6.636.24140/README.md`

 * *Files identical despite different names*

### Comparing `mo_files-6.635.24139/mo_files/__init__.py` & `mo_files-6.636.24140/mo_files/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 import re
 import shutil
 from datetime import datetime
 from mimetypes import MimeTypes
 from tempfile import NamedTemporaryFile, mkdtemp
 
 from mo_dots import Null, coalesce, get_module, is_list, to_data
-from mo_files import mimetype
-from mo_files.url import URL
 from mo_future import text, is_text, ConfigParser, StringIO
-from mo_logs import Except, Log
+from mo_json import json2value
+from mo_logs import Except, logger
 from mo_logs.exceptions import get_stacktrace
 from mo_math import randoms
 
+from mo_files import mimetype
+from mo_files.url import URL
+
 
 class File(object):
     """
     ASSUMES ALL FILE CONTENT IS UTF8 ENCODED STRINGS
     """
 
     def __new__(cls, filename, key=None, buffering=2 ** 14, suffix=None):
@@ -43,15 +45,15 @@
         :param filename: STRING
         :param key: BASE64 AES KEY USED ON ENCRYPTED FILES
         :param mime_type: IN THE UNLIKELY CASE YOU WISH TO DICTATE THE mimetype
         """
         if isinstance(filename, File):
             return
         elif not is_text(filename):
-            Log.error("Expecting str, not {{type}}", type=type(filename).__name__)
+            logger.error("Expecting str, not {{type}}", type=type(filename).__name__)
 
         self.key = base642bytearray(key)
         self._mime_type = mime_type
 
         if filename == ".":
             self._filename = ""
         elif filename.startswith("~"):
@@ -233,34 +235,31 @@
 
     def read_lines(self, encoding="utf8"):
         with open(self._filename, "rb") as f:
             for line in f:
                 yield line.decode(encoding).rstrip()
 
     def read_json(self, encoding="utf8", flexible=True, leaves=True):
-        from mo_json import json2value
-
         content = self.read(encoding=encoding)
-        value = json2value(content, flexible=flexible)
-        return get_module("mo_json_config").expand(value, "file://" + self.abs_path)
+        return json2value(content, flexible=flexible)
 
     def is_directory(self):
         return os.path.isdir(self._filename)
 
     def read_bytes(self):
         try:
             if not self.parent.exists:
                 self.parent.create()
             with open(self._filename, "rb") as f:
                 if self.key:
                     return get_module("mo_math.crypto").decrypt(f.read(), self.key)
                 else:
                     return f.read()
         except Exception as e:
-            Log.error("Problem reading file {{filename}}", filename=self.abs_path, cause=e)
+            logger.error("Problem reading file {{filename}}", filename=self.abs_path, cause=e)
 
     def write_bytes(self, content):
         if not self.parent.exists:
             self.parent.create()
         with open(self._filename, "wb") as f:
             if self.key:
                 f.write(get_module("mo_math.crypto").encrypt(content, self.key))
@@ -272,26 +271,26 @@
         :param content: text, or iterable of text
         :return:
         """
         if not self.parent.exists:
             self.parent.create()
         with open(self._filename, "wb") as f:
             if is_list(content) and self.key:
-                Log.error("list of data and keys are not supported, encrypt before sending to file")
+                logger.error("list of data and keys are not supported, encrypt before sending to file")
 
             if is_list(content):
                 pass
             elif isinstance(content, text):
                 content = [content]
             elif hasattr(content, "__iter__"):
                 pass
 
             for d in content:
                 if not is_text(d):
-                    Log.error("Expecting unicode data only")
+                    logger.error("Expecting unicode data only")
                 if self.key:
                     from mo_math.aes_crypto import encrypt
 
                     f.write(encrypt(d, self.key).encode("utf8"))
                 else:
                     f.write(d.encode("utf8"))
 
@@ -322,29 +321,29 @@
                     home_path = os.path.expanduser("~")
                     path = home_path + path[1::]
 
                 with io.open(path, "rb") as f:
                     for line in f:
                         yield line.decode("utf8").rstrip()
             except Exception as e:
-                Log.error(
+                logger.error(
                     "Can not read line from {{filename}}", filename=self._filename, cause=e,
                 )
 
         return output()
 
     def append(self, content, encoding="utf8"):
         """
         add a line to file
         """
         if not self.parent.exists:
             self.parent.create()
         with open(self._filename, "ab") as output_file:
             if not is_text(content):
-                Log.error("expecting to write unicode only")
+                logger.error("expecting to write unicode only")
             output_file.write(content.encode(encoding))
             output_file.write(b"\n")
 
     def __len__(self):
         return os.path.getsize(self.abs_path)
 
     def add(self, content):
@@ -353,20 +352,20 @@
     def extend(self, content):
         try:
             if not self.parent.exists:
                 self.parent.create()
             with open(self._filename, "ab") as output_file:
                 for c in content:
                     if not isinstance(c, text):
-                        Log.error("expecting to write unicode only")
+                        logger.error("expecting to write unicode only")
 
                     output_file.write(c.encode("utf8"))
                     output_file.write(b"\n")
         except Exception as e:
-            Log.error("Could not write to file", e)
+            logger.error("Could not write to file", e)
 
     def delete(self):
         try:
             if os.path.isdir(self._filename):
                 shutil.rmtree(self._filename)
             elif os.path.isfile(self._filename):
                 os.remove(self._filename)
@@ -374,15 +373,15 @@
         except Exception as cause:
             cause = Except.wrap(cause)
             if (
                 "The system cannot find the path specified" in cause
                 or "The system cannot find the file specified" in cause
             ):
                 return
-            Log.error("Could not remove file", cause)
+            logger.error("Could not remove file", cause)
 
     def backup(self):
         path = self._filename.split("/")
         names = path[-1].split(".")
         if len(names) == 1 or names[0] == "":
             backup = File(self._filename + ".backup " + datetime.utcnow().strftime("%Y%m%d %H%M%S"))
         else:
@@ -395,15 +394,15 @@
 
     def create(self):
         try:
             os.makedirs(self.os_path)
         except FileExistsError:
             pass
         except Exception as e:
-            Log.error(
+            logger.error(
                 "Could not make directory {{dir_name}}", dir_name=self._filename, cause=e,
             )
 
     @property
     def children(self):
         try:
             return [File(self._filename + "/" + c) for c in os.listdir(self.rel_path)]
@@ -545,15 +544,15 @@
         return bytearray(base64.b64decode(value))
 
 
 def datetime2string(value, format="%Y-%m-%d %H:%M:%S"):
     try:
         return value.strftime(format)
     except Exception as e:
-        Log.error(
+        logger.error(
             "Can not format {{value}} with {{format}}", value=value, format=format, cause=e,
         )
 
 
 def join_path(*path):
     def scrub(i, p):
         p = p.replace(os.sep, "/")
@@ -618,15 +617,15 @@
                 return
             file.delete()
             return
         except Exception as e:
             e = Except.wrap(e)
             e.trace = e.trace[0:2] + caller_stack
             if num_attempts:
-                Log.warning("problem deleting file {{file}}", file=file.abs_path, cause=e)
+                logger.warning("problem deleting file {{file}}", file=file.abs_path, cause=e)
             (Till(seconds=10) | please_stop).wait()
         num_attempts += 1
 
 
 def add_suffix(filename, suffix):
     """
     ADD .suffix TO THE filename (NOT INCLUDING THE FILE EXTENSION)
```

### Comparing `mo_files-6.635.24139/mo_files/url.py` & `mo_files-6.636.24140/mo_files/url.py`

 * *Files identical despite different names*

### Comparing `mo_files-6.635.24139/mo_files.egg-info/PKG-INFO` & `mo_files-6.636.24140/mo_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-files
-Version: 6.635.24139
+Version: 6.636.24140
 Summary: More Files! Steamlined for UTF8 and JSON.
 Home-page: https://github.com/klahnakoski/mo-files
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -19,15 +19,15 @@
 License-File: LICENSE
 Requires-Dist: mo-dots==10.632.24139
 Requires-Dist: mo-future==7.584.24095
 Requires-Dist: mo-json==6.634.24139
 Requires-Dist: mo-logs==8.632.24139
 Requires-Dist: mo-math==7.632.24139
 Provides-Extra: tests
-Requires-Dist: mo-testing>=8.623.24125; extra == "tests"
+Requires-Dist: mo-testing>=8.633.24139; extra == "tests"
 
 # More Files!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-files.svg)](https://pypi.org/project/mo-files/)
 [![Build Status](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-files/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-files?branch=dev)
 [![Downloads](https://pepy.tech/badge/mo-files/month)](https://pepy.tech/project/mo-files)
```

### Comparing `mo_files-6.635.24139/setup.py` & `mo_files-6.636.24140/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Files! Steamlined for UTF8 and JSON.',
-    extras_require={"tests":["mo-testing>=8.623.24125"]},
+    extras_require={"tests":["mo-testing>=8.633.24139"]},
     include_package_data=True,
     install_requires=["mo-dots==10.632.24139","mo-future==7.584.24095","mo-json==6.634.24139","mo-logs==8.632.24139","mo-math==7.632.24139"],
     license='MPL 2.0',
     long_description="# More Files!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-files.svg)](https://pypi.org/project/mo-files/)\n[![Build Status](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-files/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-files?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-files/month)](https://pepy.tech/project/mo-files)\n\nThe `File` class makes the default assumption all files have cr-delimited unicode content that is UTF-8 encoded. This is great for JSON files. It also provides better operators over some common file manipulations.\n\n\n\n\n## Recent changes\n\n**Version 6.x**\n\nGet a little closer to Python's pathlib module standards\n\n* `stem` - to refer file name without extension\n* `os_path` - to get the os-specific absolute path for use in other Python modules\n* `rel_path` - the given path \n* `abs_path` - was `abspath`, added underscore for consistency \n\n\n\n",
     long_description_content_type='text/markdown',
     name='mo-files',
     packages=["mo_files"],
     url='https://github.com/klahnakoski/mo-files',
-    version='6.635.24139',
+    version='6.636.24140',
     zip_safe=False
 )
```

