# Comparing `tmp/runnable-0.9.0.tar.gz` & `tmp/runnable-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runnable-0.9.0.tar", max compression
+gzip compressed data, was "runnable-0.9.1.tar", max compression
```

## Comparing `runnable-0.9.0.tar` & `runnable-0.9.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    11357 2024-03-25 02:57:12.217039 runnable-0.9.0/LICENSE
--rw-r--r--   0        0        0    15677 2024-03-25 02:57:12.217039 runnable-0.9.0/README.md
--rw-r--r--   0        0        0     6316 2024-03-25 02:57:23.900922 runnable-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      619 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/__init__.py
--rw-r--r--   0        0        0     3985 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/catalog.py
--rw-r--r--   0        0        0     9589 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/cli.py
--rw-r--r--   0        0        0     1048 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/context.py
--rw-r--r--   0        0        0    25354 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/datastore.py
--rw-r--r--   0        0        0     4770 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/defaults.py
--rw-r--r--   0        0        0    15359 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/entrypoints.py
--rw-r--r--   0        0        0     2419 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/exceptions.py
--rw-r--r--   0        0        0    14484 2024-03-25 02:57:12.241039 runnable-0.9.0/runnable/executor.py
--rw-r--r--   0        0        0     3668 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/experiment_tracker.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/__init__.py
--rw-r--r--   0        0        0      761 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/catalog/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/catalog/file_system/__init__.py
--rw-r--r--   0        0        0     8958 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/catalog/file_system/implementation.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/catalog/k8s_pvc/__init__.py
--rw-r--r--   0        0        0      436 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/catalog/k8s_pvc/implementation.py
--rw-r--r--   0        0        0     1850 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/catalog/k8s_pvc/integration.py
--rw-r--r--   0        0        0    24181 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/argo/__init__.py
--rw-r--r--   0        0        0    43795 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/argo/implementation.py
--rw-r--r--   0        0        0     1276 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/argo/specification.yaml
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/k8s_job/__init__.py
--rw-r--r--   0        0        0    10259 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/k8s_job/implementation_FF.py
--rw-r--r--   0        0        0     2165 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/k8s_job/integration_FF.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/local/__init__.py
--rw-r--r--   0        0        0     2468 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/local/implementation.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/local_container/__init__.py
--rw-r--r--   0        0        0    13979 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/local_container/implementation.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/mocked/__init__.py
--rw-r--r--   0        0        0     5082 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/mocked/implementation.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/retry/__init__.py
--rw-r--r--   0        0        0     6625 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/executor/retry/implementation.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/experiment_tracker/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/experiment_tracker/mlflow/__init__.py
--rw-r--r--   0        0        0     3045 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/experiment_tracker/mlflow/implementation.py
--rw-r--r--   0        0        0    29883 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/nodes.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/chunked_file_system/__init__.py
--rw-r--r--   0        0        0     3170 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/chunked_file_system/implementation.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/chunked_k8s_pvc/__init__.py
--rw-r--r--   0        0        0      579 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/chunked_k8s_pvc/implementation.py
--rw-r--r--   0        0        0     1979 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/chunked_k8s_pvc/integration.py
--rw-r--r--   0        0        0     5155 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/db/implementation_FF.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/db/integration_FF.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/file_system/__init__.py
--rw-r--r--   0        0        0     4114 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/file_system/implementation.py
--rw-r--r--   0        0        0    19390 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/generic_chunked.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/k8s_pvc/__init__.py
--rw-r--r--   0        0        0      542 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/k8s_pvc/implementation.py
--rw-r--r--   0        0        0     1873 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/run_log_store/k8s_pvc/integration.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/secrets/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/secrets/dotenv/__init__.py
--rw-r--r--   0        0        0     3365 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/secrets/dotenv/implementation.py
--rw-r--r--   0        0        0        0 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/secrets/env_secrets/__init__.py
--rw-r--r--   0        0        0     1236 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/extensions/secrets/env_secrets/implementation.py
--rw-r--r--   0        0        0    15871 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/graph.py
--rw-r--r--   0        0        0     7176 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/integration.py
--rw-r--r--   0        0        0     8134 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/names.py
--rw-r--r--   0        0        0    16387 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/nodes.py
--rw-r--r--   0        0        0     5091 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/parameters.py
--rw-r--r--   0        0        0     2685 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/pickler.py
--rw-r--r--   0        0        0    22848 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/sdk.py
--rw-r--r--   0        0        0     2324 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/secrets.py
--rw-r--r--   0        0        0    17663 2024-03-25 02:57:12.245039 runnable-0.9.0/runnable/tasks.py
--rw-r--r--   0        0        0    19337 2024-03-25 02:57:12.249039 runnable-0.9.0/runnable/utils.py
--rw-r--r--   0        0        0    17062 1970-01-01 00:00:00.000000 runnable-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-25 08:23:15.304255 runnable-0.9.1/LICENSE
+-rw-r--r--   0        0        0    15677 2024-03-25 08:23:15.304255 runnable-0.9.1/README.md
+-rw-r--r--   0        0        0     6316 2024-03-25 08:23:30.908338 runnable-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      619 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/__init__.py
+-rw-r--r--   0        0        0     3985 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/catalog.py
+-rw-r--r--   0        0        0     9589 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/cli.py
+-rw-r--r--   0        0        0     1048 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/context.py
+-rw-r--r--   0        0        0    25354 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/datastore.py
+-rw-r--r--   0        0        0     4770 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/defaults.py
+-rw-r--r--   0        0        0    15359 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/entrypoints.py
+-rw-r--r--   0        0        0     2419 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/exceptions.py
+-rw-r--r--   0        0        0    14484 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/executor.py
+-rw-r--r--   0        0        0     3668 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/experiment_tracker.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/extensions/__init__.py
+-rw-r--r--   0        0        0      761 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/extensions/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/extensions/catalog/file_system/__init__.py
+-rw-r--r--   0        0        0     8958 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/extensions/catalog/file_system/implementation.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/extensions/catalog/k8s_pvc/__init__.py
+-rw-r--r--   0        0        0      436 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/extensions/catalog/k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     1850 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/extensions/catalog/k8s_pvc/integration.py
+-rw-r--r--   0        0        0    24187 2024-03-25 08:23:15.328255 runnable-0.9.1/runnable/extensions/executor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/argo/__init__.py
+-rw-r--r--   0        0        0    43795 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/argo/implementation.py
+-rw-r--r--   0        0        0     1276 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/argo/specification.yaml
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/k8s_job/__init__.py
+-rw-r--r--   0        0        0    10259 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/k8s_job/implementation_FF.py
+-rw-r--r--   0        0        0     2165 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/k8s_job/integration_FF.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/local/__init__.py
+-rw-r--r--   0        0        0     2468 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/local/implementation.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/local_container/__init__.py
+-rw-r--r--   0        0        0    13979 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/local_container/implementation.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/mocked/__init__.py
+-rw-r--r--   0        0        0     5082 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/mocked/implementation.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/retry/__init__.py
+-rw-r--r--   0        0        0     6625 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/executor/retry/implementation.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/experiment_tracker/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/experiment_tracker/mlflow/__init__.py
+-rw-r--r--   0        0        0     3045 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/experiment_tracker/mlflow/implementation.py
+-rw-r--r--   0        0        0    29883 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/nodes.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/chunked_file_system/__init__.py
+-rw-r--r--   0        0        0     3170 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/chunked_file_system/implementation.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/chunked_k8s_pvc/__init__.py
+-rw-r--r--   0        0        0      579 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/chunked_k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     1979 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/chunked_k8s_pvc/integration.py
+-rw-r--r--   0        0        0     5155 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/db/implementation_FF.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/db/integration_FF.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/file_system/__init__.py
+-rw-r--r--   0        0        0     4114 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/file_system/implementation.py
+-rw-r--r--   0        0        0    19390 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/generic_chunked.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/k8s_pvc/__init__.py
+-rw-r--r--   0        0        0      542 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     1873 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/run_log_store/k8s_pvc/integration.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/secrets/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/secrets/dotenv/__init__.py
+-rw-r--r--   0        0        0     3365 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/secrets/dotenv/implementation.py
+-rw-r--r--   0        0        0        0 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/secrets/env_secrets/__init__.py
+-rw-r--r--   0        0        0     1236 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/extensions/secrets/env_secrets/implementation.py
+-rw-r--r--   0        0        0    15871 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/graph.py
+-rw-r--r--   0        0        0     7176 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/integration.py
+-rw-r--r--   0        0        0     8134 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/names.py
+-rw-r--r--   0        0        0    16387 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/nodes.py
+-rw-r--r--   0        0        0     5091 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/parameters.py
+-rw-r--r--   0        0        0     2685 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/pickler.py
+-rw-r--r--   0        0        0    22931 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/sdk.py
+-rw-r--r--   0        0        0     2324 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/secrets.py
+-rw-r--r--   0        0        0    17663 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/tasks.py
+-rw-r--r--   0        0        0    19337 2024-03-25 08:23:15.332255 runnable-0.9.1/runnable/utils.py
+-rw-r--r--   0        0        0    17062 1970-01-01 00:00:00.000000 runnable-0.9.1/PKG-INFO
```

### Comparing `runnable-0.9.0/LICENSE` & `runnable-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/README.md` & `runnable-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/pyproject.toml` & `runnable-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runnable"
-version = "0.9.0"
+version = "0.9.1"
 description = "A Compute agnostic pipelining software"
 authors = ["Vijay Vammi <mesanthu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/vijayvammi/runnable"
 repository = "https://github.com/vijayvammi/runnable"
 documentation = "https://github.com/vijayvammi/runnable"
```

### Comparing `runnable-0.9.0/runnable/__init__.py` & `runnable-0.9.1/runnable/__init__.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/catalog.py` & `runnable-0.9.1/runnable/catalog.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/cli.py` & `runnable-0.9.1/runnable/cli.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/context.py` & `runnable-0.9.1/runnable/context.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/datastore.py` & `runnable-0.9.1/runnable/datastore.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/defaults.py` & `runnable-0.9.1/runnable/defaults.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/entrypoints.py` & `runnable-0.9.1/runnable/entrypoints.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/exceptions.py` & `runnable-0.9.1/runnable/exceptions.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/executor.py` & `runnable-0.9.1/runnable/executor.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/experiment_tracker.py` & `runnable-0.9.1/runnable/experiment_tracker.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/catalog/__init__.py` & `runnable-0.9.1/runnable/extensions/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/catalog/file_system/implementation.py` & `runnable-0.9.1/runnable/extensions/catalog/file_system/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/catalog/k8s_pvc/integration.py` & `runnable-0.9.1/runnable/extensions/catalog/k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/executor/__init__.py` & `runnable-0.9.1/runnable/extensions/executor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         The parameters defined in the environment variables take precedence over the parameters file.
 
         Returns:
             _type_: _description_
         """
         params: Dict[str, JsonParameter] = {}
         if self._context.parameters_file:
-            user_defined = utils.load_yaml(self._context.parameters_file)
+            user_defined = utils.load_yaml(self._context.parameters_file) or {}
 
             for key, value in user_defined.items():
                 params[key] = JsonParameter(value=value, kind="json")
 
         # Update these with some from the environment variables
         params.update(parameters.get_user_set_parameters())
         return params
```

### Comparing `runnable-0.9.0/runnable/extensions/executor/argo/implementation.py` & `runnable-0.9.1/runnable/extensions/executor/argo/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/executor/argo/specification.yaml` & `runnable-0.9.1/runnable/extensions/executor/argo/specification.yaml`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/executor/k8s_job/implementation_FF.py` & `runnable-0.9.1/runnable/extensions/executor/k8s_job/implementation_FF.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/executor/k8s_job/integration_FF.py` & `runnable-0.9.1/runnable/extensions/executor/k8s_job/integration_FF.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/executor/local/implementation.py` & `runnable-0.9.1/runnable/extensions/executor/local/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/executor/local_container/implementation.py` & `runnable-0.9.1/runnable/extensions/executor/local_container/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/executor/mocked/implementation.py` & `runnable-0.9.1/runnable/extensions/executor/mocked/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/executor/retry/implementation.py` & `runnable-0.9.1/runnable/extensions/executor/retry/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/experiment_tracker/mlflow/implementation.py` & `runnable-0.9.1/runnable/extensions/experiment_tracker/mlflow/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/nodes.py` & `runnable-0.9.1/runnable/extensions/nodes.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/run_log_store/chunked_file_system/implementation.py` & `runnable-0.9.1/runnable/extensions/run_log_store/chunked_file_system/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/run_log_store/chunked_k8s_pvc/implementation.py` & `runnable-0.9.1/runnable/extensions/run_log_store/chunked_k8s_pvc/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/run_log_store/chunked_k8s_pvc/integration.py` & `runnable-0.9.1/runnable/extensions/run_log_store/chunked_k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/run_log_store/db/implementation_FF.py` & `runnable-0.9.1/runnable/extensions/run_log_store/db/implementation_FF.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/run_log_store/file_system/implementation.py` & `runnable-0.9.1/runnable/extensions/run_log_store/file_system/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/run_log_store/generic_chunked.py` & `runnable-0.9.1/runnable/extensions/run_log_store/generic_chunked.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/run_log_store/k8s_pvc/implementation.py` & `runnable-0.9.1/runnable/extensions/run_log_store/k8s_pvc/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/run_log_store/k8s_pvc/integration.py` & `runnable-0.9.1/runnable/extensions/run_log_store/k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/secrets/dotenv/implementation.py` & `runnable-0.9.1/runnable/extensions/secrets/dotenv/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/extensions/secrets/env_secrets/implementation.py` & `runnable-0.9.1/runnable/extensions/secrets/env_secrets/implementation.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/graph.py` & `runnable-0.9.1/runnable/graph.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/integration.py` & `runnable-0.9.1/runnable/integration.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/names.py` & `runnable-0.9.1/runnable/names.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/nodes.py` & `runnable-0.9.1/runnable/nodes.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/parameters.py` & `runnable-0.9.1/runnable/parameters.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/pickler.py` & `runnable-0.9.1/runnable/pickler.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/sdk.py` & `runnable-0.9.1/runnable/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import logging
 import os
 from abc import ABC, abstractmethod
+from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field, PrivateAttr, computed_field, field_validator, model_validator
 from rich import print
 from typing_extensions import Self
 
 from runnable import defaults, entrypoints, graph, utils
@@ -532,15 +533,14 @@
 
     def execute(
         self,
         configuration_file: str = "",
         run_id: str = "",
         tag: str = "",
         parameters_file: str = "",
-        use_cached: str = "",
         log_level: str = defaults.LOG_LEVEL,
     ):
         """
         *Execute* the Pipeline.
 
         Execution of pipeline could either be:
 
@@ -589,19 +589,21 @@
 
         run_context.dag = graph.create_graph(dag_definition)
 
         print("Working with context:")
         print(run_context)
 
         if not run_context.executor._local:
-            # We are working with non local executor
+            # We are not working with non local executor
             import inspect
 
             caller_stack = inspect.stack()[1]
-            module_to_call = f"{caller_stack.filename.replace('/', '.').replace('.py', '')}.{caller_stack.function}"
+            relative_to_root = str(Path(caller_stack.filename).relative_to(Path.cwd()))
+
+            module_to_call = f"{relative_to_root.replace('/', '.').replace('.py', '')}.{caller_stack.function}"
 
             run_context.pipeline_file = f"{module_to_call}.py"
 
         # Prepare for graph execution
         run_context.executor.prepare_for_graph_execution()
 
         logger.info("Executing the graph")
```

### Comparing `runnable-0.9.0/runnable/secrets.py` & `runnable-0.9.1/runnable/secrets.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/tasks.py` & `runnable-0.9.1/runnable/tasks.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/runnable/utils.py` & `runnable-0.9.1/runnable/utils.py`

 * *Files identical despite different names*

### Comparing `runnable-0.9.0/PKG-INFO` & `runnable-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runnable
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Compute agnostic pipelining software
 Home-page: https://github.com/vijayvammi/runnable
 License: Apache-2.0
 Author: Vijay Vammi
 Author-email: mesanthu@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
```

