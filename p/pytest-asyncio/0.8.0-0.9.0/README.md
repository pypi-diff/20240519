# Comparing `tmp/pytest-asyncio-0.8.0.tar.gz` & `tmp/pytest-asyncio-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-asyncio-0.8.0.tar", last modified: Sat Sep 23 11:36:35 2017, max compression
+gzip compressed data, was "dist/pytest-asyncio-0.9.0.tar", last modified: Sat Jul 28 14:34:09 2018, max compression
```

## Comparing `pytest-asyncio-0.8.0.tar` & `pytest-asyncio-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/
--rw-rw-r--   0 tin       (1000) tin       (1000)    11325 2016-04-22 21:30:56.000000 pytest-asyncio-0.8.0/LICENSE
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/pytest_asyncio/
--rw-rw-r--   0 tin       (1000) tin       (1000)     7043 2017-09-23 11:18:06.000000 pytest-asyncio-0.8.0/pytest_asyncio/plugin.py
--rw-rw-r--   0 tin       (1000) tin       (1000)       79 2017-09-23 11:35:52.000000 pytest-asyncio-0.8.0/pytest_asyncio/__init__.py
--rw-rw-r--   0 tin       (1000) tin       (1000)      211 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/setup.cfg
--rw-rw-r--   0 tin       (1000) tin       (1000)     9091 2017-09-23 11:35:46.000000 pytest-asyncio-0.8.0/README.rst
--rw-rw-r--   0 tin       (1000) tin       (1000)     1479 2017-09-23 11:29:05.000000 pytest-asyncio-0.8.0/setup.py
--rw-rw-r--   0 tin       (1000) tin       (1000)    11801 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/PKG-INFO
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/pytest_asyncio.egg-info/
--rw-rw-r--   0 tin       (1000) tin       (1000)      319 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/pytest_asyncio.egg-info/SOURCES.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)        1 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/pytest_asyncio.egg-info/dependency_links.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)      104 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/pytest_asyncio.egg-info/requires.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)    11801 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/pytest_asyncio.egg-info/PKG-INFO
--rw-rw-r--   0 tin       (1000) tin       (1000)       44 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/pytest_asyncio.egg-info/entry_points.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)       15 2017-09-23 11:36:35.000000 pytest-asyncio-0.8.0/pytest_asyncio.egg-info/top_level.txt
+drwxr-xr-x   0 tin        (501) staff       (20)        0 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/
+-rw-r--r--   0 tin        (501) staff       (20)    11666 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/PKG-INFO
+drwxr-xr-x   0 tin        (501) staff       (20)        0 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/pytest_asyncio/
+-rw-r--r--   0 tin        (501) staff       (20)       79 2018-07-28 14:33:19.000000 pytest-asyncio-0.9.0/pytest_asyncio/__init__.py
+-rw-r--r--   0 tin        (501) staff       (20)     6327 2018-07-28 14:17:05.000000 pytest-asyncio-0.9.0/pytest_asyncio/plugin.py
+drwxr-xr-x   0 tin        (501) staff       (20)        0 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/pytest_asyncio.egg-info/
+-rw-r--r--   0 tin        (501) staff       (20)    11666 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/pytest_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 tin        (501) staff       (20)      311 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/pytest_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 tin        (501) staff       (20)       44 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/pytest_asyncio.egg-info/entry_points.txt
+-rw-r--r--   0 tin        (501) staff       (20)      104 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/pytest_asyncio.egg-info/requires.txt
+-rw-r--r--   0 tin        (501) staff       (20)       15 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/pytest_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 tin        (501) staff       (20)        1 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/pytest_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 tin        (501) staff       (20)     1517 2018-07-28 14:28:00.000000 pytest-asyncio-0.9.0/setup.py
+-rw-r--r--   0 tin        (501) staff       (20)      211 2018-07-28 14:34:09.000000 pytest-asyncio-0.9.0/setup.cfg
+-rw-r--r--   0 tin        (501) staff       (20)     8932 2018-07-28 14:32:16.000000 pytest-asyncio-0.9.0/README.rst
```

### Comparing `pytest-asyncio-0.8.0/pytest_asyncio/plugin.py` & `pytest-asyncio-0.9.0/pytest_asyncio/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """pytest-asyncio implementation."""
 import asyncio
 import contextlib
 import inspect
 import socket
-from concurrent.futures import ProcessPoolExecutor
 
 import pytest
 from _pytest.python import transfer_markers
 
 try:
     from async_generator import isasyncgenfunction
 except ImportError:
@@ -21,35 +20,29 @@
 
 def pytest_configure(config):
     """Inject documentation."""
     config.addinivalue_line("markers",
                             "asyncio: "
                             "mark the test as a coroutine, it will be "
                             "run using an asyncio event loop")
-    config.addinivalue_line("markers",
-                            "asyncio_process_pool: "
-                            "mark the test as a coroutine, it will be "
-                            "run using an asyncio event loop with a process "
-                            "pool")
 
 
 @pytest.mark.tryfirst
 def pytest_pycollect_makeitem(collector, name, obj):
     """A pytest hook to collect asyncio coroutines."""
     if collector.funcnamefilter(name) and _is_coroutine(obj):
         item = pytest.Function(name, parent=collector)
 
         # Due to how pytest test collection works, module-level pytestmarks
         # are applied after the collection step. Since this is the collection
         # step, we look ourselves.
         transfer_markers(obj, item.cls, item.module)
         item = pytest.Function(name, parent=collector)  # To reload keywords.
 
-        if ('asyncio' in item.keywords or
-            'asyncio_process_pool' in item.keywords):
+        if 'asyncio' in item.keywords:
             return list(collector._genfunctions(name, obj))
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_fixture_setup(fixturedef, request):
     """Adjust the event loop policy when an event loop is produced."""
     if isasyncgenfunction(fixturedef.func):
@@ -166,36 +159,26 @@
             item.fixturenames.append(fixture)
 
 
 # maps marker to the name of the event loop fixture that will be available
 # to marked test functions
 _markers_2_fixtures = {
     'asyncio': 'event_loop',
-    'asyncio_process_pool': 'event_loop_process_pool',
 }
 
 
 @pytest.yield_fixture
 def event_loop(request):
     """Create an instance of the default event loop for each test case."""
     loop = asyncio.get_event_loop_policy().new_event_loop()
     yield loop
     loop.close()
 
 
 @pytest.fixture
-def event_loop_process_pool(event_loop):
-    """Create a fresh instance of the default event loop.
-
-    The event loop will have a process pool set as the default executor."""
-    event_loop.set_default_executor(ProcessPoolExecutor())
-    return event_loop
-
-
-@pytest.fixture
 def unused_tcp_port():
     """Find an unused localhost TCP port from 1024-65535 and return it."""
     with contextlib.closing(socket.socket()) as sock:
         sock.bind(('127.0.0.1', 0))
         return sock.getsockname()[1]
```

### Comparing `pytest-asyncio-0.8.0/README.rst` & `pytest-asyncio-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 .. image:: https://img.shields.io/pypi/v/pytest-asyncio.svg
     :target: https://pypi.python.org/pypi/pytest-asyncio
 .. image:: https://travis-ci.org/pytest-dev/pytest-asyncio.svg?branch=master
     :target: https://travis-ci.org/pytest-dev/pytest-asyncio
 .. image:: https://coveralls.io/repos/pytest-dev/pytest-asyncio/badge.svg
     :target: https://coveralls.io/r/pytest-dev/pytest-asyncio
+.. image:: https://img.shields.io/pypi/pyversions/pytest-asyncio.svg
+    :target: https://github.com/pytest-dev/pytest-asyncio
+    :alt: Supported Python versions
 
 pytest-asyncio is an Apache2 licensed library, written in Python, for testing
 asyncio code with pytest.
 
 asyncio code is usually written in the form of coroutines, which makes it
 slightly more difficult to test using normal testing tools. pytest-asyncio
 provides useful fixtures and markers to make testing easier.
@@ -84,20 +87,14 @@
         yield loop
         loop.close()
 
 If the ``pytest.mark.asyncio`` marker is applied, a pytest hook will
 ensure the produced loop is set as the default global loop.
 Fixtures depending on the ``event_loop`` fixture can expect the policy to be properly modified when they run.
 
-``event_loop_process_pool``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-The ``event_loop_process_pool`` fixture is almost identical to the
-``event_loop`` fixture, except the created event loop will have a
-``concurrent.futures.ProcessPoolExecutor`` set as the default executor.
-
 ``unused_tcp_port``
 ~~~~~~~~~~~~~~~~~~~
 Finds and yields a single unused TCP port on the localhost interface. Useful for
 binding temporary test servers.
 
 ``unused_tcp_port_factory``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -172,23 +169,24 @@
     async def test_example(event_loop):
         """No marker!"""
         await asyncio.sleep(0, loop=event_loop)
 
 .. |pytestmark| replace:: ``pytestmark``
 .. _pytestmark: http://doc.pytest.org/en/latest/example/markers.html#marking-whole-classes-or-modules
 
-``pytest.mark.asyncio_process_pool``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-The ``asyncio_process_pool`` marker is almost identical to the ``asyncio``
-marker, except the event loop used will have a
-``concurrent.futures.ProcessPoolExecutor`` set as the default executor.
-
 Changelog
 ---------
 
+0.9.0 (2018-07-28)
+~~~~~~~~~~~~~~~~~~
+- Python 3.7 support.
+- Remove ``event_loop_process_pool`` fixture and
+  ``pytest.mark.asyncio_process_pool`` marker (see
+  https://bugs.python.org/issue34075 for deprecation and removal details)
+
 0.8.0 (2017-09-23)
 ~~~~~~~~~~~~~~~~~~
 - Improve integration with other packages (like aiohttp) with more careful event loop handling.
   `#64` <https://github.com/pytest-dev/pytest-asyncio/pull/64>
 
 0.7.0 (2017-09-08)
 ~~~~~~~~~~~~~~~~~~
```

### Comparing `pytest-asyncio-0.8.0/setup.py` & `pytest-asyncio-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import re
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 
 def find_version():
-    version_file = Path(__file__).parent.joinpath('pytest_asyncio', '__init__.py').read_text()
-    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
-                              version_file, re.M)
+    version_file = (
+        Path(__file__)
+        .parent.joinpath("pytest_asyncio", "__init__.py")
+        .read_text()
+    )
+    version_match = re.search(
+        r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M
+    )
     if version_match:
         return version_match.group(1)
 
     raise RuntimeError("Unable to find version string.")
 
 
 setup(
-    name='pytest-asyncio',
+    name="pytest-asyncio",
     version=find_version(),
     packages=find_packages(),
-    url='https://github.com/pytest-dev/pytest-asyncio',
-    license='Apache 2.0',
-    author='Tin Tvrtković',
-    author_email='tinchester@gmail.com',
-    description='Pytest support for asyncio.',
-    long_description=Path(__file__).parent.joinpath('README.rst').read_text(),
+    url="https://github.com/pytest-dev/pytest-asyncio",
+    license="Apache 2.0",
+    author="Tin Tvrtković",
+    author_email="tinchester@gmail.com",
+    description="Pytest support for asyncio.",
+    long_description=Path(__file__).parent.joinpath("README.rst").read_text(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Topic :: Software Development :: Testing",
         "Framework :: Pytest",
     ],
-    python_requires='>= 3.5',
-    install_requires=[
-        'pytest >= 3.0.6',
-    ],
+    python_requires=">= 3.5",
+    install_requires=["pytest >= 3.0.6"],
     extras_require={
-        ':python_version == "3.5"': 'async_generator >= 1.3',
-        'testing': ['coverage', 'async_generator >= 1.3'],
+        ':python_version == "3.5"': "async_generator >= 1.3",
+        "testing": ["coverage", "async_generator >= 1.3"],
     },
-    entry_points={
-        'pytest11': ['asyncio = pytest_asyncio.plugin'],
-    }
+    entry_points={"pytest11": ["asyncio = pytest_asyncio.plugin"]},
 )
```

### Comparing `pytest-asyncio-0.8.0/PKG-INFO` & `pytest-asyncio-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-asyncio
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pytest support for asyncio.
 Home-page: https://github.com/pytest-dev/pytest-asyncio
 Author: Tin Tvrtković
 Author-email: tinchester@gmail.com
 License: Apache 2.0
-Description-Content-Type: UNKNOWN
 Description: pytest-asyncio: pytest support for asyncio
         ==========================================
         
         .. image:: https://img.shields.io/pypi/v/pytest-asyncio.svg
             :target: https://pypi.python.org/pypi/pytest-asyncio
         .. image:: https://travis-ci.org/pytest-dev/pytest-asyncio.svg?branch=master
             :target: https://travis-ci.org/pytest-dev/pytest-asyncio
         .. image:: https://coveralls.io/repos/pytest-dev/pytest-asyncio/badge.svg
             :target: https://coveralls.io/r/pytest-dev/pytest-asyncio
+        .. image:: https://img.shields.io/pypi/pyversions/pytest-asyncio.svg
+            :target: https://github.com/pytest-dev/pytest-asyncio
+            :alt: Supported Python versions
         
         pytest-asyncio is an Apache2 licensed library, written in Python, for testing
         asyncio code with pytest.
         
         asyncio code is usually written in the form of coroutines, which makes it
         slightly more difficult to test using normal testing tools. pytest-asyncio
         provides useful fixtures and markers to make testing easier.
@@ -93,20 +95,14 @@
                 yield loop
                 loop.close()
         
         If the ``pytest.mark.asyncio`` marker is applied, a pytest hook will
         ensure the produced loop is set as the default global loop.
         Fixtures depending on the ``event_loop`` fixture can expect the policy to be properly modified when they run.
         
-        ``event_loop_process_pool``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        The ``event_loop_process_pool`` fixture is almost identical to the
-        ``event_loop`` fixture, except the created event loop will have a
-        ``concurrent.futures.ProcessPoolExecutor`` set as the default executor.
-        
         ``unused_tcp_port``
         ~~~~~~~~~~~~~~~~~~~
         Finds and yields a single unused TCP port on the localhost interface. Useful for
         binding temporary test servers.
         
         ``unused_tcp_port_factory``
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -181,23 +177,24 @@
             async def test_example(event_loop):
                 """No marker!"""
                 await asyncio.sleep(0, loop=event_loop)
         
         .. |pytestmark| replace:: ``pytestmark``
         .. _pytestmark: http://doc.pytest.org/en/latest/example/markers.html#marking-whole-classes-or-modules
         
-        ``pytest.mark.asyncio_process_pool``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        The ``asyncio_process_pool`` marker is almost identical to the ``asyncio``
-        marker, except the event loop used will have a
-        ``concurrent.futures.ProcessPoolExecutor`` set as the default executor.
-        
         Changelog
         ---------
         
+        0.9.0 (2018-07-28)
+        ~~~~~~~~~~~~~~~~~~
+        - Python 3.7 support.
+        - Remove ``event_loop_process_pool`` fixture and
+          ``pytest.mark.asyncio_process_pool`` marker (see
+          https://bugs.python.org/issue34075 for deprecation and removal details)
+        
         0.8.0 (2017-09-23)
         ~~~~~~~~~~~~~~~~~~
         - Improve integration with other packages (like aiohttp) with more careful event loop handling.
           `#64` <https://github.com/pytest-dev/pytest-asyncio/pull/64>
         
         0.7.0 (2017-09-08)
         ~~~~~~~~~~~~~~~~~~
@@ -267,10 +264,12 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
 Requires-Python: >= 3.5
+Provides-Extra: testing
```

### Comparing `pytest-asyncio-0.8.0/pytest_asyncio.egg-info/PKG-INFO` & `pytest-asyncio-0.9.0/pytest_asyncio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-asyncio
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pytest support for asyncio.
 Home-page: https://github.com/pytest-dev/pytest-asyncio
 Author: Tin Tvrtković
 Author-email: tinchester@gmail.com
 License: Apache 2.0
-Description-Content-Type: UNKNOWN
 Description: pytest-asyncio: pytest support for asyncio
         ==========================================
         
         .. image:: https://img.shields.io/pypi/v/pytest-asyncio.svg
             :target: https://pypi.python.org/pypi/pytest-asyncio
         .. image:: https://travis-ci.org/pytest-dev/pytest-asyncio.svg?branch=master
             :target: https://travis-ci.org/pytest-dev/pytest-asyncio
         .. image:: https://coveralls.io/repos/pytest-dev/pytest-asyncio/badge.svg
             :target: https://coveralls.io/r/pytest-dev/pytest-asyncio
+        .. image:: https://img.shields.io/pypi/pyversions/pytest-asyncio.svg
+            :target: https://github.com/pytest-dev/pytest-asyncio
+            :alt: Supported Python versions
         
         pytest-asyncio is an Apache2 licensed library, written in Python, for testing
         asyncio code with pytest.
         
         asyncio code is usually written in the form of coroutines, which makes it
         slightly more difficult to test using normal testing tools. pytest-asyncio
         provides useful fixtures and markers to make testing easier.
@@ -93,20 +95,14 @@
                 yield loop
                 loop.close()
         
         If the ``pytest.mark.asyncio`` marker is applied, a pytest hook will
         ensure the produced loop is set as the default global loop.
         Fixtures depending on the ``event_loop`` fixture can expect the policy to be properly modified when they run.
         
-        ``event_loop_process_pool``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        The ``event_loop_process_pool`` fixture is almost identical to the
-        ``event_loop`` fixture, except the created event loop will have a
-        ``concurrent.futures.ProcessPoolExecutor`` set as the default executor.
-        
         ``unused_tcp_port``
         ~~~~~~~~~~~~~~~~~~~
         Finds and yields a single unused TCP port on the localhost interface. Useful for
         binding temporary test servers.
         
         ``unused_tcp_port_factory``
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -181,23 +177,24 @@
             async def test_example(event_loop):
                 """No marker!"""
                 await asyncio.sleep(0, loop=event_loop)
         
         .. |pytestmark| replace:: ``pytestmark``
         .. _pytestmark: http://doc.pytest.org/en/latest/example/markers.html#marking-whole-classes-or-modules
         
-        ``pytest.mark.asyncio_process_pool``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        The ``asyncio_process_pool`` marker is almost identical to the ``asyncio``
-        marker, except the event loop used will have a
-        ``concurrent.futures.ProcessPoolExecutor`` set as the default executor.
-        
         Changelog
         ---------
         
+        0.9.0 (2018-07-28)
+        ~~~~~~~~~~~~~~~~~~
+        - Python 3.7 support.
+        - Remove ``event_loop_process_pool`` fixture and
+          ``pytest.mark.asyncio_process_pool`` marker (see
+          https://bugs.python.org/issue34075 for deprecation and removal details)
+        
         0.8.0 (2017-09-23)
         ~~~~~~~~~~~~~~~~~~
         - Improve integration with other packages (like aiohttp) with more careful event loop handling.
           `#64` <https://github.com/pytest-dev/pytest-asyncio/pull/64>
         
         0.7.0 (2017-09-08)
         ~~~~~~~~~~~~~~~~~~
@@ -267,10 +264,12 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
 Requires-Python: >= 3.5
+Provides-Extra: testing
```

