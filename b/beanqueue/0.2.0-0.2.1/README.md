# Comparing `tmp/beanqueue-0.2.0.tar.gz` & `tmp/beanqueue-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanqueue-0.2.0.tar", max compression
+gzip compressed data, was "beanqueue-0.2.1.tar", max compression
```

## Comparing `beanqueue-0.2.0.tar` & `beanqueue-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1072 2024-05-19 00:56:40.832924 beanqueue-0.2.0/LICENSE
--rw-r--r--   0        0        0    12002 2024-05-19 00:56:40.832924 beanqueue-0.2.0/README.md
--rw-r--r--   0        0        0      375 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/__init__.py
--rw-r--r--   0        0        0     9585 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/app.py
--rw-r--r--   0        0        0        0 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/__init__.py
--rw-r--r--   0        0        0      511 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/create_tables.py
--rw-r--r--   0        0        0      431 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/process.py
--rw-r--r--   0        0        0     1107 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/submit.py
--rw-r--r--   0        0        0      363 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/utils.py
--rw-r--r--   0        0        0     1740 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/config.py
--rw-r--r--   0        0        0      195 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/constants.py
--rw-r--r--   0        0        0        0 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/db/__init__.py
--rw-r--r--   0        0        0       83 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/db/base.py
--rw-r--r--   0        0        0      152 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/db/session.py
--rw-r--r--   0        0        0       60 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/events.py
--rw-r--r--   0        0        0      257 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/models/__init__.py
--rw-r--r--   0        0        0      179 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/models/helpers.py
--rw-r--r--   0        0        0     4243 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/models/task.py
--rw-r--r--   0        0        0     2385 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/models/worker.py
--rw-r--r--   0        0        0        0 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/processors/__init__.py
--rw-r--r--   0        0        0     2301 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/processors/processor.py
--rw-r--r--   0        0        0     1588 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/processors/registry.py
--rw-r--r--   0        0        0        0 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/services/__init__.py
--rw-r--r--   0        0        0     3628 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/services/dispatch.py
--rw-r--r--   0        0        0     3055 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/services/worker.py
--rw-r--r--   0        0        0      219 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/utils.py
--rw-r--r--   0        0        0      630 2024-05-19 00:56:40.832924 beanqueue-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    12743 1970-01-01 00:00:00.000000 beanqueue-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-19 05:55:20.236622 beanqueue-0.2.1/LICENSE
+-rw-r--r--   0        0        0    12022 2024-05-19 05:55:20.236622 beanqueue-0.2.1/README.md
+-rw-r--r--   0        0        0      375 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/__init__.py
+-rw-r--r--   0        0        0    12259 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/app.py
+-rw-r--r--   0        0        0        0 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/__init__.py
+-rw-r--r--   0        0        0      511 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/create_tables.py
+-rw-r--r--   0        0        0      431 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/process.py
+-rw-r--r--   0        0        0     1107 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/submit.py
+-rw-r--r--   0        0        0      363 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/cmds/utils.py
+-rw-r--r--   0        0        0     2001 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/config.py
+-rw-r--r--   0        0        0      195 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/constants.py
+-rw-r--r--   0        0        0        0 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/db/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/db/base.py
+-rw-r--r--   0        0        0      152 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/db/session.py
+-rw-r--r--   0        0        0       60 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/events.py
+-rw-r--r--   0        0        0      257 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/models/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/models/helpers.py
+-rw-r--r--   0        0        0     4243 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/models/task.py
+-rw-r--r--   0        0        0     2385 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/models/worker.py
+-rw-r--r--   0        0        0        0 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/processors/__init__.py
+-rw-r--r--   0        0        0     2301 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/processors/processor.py
+-rw-r--r--   0        0        0     1588 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/processors/registry.py
+-rw-r--r--   0        0        0        0 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/services/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/services/dispatch.py
+-rw-r--r--   0        0        0     3055 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/services/worker.py
+-rw-r--r--   0        0        0      219 2024-05-19 05:55:20.236622 beanqueue-0.2.1/bq/utils.py
+-rw-r--r--   0        0        0      630 2024-05-19 05:55:20.240622 beanqueue-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12763 1970-01-01 00:00:00.000000 beanqueue-0.2.1/PKG-INFO
```

### Comparing `beanqueue-0.2.0/LICENSE` & `beanqueue-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.0/README.md` & `beanqueue-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     PROCESSOR_PACKAGES=["my_pkgs.processors"],
     DATABASE_URL=str(config.DATABASE_URL),
     BATCH_SIZE=10,
 )
 app = bq.BeanQueue(config=config)
 ```
 
-Then you can pass `--app` argument pointing to the app object to the process command like this:
+Then you can pass `--app` argument (or `-a` for short) pointing to the app object to the process command like this:
 
 ```bash
 python -m bq.cmds.process -a my_pkgs.bq.app images
 ```
 
 Or if you prefer to define your own process command, you can also call `process_tasks` of the `BeanQueue` object directly like this:
```

### Comparing `beanqueue-0.2.0/bq/app.py` & `beanqueue-0.2.1/bq/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import functools
 import importlib
+import json
 import logging
 import platform
 import sys
 import threading
 import time
 import typing
+from wsgiref.simple_server import make_server
 
 import venusian
 from sqlalchemy import func
 from sqlalchemy.engine import create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session as DBSession
 from sqlalchemy.pool import SingletonThreadPool
@@ -146,23 +148,80 @@
                 db.commit()
 
             if current_worker.state != models.WorkerState.RUNNING:
                 # This probably means we are somehow very slow to update the heartbeat in time, or the timeout window
                 # is set too short. It could also be the administrator update the worker state to something else than
                 # RUNNING. Regardless the reason, let's stop processing.
                 logger.warning(
-                    "Current worker %s state is %s instead of running, quit processing"
+                    "Current worker %s state is %s instead of running, quit processing",
+                    current_worker.id,
+                    current_worker.state,
                 )
                 sys.exit(0)
 
             time.sleep(self.config.WORKER_HEARTBEAT_PERIOD)
             current_worker.last_heartbeat = func.now()
             db.add(current_worker)
             db.commit()
 
+    def _serve_http_request(
+        self, worker_id: typing.Any, environ: dict, start_response: typing.Callable
+    ) -> list[bytes]:
+        path = environ["PATH_INFO"]
+        if path == "/healthz":
+            db = self.make_session()
+            worker_service = self._make_worker_service(db)
+            worker = worker_service.get_worker(worker_id)
+            if worker is not None and worker.state == models.WorkerState.RUNNING:
+                start_response(
+                    "200 OK",
+                    [
+                        ("Content-Type", "application/json"),
+                    ],
+                )
+                return [
+                    json.dumps(dict(status="ok", worker_id=str(worker_id))).encode(
+                        "utf8"
+                    )
+                ]
+            else:
+                logger.warning("Bad worker %s state %s", worker_id, worker.state)
+                start_response(
+                    "500 Internal Server Error",
+                    [
+                        ("Content-Type", "application/json"),
+                    ],
+                )
+                return [
+                    json.dumps(
+                        dict(
+                            status="internal error",
+                            worker_id=str(worker_id),
+                            state=str(worker.state),
+                        )
+                    ).encode("utf8")
+                ]
+        # TODO: add other metrics endpoints
+        start_response(
+            "404 NOT FOUND",
+            [
+                ("Content-Type", "application/json"),
+            ],
+        )
+        return [json.dumps(dict(status="not found")).encode("utf8")]
+
+    def run_metrics_http_server(self, worker_id: typing.Any):
+        host = self.config.METRICS_HTTP_SERVER_INTERFACE
+        port = self.config.METRICS_HTTP_SERVER_PORT
+        with make_server(
+            host, port, functools.partial(self._serve_http_request, worker_id)
+        ) as httpd:
+            logger.info("Run metrics HTTP server on %s:%s", host, port)
+            httpd.serve_forever()
+
     def process_tasks(
         self,
         channels: tuple[str, ...],
     ):
         db = self.make_session()
         if not channels:
             channels = [constants.DEFAULT_CHANNEL]
@@ -190,14 +249,23 @@
         )
 
         worker = work_service.make_worker(name=platform.node(), channels=channels)
         db.add(worker)
         dispatch_service.listen(channels)
         db.commit()
 
+        metrics_server_thread = None
+        if self.config.METRICS_HTTP_SERVER_ENABLED:
+            metrics_server_thread = threading.Thread(
+                target=self.run_metrics_http_server,
+                args=(worker.id,),
+            )
+            metrics_server_thread.daemon = True
+            metrics_server_thread.start()
+
         logger.info("Created worker %s, name=%s", worker.id, worker.name)
         events.worker_init.send(self, worker=worker)
 
         logger.info("Processing tasks in channels = %s ...", channels)
 
         worker_update_thread = threading.Thread(
             target=functools.partial(
@@ -245,14 +313,16 @@
                 except TimeoutError:
                     logger.debug("Poll timeout, try again")
                     continue
         except (SystemExit, KeyboardInterrupt):
             db.rollback()
             logger.info("Shutting down ...")
             worker_update_thread.join(5)
+            if metrics_server_thread is not None:
+                metrics_server_thread.join(5)
 
         worker.state = models.WorkerState.SHUTDOWN
         db.add(worker)
         task_count = self.worker_service_cls.reschedule_dead_tasks([worker.id])
         logger.info("Reschedule %s tasks", task_count)
         dispatch_service.notify(channels)
         db.commit()
```

### Comparing `beanqueue-0.2.0/bq/cmds/submit.py` & `beanqueue-0.2.1/bq/cmds/submit.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.0/bq/config.py` & `beanqueue-0.2.1/bq/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,14 +26,23 @@
 
     # which task model to use
     TASK_MODEL: str = "bq.Task"
 
     # which worker model to use
     WORKER_MODEL: str = "bq.Worker"
 
+    # Enable metrics HTTP server
+    METRICS_HTTP_SERVER_ENABLED: bool = True
+
+    # the metrics http server interface to listen
+    METRICS_HTTP_SERVER_INTERFACE: str = ""
+
+    # the metrics http server port to listen
+    METRICS_HTTP_SERVER_PORT: int = 8000
+
     POSTGRES_SERVER: str = "localhost"
     POSTGRES_USER: str = "bq"
     POSTGRES_PASSWORD: str = ""
     POSTGRES_DB: str = "bq"
     # The URL of postgresql database to connect
     DATABASE_URL: typing.Optional[PostgresDsn] = None
```

### Comparing `beanqueue-0.2.0/bq/models/task.py` & `beanqueue-0.2.1/bq/models/task.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.0/bq/models/worker.py` & `beanqueue-0.2.1/bq/models/worker.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.0/bq/processors/processor.py` & `beanqueue-0.2.1/bq/processors/processor.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.0/bq/processors/registry.py` & `beanqueue-0.2.1/bq/processors/registry.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.0/bq/services/dispatch.py` & `beanqueue-0.2.1/bq/services/dispatch.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.0/bq/services/worker.py` & `beanqueue-0.2.1/bq/services/worker.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.2.0/pyproject.toml` & `beanqueue-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanqueue"
-version = "0.2.0"
+version = "0.2.1"
 description = "BeanQueue or BQ for short, PostgreSQL SKIP LOCK based worker queue library"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "bq" },
 ]
```

### Comparing `beanqueue-0.2.0/PKG-INFO` & `beanqueue-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanqueue
-Version: 0.2.0
+Version: 0.2.1
 Summary: BeanQueue or BQ for short, PostgreSQL SKIP LOCK based worker queue library
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -147,15 +147,15 @@
     PROCESSOR_PACKAGES=["my_pkgs.processors"],
     DATABASE_URL=str(config.DATABASE_URL),
     BATCH_SIZE=10,
 )
 app = bq.BeanQueue(config=config)
 ```
 
-Then you can pass `--app` argument pointing to the app object to the process command like this:
+Then you can pass `--app` argument (or `-a` for short) pointing to the app object to the process command like this:
 
 ```bash
 python -m bq.cmds.process -a my_pkgs.bq.app images
 ```
 
 Or if you prefer to define your own process command, you can also call `process_tasks` of the `BeanQueue` object directly like this:
```

