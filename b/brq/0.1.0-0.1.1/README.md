# Comparing `tmp/brq-0.1.0.tar.gz` & `tmp/brq-0.1.1.tar.gz`

## Comparing `brq-0.1.0.tar` & `brq-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 brq-0.1.0/.coveragerc
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 brq-0.1.0/.editorconfig
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 brq-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 brq-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 brq-0.1.0/FUNDING.yml
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 brq-0.1.0/RELEASE.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 brq-0.1.0/pytest.ini
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 brq-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 brq-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 brq-0.1.0/.github/ISSUE_TEMPLATE/doc_request.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 brq-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 brq-0.1.0/.github/ISSUE_TEMPLATE/good_first_issue.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 brq-0.1.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 brq-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 brq-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 brq-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    63735 2020-02-02 00:00:00.000000 brq-0.1.0/assets/Architecture.png
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 brq-0.1.0/brq/__init__.py
--rw-r--r--   0        0        0    10601 2020-02-02 00:00:00.000000 brq-0.1.0/brq/consumer.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 brq-0.1.0/brq/daemon.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 brq-0.1.0/brq/defer_operator.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 brq-0.1.0/brq/log.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 brq-0.1.0/brq/models.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 brq-0.1.0/brq/producer.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 brq-0.1.0/brq/rds.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 brq-0.1.0/brq/tools.py
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 brq-0.1.0/dev/start-redis.sh
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 brq-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 brq-0.1.0/docs/README.md
--rwxr-xr-x   0        0        0     4701 2020-02-02 00:00:00.000000 brq-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 brq-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 brq-0.1.0/docs/source/usage.rst
--rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 brq-0.1.0/drawio/Architecture.drawio
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 brq-0.1.0/examples/defer_job/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 brq-0.1.0/examples/defer_job/consumer.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 brq-0.1.0/examples/defer_job/producer.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 brq-0.1.0/examples/dockerfile/Dockerfile.consumer
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 brq-0.1.0/examples/echo/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 brq-0.1.0/examples/echo/consumer.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 brq-0.1.0/examples/echo/producer.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 brq-0.1.0/examples/process_dead_message/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 brq-0.1.0/examples/process_dead_message/consumer.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 brq-0.1.0/examples/process_dead_message/dead_message_consumer.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 brq-0.1.0/examples/process_dead_message/producer.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 brq-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 brq-0.1.0/tests/test_brq.py
--rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 brq-0.1.0/.gitignore
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 brq-0.1.0/LICENSE
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 brq-0.1.0/README.md
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 brq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 brq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 brq-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 brq-0.1.1/.editorconfig
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 brq-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 brq-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 brq-0.1.1/FUNDING.yml
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 brq-0.1.1/RELEASE.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 brq-0.1.1/pytest.ini
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 brq-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 brq-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 brq-0.1.1/.github/ISSUE_TEMPLATE/doc_request.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 brq-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 brq-0.1.1/.github/ISSUE_TEMPLATE/good_first_issue.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 brq-0.1.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 brq-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 brq-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 brq-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    63735 2020-02-02 00:00:00.000000 brq-0.1.1/assets/Architecture.png
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 brq-0.1.1/brq/__init__.py
+-rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 brq-0.1.1/brq/consumer.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 brq-0.1.1/brq/daemon.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 brq-0.1.1/brq/defer_operator.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 brq-0.1.1/brq/log.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 brq-0.1.1/brq/models.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 brq-0.1.1/brq/producer.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 brq-0.1.1/brq/rds.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 brq-0.1.1/brq/tools.py
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 brq-0.1.1/dev/start-redis.sh
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 brq-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 brq-0.1.1/docs/README.md
+-rwxr-xr-x   0        0        0     4701 2020-02-02 00:00:00.000000 brq-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 brq-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 brq-0.1.1/docs/source/usage.rst
+-rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 brq-0.1.1/drawio/Architecture.drawio
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 brq-0.1.1/examples/defer_job/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 brq-0.1.1/examples/defer_job/consumer.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 brq-0.1.1/examples/defer_job/producer.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 brq-0.1.1/examples/dockerfile/Dockerfile.consumer
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 brq-0.1.1/examples/echo/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 brq-0.1.1/examples/echo/consumer.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 brq-0.1.1/examples/echo/producer.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 brq-0.1.1/examples/process_dead_message/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 brq-0.1.1/examples/process_dead_message/consumer.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 brq-0.1.1/examples/process_dead_message/dead_message_consumer.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 brq-0.1.1/examples/process_dead_message/producer.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 brq-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 brq-0.1.1/tests/test_brq.py
+-rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 brq-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 brq-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 brq-0.1.1/README.md
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 brq-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 brq-0.1.1/PKG-INFO
```

### Comparing `brq-0.1.0/.pre-commit-config.yaml` & `brq-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/RELEASE.md` & `brq-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `brq-0.1.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `brq-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/.github/ISSUE_TEMPLATE/doc_request.md` & `brq-0.1.1/.github/ISSUE_TEMPLATE/doc_request.md`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `brq-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/.github/ISSUE_TEMPLATE/good_first_issue.md` & `brq-0.1.1/.github/ISSUE_TEMPLATE/good_first_issue.md`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/.github/workflows/python-package.yml` & `brq-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/.github/workflows/python-publish.yml` & `brq-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/assets/Architecture.png` & `brq-0.1.1/assets/Architecture.png`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/brq/consumer.py` & `brq-0.1.1/brq/consumer.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,54 +55,80 @@
     async def cleanup(self):
         """
         Cleanup, implement in subclass
         """
 
 
 class Consumer(DeferOperator, RunnableMixin):
+    """
+    A consumer for redis stream.
+
+    When many replicas of one kind of consumer are created, they should be in **the same** group.
+    When many kind of consumers are created, they should be in **different** groups.
+
+    See [example](https://github.com/Wh1isper/brq/tree/main/examples) for running example.
+
+    Args:
+        redis(redis.Redis | redis.RedisCluster): Redis client.
+        awaitable_function(Callable[[Any], Awaitable[Any]]): The function to be called.
+        register_function_name(str): The function name to be registered, if None, will use the function name of `awaitable_function`.
+        group_name(str, default="default-workers"): The group name. All replicas should be in the same group.
+        consumer_identifier(str, default=os.getenv(CONSUMER_IDENTIFIER_ENV, uuid.uuid4().hex)): The consumer identifier. For restarting in some special case.
+        count_per_fetch(int, default=1): The count of message per fetch.
+        block_time(int, default=1): The block time of reading stream.
+        expire_time(int, default=60*60): The expire time of a message. Expired messages will be moved to dead queue.
+        process_timeout(int, default=60): The timeout of a job. If a job is not finished in this time, it will be reprocessed.
+        retry_lock_time(int, default=300): The lock time for retrying. Only one consumer can retry jobs at a time.
+        retry_cooldown(int, default=60): The cooldown time between retrying.
+        redis_prefix(str, default="brq"): The prefix of redis key.
+        redis_seperator(str, default=":"): The seperator of redis key.
+        enable_enque_deferred_job(bool, default=True): Whether to enable enque deferred job. If not, this consumer won't enque deferred jobs.
+        max_message_len(int, default=1000): The maximum length of a message. Follow redis stream `maxlen`.
+        delete_messgae_after_process(bool, default=False): Whether to delete message after process. If many consumer groups are used, this should be set to False.
+        run_parallel(bool, default=False): Whether to run in parallel.
+    """
+
     def __init__(
         self,
         redis: redis.Redis | redis.RedisCluster,
         awaitable_function: Callable[[Any], Awaitable[Any]],
         register_function_name: str = None,
         group_name="default-workers",
         consumer_identifier: str = os.getenv(CONSUMER_IDENTIFIER_ENV, uuid.uuid4().hex),
         count_per_fetch: int = 1,
         block_time: int = 1,
-        pool_time: int = 5,
         expire_time: int = 60 * 60,
         process_timeout: int = 60,
         retry_lock_time: int = 300,
         retry_cooldown: int = 60,
         redis_prefix: str = "brq",
         redis_seperator: str = ":",
         enable_enque_deferred_job: bool = True,
-        max_message_size: int = 1000,
+        max_message_len: int = 1000,
         delete_messgae_after_process: bool = False,
         run_parallel: bool = False,
     ):
         super().__init__(redis, redis_prefix, redis_seperator)
         self._stop_event = asyncio.Event()
         self._task: None | asyncio.Task = None
 
         self.awaitable_function = awaitable_function
         self.register_function_name = register_function_name or awaitable_function.__name__
         self.group_name = group_name
         self.consumer_identifier = consumer_identifier
         self.count_per_fetch = count_per_fetch
 
         self.block_time = block_time
-        self.pool_time = pool_time
         self.expire_time = expire_time
         self.process_timeout = process_timeout
         self.retry_lock_time = retry_lock_time
         self.retry_cooldown = retry_cooldown
 
         self.enable_enque_deferred_job = enable_enque_deferred_job
-        self.max_message_size = max_message_size
+        self.max_message_len = max_message_len
         self.delete_messgae_after_process = delete_messgae_after_process
         self.run_parallel = run_parallel
 
     @property
     def retry_lock_key(self) -> str:
         return self.get_redis_key(self.stream_name, self.group_name, "lock")
 
@@ -294,15 +320,15 @@
         except redis.ResponseError as e:
             if e.args[0] != "BUSYGROUP Consumer Group name already exists":
                 raise
             logger.info(f"Consumer group already exists: {self.group_name}, skipping...")
 
     async def run(self):
         if self.enable_enque_deferred_job:
-            await self.enque_deferred_job(self.register_function_name, self.max_message_size)
+            await self.enque_deferred_job(self.register_function_name, self.max_message_len)
         await self._consume()
 
     async def cleanup(self):
         await self.redis.xgroup_delconsumer(
             self.stream_name, self.group_name, self.consumer_identifier
         )
         if await self._release_retry_lock():
```

### Comparing `brq-0.1.0/brq/daemon.py` & `brq-0.1.1/brq/daemon.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/brq/defer_operator.py` & `brq-0.1.1/brq/defer_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,12 +37,12 @@
         stream_name = self.get_stream_name(function_name)
 
         elements = await self.redis.eval(
             lua_script,
             2,
             defer_key,
             stream_name,
-            await self.get_current_timestamp(self.redis),
+            await self.get_current_timestamp_ms(self.redis),
             maxlen,
         )
         if elements:
             logger.info(f"Enqueued deferred jobs: {elements}")
```

### Comparing `brq-0.1.0/brq/models.py` & `brq-0.1.1/brq/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Job(BaseModel):
     args: list
     kwargs: dict
     create_at: int
     """
-    Timestamp in seconds
+    Timestamp in milliseconds
     """
 
     @classmethod
     def from_redis(cls, serialized: str) -> Job:
         return cls.model_validate_json(serialized)
 
     @classmethod
```

### Comparing `brq-0.1.0/brq/rds.py` & `brq-0.1.1/brq/rds.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/brq/tools.py` & `brq-0.1.1/brq/tools.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/docs/Makefile` & `brq-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/docs/source/conf.py` & `brq-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/drawio/Architecture.drawio` & `brq-0.1.1/drawio/Architecture.drawio`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/examples/defer_job/consumer.py` & `brq-0.1.1/examples/defer_job/consumer.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/examples/defer_job/producer.py` & `brq-0.1.1/examples/echo/producer.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,14 @@
         host=os.getenv("REDIS_HOST", "localhost"),
         port=int(os.getenv("REDIS_PORT", 6379)),
         db=int(os.getenv("REDIS_DB", 0)),
         cluster=bool(os.getenv("REDIS_CLUSTER", False)),
         tls=bool(os.getenv("REDIS_TLS", False)),
     )
     async with get_redis_client(redis_url) as async_redis_client:
-        await Producer(async_redis_client).run_job("echo", ["hello"], defer_seconds=10)
+        await Producer(async_redis_client).run_job("echo", ["hello"])
 
 
 if __name__ == "__main__":
     import asyncio
 
     asyncio.run(main())
```

### Comparing `brq-0.1.0/examples/echo/consumer.py` & `brq-0.1.1/examples/echo/consumer.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/examples/echo/producer.py` & `brq-0.1.1/examples/process_dead_message/producer.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/examples/process_dead_message/consumer.py` & `brq-0.1.1/examples/process_dead_message/consumer.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/examples/process_dead_message/dead_message_consumer.py` & `brq-0.1.1/examples/process_dead_message/dead_message_consumer.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/examples/process_dead_message/producer.py` & `brq-0.1.1/examples/defer_job/producer.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         host=os.getenv("REDIS_HOST", "localhost"),
         port=int(os.getenv("REDIS_PORT", 6379)),
         db=int(os.getenv("REDIS_DB", 0)),
         cluster=bool(os.getenv("REDIS_CLUSTER", False)),
         tls=bool(os.getenv("REDIS_TLS", False)),
     )
     async with get_redis_client(redis_url) as async_redis_client:
-        await Producer(async_redis_client).run_job("echo", ["hello"])
+        await Producer(async_redis_client).run_job("echo", ["hello"], defer_seconds=10)
+        print(await Producer(async_redis_client).get_deferred_jobs("echo"))
 
 
 if __name__ == "__main__":
     import asyncio
 
     asyncio.run(main())
```

### Comparing `brq-0.1.0/tests/conftest.py` & `brq-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/tests/test_brq.py` & `brq-0.1.1/tests/test_brq.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 
 
 async def test_deferred_job(async_redis_client, capfd):
     producer = Producer(async_redis_client)
     consumer = Consumer(async_redis_client, mock_consume)
 
     await producer.run_job("mock_consume", ["hello"], defer_seconds=1)
+    assert await producer.get_deferred_jobs("mock_consume")
     await consumer.initialize()
     await consumer.run()
     out, err = capfd.readouterr()
     assert "hello" not in out
     await asyncio.sleep(1.1)
     await consumer.run()
     out, err = capfd.readouterr()
```

### Comparing `brq-0.1.0/.gitignore` & `brq-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/LICENSE` & `brq-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/README.md` & `brq-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 # brq
 
 ![Architecture.png](./assets/Architecture.png)
 
 ## Prerequisites
 
-Redis >= 6.2, tested with latest docker image
+Redis >= 7, tested with latest docker image
 
 ## Install
 
 `pip install brq`
 
 ## Feature
 
-> See [examples](%22./examples%22) for runnable examples.
+> See [examples](%22./examples%22) for running examples.
 
 - Defer job
 - Automatic retry job
 - Dead queue
 - Multiple consumers
 
-## Echo jobs overview
+## Echo job overview
 
 ### Producer
 
 ```python
 import os
 
 from brq.producer import Producer
```

### Comparing `brq-0.1.0/pyproject.toml` & `brq-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brq-0.1.0/PKG-INFO` & `brq-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: brq
-Version: 0.1.0
+Version: 0.1.1
 Summary: brq
 Project-URL: Source, https://github.com/wh1isper/brq
 Author-email: wh1isper <9573586@qq.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: brq
 Classifier: Programming Language :: Python :: 3
@@ -40,30 +40,30 @@
 
 # brq
 
 ![Architecture.png](./assets/Architecture.png)
 
 ## Prerequisites
 
-Redis >= 6.2, tested with latest docker image
+Redis >= 7, tested with latest docker image
 
 ## Install
 
 `pip install brq`
 
 ## Feature
 
-> See [examples](%22./examples%22) for runnable examples.
+> See [examples](%22./examples%22) for running examples.
 
 - Defer job
 - Automatic retry job
 - Dead queue
 - Multiple consumers
 
-## Echo jobs overview
+## Echo job overview
 
 ### Producer
 
 ```python
 import os
 
 from brq.producer import Producer
```

