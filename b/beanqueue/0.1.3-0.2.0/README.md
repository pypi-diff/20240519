# Comparing `tmp/beanqueue-0.1.3.tar.gz` & `tmp/beanqueue-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanqueue-0.1.3.tar", max compression
+gzip compressed data, was "beanqueue-0.2.0.tar", max compression
```

## Comparing `beanqueue-0.1.3.tar` & `beanqueue-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0     1072 2024-05-17 22:52:04.409528 beanqueue-0.1.3/LICENSE
--rw-r--r--   0        0        0    11939 2024-05-17 22:52:04.409528 beanqueue-0.1.3/README.md
--rw-r--r--   0        0        0      440 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/__init__.py
--rw-r--r--   0        0        0        0 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/cmds/__init__.py
--rw-r--r--   0        0        0      609 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/cmds/create_tables.py
--rw-r--r--   0        0        0     6579 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/cmds/process.py
--rw-r--r--   0        0        0     1148 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/cmds/submit.py
--rw-r--r--   0        0        0     1740 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/config.py
--rw-r--r--   0        0        0      195 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/constants.py
--rw-r--r--   0        0        0     2332 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/container.py
--rw-r--r--   0        0        0        0 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/db/__init__.py
--rw-r--r--   0        0        0       83 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/db/base.py
--rw-r--r--   0        0        0      152 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/db/session.py
--rw-r--r--   0        0        0      257 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/models/__init__.py
--rw-r--r--   0        0        0      179 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/models/helpers.py
--rw-r--r--   0        0        0     4243 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/models/task.py
--rw-r--r--   0        0        0     2385 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/models/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/processors/__init__.py
--rw-r--r--   0        0        0     4522 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/processors/registry.py
--rw-r--r--   0        0        0        0 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/services/__init__.py
--rw-r--r--   0        0        0     3628 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/services/dispatch.py
--rw-r--r--   0        0        0     3055 2024-05-17 22:52:04.409528 beanqueue-0.1.3/bq/services/worker.py
--rw-r--r--   0        0        0      643 2024-05-17 22:52:04.409528 beanqueue-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    12693 1970-01-01 00:00:00.000000 beanqueue-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-19 00:56:40.832924 beanqueue-0.2.0/LICENSE
+-rw-r--r--   0        0        0    12002 2024-05-19 00:56:40.832924 beanqueue-0.2.0/README.md
+-rw-r--r--   0        0        0      375 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/__init__.py
+-rw-r--r--   0        0        0     9585 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/app.py
+-rw-r--r--   0        0        0        0 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/__init__.py
+-rw-r--r--   0        0        0      511 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/create_tables.py
+-rw-r--r--   0        0        0      431 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/process.py
+-rw-r--r--   0        0        0     1107 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/submit.py
+-rw-r--r--   0        0        0      363 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/cmds/utils.py
+-rw-r--r--   0        0        0     1740 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/config.py
+-rw-r--r--   0        0        0      195 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/constants.py
+-rw-r--r--   0        0        0        0 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/db/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/db/base.py
+-rw-r--r--   0        0        0      152 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/db/session.py
+-rw-r--r--   0        0        0       60 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/events.py
+-rw-r--r--   0        0        0      257 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/models/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/models/helpers.py
+-rw-r--r--   0        0        0     4243 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/models/task.py
+-rw-r--r--   0        0        0     2385 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/models/worker.py
+-rw-r--r--   0        0        0        0 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/processors/__init__.py
+-rw-r--r--   0        0        0     2301 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/processors/processor.py
+-rw-r--r--   0        0        0     1588 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/processors/registry.py
+-rw-r--r--   0        0        0        0 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/services/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/services/dispatch.py
+-rw-r--r--   0        0        0     3055 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/services/worker.py
+-rw-r--r--   0        0        0      219 2024-05-19 00:56:40.832924 beanqueue-0.2.0/bq/utils.py
+-rw-r--r--   0        0        0      630 2024-05-19 00:56:40.832924 beanqueue-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12743 1970-01-01 00:00:00.000000 beanqueue-0.2.0/PKG-INFO
```

### Comparing `beanqueue-0.1.3/LICENSE` & `beanqueue-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.3/README.md` & `beanqueue-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,25 +26,28 @@
 ```python
 from sqlalchemy.orm import Session
 
 import bq
 from .. import models
 from .. import image_utils
 
-@bq.processor(channel="images")
+app = bq.BeanQueue()
+
+@app.processor(channel="images")
 def resize_image(db: Session, task: bq.Task, width: int, height: int):
     image = db.query(models.Image).filter(models.Image.task == task).one()
     image_utils.resize(image, size=(width, height))
     db.add(image)
     # by default the `processor` decorator has `auto_complete` flag turns on,
     # so it will commit the db changes for us automatically
 ```
 
 The `db` and `task` keyword arguments are optional.
 If you don't need to access the task object, you can simply define the function without these two parameters.
+We also provide an optional `savepoint` argument in case if you want to rollback database changes you made.
 
 To submit a task, you can either use `bq.Task` model object to construct the task object, insert into the
 database session and commit.
 
 ```python
 import bq
 from .db import Session
@@ -106,36 +109,43 @@
 
 ### Configurations
 
 Configurations can be modified by setting environment variables with `BQ_` prefix.
 For example, to set the python packages to scan for processors, you can set `BQ_PROCESSOR_PACKAGES`.
 To change the PostgreSQL database to connect to, you can set `BQ_DATABASE_URL`.
 The complete definition of configurations can be found at the [bq/config.py](bq/config.py) module.
-For now, the configurations only affect command line tools.
 
-If you want to configure BeanQueue programmatically for the command lines, you can override our [dependency-injector](https://python-dependency-injector.ets-labs.org/)'s container defined at [bq/container.py](bq/container.py) and call the command function manually.
+If you want to configure BeanQueue programmatically, you can pass in `Config` object to the `bq.BeanQueue` object when creating.
 For example:
 
 ```python
 import bq
-from bq.cmds.process import process_tasks
 from .my_config import config
 
 container = bq.Container()
 container.wire(packages=[bq])
 config = bq.Config(
     PROCESSOR_PACKAGES=["my_pkgs.processors"],
     DATABASE_URL=str(config.DATABASE_URL),
     BATCH_SIZE=10,
 )
-with container.config.override(config):
-    process_tasks(channels=("images",))
+app = bq.BeanQueue(config=config)
+```
+
+Then you can pass `--app` argument pointing to the app object to the process command like this:
+
+```bash
+python -m bq.cmds.process -a my_pkgs.bq.app images
 ```
 
-Many other behaviors of this framework can also be modified by overriding the container defined at [bq/container.py](bq/container.py).
+Or if you prefer to define your own process command, you can also call `process_tasks` of the `BeanQueue` object directly like this:
+
+```python
+app.process_tasks(channels=("images",))
+```
 
 ### Define your own tables
 
 BeanQueue is designed to be as customizable as much as possible.
 Of course, you can define your own SQLAlchemy model instead of using the ones we provided. 
 
 To make defining your own `Task` model or `Worker` model much easier, you can use our mixin classes:
@@ -207,15 +217,15 @@
 ```python
 import bq
 config = bq.Config(
     TASK_MODEL="my_pkgs.models.Task",
     WORKER_MODEL="my_pkgs.models.Worker",
     # ... other configs
 )
-# Override container...
+app = bq.BeanQueue(config)
 ```
 
 ## Why?
 
 There are countless worker queue projects. Why make yet another one?
 The primary issue with most worker queue tools is their reliance on a standalone broker server.
 Our worker queue tasks frequently interact with the database, and the atomic nature of database transactions is great for data integrity.
```

### Comparing `beanqueue-0.1.3/bq/cmds/process.py` & `beanqueue-0.2.0/bq/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,186 +3,258 @@
 import logging
 import platform
 import sys
 import threading
 import time
 import typing
 
-import click
-from dependency_injector.wiring import inject
-from dependency_injector.wiring import Provide
+import venusian
 from sqlalchemy import func
+from sqlalchemy.engine import create_engine
+from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session as DBSession
+from sqlalchemy.pool import SingletonThreadPool
 
-from .. import constants
-from .. import models
-from ..config import Config
-from ..container import Container
-from ..processors.registry import collect
-from ..services.dispatch import DispatchService
-from ..services.worker import WorkerService
-
-
-@inject
-def update_workers(
-    worker_id: typing.Any,
-    config: Config = Provide[Container.config],
-    session_factory: typing.Callable = Provide[Container.session_factory],
-    make_dispatch_service: typing.Callable = Provide[Container.make_dispatch_service],
-    make_worker_service: typing.Callable = Provide[Container.make_worker_service],
-):
-    db: DBSession = session_factory()
-    worker_service: WorkerService = make_worker_service(session=db)
-    dispatch_service: DispatchService = make_dispatch_service(session=db)
-    current_worker = worker_service.get_worker(worker_id)
-    logger = logging.getLogger(__name__)
-    logger.info(
-        "Updating worker %s with heartbeat_period=%s, heartbeat_timeout=%s",
-        current_worker.id,
-        config.WORKER_HEARTBEAT_PERIOD,
-        config.WORKER_HEARTBEAT_TIMEOUT,
-    )
-    while True:
-        dead_workers = worker_service.fetch_dead_workers(
-            timeout=config.WORKER_HEARTBEAT_TIMEOUT
-        )
-        task_count = worker_service.reschedule_dead_tasks(
-            # TODO: a better way to abstract this?
-            dead_workers.with_entities(current_worker.__class__.id)
-        )
-        found_dead_worker = False
-        for dead_worker in dead_workers:
-            found_dead_worker = True
-            logger.info(
-                "Found dead worker %s (name=%s), reschedule %s dead tasks in channels %s",
-                dead_worker.id,
-                dead_worker.name,
-                task_count,
-                dead_worker.channels,
-            )
-            dispatch_service.notify(dead_worker.channels)
-        if found_dead_worker:
-            db.commit()
+from . import constants
+from . import events
+from . import models
+from .config import Config
+from .db.session import SessionMaker
+from .processors.processor import Processor
+from .processors.processor import ProcessorHelper
+from .processors.registry import collect
+from .services.dispatch import DispatchService
+from .services.worker import WorkerService
+from .utils import load_module_var
+
+logger = logging.getLogger(__name__)
+
+
+class BeanQueue:
+    def __init__(
+        self,
+        config: Config | None = None,
+        session_cls: DBSession = SessionMaker,
+        worker_service_cls: typing.Type[WorkerService] = WorkerService,
+        dispatch_service_cls: typing.Type[DispatchService] = DispatchService,
+        engine: Engine | None = None,
+    ):
+        self.config = config if config is not None else Config()
+        self.session_cls = session_cls
+        self.worker_service_cls = worker_service_cls
+        self.dispatch_service_cls = dispatch_service_cls
+        self._engine = engine
+
+    def create_default_engine(self):
+        return create_engine(
+            str(self.config.DATABASE_URL), poolclass=SingletonThreadPool
+        )
 
-        if current_worker.state != models.WorkerState.RUNNING:
-            # This probably means we are somehow very slow to update the heartbeat in time, or the timeout window
-            # is set too short. It could also be the administrator update the worker state to something else than
-            # RUNNING. Regardless the reason, let's stop processing.
-            logger.warning(
-                "Current worker %s state is %s instead of running, quit processing"
+    def make_session(self) -> DBSession:
+        return self.session_cls(bind=self.engine)
+
+    @property
+    def engine(self) -> Engine:
+        if self._engine is None:
+            self._engine = self.create_default_engine()
+        return self._engine
+
+    @property
+    def task_model(self) -> typing.Type[models.Task]:
+        return load_module_var(self.config.TASK_MODEL)
+
+    @property
+    def worker_model(self) -> typing.Type[models.Worker]:
+        return load_module_var(self.config.WORKER_MODEL)
+
+    def _make_worker_service(self, session: DBSession):
+        return self.worker_service_cls(
+            session=session, task_model=self.task_model, worker_model=self.worker_model
+        )
+
+    def _make_dispatch_service(self, session: DBSession):
+        return self.dispatch_service_cls(session=session, task_model=self.task_model)
+
+    def processor(
+        self,
+        channel: str = constants.DEFAULT_CHANNEL,
+        auto_complete: bool = True,
+        auto_rollback_on_exc: bool = True,
+        task_model: typing.Type | None = None,
+    ) -> typing.Callable:
+        def decorator(wrapped: typing.Callable):
+            processor = Processor(
+                module=wrapped.__module__,
+                name=wrapped.__name__,
+                channel=channel,
+                func=wrapped,
+                auto_complete=auto_complete,
+                auto_rollback_on_exc=auto_rollback_on_exc,
+            )
+            helper_obj = ProcessorHelper(
+                processor,
+                task_cls=task_model if task_model is not None else self.task_model,
             )
-            sys.exit(0)
 
-        time.sleep(config.WORKER_HEARTBEAT_PERIOD)
-        current_worker.last_heartbeat = func.now()
-        db.add(current_worker)
-        db.commit()
+            def callback(scanner: venusian.Scanner, name: str, ob: typing.Callable):
+                if processor.name != name:
+                    raise ValueError("Name is not the same")
+                scanner.registry.add(processor)
 
+            venusian.attach(
+                helper_obj, callback, category=constants.BQ_PROCESSOR_CATEGORY
+            )
+            return helper_obj
+
+        return decorator
 
-@inject
-def process_tasks(
-    channels: tuple[str, ...],
-    config: Config = Provide[Container.config],
-    db: DBSession = Provide[Container.session],
-    dispatch_service: DispatchService = Provide[Container.dispatch_service],
-    worker_service: WorkerService = Provide[Container.worker_service],
-):
-    logger = logging.getLogger(__name__)
-
-    if not channels:
-        channels = [constants.DEFAULT_CHANNEL]
-
-    if not config.PROCESSOR_PACKAGES:
-        logger.error("No PROCESSOR_PACKAGES provided")
-        sys.exit(-1)
-
-    logger.info("Scanning packages %s", config.PROCESSOR_PACKAGES)
-    pkgs = list(map(importlib.import_module, config.PROCESSOR_PACKAGES))
-    registry = collect(pkgs)
-    for channel, module_processors in registry.processors.items():
-        logger.info("Collected processors with channel %r", channel)
-        for module, func_processors in module_processors.items():
-            for processor in func_processors.values():
+    def update_workers(
+        self,
+        worker_id: typing.Any,
+    ):
+        db = self.make_session()
+
+        worker_service = self._make_worker_service(db)
+        dispatch_service = self._make_dispatch_service(db)
+
+        current_worker = worker_service.get_worker(worker_id)
+        logger.info(
+            "Updating worker %s with heartbeat_period=%s, heartbeat_timeout=%s",
+            current_worker.id,
+            self.config.WORKER_HEARTBEAT_PERIOD,
+            self.config.WORKER_HEARTBEAT_TIMEOUT,
+        )
+        while True:
+            dead_workers = worker_service.fetch_dead_workers(
+                timeout=self.config.WORKER_HEARTBEAT_TIMEOUT
+            )
+            task_count = worker_service.reschedule_dead_tasks(
+                # TODO: a better way to abstract this?
+                dead_workers.with_entities(current_worker.__class__.id)
+            )
+            found_dead_worker = False
+            for dead_worker in dead_workers:
+                found_dead_worker = True
                 logger.info(
-                    "  Processor module %r, processor %r", module, processor.name
+                    "Found dead worker %s (name=%s), reschedule %s dead tasks in channels %s",
+                    dead_worker.id,
+                    dead_worker.name,
+                    task_count,
+                    dead_worker.channels,
                 )
+                dispatch_service.notify(dead_worker.channels)
+            if found_dead_worker:
+                db.commit()
+
+            if current_worker.state != models.WorkerState.RUNNING:
+                # This probably means we are somehow very slow to update the heartbeat in time, or the timeout window
+                # is set too short. It could also be the administrator update the worker state to something else than
+                # RUNNING. Regardless the reason, let's stop processing.
+                logger.warning(
+                    "Current worker %s state is %s instead of running, quit processing"
+                )
+                sys.exit(0)
 
-    worker = worker_service.make_worker(name=platform.node(), channels=channels)
-    db.add(worker)
-    dispatch_service.listen(channels)
-    db.commit()
-
-    logger.info("Created worker %s, name=%s", worker.id, worker.name)
-    logger.info("Processing tasks in channels = %s ...", channels)
-
-    worker_update_thread = threading.Thread(
-        target=functools.partial(
-            update_workers,
-            worker_id=worker.id,
-        ),
-        name="update_workers",
-    )
-    worker_update_thread.daemon = True
-    worker_update_thread.start()
-
-    worker_id = worker.id
+            time.sleep(self.config.WORKER_HEARTBEAT_PERIOD)
+            current_worker.last_heartbeat = func.now()
+            db.add(current_worker)
+            db.commit()
 
-    try:
-        while True:
-            while True:
-                tasks = dispatch_service.dispatch(
-                    channels,
-                    worker_id=worker_id,
-                    limit=config.BATCH_SIZE,
-                ).all()
-                for task in tasks:
+    def process_tasks(
+        self,
+        channels: tuple[str, ...],
+    ):
+        db = self.make_session()
+        if not channels:
+            channels = [constants.DEFAULT_CHANNEL]
+
+        if not self.config.PROCESSOR_PACKAGES:
+            logger.error("No PROCESSOR_PACKAGES provided")
+            raise ValueError("No PROCESSOR_PACKAGES provided")
+
+        logger.info("Scanning packages %s", self.config.PROCESSOR_PACKAGES)
+        pkgs = list(map(importlib.import_module, self.config.PROCESSOR_PACKAGES))
+        registry = collect(pkgs)
+        for channel, module_processors in registry.processors.items():
+            logger.info("Collected processors with channel %r", channel)
+            for module, func_processors in module_processors.items():
+                for processor in func_processors.values():
                     logger.info(
-                        "Processing task %s, channel=%s, module=%s, func=%s",
-                        task.id,
-                        task.channel,
-                        task.module,
-                        task.func_name,
+                        "  Processor module=%r, name=%r", module, processor.name
                     )
-                    # TODO: support processor pool and other approaches to dispatch the workload
-                    registry.process(task)
-                if not tasks:
-                    # we should try to keep dispatching until we cannot find tasks
-                    break
-                else:
-                    db.commit()
-            # we will not see notifications in a transaction, need to close the transaction first before entering
-            # polling
-            db.close()
-            try:
-                for notification in dispatch_service.poll(timeout=config.POLL_TIMEOUT):
-                    logger.debug("Receive notification %s", notification)
-            except TimeoutError:
-                logger.debug("Poll timeout, try again")
-                continue
-    except (SystemExit, KeyboardInterrupt):
-        db.rollback()
-        logger.info("Shutting down ...")
-        worker_update_thread.join(5)
-
-    worker.state = models.WorkerState.SHUTDOWN
-    db.add(worker)
-    task_count = worker_service.reschedule_dead_tasks([worker.id])
-    logger.info("Reschedule %s tasks", task_count)
-    dispatch_service.notify(channels)
-    db.commit()
-
-    logger.info("Shutdown gracefully")
-
-
-@click.command()
-@click.argument("channels", nargs=-1)
-def main(
-    channels: tuple[str, ...],
-):
-    process_tasks(channels)
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.INFO)
-    container = Container()
-    container.wire(modules=[__name__])
-    main()
+
+        dispatch_service = self.dispatch_service_cls(
+            session=db, task_model=self.task_model
+        )
+        work_service = self.worker_service_cls(
+            session=db, task_model=self.task_model, worker_model=self.worker_model
+        )
+
+        worker = work_service.make_worker(name=platform.node(), channels=channels)
+        db.add(worker)
+        dispatch_service.listen(channels)
+        db.commit()
+
+        logger.info("Created worker %s, name=%s", worker.id, worker.name)
+        events.worker_init.send(self, worker=worker)
+
+        logger.info("Processing tasks in channels = %s ...", channels)
+
+        worker_update_thread = threading.Thread(
+            target=functools.partial(
+                self.update_workers,
+                worker_id=worker.id,
+            ),
+            name="update_workers",
+        )
+        worker_update_thread.daemon = True
+        worker_update_thread.start()
+
+        worker_id = worker.id
+
+        try:
+            while True:
+                while True:
+                    tasks = dispatch_service.dispatch(
+                        channels,
+                        worker_id=worker_id,
+                        limit=self.config.BATCH_SIZE,
+                    ).all()
+                    for task in tasks:
+                        logger.info(
+                            "Processing task %s, channel=%s, module=%s, func=%s",
+                            task.id,
+                            task.channel,
+                            task.module,
+                            task.func_name,
+                        )
+                        # TODO: support processor pool and other approaches to dispatch the workload
+                        registry.process(task)
+                    if not tasks:
+                        # we should try to keep dispatching until we cannot find tasks
+                        break
+                    else:
+                        db.commit()
+                # we will not see notifications in a transaction, need to close the transaction first before entering
+                # polling
+                db.close()
+                try:
+                    for notification in dispatch_service.poll(
+                        timeout=self.config.POLL_TIMEOUT
+                    ):
+                        logger.debug("Receive notification %s", notification)
+                except TimeoutError:
+                    logger.debug("Poll timeout, try again")
+                    continue
+        except (SystemExit, KeyboardInterrupt):
+            db.rollback()
+            logger.info("Shutting down ...")
+            worker_update_thread.join(5)
+
+        worker.state = models.WorkerState.SHUTDOWN
+        db.add(worker)
+        task_count = self.worker_service_cls.reschedule_dead_tasks([worker.id])
+        logger.info("Reschedule %s tasks", task_count)
+        dispatch_service.notify(channels)
+        db.commit()
+
+        logger.info("Shutdown gracefully")
```

### Comparing `beanqueue-0.1.3/bq/config.py` & `beanqueue-0.2.0/bq/config.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.3/bq/models/task.py` & `beanqueue-0.2.0/bq/models/task.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.3/bq/models/worker.py` & `beanqueue-0.2.0/bq/models/worker.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.3/bq/services/dispatch.py` & `beanqueue-0.2.0/bq/services/dispatch.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.3/bq/services/worker.py` & `beanqueue-0.2.0/bq/services/worker.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.3/pyproject.toml` & `beanqueue-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "beanqueue"
-version = "0.1.3"
+version = "0.2.0"
 description = "BeanQueue or BQ for short, PostgreSQL SKIP LOCK based worker queue library"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "bq" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sqlalchemy = "^2.0.30"
 venusian = "^3.1.0"
 click = "^8.1.7"
-dependency-injector = "^4.41.0"
 pydantic-settings = "^2.2.1"
 pg-activity = "^3.5.1"
+blinker = "^1.8.2"
 
 
 [tool.poetry.group.dev.dependencies]
 psycopg2-binary = "^2.9.9"
 pytest-factoryboy = "^2.7.0"
 
 [build-system]
```

### Comparing `beanqueue-0.1.3/PKG-INFO` & `beanqueue-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: beanqueue
-Version: 0.1.3
+Version: 0.2.0
 Summary: BeanQueue or BQ for short, PostgreSQL SKIP LOCK based worker queue library
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: blinker (>=1.8.2,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: dependency-injector (>=4.41.0,<5.0.0)
 Requires-Dist: pg-activity (>=3.5.1,<4.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Requires-Dist: venusian (>=3.1.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # BeanQueue  [![CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/bq/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-extract/tree/master)
@@ -46,25 +46,28 @@
 ```python
 from sqlalchemy.orm import Session
 
 import bq
 from .. import models
 from .. import image_utils
 
-@bq.processor(channel="images")
+app = bq.BeanQueue()
+
+@app.processor(channel="images")
 def resize_image(db: Session, task: bq.Task, width: int, height: int):
     image = db.query(models.Image).filter(models.Image.task == task).one()
     image_utils.resize(image, size=(width, height))
     db.add(image)
     # by default the `processor` decorator has `auto_complete` flag turns on,
     # so it will commit the db changes for us automatically
 ```
 
 The `db` and `task` keyword arguments are optional.
 If you don't need to access the task object, you can simply define the function without these two parameters.
+We also provide an optional `savepoint` argument in case if you want to rollback database changes you made.
 
 To submit a task, you can either use `bq.Task` model object to construct the task object, insert into the
 database session and commit.
 
 ```python
 import bq
 from .db import Session
@@ -126,36 +129,43 @@
 
 ### Configurations
 
 Configurations can be modified by setting environment variables with `BQ_` prefix.
 For example, to set the python packages to scan for processors, you can set `BQ_PROCESSOR_PACKAGES`.
 To change the PostgreSQL database to connect to, you can set `BQ_DATABASE_URL`.
 The complete definition of configurations can be found at the [bq/config.py](bq/config.py) module.
-For now, the configurations only affect command line tools.
 
-If you want to configure BeanQueue programmatically for the command lines, you can override our [dependency-injector](https://python-dependency-injector.ets-labs.org/)'s container defined at [bq/container.py](bq/container.py) and call the command function manually.
+If you want to configure BeanQueue programmatically, you can pass in `Config` object to the `bq.BeanQueue` object when creating.
 For example:
 
 ```python
 import bq
-from bq.cmds.process import process_tasks
 from .my_config import config
 
 container = bq.Container()
 container.wire(packages=[bq])
 config = bq.Config(
     PROCESSOR_PACKAGES=["my_pkgs.processors"],
     DATABASE_URL=str(config.DATABASE_URL),
     BATCH_SIZE=10,
 )
-with container.config.override(config):
-    process_tasks(channels=("images",))
+app = bq.BeanQueue(config=config)
+```
+
+Then you can pass `--app` argument pointing to the app object to the process command like this:
+
+```bash
+python -m bq.cmds.process -a my_pkgs.bq.app images
 ```
 
-Many other behaviors of this framework can also be modified by overriding the container defined at [bq/container.py](bq/container.py).
+Or if you prefer to define your own process command, you can also call `process_tasks` of the `BeanQueue` object directly like this:
+
+```python
+app.process_tasks(channels=("images",))
+```
 
 ### Define your own tables
 
 BeanQueue is designed to be as customizable as much as possible.
 Of course, you can define your own SQLAlchemy model instead of using the ones we provided. 
 
 To make defining your own `Task` model or `Worker` model much easier, you can use our mixin classes:
@@ -227,15 +237,15 @@
 ```python
 import bq
 config = bq.Config(
     TASK_MODEL="my_pkgs.models.Task",
     WORKER_MODEL="my_pkgs.models.Worker",
     # ... other configs
 )
-# Override container...
+app = bq.BeanQueue(config)
 ```
 
 ## Why?
 
 There are countless worker queue projects. Why make yet another one?
 The primary issue with most worker queue tools is their reliance on a standalone broker server.
 Our worker queue tasks frequently interact with the database, and the atomic nature of database transactions is great for data integrity.
```

