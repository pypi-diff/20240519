# Comparing `tmp/beanqueue-0.2.1.tar.gz` & `tmp/beanqueue-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanqueue-0.2.1.tar", max compression
+gzip compressed data, was "beanqueue-0.2.2.tar", max compression
```

## Comparing `beanqueue-0.2.1.tar` & `beanqueue-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1072 2024-05-19 05:55:20.236622 beanqueue-0.2.1/LICENSE
--rw-r--r--   0        0        0    12022 2024-05-19 05:55:20.236622 beanqueue-0.2.1/README.md
--rw-r--r--   0        0        0      375 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/__init__.py
--rw-r--r--   0        0        0    12259 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/app.py
--rw-r--r--   0        0        0        0 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/__init__.py
--rw-r--r--   0        0        0      511 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/create_tables.py
--rw-r--r--   0        0        0      431 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/process.py
--rw-r--r--   0        0        0     1107 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/submit.py
--rw-r--r--   0        0        0      363 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/utils.py
--rw-r--r--   0        0        0     2001 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/config.py
--rw-r--r--   0        0        0      195 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/constants.py
--rw-r--r--   0        0        0        0 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/db/__init__.py
--rw-r--r--   0        0        0       83 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/db/base.py
--rw-r--r--   0        0        0      152 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/db/session.py
--rw-r--r--   0        0        0       60 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/events.py
--rw-r--r--   0        0        0      257 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/models/__init__.py
--rw-r--r--   0        0        0      179 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/models/helpers.py
--rw-r--r--   0        0        0     4243 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/models/task.py
--rw-r--r--   0        0        0     2385 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/models/worker.py
--rw-r--r--   0        0        0        0 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/processors/__init__.py
--rw-r--r--   0        0        0     2301 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/processors/processor.py
--rw-r--r--   0        0        0     1588 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/processors/registry.py
--rw-r--r--   0        0        0        0 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/services/__init__.py
--rw-r--r--   0        0        0     3628 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/services/dispatch.py
--rw-r--r--   0        0        0     3055 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/services/worker.py
--rw-r--r--   0        0        0      219 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/utils.py
--rw-r--r--   0        0        0      630 2024-05-19 05:55:20.240622 beanqueue-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    12763 1970-01-01 00:00:00.000000 beanqueue-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-19 06:44:27.236056 beanqueue-0.2.2/LICENSE
+-rw-r--r--   0        0        0    12022 2024-05-19 06:44:27.236056 beanqueue-0.2.2/README.md
+-rw-r--r--   0        0        0      375 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/__init__.py
+-rw-r--r--   0        0        0    12947 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/app.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/cmds/__init__.py
+-rw-r--r--   0        0        0      511 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/cmds/create_tables.py
+-rw-r--r--   0        0        0      431 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/cmds/process.py
+-rw-r--r--   0        0        0     1107 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/cmds/submit.py
+-rw-r--r--   0        0        0      363 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/cmds/utils.py
+-rw-r--r--   0        0        0     2094 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/config.py
+-rw-r--r--   0        0        0      195 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/constants.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/db/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/db/base.py
+-rw-r--r--   0        0        0      152 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/db/session.py
+-rw-r--r--   0        0        0       60 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/events.py
+-rw-r--r--   0        0        0      257 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/models/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/models/helpers.py
+-rw-r--r--   0        0        0     4243 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/models/task.py
+-rw-r--r--   0        0        0     2385 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/models/worker.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/processors/__init__.py
+-rw-r--r--   0        0        0     2301 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/processors/processor.py
+-rw-r--r--   0        0        0     1588 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/processors/registry.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/services/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/services/dispatch.py
+-rw-r--r--   0        0        0     3055 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/services/worker.py
+-rw-r--r--   0        0        0      219 2024-05-19 06:44:27.236056 beanqueue-0.2.2/bq/utils.py
+-rw-r--r--   0        0        0      630 2024-05-19 06:44:27.236056 beanqueue-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    12763 1970-01-01 00:00:00.000000 beanqueue-0.2.2/PKG-INFO
```

### Comparing `beanqueue-0.2.1/LICENSE` & `beanqueue-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/README.md` & `beanqueue-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/bq/app.py` & `beanqueue-0.2.2/bq/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import platform
 import sys
 import threading
 import time
 import typing
 from wsgiref.simple_server import make_server
+from wsgiref.simple_server import WSGIRequestHandler
 
 import venusian
 from sqlalchemy import func
 from sqlalchemy.engine import create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session as DBSession
 from sqlalchemy.pool import SingletonThreadPool
@@ -27,14 +28,29 @@
 from .services.dispatch import DispatchService
 from .services.worker import WorkerService
 from .utils import load_module_var
 
 logger = logging.getLogger(__name__)
 
 
+class WSGIRequestHandlerWithLogger(WSGIRequestHandler):
+    logger = logging.getLogger("metrics_server")
+
+    def log_message(self, format, *args):
+        message = format % args
+        self.logger.info(
+            "%s - - [%s] %s\n"
+            % (
+                self.address_string(),
+                self.log_date_time_string(),
+                message.translate(self._control_char_table),
+            )
+        )
+
+
 class BeanQueue:
     def __init__(
         self,
         config: Config | None = None,
         session_cls: DBSession = SessionMaker,
         worker_service_cls: typing.Type[WorkerService] = WorkerService,
         dispatch_service_cls: typing.Type[DispatchService] = DispatchService,
@@ -209,15 +225,18 @@
         )
         return [json.dumps(dict(status="not found")).encode("utf8")]
 
     def run_metrics_http_server(self, worker_id: typing.Any):
         host = self.config.METRICS_HTTP_SERVER_INTERFACE
         port = self.config.METRICS_HTTP_SERVER_PORT
         with make_server(
-            host, port, functools.partial(self._serve_http_request, worker_id)
+            host,
+            port,
+            functools.partial(self._serve_http_request, worker_id),
+            handler_class=WSGIRequestHandlerWithLogger,
         ) as httpd:
             logger.info("Run metrics HTTP server on %s:%s", host, port)
             httpd.serve_forever()
 
     def process_tasks(
         self,
         channels: tuple[str, ...],
@@ -251,14 +270,17 @@
         worker = work_service.make_worker(name=platform.node(), channels=channels)
         db.add(worker)
         dispatch_service.listen(channels)
         db.commit()
 
         metrics_server_thread = None
         if self.config.METRICS_HTTP_SERVER_ENABLED:
+            WSGIRequestHandlerWithLogger.logger.setLevel(
+                self.config.METRICS_HTTP_SERVER_LOG_LEVEL
+            )
             metrics_server_thread = threading.Thread(
                 target=self.run_metrics_http_server,
                 args=(worker.id,),
             )
             metrics_server_thread.daemon = True
             metrics_server_thread.start()
```

### Comparing `beanqueue-0.2.1/bq/cmds/submit.py` & `beanqueue-0.2.2/bq/cmds/submit.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/bq/config.py` & `beanqueue-0.2.2/bq/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 
     # the metrics http server interface to listen
     METRICS_HTTP_SERVER_INTERFACE: str = ""
 
     # the metrics http server port to listen
     METRICS_HTTP_SERVER_PORT: int = 8000
 
+    # default log level for metrics http server
+    METRICS_HTTP_SERVER_LOG_LEVEL: int = 30
+
     POSTGRES_SERVER: str = "localhost"
     POSTGRES_USER: str = "bq"
     POSTGRES_PASSWORD: str = ""
     POSTGRES_DB: str = "bq"
     # The URL of postgresql database to connect
     DATABASE_URL: typing.Optional[PostgresDsn] = None
```

### Comparing `beanqueue-0.2.1/bq/models/task.py` & `beanqueue-0.2.2/bq/models/task.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/bq/models/worker.py` & `beanqueue-0.2.2/bq/models/worker.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/bq/processors/processor.py` & `beanqueue-0.2.2/bq/processors/processor.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/bq/processors/registry.py` & `beanqueue-0.2.2/bq/processors/registry.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/bq/services/dispatch.py` & `beanqueue-0.2.2/bq/services/dispatch.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/bq/services/worker.py` & `beanqueue-0.2.2/bq/services/worker.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.1/pyproject.toml` & `beanqueue-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanqueue"
-version = "0.2.1"
+version = "0.2.2"
 description = "BeanQueue or BQ for short, PostgreSQL SKIP LOCK based worker queue library"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "bq" },
 ]
```

### Comparing `beanqueue-0.2.1/PKG-INFO` & `beanqueue-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanqueue
-Version: 0.2.1
+Version: 0.2.2
 Summary: BeanQueue or BQ for short, PostgreSQL SKIP LOCK based worker queue library
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

