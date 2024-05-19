# Comparing `tmp/astrometry_net_client-0.4.0.tar.gz` & `tmp/astrometry_net_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrometry_net_client-0.4.0.tar", last modified: Sun May  5 12:28:02 2024, max compression
+gzip compressed data, was "astrometry_net_client-0.5.0.tar", last modified: Sun May 19 19:19:33 2024, max compression
```

## Comparing `astrometry_net_client-0.4.0.tar` & `astrometry_net_client-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/
--rw-r--r--   0 sten      (1000) sten      (1000)     1067 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/LICENSE
--rw-r--r--   0 sten      (1000) sten      (1000)     6382 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/PKG-INFO
--rw-r--r--   0 sten      (1000) sten      (1000)     5396 2022-08-30 09:48:22.000000 astrometry_net_client-0.4.0/README.rst
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-05 12:28:02.252670 astrometry_net_client-0.4.0/astrometry_net_client/
--rw-r--r--   0 sten      (1000) sten      (1000)      345 2022-11-02 18:32:15.000000 astrometry_net_client-0.4.0/astrometry_net_client/__init__.py
--rw-r--r--   0 sten      (1000) sten      (1000)     8524 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/astrometry_net_client/client.py
--rw-r--r--   0 sten      (1000) sten      (1000)      490 2024-02-18 13:44:35.000000 astrometry_net_client-0.4.0/astrometry_net_client/config.py
--rw-r--r--   0 sten      (1000) sten      (1000)      663 2022-11-02 18:32:13.000000 astrometry_net_client-0.4.0/astrometry_net_client/exceptions.py
--rw-r--r--   0 sten      (1000) sten      (1000)     6658 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/astrometry_net_client/request.py
--rw-r--r--   0 sten      (1000) sten      (1000)     5036 2022-11-02 18:32:23.000000 astrometry_net_client-0.4.0/astrometry_net_client/session.py
--rw-r--r--   0 sten      (1000) sten      (1000)     8088 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/astrometry_net_client/settings.py
--rw-r--r--   0 sten      (1000) sten      (1000)    16640 2024-02-18 13:44:35.000000 astrometry_net_client-0.4.0/astrometry_net_client/statusables.py
--rw-r--r--   0 sten      (1000) sten      (1000)     5028 2024-02-18 13:44:35.000000 astrometry_net_client-0.4.0/astrometry_net_client/uploads.py
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/
--rw-r--r--   0 sten      (1000) sten      (1000)     6382 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/PKG-INFO
--rw-r--r--   0 sten      (1000) sten      (1000)      731 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/SOURCES.txt
--rw-r--r--   0 sten      (1000) sten      (1000)        1 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/dependency_links.txt
--rw-r--r--   0 sten      (1000) sten      (1000)       24 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/requires.txt
--rw-r--r--   0 sten      (1000) sten      (1000)       22 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/top_level.txt
--rw-r--r--   0 sten      (1000) sten      (1000)      273 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/setup.cfg
--rw-r--r--   0 sten      (1000) sten      (1000)     1197 2024-05-05 12:23:34.000000 astrometry_net_client-0.4.0/setup.py
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/tests/
--rw-r--r--   0 sten      (1000) sten      (1000)     2992 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test.py
--rw-r--r--   0 sten      (1000) sten      (1000)     1660 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/tests/test_client.py
--rw-r--r--   0 sten      (1000) sten      (1000)     2489 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test_job.py
--rw-r--r--   0 sten      (1000) sten      (1000)     2352 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/tests/test_online.py
--rw-r--r--   0 sten      (1000) sten      (1000)     1736 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test_session.py
--rw-r--r--   0 sten      (1000) sten      (1000)     3673 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test_settings.py
--rw-r--r--   0 sten      (1000) sten      (1000)     2987 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test_statusables.py
--rw-r--r--   0 sten      (1000) sten      (1000)     1618 2024-02-18 13:44:35.000000 astrometry_net_client-0.4.0/tests/test_upload.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-19 19:19:33.034802 astrometry_net_client-0.5.0/
+-rw-r--r--   0 sten      (1000) sten      (1000)     1067 2022-08-30 07:13:54.000000 astrometry_net_client-0.5.0/LICENSE
+-rw-r--r--   0 sten      (1000) sten      (1000)     6783 2024-05-19 19:19:33.034802 astrometry_net_client-0.5.0/PKG-INFO
+-rw-r--r--   0 sten      (1000) sten      (1000)     5695 2024-05-19 18:38:50.000000 astrometry_net_client-0.5.0/README.rst
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-19 19:19:33.034802 astrometry_net_client-0.5.0/astrometry_net_client/
+-rw-r--r--   0 sten      (1000) sten      (1000)      345 2022-11-02 18:32:15.000000 astrometry_net_client-0.5.0/astrometry_net_client/__init__.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     8524 2023-07-23 10:22:46.000000 astrometry_net_client-0.5.0/astrometry_net_client/client.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      490 2024-02-18 13:44:35.000000 astrometry_net_client-0.5.0/astrometry_net_client/config.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      663 2022-11-02 18:32:13.000000 astrometry_net_client-0.5.0/astrometry_net_client/exceptions.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     6659 2024-05-19 19:12:52.000000 astrometry_net_client-0.5.0/astrometry_net_client/request.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-19 19:19:33.034802 astrometry_net_client-0.5.0/astrometry_net_client/scripts/
+-rw-r--r--   0 sten      (1000) sten      (1000)     7506 2024-05-19 19:08:28.000000 astrometry_net_client-0.5.0/astrometry_net_client/scripts/anc_upload.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     5036 2022-11-02 18:32:23.000000 astrometry_net_client-0.5.0/astrometry_net_client/session.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     8088 2023-07-23 10:22:46.000000 astrometry_net_client-0.5.0/astrometry_net_client/settings.py
+-rw-r--r--   0 sten      (1000) sten      (1000)    16640 2024-02-18 13:44:35.000000 astrometry_net_client-0.5.0/astrometry_net_client/statusables.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     5028 2024-02-18 13:44:35.000000 astrometry_net_client-0.5.0/astrometry_net_client/uploads.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-19 19:19:33.034802 astrometry_net_client-0.5.0/astrometry_net_client.egg-info/
+-rw-r--r--   0 sten      (1000) sten      (1000)     6783 2024-05-19 19:19:33.000000 astrometry_net_client-0.5.0/astrometry_net_client.egg-info/PKG-INFO
+-rw-r--r--   0 sten      (1000) sten      (1000)      838 2024-05-19 19:19:33.000000 astrometry_net_client-0.5.0/astrometry_net_client.egg-info/SOURCES.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)        1 2024-05-19 19:19:33.000000 astrometry_net_client-0.5.0/astrometry_net_client.egg-info/dependency_links.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       77 2024-05-19 19:19:33.000000 astrometry_net_client-0.5.0/astrometry_net_client.egg-info/entry_points.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       24 2024-05-19 19:19:33.000000 astrometry_net_client-0.5.0/astrometry_net_client.egg-info/requires.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       22 2024-05-19 19:19:33.000000 astrometry_net_client-0.5.0/astrometry_net_client.egg-info/top_level.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)     1197 2024-05-19 19:07:04.000000 astrometry_net_client-0.5.0/pyproject.toml
+-rw-r--r--   0 sten      (1000) sten      (1000)      273 2024-05-19 19:19:33.034802 astrometry_net_client-0.5.0/setup.cfg
+-rw-r--r--   0 sten      (1000) sten      (1000)      149 2024-05-19 19:07:14.000000 astrometry_net_client-0.5.0/setup.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-19 19:19:33.034802 astrometry_net_client-0.5.0/tests/
+-rw-r--r--   0 sten      (1000) sten      (1000)     2992 2022-08-30 07:13:54.000000 astrometry_net_client-0.5.0/tests/test.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     1660 2023-07-23 10:22:46.000000 astrometry_net_client-0.5.0/tests/test_client.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2489 2022-08-30 07:13:54.000000 astrometry_net_client-0.5.0/tests/test_job.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2352 2023-07-23 10:22:46.000000 astrometry_net_client-0.5.0/tests/test_online.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     1736 2022-08-30 07:13:54.000000 astrometry_net_client-0.5.0/tests/test_session.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     3673 2022-08-30 07:13:54.000000 astrometry_net_client-0.5.0/tests/test_settings.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2987 2022-08-30 07:13:54.000000 astrometry_net_client-0.5.0/tests/test_statusables.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     1618 2024-02-18 13:44:35.000000 astrometry_net_client-0.5.0/tests/test_upload.py
```

### Comparing `astrometry_net_client-0.4.0/LICENSE` & `astrometry_net_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/PKG-INFO` & `astrometry_net_client-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: astrometry_net_client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python interface for the Astrometry.net API.
-Home-page: https://github.com/StenSipma/astrometry_net_client
-Author: Sten Sipma
-Author-email: sten.sipma@ziggo.nl
-Keywords: astronomy astrometry client coordinates wcs api
+Author-email: Sten Sipma <sten.sipma@ziggo.nl>
+Project-URL: Repository, https://github.com/StenSipma/astrometry_net_client
+Project-URL: Documentation, https://astrometry-net-client.readthedocs.io/en/latest/index.html
+Keywords: astronomy,astrometry,client,coordinates,wcs,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,31 +35,49 @@
    :target: https://github.com/StenSipma/astrometry_net_client/actions?query=workflow%3A%22Build+%26+Tests%22
    :alt: Build & Tests Status
 
 .. note:: 
    The package is still in development, but it can already be used. 
    Do not hesitate to leave any feedback (positive or negative)!
 
+Quickstart
+----------
+
+Install the package via pip:
+
+.. code:: bash
+
+        pip install astrometry-net-client
+
+Get your API key from: `api_help`_, and paste it in a plaintext file (name it something like `key`).
+
+A script called `anc_upload` should be included with the install.
+
+.. _api_help: https://nova.astrometry.net/api_help
+
+
+
 Introduction
 ------------
 
-This package is meant to be a simple but extensible interface for the `Astrometry.net API`_. A higher level interface is offered through the ``Client`` class, combining most functionality. However, if you want more control over the requests (e.g. by manually checking the responses), you can also use the ``Job``, ``Submission`` and ``UploadFile`` classes directly.
+This package is meant to be a simple but extensible interface for the `Astrometry.net API`_.
+A higher level interface is offered through the ``Client`` class, combining most functionality.
+However, if you want more control over the requests (e.g. by manually checking the responses), you can also use the ``Job``, ``Submission`` and ``UploadFile`` classes directly.
 
 The structure of these classes tries to follow the pattern of the API itself, which is essentially:
 
 1. Upload some file (``UploadFile``), which requires an API key & a login (``Session``)
 2. The upload creates a submission (``Submission``), unique for each upload. This has to do some general processing, even before the uploaded image is processed.
 3. When the submission is done preprocessing, and the system is ready to process the uploaded file, a job (``Job``) is spawned for each image.
 4. The job then takes some time to process, and when it is done it can either be successful or fail.
 5. When successful, some information (e.g. found objects) and result files like the generated WCS header can be retrieved.
 
 Using this package, these steps are (note that this is not the ideal way to upload multiple files):
 
 .. code:: python
-   :number-lines:
    
     from astrometry_net_client import Session
     from astrometry_net_client import FileUpload
 
     s = Session(api_key='xxxxxxxxx')
     upl = FileUpload('some/file/name', session=s) # 1.
     submission = upl.submit()                     # 2.
@@ -69,15 +87,14 @@
     if job.success():
         wcs = job.wcs_file()                      # 5. (only if successful)
     print(job.info())                             # works even though the job failed
 
 Or with the higher level ``Client`` :
 
 .. code:: python
-   :number-lines:
    
     from astrometry_net_client import Client
 
     c = Client(api_key='xxxxxxxxxx')
 
     # WARNING: this can take a while, as it blocks until the file is solved.
     # wcs will be None if upload is not successful
```

### Comparing `astrometry_net_client-0.4.0/README.rst` & `astrometry_net_client-0.5.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -10,31 +10,49 @@
    :target: https://github.com/StenSipma/astrometry_net_client/actions?query=workflow%3A%22Build+%26+Tests%22
    :alt: Build & Tests Status
 
 .. note:: 
    The package is still in development, but it can already be used. 
    Do not hesitate to leave any feedback (positive or negative)!
 
+Quickstart
+----------
+
+Install the package via pip:
+
+.. code:: bash
+
+        pip install astrometry-net-client
+
+Get your API key from: `api_help`_, and paste it in a plaintext file (name it something like `key`).
+
+A script called `anc_upload` should be included with the install.
+
+.. _api_help: https://nova.astrometry.net/api_help
+
+
+
 Introduction
 ------------
 
-This package is meant to be a simple but extensible interface for the `Astrometry.net API`_. A higher level interface is offered through the ``Client`` class, combining most functionality. However, if you want more control over the requests (e.g. by manually checking the responses), you can also use the ``Job``, ``Submission`` and ``UploadFile`` classes directly.
+This package is meant to be a simple but extensible interface for the `Astrometry.net API`_.
+A higher level interface is offered through the ``Client`` class, combining most functionality.
+However, if you want more control over the requests (e.g. by manually checking the responses), you can also use the ``Job``, ``Submission`` and ``UploadFile`` classes directly.
 
 The structure of these classes tries to follow the pattern of the API itself, which is essentially:
 
 1. Upload some file (``UploadFile``), which requires an API key & a login (``Session``)
 2. The upload creates a submission (``Submission``), unique for each upload. This has to do some general processing, even before the uploaded image is processed.
 3. When the submission is done preprocessing, and the system is ready to process the uploaded file, a job (``Job``) is spawned for each image.
 4. The job then takes some time to process, and when it is done it can either be successful or fail.
 5. When successful, some information (e.g. found objects) and result files like the generated WCS header can be retrieved.
 
 Using this package, these steps are (note that this is not the ideal way to upload multiple files):
 
 .. code:: python
-   :number-lines:
    
     from astrometry_net_client import Session
     from astrometry_net_client import FileUpload
 
     s = Session(api_key='xxxxxxxxx')
     upl = FileUpload('some/file/name', session=s) # 1.
     submission = upl.submit()                     # 2.
@@ -44,15 +62,14 @@
     if job.success():
         wcs = job.wcs_file()                      # 5. (only if successful)
     print(job.info())                             # works even though the job failed
 
 Or with the higher level ``Client`` :
 
 .. code:: python
-   :number-lines:
    
     from astrometry_net_client import Client
 
     c = Client(api_key='xxxxxxxxxx')
 
     # WARNING: this can take a while, as it blocks until the file is solved.
     # wcs will be None if upload is not successful
```

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client/client.py` & `astrometry_net_client-0.5.0/astrometry_net_client/client.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client/exceptions.py` & `astrometry_net_client-0.5.0/astrometry_net_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client/request.py` & `astrometry_net_client-0.5.0/astrometry_net_client/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def __init__(
         self,
         url: Optional[str] = None,
         method: str = "get",
         data: Optional[dict] = None,
         settings: Optional[Settings] = None,
-        **kwargs
+        **kwargs,
     ):
         self.data = {} if data is None else data.copy()
         self.settings = {} if settings is None else settings.copy()
         self.arguments = kwargs
         if url is not None:
             self.url = url
```

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client/session.py` & `astrometry_net_client-0.5.0/astrometry_net_client/session.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client/settings.py` & `astrometry_net_client-0.5.0/astrometry_net_client/settings.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client/statusables.py` & `astrometry_net_client-0.5.0/astrometry_net_client/statusables.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client/uploads.py` & `astrometry_net_client-0.5.0/astrometry_net_client/uploads.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client.egg-info/PKG-INFO` & `astrometry_net_client-0.5.0/astrometry_net_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: astrometry_net_client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python interface for the Astrometry.net API.
-Home-page: https://github.com/StenSipma/astrometry_net_client
-Author: Sten Sipma
-Author-email: sten.sipma@ziggo.nl
-Keywords: astronomy astrometry client coordinates wcs api
+Author-email: Sten Sipma <sten.sipma@ziggo.nl>
+Project-URL: Repository, https://github.com/StenSipma/astrometry_net_client
+Project-URL: Documentation, https://astrometry-net-client.readthedocs.io/en/latest/index.html
+Keywords: astronomy,astrometry,client,coordinates,wcs,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,31 +35,49 @@
    :target: https://github.com/StenSipma/astrometry_net_client/actions?query=workflow%3A%22Build+%26+Tests%22
    :alt: Build & Tests Status
 
 .. note:: 
    The package is still in development, but it can already be used. 
    Do not hesitate to leave any feedback (positive or negative)!
 
+Quickstart
+----------
+
+Install the package via pip:
+
+.. code:: bash
+
+        pip install astrometry-net-client
+
+Get your API key from: `api_help`_, and paste it in a plaintext file (name it something like `key`).
+
+A script called `anc_upload` should be included with the install.
+
+.. _api_help: https://nova.astrometry.net/api_help
+
+
+
 Introduction
 ------------
 
-This package is meant to be a simple but extensible interface for the `Astrometry.net API`_. A higher level interface is offered through the ``Client`` class, combining most functionality. However, if you want more control over the requests (e.g. by manually checking the responses), you can also use the ``Job``, ``Submission`` and ``UploadFile`` classes directly.
+This package is meant to be a simple but extensible interface for the `Astrometry.net API`_.
+A higher level interface is offered through the ``Client`` class, combining most functionality.
+However, if you want more control over the requests (e.g. by manually checking the responses), you can also use the ``Job``, ``Submission`` and ``UploadFile`` classes directly.
 
 The structure of these classes tries to follow the pattern of the API itself, which is essentially:
 
 1. Upload some file (``UploadFile``), which requires an API key & a login (``Session``)
 2. The upload creates a submission (``Submission``), unique for each upload. This has to do some general processing, even before the uploaded image is processed.
 3. When the submission is done preprocessing, and the system is ready to process the uploaded file, a job (``Job``) is spawned for each image.
 4. The job then takes some time to process, and when it is done it can either be successful or fail.
 5. When successful, some information (e.g. found objects) and result files like the generated WCS header can be retrieved.
 
 Using this package, these steps are (note that this is not the ideal way to upload multiple files):
 
 .. code:: python
-   :number-lines:
    
     from astrometry_net_client import Session
     from astrometry_net_client import FileUpload
 
     s = Session(api_key='xxxxxxxxx')
     upl = FileUpload('some/file/name', session=s) # 1.
     submission = upl.submit()                     # 2.
@@ -69,15 +87,14 @@
     if job.success():
         wcs = job.wcs_file()                      # 5. (only if successful)
     print(job.info())                             # works even though the job failed
 
 Or with the higher level ``Client`` :
 
 .. code:: python
-   :number-lines:
    
     from astrometry_net_client import Client
 
     c = Client(api_key='xxxxxxxxxx')
 
     # WARNING: this can take a while, as it blocks until the file is solved.
     # wcs will be None if upload is not successful
```

### Comparing `astrometry_net_client-0.4.0/astrometry_net_client.egg-info/SOURCES.txt` & `astrometry_net_client-0.5.0/astrometry_net_client.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 LICENSE
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 astrometry_net_client/__init__.py
 astrometry_net_client/client.py
 astrometry_net_client/config.py
 astrometry_net_client/exceptions.py
 astrometry_net_client/request.py
 astrometry_net_client/session.py
 astrometry_net_client/settings.py
 astrometry_net_client/statusables.py
 astrometry_net_client/uploads.py
 astrometry_net_client.egg-info/PKG-INFO
 astrometry_net_client.egg-info/SOURCES.txt
 astrometry_net_client.egg-info/dependency_links.txt
+astrometry_net_client.egg-info/entry_points.txt
 astrometry_net_client.egg-info/requires.txt
 astrometry_net_client.egg-info/top_level.txt
+astrometry_net_client/scripts/anc_upload.py
 tests/test.py
 tests/test_client.py
 tests/test_job.py
 tests/test_online.py
 tests/test_session.py
 tests/test_settings.py
 tests/test_statusables.py
```

### Comparing `astrometry_net_client-0.4.0/tests/test.py` & `astrometry_net_client-0.5.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/tests/test_client.py` & `astrometry_net_client-0.5.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/tests/test_job.py` & `astrometry_net_client-0.5.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/tests/test_online.py` & `astrometry_net_client-0.5.0/tests/test_online.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/tests/test_session.py` & `astrometry_net_client-0.5.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/tests/test_settings.py` & `astrometry_net_client-0.5.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/tests/test_statusables.py` & `astrometry_net_client-0.5.0/tests/test_statusables.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.4.0/tests/test_upload.py` & `astrometry_net_client-0.5.0/tests/test_upload.py`

 * *Files identical despite different names*

