# Comparing `tmp/mara-2.0.0.tar.gz` & `tmp/mara-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mara-2.0.0.tar", last modified: Fri Nov 18 01:29:38 2022, max compression
+gzip compressed data, was "mara-2.1.0.tar", last modified: Sat May 18 13:07:52 2024, max compression
```

## Comparing `mara-2.0.0.tar` & `mara-2.1.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.766698 mara-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2022-11-18 01:29:33.000000 mara-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3020 2022-11-18 01:29:38.766698 mara-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2022-11-18 01:29:33.000000 mara-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.762699 mara-2.0.0/mara/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2022-11-18 01:29:33.000000 mara-2.0.0/mara/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.766698 mara-2.0.0/mara/app/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2022-11-18 01:29:33.000000 mara-2.0.0/mara/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6330 2022-11-18 01:29:33.000000 mara-2.0.0/mara/app/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     5036 2022-11-18 01:29:33.000000 mara-2.0.0/mara/app/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2022-11-18 01:29:33.000000 mara-2.0.0/mara/app/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.766698 mara-2.0.0/mara/clients/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-18 01:29:33.000000 mara-2.0.0/mara/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2338 2022-11-18 01:29:33.000000 mara-2.0.0/mara/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2022-11-18 01:29:33.000000 mara-2.0.0/mara/clients/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)     1855 2022-11-18 01:29:33.000000 mara-2.0.0/mara/clients/telnet.py
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-18 01:29:33.000000 mara-2.0.0/mara/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.766698 mara-2.0.0/mara/events/
--rw-r--r--   0 runner    (1001) docker     (122)      329 2022-11-18 01:29:33.000000 mara-2.0.0/mara/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      533 2022-11-18 01:29:33.000000 mara-2.0.0/mara/events/app.py
--rw-r--r--   0 runner    (1001) docker     (122)      790 2022-11-18 01:29:33.000000 mara-2.0.0/mara/events/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2022-11-18 01:29:33.000000 mara-2.0.0/mara/events/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2022-11-18 01:29:33.000000 mara-2.0.0/mara/events/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.766698 mara-2.0.0/mara/servers/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-18 01:29:33.000000 mara-2.0.0/mara/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2760 2022-11-18 01:29:33.000000 mara-2.0.0/mara/servers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2022-11-18 01:29:33.000000 mara-2.0.0/mara/servers/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2022-11-18 01:29:33.000000 mara-2.0.0/mara/servers/telnet.py
--rw-r--r--   0 runner    (1001) docker     (122)      180 2022-11-18 01:29:33.000000 mara-2.0.0/mara/status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.766698 mara-2.0.0/mara/storage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:33.000000 mara-2.0.0/mara/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2022-11-18 01:29:33.000000 mara-2.0.0/mara/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2022-11-18 01:29:33.000000 mara-2.0.0/mara/storage/dict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.766698 mara-2.0.0/mara/timers/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-18 01:29:33.000000 mara-2.0.0/mara/timers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2022-11-18 01:29:33.000000 mara-2.0.0/mara/timers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      633 2022-11-18 01:29:33.000000 mara-2.0.0/mara/timers/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 01:29:38.762699 mara-2.0.0/mara.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3020 2022-11-18 01:29:38.000000 mara-2.0.0/mara.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      762 2022-11-18 01:29:38.000000 mara-2.0.0/mara.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-18 01:29:38.000000 mara-2.0.0/mara.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-18 01:29:38.000000 mara-2.0.0/mara.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-11-18 01:29:38.000000 mara-2.0.0/mara.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-18 01:29:38.000000 mara-2.0.0/mara.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2022-11-18 01:29:38.770698 mara-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      513 2022-11-18 01:29:33.000000 mara-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.300925 mara-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-18 13:07:49.000000 mara-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-18 13:07:52.300925 mara-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-18 13:07:49.000000 mara-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.296925 mara-2.1.0/mara/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-18 13:07:49.000000 mara-2.1.0/mara/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.296925 mara-2.1.0/mara/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 13:07:49.000000 mara-2.1.0/mara/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-18 13:07:49.000000 mara-2.1.0/mara/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-18 13:07:49.000000 mara-2.1.0/mara/app/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-18 13:07:49.000000 mara-2.1.0/mara/app/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 13:07:49.000000 mara-2.1.0/mara/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.296925 mara-2.1.0/mara/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-18 13:07:49.000000 mara-2.1.0/mara/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-18 13:07:49.000000 mara-2.1.0/mara/events/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-18 13:07:49.000000 mara-2.1.0/mara/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-18 13:07:49.000000 mara-2.1.0/mara/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-18 13:07:49.000000 mara-2.1.0/mara/events/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.296925 mara-2.1.0/mara/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.300925 mara-2.1.0/mara/servers/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/connections/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/connections/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/connections/socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/connections/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-18 13:07:49.000000 mara-2.1.0/mara/servers/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-18 13:07:49.000000 mara-2.1.0/mara/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.300925 mara-2.1.0/mara/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:49.000000 mara-2.1.0/mara/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-18 13:07:49.000000 mara-2.1.0/mara/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-18 13:07:49.000000 mara-2.1.0/mara/storage/dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.300925 mara-2.1.0/mara/timers/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-18 13:07:49.000000 mara-2.1.0/mara/timers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-18 13:07:49.000000 mara-2.1.0/mara/timers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-18 13:07:49.000000 mara-2.1.0/mara/timers/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 13:07:52.296925 mara-2.1.0/mara.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-18 13:07:52.000000 mara-2.1.0/mara.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-18 13:07:52.000000 mara-2.1.0/mara.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:07:52.000000 mara-2.1.0/mara.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 13:07:52.000000 mara-2.1.0/mara.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 13:07:52.000000 mara-2.1.0/mara.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 13:07:52.000000 mara-2.1.0/mara.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-18 13:07:52.300925 mara-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-18 13:07:49.000000 mara-2.1.0/setup.py
```

### Comparing `mara-2.0.0/LICENSE` & `mara-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/PKG-INFO` & `mara-2.1.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,22 @@
-Metadata-Version: 2.1
-Name: mara
-Version: 2.0.0
-Summary: A framework for network services
-Home-page: https://radiac.net/projects/mara/
-Author: Richard Terry
-Author-email: code@radiac.net
-License: BSD
-Project-URL: Documentation, https://radiac.net/projects/mara/documentation/
-Project-URL: Source, https://github.com/radiac/mara
-Project-URL: Tracker, https://github.com/radiac/mara/issues
-Keywords: socket telnet http websocket
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Provides-Extra: telnet
-License-File: LICENSE
-
 =======================================
 Mara - Python network service framework
 =======================================
 
-An asynchronous event-based python framework designed for building TCP/IP services, such
-as telnet, HTTP and websocket servers.
+An asynchronous event-based python framework designed for building TCP/IP services - run
+multiple socket, telnet, HTTP and websocket servers from a single async process.
 
 .. image:: https://img.shields.io/pypi/v/mara.svg
     :target: https://pypi.org/project/mara/
     :alt: PyPI
 
+.. image:: https://readthedocs.org/projects/python-mara/badge/?version=latest
+    :target: https://python-mara.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
 .. image:: https://github.com/radiac/mara/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/radiac/mara/actions/workflows/ci.yml
     :alt: Tests
 
 .. image:: https://codecov.io/gh/radiac/mara/branch/main/graph/badge.svg?token=BCNM45T6GI
     :target: https://codecov.io/gh/radiac/mara
     :alt: Test coverage
@@ -49,52 +26,59 @@
 * Source code: https://github.com/radiac/mara
 
 
 Features
 ========
 
 * Asynchronous event-based framework
-* Supports multiple servers
+* Supports multiple servers - text, telnet, HTTP and websockets included
 
 Requires Python 3.10 or later, see installation.
 
-See the `Documentation <http://radiac.net/projects/mara/documentation/>`_
+See the `Documentation <https://python-mara.readthedocs.io/en/latest/>`_
 for details of how Mara works.
 
-Note: Version 2.0.z is in development, and the API is subject to change without notice.
-The last release to support Python 2 and 3.9 was version 0.6.3.
+Note: The last release to support Python 2 and 3.9 was version 0.6.3.
 
 
 Quickstart
 ==========
 
 Install Mara with ``pip install mara``, then write your service using
-`event handlers <http://radiac.net/projects/mara/documentation/api/events/>`_.
+`event handlers <https://python-mara.readthedocs.io/en/latest/events.html>`_.
 
 A minimal Mara service looks something like this::
 
     from mara import App, events
     from mara.servers.socket import SocketServer
 
     app = App()
     app.add_server(SocketServer(host="127.0.0.1", port=9000))
 
-    @app.listen(events.Receive)
+    @app.on(events.Receive)
     async def echo(event: events.Receive):
-        event.client.write(event.data)
+        event.connection.write(event.data)
 
     app.run()
 
 
 Save it as ``echo.py`` and run it::
 
     $ python echo.py
     Server listening: Socket 127.0.0.1:9000
 
 
-Take a look at the
-`examples <https://github.com/radiac/mara/tree/master/examples>`_ to see how to
-start writing more complex services, or read the
-`documentation <http://radiac.net/projects/mara/documentation/>`_ for
-details of how Mara works.
+More examples
+=============
+
+Take a look at the `examples <https://github.com/radiac/mara/tree/master/examples>`_ to
+see how to start writing more complex services:
+
+* Chat over a raw text TCP socket, or one with TLS encryption
+* Chat over a telnet server
+* Chat over a websocket server
+* Two servers, one process: chat between a websocket and a telnet server
+
 
+Read the `documentation <https://python-mara.readthedocs.io/en/latest/>`_ for details of
+how Mara works.
```

### Comparing `mara-2.0.0/mara/app/app.py` & `mara-2.1.0/mara/app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,38 +5,35 @@
 from typing import TYPE_CHECKING, Any, Coroutine, List
 
 from ..events import Event, PostStart, PostStop, PreStart, PreStop
 from ..status import Status
 from . import event_manager
 from .logging import configure as configure_logging
 
-
 if TYPE_CHECKING:
     from ..servers import AbstractServer
     from ..timers import AbstractTimer
 
 configure_logging()
 logger = logging.getLogger("mara.app")
 
 
 class App:
     """
-    Orchestrate servers, clients and tasks
+    Orchestrate servers and tasks
     """
 
     loop: asyncio.AbstractEventLoop | None = None
     servers: List[AbstractServer]
     events: event_manager.EventManager
     timers: List[AbstractTimer]
     _status: Status = Status.IDLE
 
     def __init__(self):
         self.servers = []
-        # TODO: move clients to server
-        self.clients = []
         self.timers = []
 
         self.events = event_manager.EventManager(self)
 
     def add_server(self, server: AbstractServer) -> AbstractServer:
         """
         Add a new Server instance to the async loop
@@ -105,26 +102,28 @@
 
         This will start any Servers which have been added with ``add_server()``
         """
         self._status = Status.STARTING
 
         # TODO: Should add some more logic around here from asyncio.run
         self.loop = loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
         logger.debug("Loop starting")
         loop.run_until_complete(self.events.trigger(PreStart()))
 
         for server in self.servers:
             self.create_task(server.run(self))
 
         for timer in self.timers:
             self.create_task(timer.run(self))
 
         logger.debug("Loop running")
         self._status = Status.RUNNING
         loop.run_until_complete(self.events.trigger(PostStart()))
+
         try:
             loop.run_forever()
         finally:
             logger.debug("Loop stopping")
             self._status = Status.STOPPING
             loop.run_until_complete(self.events.trigger(PreStop()))
             loop.run_until_complete(loop.shutdown_asyncgens())
@@ -148,15 +147,15 @@
         try:
             task.result()
         except asyncio.CancelledError:
             pass
         except Exception:
             logger.exception("Task failed")
 
-    def listen(
+    def on(
         self,
         event_class: type[Event],
         handler: event_manager.HandlerType | None = None,
         **filters: event_manager.FilterType,
     ):
         """
         Bind a handler callback to the specified event class, and to its subclasses
@@ -165,19 +164,25 @@
 
             event_class (Type[Event]): The Event class to listen for
             handler (Awaitable | None): The handler, if not being decorated
             **filters: Key value pairs to match against inbound events
 
         Can be called directly::
 
-            app.listen(Event, handler)
+            app.on(Event, handler)
 
         or can be called as a decorator with no handler argument::
 
-            @app.listen(Event)
+            @app.on(Event)
+            async def callback(event):
+                ...
+
+        and can filter based on event attributes
+
+            @app.on(ServerEvent, server=telnet)
             async def callback(event):
                 ...
         """
         return self.events.listen(event_class, handler, **filters)
 
     @property
     def status(self):
```

### Comparing `mara-2.0.0/mara/app/event_manager.py` & `mara-2.1.0/mara/app/event_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from __future__ import annotations
 
 import logging
 from collections import defaultdict
+from collections.abc import Awaitable, Callable
 from typing import TYPE_CHECKING, Any
 
 from ..events import Event
 
+# Type aliases
+HandlerType = Callable[[Event], Awaitable[None]]
+FilterType = dict[str, Any]
+EventsType = dict[type[Event], list[tuple[HandlerType, FilterType]]]
 
 if TYPE_CHECKING:
-    from collections.abc import Awaitable, Callable
-
     from .app import App
 
-    # Type aliases
-    HandlerType = Callable[[Event], Awaitable[None]]
-    FilterType = dict[str, Any]
-    EventsType = dict[type[Event], list[tuple[HandlerType, FilterType]]]
-
 
 logger = logging.getLogger("mara.event")
 
 
 class EventManager:
     """
     Internal event manager
```

### Comparing `mara-2.0.0/mara/app/logging.py` & `mara-2.1.0/mara/app/logging.py`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/mara/clients/base.py` & `mara-2.1.0/mara/servers/connections/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from ..events import Connect, Disconnect, Receive
-from ..storage.dict import DictStore
-
+from ...events import Connect, Disconnect, Receive
+from ...storage.dict import DictStore
 
 if TYPE_CHECKING:
-    from ..servers import AbstractServer
+    from ..base import AbstractServer
 
 
 ContentType = TypeVar("ContentType")
 
-logger = logging.getLogger("mara.client")
+logger = logging.getLogger("mara.connection")
 
 
-class AbstractClient(Generic[ContentType]):
+class AbstractConnection(Generic[ContentType]):
     server: AbstractServer
     connected: bool
     read_task: asyncio.Task
     write_task: asyncio.Task
     write_queue: asyncio.Queue
     session: DictStore
 
@@ -53,34 +52,38 @@
     async def _write(self, data: ContentType):
         """
         Write to the connection
         """
         raise NotImplementedError()
 
     async def close(self):
-        logger.info(f"Client {self} closed")
+        logger.info(f"Connection {self} closed")
         await self.server.disconnected(self)
 
     def run(self):
         """
-        Add the client read and write tasks to the app's loop
+        Add the connection read and write tasks to the app's loop
         """
+        if not self.server.app:
+            raise ValueError("Connection read loop must be part of an active server")
         self.read_task = self.server.app.create_task(self._read_loop())
         self.write_task = self.server.app.create_task(self._write_loop())
 
     async def _read_loop(self):
         app = self.server.app
+        if not app:
+            raise ValueError("Connection read loop must be part of an active server")
         await app.events.trigger(Connect(self))
-        logger.info(f"Client {self} connected")
+        logger.info(f"Connection {self} connected")
         while self.connected:
             data: ContentType = await self.read()
             if data:
                 await app.events.trigger(Receive(self, data))
 
-        logger.info(f"Client {self} disconnected")
+        logger.info(f"Connection {self} disconnected")
         await app.events.trigger(Disconnect(self))
 
     async def _write_loop(self):
         while self.connected:
             data: ContentType = await self.write_queue.get()
             await self._write(data)
             self.write_queue.task_done()
```

### Comparing `mara-2.0.0/mara/clients/socket.py` & `mara-2.1.0/mara/servers/connections/socket.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Protocol
 
-from .base import AbstractClient
-
+from .base import AbstractConnection
 
 if TYPE_CHECKING:
     from ..servers import AbstractServer
 
 
-class ClientCanStream(Protocol):
-
+class ConnectionCanStream(Protocol):
     reader: asyncio.StreamReader
     writer: asyncio.StreamWriter
 
     def __init__(
         self,
         server: AbstractServer,
         reader: asyncio.StreamReader,
         writer: asyncio.StreamWriter,
-    ):
-        ...
+    ): ...
 
 
-class SocketMixin(AbstractClient):
+class SocketMixin(AbstractConnection):
     """
-    Mixin for any client class which uses byte sockets
+    Mixin for any connection class which uses byte sockets
     """
 
     reader: asyncio.StreamReader
     writer: asyncio.StreamWriter
 
     def __init__(
         self,
@@ -63,27 +60,27 @@
         # Terminate the listener loop
         # TODO
         # this.listener_task
 
         await super().close()
 
 
-class SocketClient(SocketMixin, AbstractClient[bytes]):
+class SocketConnection(SocketMixin, AbstractConnection[bytes]):
     """
     Read and write bytes
     """
 
     async def read(self) -> bytes:
         # TODO: read size and buffers
         data = await self.reader.read(1024)
         self._check_is_active()
         return data
 
 
-class TextClient(SocketMixin, AbstractClient[str]):
+class TextConnection(SocketMixin, AbstractConnection[str]):
     """
     Read and write unicode over an underlying byte socket
     """
 
     async def read(self) -> str:
         # TODO: read size and buffers
         try:
```

### Comparing `mara-2.0.0/mara/clients/telnet.py` & `mara-2.1.0/mara/servers/connections/telnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from telnetlib3 import TelnetReader, TelnetWriter
 
-from .base import AbstractClient
-
+from .base import AbstractConnection
 
 if TYPE_CHECKING:
     from ..servers.telnet import TelnetServer
 
 
-class TelnetClient(AbstractClient[str]):
+class TelnetConnection(AbstractConnection[str]):
     reader: TelnetReader
     writer: TelnetWriter
     _str: str | None = None
 
     def __init__(
         self,
         server: TelnetServer,
```

### Comparing `mara-2.0.0/mara/events/app.py` & `mara-2.1.0/mara/events/app.py`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/mara/events/base.py` & `mara-2.1.0/mara/events/base.py`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/mara/events/server.py` & `mara-2.1.0/mara/events/server.py`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/mara/servers/telnet.py` & `mara-2.1.0/mara/servers/telnet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """
 Telnet server
 
 Wrapper around telnetlib3, https://pypi.org/project/telnetlib3/
 """
-from __future__ import annotations
 
-from telnetlib3 import TelnetReader, TelnetWriter
+from __future__ import annotations
 
-from ..clients.telnet import TelnetClient
 from ..constants import DEFAULT_HOST, DEFAULT_PORT
 from .base import AbstractAsyncioServer
-
+from .connections.telnet import TelnetConnection
 
 try:
     import telnetlib3
 except ImportError:
     raise ValueError("telnetlib3 not found - pip install mara[telnet]")
 
 
 class TelnetServer(AbstractAsyncioServer):
-    client_class: type[TelnetClient] = TelnetClient
+    connection_class: type[TelnetConnection] = TelnetConnection
 
     def __init__(
         self, host: str = DEFAULT_HOST, port: int = DEFAULT_PORT, **telnet_kwargs
     ):
         self.host = host
         self.port = port
 
@@ -35,22 +33,23 @@
         super().__init__()
 
     def __str__(self):
         return f"Telnet {self.host}:{self.port}"
 
     async def create(self):
         await super().create()
-        loop = self.app.loop
-        if loop is None:
+        if not self.app or (loop := self.app.loop) is None:
             raise ValueError("Cannot start TelnetServer without running loop")
 
         self.server = await loop.create_server(
             protocol_factory=lambda: telnetlib3.TelnetServer(**self.telnet_kwargs),
             host=self.host,
             port=self.port,
         )
 
-    async def handle_connect(self, reader: TelnetReader, writer: TelnetWriter):
-        client: TelnetClient = self.client_class(
+    async def handle_connect(
+        self, reader: telnetlib3.TelnetReader, writer: telnetlib3.TelnetWriter
+    ):
+        connection: TelnetConnection = self.connection_class(
             server=self, reader=reader, writer=writer
         )
-        await self.connected(client)
+        await self.connected(connection)
```

### Comparing `mara-2.0.0/mara/storage/base.py` & `mara-2.1.0/mara/storage/base.py`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/mara/storage/dict.py` & `mara-2.1.0/mara/storage/dict.py`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/mara/timers/base.py` & `mara-2.1.0/mara/timers/base.py`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/mara/timers/periodic.py` & `mara-2.1.0/mara/timers/periodic.py`

 * *Files identical despite different names*

### Comparing `mara-2.0.0/mara.egg-info/SOURCES.txt` & `mara-2.1.0/mara.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 mara.egg-info/not-zip-safe
 mara.egg-info/requires.txt
 mara.egg-info/top_level.txt
 mara/app/__init__.py
 mara/app/app.py
 mara/app/event_manager.py
 mara/app/logging.py
-mara/clients/__init__.py
-mara/clients/base.py
-mara/clients/socket.py
-mara/clients/telnet.py
 mara/events/__init__.py
 mara/events/app.py
 mara/events/base.py
-mara/events/client.py
+mara/events/connection.py
 mara/events/server.py
 mara/servers/__init__.py
 mara/servers/base.py
+mara/servers/http.py
 mara/servers/socket.py
 mara/servers/telnet.py
+mara/servers/connections/__init__.py
+mara/servers/connections/base.py
+mara/servers/connections/http.py
+mara/servers/connections/socket.py
+mara/servers/connections/telnet.py
 mara/storage/__init__.py
 mara/storage/base.py
 mara/storage/dict.py
 mara/timers/__init__.py
 mara/timers/base.py
 mara/timers/periodic.py
```

### Comparing `mara-2.0.0/setup.cfg` & `mara-2.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Topic :: Internet
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.10
 url = https://radiac.net/projects/mara/
 project_urls = 
-	Documentation = https://radiac.net/projects/mara/documentation/
+	Documentation = https://python-mara.readthedocs.io/
 	Source = https://github.com/radiac/mara
 	Tracker = https://github.com/radiac/mara/issues
 
 [options]
 python_requires = >=3.10
 packages = find:
 include_package_data = true
@@ -31,17 +31,19 @@
 
 [options.packages.find]
 exclude = tests*
 
 [options.extras_require]
 telnet = 
 	telnetlib3
+http = 
+	aiohttp
 
 [tool:pytest]
-addopts = --black --flake8 --mypy --cov=mara --cov-report=term --cov-report=html
+addopts = --cov=mara --cov-report=term --cov-report=html
 pythonpath = .
 asyncio_mode = auto
 
 [coverage:run]
 parallel = True
 
 [flake8]
```

### Comparing `mara-2.0.0/setup.py` & `mara-2.1.0/setup.py`

 * *Files identical despite different names*

