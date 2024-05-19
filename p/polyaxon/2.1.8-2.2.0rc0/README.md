# Comparing `tmp/polyaxon-2.1.8.tar.gz` & `tmp/polyaxon-2.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyaxon-2.1.8.tar", last modified: Sat Apr 20 12:26:12 2024, max compression
+gzip compressed data, was "polyaxon-2.2.0rc0.tar", last modified: Sun May 19 19:30:41 2024, max compression
```

## Comparing `polyaxon-2.1.8.tar` & `polyaxon-2.2.0rc0.tar`

### file list

```diff
@@ -1,712 +1,732 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.401638 polyaxon-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-20 12:26:02.000000 polyaxon-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-04-20 12:26:12.401638 polyaxon-2.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.301638 polyaxon-2.1.8/polyaxon/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.301638 polyaxon-2.1.8/polyaxon/_auxiliaries/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_auxiliaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_auxiliaries/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_auxiliaries/default_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_auxiliaries/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_auxiliaries/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_auxiliaries/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_auxiliaries/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.305638 polyaxon-2.1.8/polyaxon/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18350 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8278 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/init.py
--rw-r--r--   0 runner    (1001) docker     (127)    17942 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    74093 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/port_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/project_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    17194 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.309638 polyaxon-2.1.8/polyaxon/_cli/services/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/clean_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/services/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.309638 polyaxon-2.1.8/polyaxon/_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.309638 polyaxon-2.1.8/polyaxon/_client/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/decorators/client_call_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/decorators/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/decorators/is_managed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/impersonate.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/init.py
--rw-r--r--   0 runner    (1001) docker     (127)    65375 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/project.py
--rw-r--r--   0 runner    (1001) docker     (127)   118286 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.309638 polyaxon-2.1.8/polyaxon/_client/transport/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/transport/http_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/transport/periodic_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/transport/retry_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/transport/socket_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/transport/threaded_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/transport/ws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.313638 polyaxon-2.1.8/polyaxon/_client/workers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/workers/base_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/workers/periodic_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_client/workers/queue_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.313638 polyaxon-2.1.8/polyaxon/_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.313638 polyaxon-2.1.8/polyaxon/_compiler/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/dask_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.313638 polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/mx_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/pytroch_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/tf_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/xgb_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/ray_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/contexts/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.313638 polyaxon-2.1.8/polyaxon/_compiler/lineage/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/lineage/artifacts_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/lineage/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/lineage/io_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.313638 polyaxon-2.1.8/polyaxon/_compiler/resolver/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/resolver/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_compiler/resolver/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.317638 polyaxon-2.1.8/polyaxon/_config/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_config/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_config/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_config/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_config/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.317638 polyaxon-2.1.8/polyaxon/_connections/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_connections/kinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_connections/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.317638 polyaxon-2.1.8/polyaxon/_constants/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_constants/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_constants/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.317638 polyaxon-2.1.8/polyaxon/_containers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_containers/names.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_containers/pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_containers/statuses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.317638 polyaxon-2.1.8/polyaxon/_contexts/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_contexts/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_contexts/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_contexts/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_contexts/refs.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_contexts/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.317638 polyaxon-2.1.8/polyaxon/_deploy/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.321638 polyaxon-2.1.8/polyaxon/_deploy/operators/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/operators/cmd_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/operators/compose.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/operators/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/operators/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/operators/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/operators/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/operators/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.321638 polyaxon-2.1.8/polyaxon/_deploy/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/deployment_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/ingress.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/root_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/security_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/service_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_deploy/schemas/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.325638 polyaxon-2.1.8/polyaxon/_docker/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.325638 polyaxon-2.1.8/polyaxon/_docker/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/builder/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/builder/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.325638 polyaxon-2.1.8/polyaxon/_docker/converter/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.325638 polyaxon-2.1.8/polyaxon/_docker/converter/base/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/base/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/base/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/base/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20203 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/base/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/base/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/base/mounts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.325638 polyaxon-2.1.8/polyaxon/_docker/converter/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/converters/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/converters/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/converter/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/docker_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_docker/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.325638 polyaxon-2.1.8/polyaxon/_env_vars/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_env_vars/getters/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/getters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/getters/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/getters/owner_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/getters/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/getters/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/getters/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/getters/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/getters/versioned_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_env_vars/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/builds/
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/builds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/cache/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/component/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/component/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/component/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/component/component_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/containers/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/containers/container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/dags/
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/dags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/early_stopping/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/environment/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/events/
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/events/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/hooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/init/
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.329638 polyaxon-2.1.8/polyaxon/_flow/io/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29405 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/io/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.333638 polyaxon-2.1.8/polyaxon/_flow/joins/
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/joins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.333638 polyaxon-2.1.8/polyaxon/_flow/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/random_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/matrix/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.333638 polyaxon-2.1.8/polyaxon/_flow/mounts/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/mounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/mounts/artifacts_mounts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.333638 polyaxon-2.1.8/polyaxon/_flow/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.333638 polyaxon-2.1.8/polyaxon/_flow/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/operations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/operations/compiled_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23717 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.333638 polyaxon-2.1.8/polyaxon/_flow/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/optimization/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.337638 polyaxon-2.1.8/polyaxon/_flow/params/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/params/ops_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    18455 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/params/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.337638 polyaxon-2.1.8/polyaxon/_flow/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.337638 polyaxon-2.1.8/polyaxon/_flow/references/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/references/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/references/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/references/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/references/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/references/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.337638 polyaxon-2.1.8/polyaxon/_flow/run/
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)    22891 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.337638 polyaxon-2.1.8/polyaxon/_flow/run/dask/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/dask/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/dask/replica.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.341638 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/clean_pod_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/mx_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/pytorch_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/replica.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/tf_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/xgboost_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.341638 polyaxon-2.1.8/polyaxon/_flow/run/ray/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/ray/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/ray/replica.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/run/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.341638 polyaxon-2.1.8/polyaxon/_flow/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/schedules/cron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/schedules/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/schedules/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/schedules/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.341638 polyaxon-2.1.8/polyaxon/_flow/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.341638 polyaxon-2.1.8/polyaxon/_flow/termination/
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/termination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_flow/trigger_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.345638 polyaxon-2.1.8/polyaxon/_fs/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_fs/async_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_fs/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_fs/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_fs/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_fs/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_fs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_fs/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.345638 polyaxon-2.1.8/polyaxon/_init/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_init/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_init/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_init/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_init/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_init/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_init/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.345638 polyaxon-2.1.8/polyaxon/_k8s/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.345638 polyaxon-2.1.8/polyaxon/_k8s/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/agent/async_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.345638 polyaxon-2.1.8/polyaxon/_k8s/converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.349638 polyaxon-2.1.8/polyaxon/_k8s/converter/base/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/base/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/base/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/base/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20404 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/base/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/base/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/base/mounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/base/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.349638 polyaxon-2.1.8/polyaxon/_k8s/converter/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/common/accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/common/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/common/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.349638 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/dask_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.349638 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/mx_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/pytroch_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/tf_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/xgboost_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/ray_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/converters/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.353638 polyaxon-2.1.8/polyaxon/_k8s/converter/pod/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/pod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/pod/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/converter/pod/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.353638 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/crd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/dask_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.357638 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/mx_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/pytorch_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/tf_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/xgb_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/ray_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/custom_resources/setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.357638 polyaxon-2.1.8/polyaxon/_k8s/executor/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/executor/async_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/executor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/k8s_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.357638 polyaxon-2.1.8/polyaxon/_k8s/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/logging/async_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/logging/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.357638 polyaxon-2.1.8/polyaxon/_k8s/manager/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/manager/async_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    30143 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/pods.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_k8s/replica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.361638 polyaxon-2.1.8/polyaxon/_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/compose.py
--rw-r--r--   0 runner    (1001) docker     (127)    14441 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/home.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/ignore.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_managers/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.361638 polyaxon-2.1.8/polyaxon/_notifiers/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_notifiers/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.361638 polyaxon-2.1.8/polyaxon/_operations/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_operations/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_operations/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_operations/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.361638 polyaxon-2.1.8/polyaxon/_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_plugins/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.361638 polyaxon-2.1.8/polyaxon/_polyaxonfile/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.361638 polyaxon-2.1.8/polyaxon/_polyaxonfile/manager/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/manager/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/manager/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.361638 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/compiled_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/kinds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.365638 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/libs/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/libs/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/libs/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.365638 polyaxon-2.1.8/polyaxon/_pql/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_pql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17840 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_pql/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_pql/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_pql/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.365638 polyaxon-2.1.8/polyaxon/_runner/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.365638 polyaxon-2.1.8/polyaxon/_runner/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/agent/async_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/agent/base_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/agent/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/agent/sync_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.365638 polyaxon-2.1.8/polyaxon/_runner/converter/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.365638 polyaxon-2.1.8/polyaxon/_runner/converter/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/common/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/common/volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)    38005 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.369638 polyaxon-2.1.8/polyaxon/_runner/converter/init/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/init/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/init/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/init/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/init/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/init/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/init/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/converter/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_runner/kinds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.369638 polyaxon-2.1.8/polyaxon/_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/home.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/installation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.373638 polyaxon-2.1.8/polyaxon/_schemas/types/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/clipped.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/types/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_schemas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.373638 polyaxon-2.1.8/polyaxon/_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.377638 polyaxon-2.1.8/polyaxon/_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   162788 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/agents_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/artifacts_stores_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35802 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/auth_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54365 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/connections_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53802 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/dashboards_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   291838 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/organizations_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54930 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/presets_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    65408 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/project_dashboards_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    65058 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/project_searches_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   244751 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/projects_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    77083 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/queues_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   520199 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/runs_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53284 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/searches_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   101005 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/service_accounts_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    59912 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/tags_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    99021 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/teams_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    72638 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/users_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18440 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/api/versions_v1_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.381638 polyaxon-2.1.8/polyaxon/_sdk/async_client/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/async_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/async_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/async_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/base_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15103 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.393638 polyaxon-2.1.8/polyaxon/_sdk/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_agent_reconcile_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_agent_state_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_agent_state_response_agent_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_agent_status_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_analytics_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_artifact_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_dashboard_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_entities_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_entities_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_entity_notification_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_entity_stage_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_entity_status_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_events_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_activities_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_bookmarks_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_dashboards_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_organization_members_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_organizations_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_presets_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_project_versions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_queues_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_run_artifacts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_run_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_run_edges_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_searches_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_service_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_team_members_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_teams_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_list_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_operation_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_organization_member.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_password_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_preset.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_project_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run_edge_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run_edges_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run_reference_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_search_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_section_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_settings_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_team.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_team_member.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_team_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_trial_start.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_user_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_user_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_user_singup.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.393638 polyaxon-2.1.8/polyaxon/_sdk/sync_client/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/sync_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28509 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/sync_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sdk/sync_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.393638 polyaxon-2.1.8/polyaxon/_services/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_services/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_services/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_services/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.393638 polyaxon-2.1.8/polyaxon/_sidecar/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.393638 polyaxon-2.1.8/polyaxon/_sidecar/container/
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/container/intervals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.393638 polyaxon-2.1.8/polyaxon/_sidecar/container/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/container/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/container/monitors/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/container/monitors/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/container/monitors/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/ignore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_sidecar/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.397638 polyaxon-2.1.8/polyaxon/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/cli_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.397638 polyaxon-2.1.8/polyaxon/_utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/backfill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/bo.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    12332 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    22124 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fixtures/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/fqn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/host_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_utils/urls_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.397638 polyaxon-2.1.8/polyaxon/_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/_vendor/shell_pty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5531 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/polyaxonfile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.397638 polyaxon-2.1.8/polyaxon/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.401638 polyaxon-2.1.8/polyaxon/tracking/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/fastai.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/fastai_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/ignite.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/pytorch_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/scikit.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/contrib/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tracking/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.401638 polyaxon-2.1.8/polyaxon/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tuners/bayesian_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tuners/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tuners/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tuners/hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tuners/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/tuners/random_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.301638 polyaxon-2.1.8/polyaxon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-04-20 12:26:12.000000 polyaxon-2.1.8/polyaxon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-04-20 12:26:12.000000 polyaxon-2.1.8/polyaxon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:12.000000 polyaxon-2.1.8/polyaxon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-20 12:26:12.000000 polyaxon-2.1.8/polyaxon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-20 12:26:12.000000 polyaxon-2.1.8/polyaxon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 12:26:12.000000 polyaxon-2.1.8/polyaxon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:12.401638 polyaxon-2.1.8/polyaxon_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-20 12:26:02.000000 polyaxon-2.1.8/polyaxon_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-20 12:26:12.401638 polyaxon-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-20 12:26:02.000000 polyaxon-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.849057 polyaxon-2.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-19 19:30:41.849057 polyaxon-2.2.0rc0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.753058 polyaxon-2.2.0rc0/polyaxon/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.757058 polyaxon-2.2.0rc0/polyaxon/_auxiliaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_auxiliaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_auxiliaries/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_auxiliaries/default_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_auxiliaries/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_auxiliaries/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_auxiliaries/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_auxiliaries/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.757058 polyaxon-2.2.0rc0/polyaxon/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18350 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8278 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17942 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74918 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/port_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17194 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.761057 polyaxon-2.2.0rc0/polyaxon/_cli/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/clean_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/services/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.761057 polyaxon-2.2.0rc0/polyaxon/_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.761057 polyaxon-2.2.0rc0/polyaxon/_client/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/decorators/client_call_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/decorators/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/decorators/is_managed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/impersonate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65375 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118286 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.761057 polyaxon-2.2.0rc0/polyaxon/_client/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/transport/http_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/transport/periodic_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/transport/retry_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/transport/socket_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/transport/threaded_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/transport/ws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.765057 polyaxon-2.2.0rc0/polyaxon/_client/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/workers/base_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/workers/periodic_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_client/workers/queue_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.765057 polyaxon-2.2.0rc0/polyaxon/_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.765057 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/dask_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.765057 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/pytroch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/xgb_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/ray_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.765057 polyaxon-2.2.0rc0/polyaxon/_compiler/lineage/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/lineage/artifacts_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/lineage/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/lineage/io_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.765057 polyaxon-2.2.0rc0/polyaxon/_compiler/resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/resolver/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_compiler/resolver/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.769057 polyaxon-2.2.0rc0/polyaxon/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_config/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_config/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_config/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_config/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.769057 polyaxon-2.2.0rc0/polyaxon/_connections/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_connections/kinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_connections/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.769057 polyaxon-2.2.0rc0/polyaxon/_constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_constants/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_constants/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.769057 polyaxon-2.2.0rc0/polyaxon/_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_containers/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_containers/pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_containers/statuses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.769057 polyaxon-2.2.0rc0/polyaxon/_contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_contexts/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_contexts/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_contexts/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_contexts/refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_contexts/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.769057 polyaxon-2.2.0rc0/polyaxon/_deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.773058 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/cmd_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/operators/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.773058 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/deployment_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/ingress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/root_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/security_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/service_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.773058 polyaxon-2.2.0rc0/polyaxon/_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.777058 polyaxon-2.2.0rc0/polyaxon/_docker/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/builder/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/builder/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.777058 polyaxon-2.2.0rc0/polyaxon/_docker/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.777058 polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20203 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/mounts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.777058 polyaxon-2.2.0rc0/polyaxon/_docker/converter/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/converters/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/converters/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/converter/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/docker_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_docker/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.777058 polyaxon-2.2.0rc0/polyaxon/_env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.777058 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/owner_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/versioned_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_env_vars/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.777058 polyaxon-2.2.0rc0/polyaxon/_flow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/builds/
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/builds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/cache/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/component/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/component/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/component/component_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/containers/container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/dags/
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/dags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/early_stopping/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/events/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/init/
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29405 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/io/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.781057 polyaxon-2.2.0rc0/polyaxon/_flow/joins/
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/joins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.785057 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/matrix/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.785057 polyaxon-2.2.0rc0/polyaxon/_flow/mounts/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/mounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/mounts/artifacts_mounts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.785057 polyaxon-2.2.0rc0/polyaxon/_flow/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.785057 polyaxon-2.2.0rc0/polyaxon/_flow/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/operations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/operations/compiled_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23717 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.785057 polyaxon-2.2.0rc0/polyaxon/_flow/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/optimization/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.785057 polyaxon-2.2.0rc0/polyaxon/_flow/params/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/params/ops_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18455 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/params/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.785057 polyaxon-2.2.0rc0/polyaxon/_flow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.785057 polyaxon-2.2.0rc0/polyaxon/_flow/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/references/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/references/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/references/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/references/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/references/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.789057 polyaxon-2.2.0rc0/polyaxon/_flow/run/
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22891 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.789057 polyaxon-2.2.0rc0/polyaxon/_flow/run/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/dask/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/dask/replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.789057 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/clean_pod_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/pytorch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/xgboost_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.789057 polyaxon-2.2.0rc0/polyaxon/_flow/run/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/ray/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/ray/replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/run/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.793057 polyaxon-2.2.0rc0/polyaxon/_flow/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/schedules/cron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/schedules/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/schedules/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/schedules/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.793057 polyaxon-2.2.0rc0/polyaxon/_flow/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.793057 polyaxon-2.2.0rc0/polyaxon/_flow/termination/
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/termination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_flow/trigger_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.793057 polyaxon-2.2.0rc0/polyaxon/_fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_fs/async_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_fs/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_fs/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_fs/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_fs/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_fs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_fs/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.793057 polyaxon-2.2.0rc0/polyaxon/_init/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_init/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_init/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_init/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_init/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_init/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_init/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.797057 polyaxon-2.2.0rc0/polyaxon/_k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.797057 polyaxon-2.2.0rc0/polyaxon/_k8s/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/agent/async_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.797057 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.797057 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20404 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/mounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.797057 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/common/accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/common/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/common/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.797057 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/dask_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.801057 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/pytroch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/xgboost_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/ray_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.801057 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/pod/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/pod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/pod/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/converter/pod/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.801057 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/crd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/dask_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.801057 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/pytorch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/xgb_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/ray_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.805057 polyaxon-2.2.0rc0/polyaxon/_k8s/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/executor/async_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/executor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/k8s_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.805057 polyaxon-2.2.0rc0/polyaxon/_k8s/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/logging/async_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/logging/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.805057 polyaxon-2.2.0rc0/polyaxon/_k8s/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/manager/async_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30143 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_k8s/replica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.805057 polyaxon-2.2.0rc0/polyaxon/_local_process/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.805057 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.805057 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/base/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/base/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/base/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/base/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/base/mounts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.805057 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/converters/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/converters/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/converter/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_local_process/process_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.809057 polyaxon-2.2.0rc0/polyaxon/_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14441 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_managers/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.809057 polyaxon-2.2.0rc0/polyaxon/_notifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_notifiers/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.809057 polyaxon-2.2.0rc0/polyaxon/_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_operations/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_operations/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_operations/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.809057 polyaxon-2.2.0rc0/polyaxon/_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_plugins/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.809057 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.809057 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/manager/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/manager/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.813057 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/compiled_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/kinds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.813057 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/libs/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/libs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/libs/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.813057 polyaxon-2.2.0rc0/polyaxon/_pql/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_pql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17840 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_pql/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_pql/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_pql/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.813057 polyaxon-2.2.0rc0/polyaxon/_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.813057 polyaxon-2.2.0rc0/polyaxon/_runner/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/agent/async_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/agent/base_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/agent/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/agent/sync_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.813057 polyaxon-2.2.0rc0/polyaxon/_runner/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.817057 polyaxon-2.2.0rc0/polyaxon/_runner/converter/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/common/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/common/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38005 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.817057 polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/converter/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_runner/kinds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.817057 polyaxon-2.2.0rc0/polyaxon/_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.821057 polyaxon-2.2.0rc0/polyaxon/_schemas/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/clipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/types/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_schemas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.821057 polyaxon-2.2.0rc0/polyaxon/_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.829057 polyaxon-2.2.0rc0/polyaxon/_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162788 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/agents_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/artifacts_stores_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35802 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/auth_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54365 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/connections_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53802 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/dashboards_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   291838 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/organizations_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54930 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/presets_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65408 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/project_dashboards_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65058 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/project_searches_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   251855 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/projects_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77083 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/queues_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   519239 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/runs_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53284 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/searches_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101005 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/service_accounts_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59912 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/tags_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   197711 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/teams_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80904 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/users_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18440 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/api/versions_v1_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.829057 polyaxon-2.2.0rc0/polyaxon/_sdk/async_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/async_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/async_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/async_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15103 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.837057 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_agent_reconcile_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_agent_state_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_agent_state_response_agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_agent_status_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_analytics_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_artifact_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_dashboard_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_entities_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_entities_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_entity_notification_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_entity_stage_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_entity_status_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_activities_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_bookmarks_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_dashboards_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_organization_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_organizations_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_presets_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_project_versions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_queues_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_run_artifacts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_run_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_run_edges_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_searches_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_service_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_team_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_teams_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_list_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_operation_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_password_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_project_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run_edge_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run_edges_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run_reference_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_search_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_section_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_settings_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_team_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_trial_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_user_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_user_singup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.841057 polyaxon-2.2.0rc0/polyaxon/_sdk/sync_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/sync_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28509 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/sync_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sdk/sync_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.841057 polyaxon-2.2.0rc0/polyaxon/_services/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_services/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_services/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_services/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.841057 polyaxon-2.2.0rc0/polyaxon/_sidecar/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.841057 polyaxon-2.2.0rc0/polyaxon/_sidecar/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/container/intervals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.841057 polyaxon-2.2.0rc0/polyaxon/_sidecar/container/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/container/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/container/monitors/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/container/monitors/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/container/monitors/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_sidecar/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.841057 polyaxon-2.2.0rc0/polyaxon/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/cli_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.845057 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/bo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12332 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22124 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/fqn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/host_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_utils/urls_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.845057 polyaxon-2.2.0rc0/polyaxon/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/_vendor/shell_pty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5531 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/polyaxonfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.845057 polyaxon-2.2.0rc0/polyaxon/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.845057 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/fastai_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/ignite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/pytorch_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/scikit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/contrib/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tracking/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.845057 polyaxon-2.2.0rc0/polyaxon/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tuners/bayesian_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tuners/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tuners/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tuners/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tuners/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/tuners/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.753058 polyaxon-2.2.0rc0/polyaxon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-19 19:30:41.000000 polyaxon-2.2.0rc0/polyaxon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22601 2024-05-19 19:30:41.000000 polyaxon-2.2.0rc0/polyaxon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:41.000000 polyaxon-2.2.0rc0/polyaxon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 19:30:41.000000 polyaxon-2.2.0rc0/polyaxon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-19 19:30:41.000000 polyaxon-2.2.0rc0/polyaxon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 19:30:41.000000 polyaxon-2.2.0rc0/polyaxon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:41.849057 polyaxon-2.2.0rc0/polyaxon_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/polyaxon_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-19 19:30:41.849057 polyaxon-2.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-19 19:30:34.000000 polyaxon-2.2.0rc0/setup.py
```

### Comparing `polyaxon-2.1.8/PKG-INFO` & `polyaxon-2.2.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyaxon
-Version: 2.1.8
+Version: 2.2.0rc0
 Summary: Command Line Interface (CLI) and client to interact with Polyaxon API.
 Home-page: https://github.com/polyaxon/polyaxon
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
@@ -47,15 +47,15 @@
 Provides-Extra: sandbox
 
 [![License: Apache 2](https://img.shields.io/badge/License-apache2-blue.svg?style=flat&longCache=true)](LICENSE)
 [![Polyaxon API](https://img.shields.io/docker/pulls/polyaxon/polyaxon-api)](https://hub.docker.com/r/polyaxon/polyaxon-api)
 [![Slack](https://img.shields.io/badge/Slack-1.5k%20members-blue.svg?style=flat&logo=slack&longCache=true)](https://polyaxon.com/slack/)
 
 [![Docs](https://img.shields.io/badge/docs-stable-brightgreen.svg?style=flat&longCache=true)](https://polyaxon.com/docs/)
-[![Release](https://img.shields.io/badge/release-v2.1.8-brightgreen.svg?longCache=true)](https://polyaxon.com/docs/releases/2-1/)
+[![Release](https://img.shields.io/badge/release-v2.2.0-brightgreen.svg?longCache=true)](https://polyaxon.com/docs/releases/2-1/)
 [![GitHub](https://img.shields.io/badge/issue_tracker-github-blue?style=flat&logo=github&longCache=true)](https://github.com/polyaxon/polyaxon/issues)
 [![GitHub](https://img.shields.io/badge/roadmap-github-blue?style=flat&logo=github&longCache=true)](https://github.com/orgs/polyaxon/projects/5)
 
 [![CLI](https://github.com/polyaxon/cli/actions/workflows/cli.yml/badge.svg)](https://github.com/polyaxon/cli/actions/workflows/cli.yml)
 [![Polyaxon](https://github.com/polyaxon/polyaxon/actions/workflows/cli.yml/badge.svg)](https://github.com/polyaxon/polyaxon/actions/workflows/cli.yml)
 [![Haupt](https://github.com/polyaxon/polyaxon/actions/workflows/haupt.yml/badge.svg)](https://github.com/polyaxon/polyaxon/actions/workflows/haupt.yml)
 [![Hypertune](https://github.com/polyaxon/polyaxon/actions/workflows/hypertune.yml/badge.svg)](https://github.com/polyaxon/polyaxon/actions/workflows/hypertune.yml)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polyaxon Version: 2.1.8 Summary: Command Line
+Metadata-Version: 2.1 Name: polyaxon Version: 2.2.0rc0 Summary: Command Line
 Interface (CLI) and client to interact with Polyaxon API. Home-page: https://
 github.com/polyaxon/polyaxon Author: Polyaxon, Inc. Author-email:
 contact@polyaxon.com Maintainer: Polyaxon, Inc. Maintainer-email:
 contact@polyaxon.com License: Apache 2.0 Keywords:
 polyaxon,aws,s3,microsoft,azure,google cloud storage,gcs,deep-learning,machine-
 learning,data-science,neural-networks,artificial-intelligence,ai,reinforcement-
 learning,kubernetes,aws,microsoft,azure,google cloud,tensorFlow,pytorch
@@ -28,15 +28,15 @@
 img.shields.io/badge/License-apache2-blue.svg?style=flat&longCache=true)]
 (LICENSE) [![Polyaxon API](https://img.shields.io/docker/pulls/polyaxon/
 polyaxon-api)](https://hub.docker.com/r/polyaxon/polyaxon-api) [![Slack](https:
 //img.shields.io/badge/Slack-1.5k%20members-
 blue.svg?style=flat&logo=slack&longCache=true)](https://polyaxon.com/slack/) [!
 [Docs](https://img.shields.io/badge/docs-stable-
 brightgreen.svg?style=flat&longCache=true)](https://polyaxon.com/docs/) [!
-[Release](https://img.shields.io/badge/release-v2.1.8-
+[Release](https://img.shields.io/badge/release-v2.2.0-
 brightgreen.svg?longCache=true)](https://polyaxon.com/docs/releases/2-1/) [!
 [GitHub](https://img.shields.io/badge/issue_tracker-github-
 blue?style=flat&logo=github&longCache=true)](https://github.com/polyaxon/
 polyaxon/issues) [![GitHub](https://img.shields.io/badge/roadmap-github-
 blue?style=flat&logo=github&longCache=true)](https://github.com/orgs/polyaxon/
 projects/5) [![CLI](https://github.com/polyaxon/cli/actions/workflows/cli.yml/
 badge.svg)](https://github.com/polyaxon/cli/actions/workflows/cli.yml) [!
```

### Comparing `polyaxon-2.1.8/polyaxon/_auxiliaries/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_auxiliaries/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_auxiliaries/cleaner.py` & `polyaxon-2.2.0rc0/polyaxon/_auxiliaries/cleaner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_auxiliaries/default_scheduling.py` & `polyaxon-2.2.0rc0/polyaxon/_auxiliaries/default_scheduling.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_auxiliaries/init.py` & `polyaxon-2.2.0rc0/polyaxon/_auxiliaries/init.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_auxiliaries/notifier.py` & `polyaxon-2.2.0rc0/polyaxon/_auxiliaries/notifier.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_auxiliaries/sidecar.py` & `polyaxon-2.2.0rc0/polyaxon/_auxiliaries/sidecar.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_auxiliaries/tuner.py` & `polyaxon-2.2.0rc0/polyaxon/_auxiliaries/tuner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/admin.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/admin.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/artifacts.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/auth.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/auth.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/check.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/check.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/completion.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/completion.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/components.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/components.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/config.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/config.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/dashboard.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/dashboard.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/errors.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/errors.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/init.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/init.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/models.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/models.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/operations.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1016,15 +1016,15 @@
 @ops.command()
 @click.option(*OPTIONS_PROJECT["args"], **OPTIONS_PROJECT["kwargs"])
 @click.option(*OPTIONS_RUN_UID["args"], **OPTIONS_RUN_UID["kwargs"])
 @click.option(
     "--executor",
     "-exc",
     type=str,
-    help="The local executor to use, possible values are: docker, k8s, process.",
+    help="The executor to use, possible values are: docker, k8s, process.",
 )
 @click.pass_context
 @clean_outputs
 def execute(ctx, project, uid, executor):
     """Execute a run on the current local machine using one of the specified executor.
 
     Uses /docs/core/cli/#caching
@@ -1125,42 +1125,67 @@
             V1Statuses.RUNNING,
             reason="CliK8SExecutor",
             message="Operation is running",
         )
         executor.create_from_run(response, default_auth=not is_in_ce())
 
     def _execute_on_local_process(response: V1Run, run_client: RunClient):
-        from polyaxon.process.executor.executor import Executor
+        from polyaxon._local_process.executor import Executor
 
         run_client.log_status(
             V1Statuses.STARTING,
             reason="CliProcessExecutor",
             message="Operation is starting",
         )
         executor = Executor()
         if not executor.manager.check():
-            raise Printer.error("Conda is required to run this command.", sys_exit=True)
+            run_client.log_failed(
+                reason="CliProcessExecutor",
+                message="Local process can't be used to run this operation.",
+            )
+            raise Printer.error(
+                "Local process can't be used to run this operation.", sys_exit=True
+            )
+
+        run_client.log_status(
+            V1Statuses.RUNNING,
+            reason="CliProcessExecutor",
+            message="Operation is running",
+        )
 
-        # def _check_conda():
-        #     from polyaxon._deploy.operators.conda import CondaOperator
-        #
-        #     conda = CondaOperator()
-        #     if not conda.check():
-        #         raise Printer.error("Conda is required to run this command.", sys_exit=True)
-        #
-        #     envs = conda.execute(["env", "list", "--json"], is_json=True)
-        #     env_names = [os.path.basename(env) for env in envs["envs"]]
-        #     if conda_env not in env_names:
-        #         raise Printer.error(
-        #             "Conda env `{}` is not installed.".format(conda_env), sys_exit=True
-        #         )
-        #
-        #     cmd_bash, cmd_args = specification.run.get_container_cmd()
-        #     cmd_args = ["source activate {}".format(conda_env)] + cmd_args
-        #     subprocess.Popen(cmd_bash + [" && ".join(cmd_args)], close_fds=True)
+        if V1RunKind.has_pipeline(response.kind):
+            has_children = True
+            while has_children:
+                pipeline_runs = run_client.list_children(
+                    query="status:created", sort="created_at", limit=1
+                )
+                if pipeline_runs.results:
+                    current_run_client = RunClient(
+                        owner=owner,
+                        project=project_name,
+                        run_uuid=pipeline_runs.results[0].uuid,
+                        manual_exceptions_handling=True,
+                    )
+                    current_run_client.refresh_data()
+                    _prepare(current_run_client.run_data, current_run_client)
+                    _execute(current_run_client.run_data, current_run_client)
+                else:
+                    has_children = False
+            return
+        else:
+            result = executor.create_from_run(response, default_auth=not is_in_ce())
+        if result["status"] == V1Statuses.SUCCEEDED:
+            run_client.log_succeeded(
+                reason="CliProcessExecutor", message="Operation was succeeded"
+            )
+        else:
+            run_client.log_failed(
+                reason="CliProcessExecutor",
+                message="Operation failed.\n{}".format(result["message"]),
+            )
 
     owner, project_name, run_uuid = get_project_run_or_local(
         project or ctx.obj.get("project"),
         uid or ctx.obj.get("run_uuid"),
         is_cli=True,
     )
```

### Comparing `polyaxon-2.1.8/polyaxon/_cli/options.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/options.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/port_forward.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/port_forward.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/project_versions.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/project_versions.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/projects.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/projects.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/run.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/run.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/services/agent.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/services/agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/services/clean_artifacts.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/services/clean_artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/services/docker.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/services/docker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/services/initializer.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/services/initializer.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/services/notifier.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/services/notifier.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/services/sidecar.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/services/sidecar.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/services/tuner.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/services/tuner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/services/wait.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/services/wait.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/session.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/session.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/utils.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_cli/version.py` & `polyaxon-2.2.0rc0/polyaxon/_cli/version.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/client.py` & `polyaxon-2.2.0rc0/polyaxon/_client/client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/decorators/client_call_handler.py` & `polyaxon-2.2.0rc0/polyaxon/_client/decorators/client_call_handler.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/impersonate.py` & `polyaxon-2.2.0rc0/polyaxon/_client/impersonate.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/project.py` & `polyaxon-2.2.0rc0/polyaxon/_client/project.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/run.py` & `polyaxon-2.2.0rc0/polyaxon/_client/run.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/store.py` & `polyaxon-2.2.0rc0/polyaxon/_client/store.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/transport/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_client/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/transport/http_transport.py` & `polyaxon-2.2.0rc0/polyaxon/_client/transport/http_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/transport/periodic_transport.py` & `polyaxon-2.2.0rc0/polyaxon/_client/transport/periodic_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/transport/retry_transport.py` & `polyaxon-2.2.0rc0/polyaxon/_client/transport/retry_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/transport/socket_transport.py` & `polyaxon-2.2.0rc0/polyaxon/_client/transport/socket_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/transport/threaded_transport.py` & `polyaxon-2.2.0rc0/polyaxon/_client/transport/threaded_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/transport/ws_client.py` & `polyaxon-2.2.0rc0/polyaxon/_client/transport/ws_client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/workers/base_worker.py` & `polyaxon-2.2.0rc0/polyaxon/_client/workers/base_worker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/workers/periodic_worker.py` & `polyaxon-2.2.0rc0/polyaxon/_client/workers/periodic_worker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_client/workers/queue_worker.py` & `polyaxon-2.2.0rc0/polyaxon/_client/workers/queue_worker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/base.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/contexts.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/contexts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/dask_job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/dask_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/mpi_job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/mpi_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/mx_job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/mx_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/paddle_job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/paddle_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/pytroch_job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/pytroch_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/tf_job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/tf_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/kubeflow/xgb_job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/kubeflow/xgb_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/ray_job.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/ray_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/contexts/service.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/contexts/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/lineage/artifacts_collector.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/lineage/artifacts_collector.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/lineage/collector.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/lineage/collector.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/lineage/io_collector.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/lineage/io_collector.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/resolver/agent.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/resolver/agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/resolver/resolver.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_compiler/resolver/runtime.py` & `polyaxon-2.2.0rc0/polyaxon/_compiler/resolver/runtime.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_config/spec.py` & `polyaxon-2.2.0rc0/polyaxon/_config/spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_connections/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_connections/schemas.py` & `polyaxon-2.2.0rc0/polyaxon/_connections/schemas.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_constants/metadata.py` & `polyaxon-2.2.0rc0/polyaxon/_constants/metadata.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_containers/names.py` & `polyaxon-2.2.0rc0/polyaxon/_containers/names.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_contexts/keys.py` & `polyaxon-2.2.0rc0/polyaxon/_contexts/keys.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_contexts/paths.py` & `polyaxon-2.2.0rc0/polyaxon/_contexts/paths.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_contexts/refs.py` & `polyaxon-2.2.0rc0/polyaxon/_contexts/refs.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_contexts/sections.py` & `polyaxon-2.2.0rc0/polyaxon/_contexts/sections.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/operators/cmd_operator.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/operators/cmd_operator.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/operators/compose.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/operators/compose.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/operators/conda.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/operators/conda.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/operators/docker.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/operators/docker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/operators/helm.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/operators/helm.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/operators/kubectl.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/operators/kubectl.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/operators/pip.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/operators/pip.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/schemas/celery.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/celery.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/schemas/deployment.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/schemas/email.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/email.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/schemas/intervals.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/intervals.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/schemas/proxy.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/proxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,8 +9,9 @@
     enabled: Optional[bool]
     use_in_ops: Optional[bool] = Field(alias="useInOps")
     http_proxy: Optional[StrictStr] = Field(alias="httpProxy")
     https_proxy: Optional[StrictStr] = Field(alias="httpsProxy")
     no_proxy: Optional[StrictStr] = Field(alias="noProxy")
     port: Optional[StrictInt]
     host: Optional[StrictStr]
+    protocol: Optional[StrictStr]
     kind: Optional[StrictStr]
```

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/schemas/security_context.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/security_context.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_deploy/schemas/service.py` & `polyaxon-2.2.0rc0/polyaxon/_deploy/schemas/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_dist.py` & `polyaxon-2.2.0rc0/polyaxon/_dist.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/builder/builder.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/builder/builder.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/builder/dockerfile.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/builder/dockerfile.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/builder/generator.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/builder/generator.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/base/base.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/base/containers.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/containers.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/base/env_vars.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/env_vars.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/base/init.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/init.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/base/main.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/main.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/base/mounts.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/base/mounts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/converters/job.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/converters/job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/converters/service.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/converters/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/converter/mixins.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/converter/mixins.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/docker_types.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/docker_types.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_docker/executor.py` & `polyaxon-2.2.0rc0/polyaxon/_docker/executor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/getters/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/getters/agent.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/getters/owner_entity.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/owner_entity.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/getters/project.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/project.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/getters/queue.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/queue.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/getters/run.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/run.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/getters/user.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/user.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/getters/versioned_entity.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/getters/versioned_entity.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_env_vars/keys.py` & `polyaxon-2.2.0rc0/polyaxon/_env_vars/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 ENV_KEYS_PROXY_SSL_ENABLED = "POLYAXON_PROXY_SSL_ENABLED"
 ENV_KEYS_PROXY_AUTH_ENABLED = "POLYAXON_PROXY_AUTH_ENABLED"
 ENV_KEYS_PROXY_AUTH_EXTERNAL = "POLYAXON_PROXY_AUTH_EXTERNAL"
 ENV_KEYS_PROXY_AUTH_USE_RESOLVER = "POLYAXON_PROXY_AUTH_USE_RESOLVER"
 ENV_KEYS_PROXY_HAS_FORWARD_PROXY = "POLYAXON_PROXY_HAS_FORWARD_PROXY"
 ENV_KEYS_PROXY_FORWARD_PROXY_PORT = "POLYAXON_PROXY_FORWARD_PROXY_PORT"
 ENV_KEYS_PROXY_FORWARD_PROXY_HOST = "POLYAXON_PROXY_FORWARD_PROXY_HOST"
+ENV_KEYS_PROXY_FORWARD_PROXY_PROTOCOL = "POLYAXON_PROXY_FORWARD_PROXY_PROTOCOL"
 ENV_KEYS_PROXY_FORWARD_PROXY_KIND = "POLYAXON_PROXY_FORWARD_PROXY_KIND"
 ENV_KEYS_UI_IN_SANDBOX = "POLYAXON_UI_IN_SANDBOX"
 ENV_KEYS_UI_ADMIN_ENABLED = "POLYAXON_UI_ADMIN_ENABLED"
 ENV_KEYS_UI_ASSETS_VERSION = "POLYAXON_UI_ASSETS_VERSION"
 ENV_KEYS_UI_ENABLED = "POLYAXON_UI_ENABLED"
 ENV_KEYS_UI_OFFLINE = "POLYAXON_UI_OFFLINE"
 ENV_KEYS_UI_BASE_URL = "POLYAXON_UI_BASE_URL"
```

### Comparing `polyaxon-2.1.8/polyaxon/_flow/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/builds/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/builds/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/cache/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/component/base.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/component/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/component/component.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/component/component.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/containers/container.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/containers/container.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/dags/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/dags/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/early_stopping/policies.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/early_stopping/policies.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/environment/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/events/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/events/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/events/enums.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/events/enums.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/hooks/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/init/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/init/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/io/io.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/io/io.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/joins/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/joins/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/bayes.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/bayes.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/enums.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/enums.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/grid_search.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/grid_search.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/hyperband.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/hyperband.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/hyperopt.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/hyperopt.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/iterative.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/iterative.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/mapping.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/mapping.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/params.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/params.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/random_search.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/random_search.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/matrix/tuner.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/matrix/tuner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/notifications/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/operations/base.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/operations/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/operations/compiled_operation.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/operations/compiled_operation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/operations/operation.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/operations/operation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/operators.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/operators.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/optimization/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/optimization/enums.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/optimization/enums.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/params/ops_params.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/params/ops_params.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/params/params.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/params/params.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/plugins/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/dag.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/dag.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/dask/dask.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/dask/dask.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/dask/replica.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/dask/replica.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/enums.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/enums.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/job.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/mpi_job.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/mpi_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/mx_job.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/mx_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/paddle_job.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/paddle_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/pytorch_job.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/pytorch_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/replica.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/replica.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/scheduling_policy.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/scheduling_policy.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/tf_job.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/tf_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/kubeflow/xgboost_job.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/kubeflow/xgboost_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/patch.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/patch.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/ray/ray.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/ray/ray.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/ray/replica.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/ray/replica.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/resources.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/resources.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/run/service.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/run/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/schedules/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/schedules/cron.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/schedules/cron.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/schedules/datetime.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/schedules/datetime.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/schedules/interval.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/schedules/interval.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/templates/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/termination/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/termination/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_flow/trigger_policies.py` & `polyaxon-2.2.0rc0/polyaxon/_flow/trigger_policies.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_fs/async_manager.py` & `polyaxon-2.2.0rc0/polyaxon/_fs/async_manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_fs/fs.py` & `polyaxon-2.2.0rc0/polyaxon/_fs/fs.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_fs/manager.py` & `polyaxon-2.2.0rc0/polyaxon/_fs/manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_fs/tar.py` & `polyaxon-2.2.0rc0/polyaxon/_fs/tar.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_fs/utils.py` & `polyaxon-2.2.0rc0/polyaxon/_fs/utils.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_fs/watcher.py` & `polyaxon-2.2.0rc0/polyaxon/_fs/watcher.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_init/artifacts.py` & `polyaxon-2.2.0rc0/polyaxon/_init/artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_init/auth.py` & `polyaxon-2.2.0rc0/polyaxon/_init/auth.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_init/dockerfile.py` & `polyaxon-2.2.0rc0/polyaxon/_init/dockerfile.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_init/file.py` & `polyaxon-2.2.0rc0/polyaxon/_init/file.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_init/git.py` & `polyaxon-2.2.0rc0/polyaxon/_init/git.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_init/tensorboard.py` & `polyaxon-2.2.0rc0/polyaxon/_init/tensorboard.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/constants.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/constants.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/base/base.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/base/containers.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/containers.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/base/env_vars.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/env_vars.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/base/init.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/init.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/base/main.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
             plugins=plugins,
             kv_env_vars=kv_env_vars,
             artifacts_store_name=artifacts_store.name if artifacts_store else None,
             connections=requested_connections,
             secrets=requested_secrets,
             config_maps=requested_config_maps,
         )
+        env += self._get_resources_env_vars(main_container.resources)
 
         # Env from
         env_from = self._get_env_from_k8s_resources(
             secrets=requested_secrets, config_maps=requested_config_maps
         )
 
         ports = [
```

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/base/mounts.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/mounts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/base/sidecar.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/base/sidecar.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/common/accelerators.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/common/accelerators.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 
 
 def requests_gpu(resources: k8s_schemas.V1ResourceRequirements) -> bool:
     if not resources:
         return False
 
     if resources.requests:
-        for key in resources.requests.keys():
-            if "gpu" in key:
+        for key, val in resources.requests.items():
+            if "gpu" in key and val is not None and val > 0:
                 return True
 
     if resources.limits:
-        for key in resources.limits.keys():
-            if "gpu" in key:
+        for key, val in resources.limits.items():
+            if "gpu" in key and val is not None and val > 0:
                 return True
 
     return False
```

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/common/annotations.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/common/annotations.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/common/volumes.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/common/volumes.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/dask_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/dask_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/helpers.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/helpers.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/mpi_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/mpi_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/mx_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/mx_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/paddle_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/paddle_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/pytroch_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/pytroch_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/tf_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/tf_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/kubeflow/xgboost_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/kubeflow/xgboost_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/ray_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/ray_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/converters/service.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/converters/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/mixins.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/mixins.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/pod/spec.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/pod/spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/converter/pod/volumes.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/converter/pod/volumes.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/crd.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/crd.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/dask_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/dask_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/common.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/common.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/mpi_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/mpi_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/mx_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/mx_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/paddle_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/paddle_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/pytorch_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/pytorch_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/tf_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/tf_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/kubeflow/xgb_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/kubeflow/xgb_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/operation.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/operation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/ray_job.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/ray_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/service.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/custom_resources/setter.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/custom_resources/setter.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/events.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/events.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/executor/async_executor.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/executor/async_executor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/executor/base.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/executor/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/k8s_schemas.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/k8s_schemas.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/k8s_validation.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/k8s_validation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/logging/async_monitor.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/logging/async_monitor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/logging/monitor.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/logging/monitor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/manager/async_manager.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/manager/async_manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/manager/base.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/manager/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/manager/manager.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/manager/manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/monitor.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/monitor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/nodes.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/nodes.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_k8s/pods.py` & `polyaxon-2.2.0rc0/polyaxon/_k8s/pods.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/agent.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/auth.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/auth.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/cli.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/cli.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/client.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/deploy.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/deploy.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/git.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/git.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/home.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/home.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/ignore.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/ignore.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/project.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/project.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/run.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/run.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_managers/user.py` & `polyaxon-2.2.0rc0/polyaxon/_managers/user.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_notifiers/spec.py` & `polyaxon-2.2.0rc0/polyaxon/_notifiers/spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_operations/cleaner.py` & `polyaxon-2.2.0rc0/polyaxon/_operations/cleaner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_operations/notifier.py` & `polyaxon-2.2.0rc0/polyaxon/_operations/notifier.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_operations/tuner.py` & `polyaxon-2.2.0rc0/polyaxon/_operations/tuner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_plugins/sentry.py` & `polyaxon-2.2.0rc0/polyaxon/_plugins/sentry.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/check.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/check.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/manager/operations.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/manager/operations.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/manager/workflows.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/manager/workflows.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/params.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/params.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/base.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/compiled_operation.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/compiled_operation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/libs/parser.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/libs/parser.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/libs/validator.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/libs/validator.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/operation.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/operation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_polyaxonfile/specs/sections.py` & `polyaxon-2.2.0rc0/polyaxon/_polyaxonfile/specs/sections.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_pql/builder.py` & `polyaxon-2.2.0rc0/polyaxon/_pql/builder.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_pql/manager.py` & `polyaxon-2.2.0rc0/polyaxon/_pql/manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_pql/parser.py` & `polyaxon-2.2.0rc0/polyaxon/_pql/parser.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/agent/async_agent.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/agent/async_agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/agent/base_agent.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/agent/base_agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/agent/client.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/agent/client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/agent/sync_agent.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/agent/sync_agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/common/containers.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/common/containers.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/converter.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/converter.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/init/artifacts.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/init/dockerfile.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/dockerfile.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/init/file.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/file.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/init/git.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/git.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/init/store.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/store.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/init/tensorboard.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/init/tensorboard.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/converter/types.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/converter/types.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_runner/executor.py` & `polyaxon-2.2.0rc0/polyaxon/_runner/executor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/agent.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/authentication.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/authentication.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/checks.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/checks.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/cli.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/cli.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/client.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/container_resources.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/container_resources.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/lifecycle.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/lifecycle.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/services.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/services.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/types/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/types/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/types/artifacts.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/types/artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/types/clipped.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/types/clipped.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/types/dockerfile.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/types/dockerfile.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/types/file.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/types/file.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/types/git.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/types/git.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_schemas/types/tensorboard.py` & `polyaxon-2.2.0rc0/polyaxon/_schemas/types/tensorboard.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/agents_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/agents_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/artifacts_stores_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/artifacts_stores_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/auth_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/auth_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/connections_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/connections_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/dashboards_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/dashboards_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/organizations_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/organizations_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1266,28 +1266,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def delete_organization_member(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> None:  # noqa: E501
         """Delete organization member details  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_organization_member(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -1305,28 +1305,28 @@
             owner, name, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def delete_organization_member_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Delete organization member details  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_organization_member_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -2245,28 +2245,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def get_organization_member(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> V1OrganizationMember:  # noqa: E501
         """Get organization member details  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_organization_member(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -2284,28 +2284,28 @@
             owner, name, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def get_organization_member_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Get organization member details  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_organization_member_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
```

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/presets_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/presets_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/project_dashboards_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/project_dashboards_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 class ProjectDashboardsV1Api(BaseApi):
     @validate_arguments
     def create_project_dashboard(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         body: Annotated[V1Dashboard, Field(..., description="Dashboard body")],
         **kwargs
     ) -> V1Dashboard:
         """Create project dashboard
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_project_dashboard(owner, project, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param body: Dashboard body (required)
         :type body: V1Dashboard
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -55,30 +55,30 @@
         )
 
     @validate_arguments
     def create_project_dashboard_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         body: Annotated[V1Dashboard, Field(..., description="Dashboard body")],
         **kwargs
     ):
         """Create project dashboard
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_project_dashboard_with_http_info(owner, project, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param body: Dashboard body (required)
         :type body: V1Dashboard
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
@@ -1065,15 +1065,15 @@
         )
 
     @validate_arguments
     def patch_project_dashboard(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         dashboard_uuid: Annotated[StrictStr, Field(..., description="UUID")],
         body: Annotated[V1Dashboard, Field(..., description="Dashboard body")],
         **kwargs
     ) -> V1Dashboard:  # noqa: E501
         """Patch project dashboard  # noqa: E501
 
@@ -1081,15 +1081,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.patch_project_dashboard(owner, project, dashboard_uuid, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param dashboard_uuid: UUID (required)
         :type dashboard_uuid: str
         :param body: Dashboard body (required)
         :type body: V1Dashboard
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1112,15 +1112,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def patch_project_dashboard_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         dashboard_uuid: Annotated[StrictStr, Field(..., description="UUID")],
         body: Annotated[V1Dashboard, Field(..., description="Dashboard body")],
         **kwargs
     ):  # noqa: E501
         """Patch project dashboard  # noqa: E501
 
@@ -1128,15 +1128,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.patch_project_dashboard_with_http_info(owner, project, dashboard_uuid, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param dashboard_uuid: UUID (required)
         :type dashboard_uuid: str
         :param body: Dashboard body (required)
         :type body: V1Dashboard
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1436,15 +1436,15 @@
         )
 
     @validate_arguments
     def update_project_dashboard(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         dashboard_uuid: Annotated[StrictStr, Field(..., description="UUID")],
         body: Annotated[V1Dashboard, Field(..., description="Dashboard body")],
         **kwargs
     ) -> V1Dashboard:  # noqa: E501
         """Update project dashboard  # noqa: E501
 
@@ -1452,15 +1452,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_project_dashboard(owner, project, dashboard_uuid, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param dashboard_uuid: UUID (required)
         :type dashboard_uuid: str
         :param body: Dashboard body (required)
         :type body: V1Dashboard
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1483,15 +1483,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def update_project_dashboard_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         dashboard_uuid: Annotated[StrictStr, Field(..., description="UUID")],
         body: Annotated[V1Dashboard, Field(..., description="Dashboard body")],
         **kwargs
     ):  # noqa: E501
         """Update project dashboard  # noqa: E501
 
@@ -1499,15 +1499,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_project_dashboard_with_http_info(owner, project, dashboard_uuid, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param dashboard_uuid: UUID (required)
         :type dashboard_uuid: str
         :param body: Dashboard body (required)
         :type body: V1Dashboard
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
```

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/project_searches_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/project_searches_v1_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 class ProjectSearchesV1Api(BaseApi):
     @validate_arguments
     def create_project_search(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         body: Annotated[V1Search, Field(..., description="Search body")],
         **kwargs
     ) -> V1Search:  # noqa: E501
         """Create project search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_project_search(owner, project, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param body: Search body (required)
         :type body: V1Search
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -55,30 +55,30 @@
         )  # noqa: E501
 
     @validate_arguments
     def create_project_search_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         body: Annotated[V1Search, Field(..., description="Search body")],
         **kwargs
     ):  # noqa: E501
         """Create project search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_project_search_with_http_info(owner, project, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param body: Search body (required)
         :type body: V1Search
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
@@ -1065,15 +1065,15 @@
         )
 
     @validate_arguments
     def patch_project_search(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         search_uuid: Annotated[StrictStr, Field(..., description="UUID")],
         body: Annotated[V1Search, Field(..., description="Search body")],
         **kwargs
     ) -> V1Search:  # noqa: E501
         """Patch project search  # noqa: E501
 
@@ -1081,15 +1081,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.patch_project_search(owner, project, search_uuid, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param search_uuid: UUID (required)
         :type search_uuid: str
         :param body: Search body (required)
         :type body: V1Search
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1112,15 +1112,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def patch_project_search_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         search_uuid: Annotated[StrictStr, Field(..., description="UUID")],
         body: Annotated[V1Search, Field(..., description="Search body")],
         **kwargs
     ):  # noqa: E501
         """Patch project search  # noqa: E501
 
@@ -1128,15 +1128,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.patch_project_search_with_http_info(owner, project, search_uuid, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param search_uuid: UUID (required)
         :type search_uuid: str
         :param body: Search body (required)
         :type body: V1Search
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1436,15 +1436,15 @@
         )
 
     @validate_arguments
     def update_project_search(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         search_uuid: Annotated[StrictStr, Field(..., description="UUID")],
         body: Annotated[V1Search, Field(..., description="Search body")],
         **kwargs
     ) -> V1Search:  # noqa: E501
         """Update project search  # noqa: E501
 
@@ -1452,15 +1452,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_project_search(owner, project, search_uuid, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param search_uuid: UUID (required)
         :type search_uuid: str
         :param body: Search body (required)
         :type body: V1Search
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1483,15 +1483,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def update_project_search_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
+            StrictStr, Field(..., description="Project under namespace")
         ],
         search_uuid: Annotated[StrictStr, Field(..., description="UUID")],
         body: Annotated[V1Search, Field(..., description="Search body")],
         **kwargs
     ):  # noqa: E501
         """Update project search  # noqa: E501
 
@@ -1499,15 +1499,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_project_search_with_http_info(owner, project, search_uuid, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
+        :param project: Project under namespace (required)
         :type project: str
         :param search_uuid: UUID (required)
         :type search_uuid: str
         :param body: Search body (required)
         :type body: V1Search
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
```

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/projects_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/projects_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 
 
 class ProjectsV1Api(BaseApi):
     @validate_arguments
     def archive_project(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> None:
         """Archive project
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.archive_project(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -56,28 +56,28 @@
         kwargs["_return_http_data_only"] = True
         return self.archive_project_with_http_info(owner, name, **kwargs)
 
     @validate_arguments
     def archive_project_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):
         """Archive project
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.archive_project_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -175,28 +175,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def bookmark_project(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> None:  # noqa: E501
         """Bookmark project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bookmark_project(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -212,28 +212,28 @@
         kwargs["_return_http_data_only"] = True
         return self.bookmark_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
     def bookmark_project_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Bookmark project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bookmark_project_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -497,14 +497,191 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
+    def create_team_project(
+        self,
+        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
+        team: Annotated[StrictStr, Field(..., description="Team")],
+        body: Annotated[V1Project, Field(..., description="Project body")],
+        **kwargs
+    ) -> V1Project:  # noqa: E501
+        """Create new project via team space  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_team_project(owner, team, body, async_req=True)
+        >>> result = thread.get()
+
+        :param owner: Owner of the namespace (required)
+        :type owner: str
+        :param team: Team (required)
+        :type team: str
+        :param body: Project body (required)
+        :type body: V1Project
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1Project
+        """
+        kwargs["_return_http_data_only"] = True
+        return self.create_team_project_with_http_info(
+            owner, team, body, **kwargs
+        )  # noqa: E501
+
+    @validate_arguments
+    def create_team_project_with_http_info(
+        self,
+        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
+        team: Annotated[StrictStr, Field(..., description="Team")],
+        body: Annotated[V1Project, Field(..., description="Project body")],
+        **kwargs
+    ):  # noqa: E501
+        """Create new project via team space  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_team_project_with_http_info(owner, team, body, async_req=True)
+        >>> result = thread.get()
+
+        :param owner: Owner of the namespace (required)
+        :type owner: str
+        :param team: Team (required)
+        :type team: str
+        :param body: Project body (required)
+        :type body: V1Project
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1Project, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = ["owner", "team", "body"]
+        _all_params.extend(
+            [
+                "async_req",
+                "_return_http_data_only",
+                "_preload_content",
+                "_request_timeout",
+                "_request_auth",
+                "_content_type",
+                "_headers",
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params["kwargs"].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_team_project" % _key
+                )
+            _params[_key] = _val
+        del _params["kwargs"]
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params["owner"]:
+            _path_params["owner"] = _params["owner"]
+
+        if _params["team"]:
+            _path_params["team"] = _params["team"]
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get("_headers", {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params["body"]:
+            _body_params = _params["body"]
+
+        # set the HTTP header `Accept`
+        _header_params["Accept"] = self.api_client.select_header_accept(
+            ["application/json"]
+        )  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get(
+            "_content_type",
+            self.api_client.select_header_content_type(["application/json"]),
+        )
+        if _content_types_list:
+            _header_params["Content-Type"] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ["ApiKey"]  # noqa: E501
+
+        _response_types_map = {
+            "200": "V1Project",
+            "204": "object",
+            "403": "object",
+            "404": "object",
+        }
+
+        return self.api_client.call_api(
+            "/api/v1/{owner}/{team}/projects/create",
+            "POST",
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get("async_req"),
+            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
+            _preload_content=_params.get("_preload_content", True),
+            _request_timeout=_params.get("_request_timeout"),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get("_request_auth"),
+        )
+
+    @validate_arguments
     def create_version(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         project: Annotated[StrictStr, Field(..., description="Project name")],
         version_kind: Annotated[
             str,
             Field(..., description="Optional kind to tell the kind of this version"),
@@ -908,28 +1085,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def delete_project(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> None:  # noqa: E501
         """Delete project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_project(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -945,28 +1122,28 @@
         kwargs["_return_http_data_only"] = True
         return self.delete_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_project_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Delete project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_project_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1248,28 +1425,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def disable_project_ci(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> None:  # noqa: E501
         """Disbale project CI  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.disable_project_ci(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -1287,28 +1464,28 @@
             owner, name, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def disable_project_ci_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Disbale project CI  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.disable_project_ci_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1406,28 +1583,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def enable_project_ci(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> None:  # noqa: E501
         """Enable project CI  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.enable_project_ci(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -1445,28 +1622,28 @@
             owner, name, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def enable_project_ci_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Enable project CI  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.enable_project_ci_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1564,28 +1741,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def get_project(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> V1Project:  # noqa: E501
         """Get project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_project(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -1601,28 +1778,28 @@
         kwargs["_return_http_data_only"] = True
         return self.get_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_project_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Get project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_project_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1978,28 +2155,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def get_project_settings(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> V1ProjectSettings:  # noqa: E501
         """Get Project settings  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_project_settings(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -2017,28 +2194,28 @@
             owner, name, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def get_project_settings_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Get Project settings  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_project_settings_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -3710,15 +3887,15 @@
         )
 
     @validate_arguments
     def list_version_names(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         kind: Annotated[str, Field(..., description="Version Kind")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -3736,15 +3913,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_version_names(owner, entity, kind, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param kind: Version Kind (required)
         :type kind: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -3775,15 +3952,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def list_version_names_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         kind: Annotated[str, Field(..., description="Version Kind")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -3801,15 +3978,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_version_names_with_http_info(owner, entity, kind, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param kind: Version Kind (required)
         :type kind: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -3946,15 +4123,15 @@
         )
 
     @validate_arguments
     def list_versions(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         kind: Annotated[str, Field(..., description="Version Kind")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -3972,15 +4149,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_versions(owner, entity, kind, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param kind: Version Kind (required)
         :type kind: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -4011,15 +4188,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def list_versions_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         kind: Annotated[str, Field(..., description="Version Kind")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -4037,15 +4214,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_versions_with_http_info(owner, entity, kind, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param kind: Version Kind (required)
         :type kind: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -4760,28 +4937,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def restore_project(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> None:  # noqa: E501
         """Restore project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.restore_project(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -4797,28 +4974,28 @@
         kwargs["_return_http_data_only"] = True
         return self.restore_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
     def restore_project_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Restore project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.restore_project_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -5128,28 +5305,28 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def unbookmark_project(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ) -> None:  # noqa: E501
         """Unbookmark project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.unbookmark_project(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -5167,28 +5344,28 @@
             owner, name, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def unbookmark_project_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        name: Annotated[StrictStr, Field(..., description="Component under namespace")],
         **kwargs
     ):  # noqa: E501
         """Unbookmark project  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.unbookmark_project_with_http_info(owner, name, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param name: Component under namesapce (required)
+        :param name: Component under namespace (required)
         :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
```

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/queues_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/queues_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/runs_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/runs_v1_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,32 +218,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def approve_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ) -> None:  # noqa: E501
         """Approve runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.approve_runs(owner, project, body, async_req=True)
+        >>> thread = api.approve_runs(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -255,39 +253,37 @@
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
         return self.approve_runs_with_http_info(
-            owner, project, body, **kwargs
+            owner, name, body, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def approve_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ):  # noqa: E501
         """Approve runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.approve_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.approve_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -308,15 +304,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -337,16 +333,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -374,15 +370,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/approve",
+            "/api/v1/{owner}/{name}/runs/approve",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -576,32 +572,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def archive_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ) -> None:  # noqa: E501
         """Archive runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.archive_runs(owner, project, body, async_req=True)
+        >>> thread = api.archive_runs(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -613,39 +607,37 @@
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
         return self.archive_runs_with_http_info(
-            owner, project, body, **kwargs
+            owner, name, body, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def archive_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ):  # noqa: E501
         """Archive runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.archive_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.archive_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -666,15 +658,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -695,16 +687,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -732,15 +724,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/archive",
+            "/api/v1/{owner}/{name}/runs/archive",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -934,32 +926,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def bookmark_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ) -> None:  # noqa: E501
         """Bookmark runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.bookmark_runs(owner, project, body, async_req=True)
+        >>> thread = api.bookmark_runs(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -971,39 +961,37 @@
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
         return self.bookmark_runs_with_http_info(
-            owner, project, body, **kwargs
+            owner, name, body, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def bookmark_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ):  # noqa: E501
         """Bookmark runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.bookmark_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.bookmark_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1024,15 +1012,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -1053,16 +1041,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -1090,15 +1078,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/bookmark",
+            "/api/v1/{owner}/{name}/runs/bookmark",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -2847,32 +2835,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def delete_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ) -> None:  # noqa: E501
         """Delete runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_runs(owner, project, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -2884,39 +2870,37 @@
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
         return self.delete_runs_with_http_info(
-            owner, project, body, **kwargs
+            owner, name, body, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def delete_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ):  # noqa: E501
         """Delete runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.delete_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -2937,15 +2921,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -2966,16 +2950,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -3003,15 +2987,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/delete",
+            "/api/v1/{owner}/{name}/runs/delete",
             "DELETE",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -4369,15 +4353,15 @@
         )
 
     @validate_arguments
     def get_run_artifacts_lineage(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -4395,15 +4379,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_artifacts_lineage(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -4434,15 +4418,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def get_run_artifacts_lineage_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -4460,15 +4444,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_artifacts_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -4605,15 +4589,15 @@
         )
 
     @validate_arguments
     def get_run_artifacts_lineage_names(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -4631,15 +4615,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_artifacts_lineage_names(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -4670,15 +4654,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def get_run_artifacts_lineage_names_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -4696,15 +4680,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_artifacts_lineage_names_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -5052,15 +5036,15 @@
         )
 
     @validate_arguments
     def get_run_clones_lineage(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -5078,15 +5062,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_clones_lineage(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -5117,15 +5101,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def get_run_clones_lineage_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -5143,15 +5127,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_clones_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -5288,15 +5272,15 @@
         )
 
     @validate_arguments
     def get_run_connections_lineage(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -5314,15 +5298,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_connections_lineage(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -5353,15 +5337,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def get_run_connections_lineage_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -5379,15 +5363,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_connections_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -5524,15 +5508,15 @@
         )
 
     @validate_arguments
     def get_run_downstream_lineage(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -5550,15 +5534,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_downstream_lineage(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -5589,15 +5573,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def get_run_downstream_lineage_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -5615,15 +5599,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_downstream_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -6962,15 +6946,15 @@
         )
 
     @validate_arguments
     def get_run_stats(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -6999,15 +6983,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_stats(owner, entity, uuid, offset, limit, sort, query, bookmarks, mode, kind, aggregate, groupby, trunc, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -7061,15 +7045,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def get_run_stats_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -7098,15 +7082,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_stats_with_http_info(owner, entity, uuid, offset, limit, sort, query, bookmarks, mode, kind, aggregate, groupby, trunc, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -7453,15 +7437,15 @@
         )
 
     @validate_arguments
     def get_run_upstream_lineage(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -7479,15 +7463,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_upstream_lineage(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -7518,15 +7502,15 @@
         )  # noqa: E501
 
     @validate_arguments
     def get_run_upstream_lineage_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         entity: Annotated[
-            StrictStr, Field(..., description="Entity name under namesapce")
+            StrictStr, Field(..., description="Entity name under namespace")
         ],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
@@ -7544,15 +7528,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_run_upstream_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param entity: Entity name under namesapce (required)
+        :param entity: Entity name under namespace (required)
         :type entity: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
@@ -8586,32 +8570,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def invalidate_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ) -> None:  # noqa: E501
         """Invalidate runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.invalidate_runs(owner, project, body, async_req=True)
+        >>> thread = api.invalidate_runs(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -8623,39 +8605,37 @@
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
         return self.invalidate_runs_with_http_info(
-            owner, project, body, **kwargs
+            owner, name, body, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def invalidate_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ):  # noqa: E501
         """Invalidate runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.invalidate_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.invalidate_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -8676,15 +8656,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -8705,16 +8685,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -8742,15 +8722,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/invalidate",
+            "/api/v1/{owner}/{name}/runs/invalidate",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -10191,32 +10171,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def restore_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ) -> None:  # noqa: E501
         """Restore runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.restore_runs(owner, project, body, async_req=True)
+        >>> thread = api.restore_runs(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -10228,39 +10206,37 @@
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
         return self.restore_runs_with_http_info(
-            owner, project, body, **kwargs
+            owner, name, body, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def restore_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ):  # noqa: E501
         """Restore runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.restore_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.restore_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -10281,15 +10257,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -10310,16 +10286,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -10347,15 +10323,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/restore",
+            "/api/v1/{owner}/{name}/runs/restore",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -10915,32 +10891,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def skip_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ) -> None:  # noqa: E501
         """Skip runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.skip_runs(owner, project, body, async_req=True)
+        >>> thread = api.skip_runs(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -10951,40 +10925,36 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
-        return self.skip_runs_with_http_info(
-            owner, project, body, **kwargs
-        )  # noqa: E501
+        return self.skip_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
     def skip_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ):  # noqa: E501
         """Skip runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.skip_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.skip_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -11005,15 +10975,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -11035,16 +11005,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
 
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
         # process the form parameters
         _form_params = []
@@ -11069,15 +11039,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/skip",
+            "/api/v1/{owner}/{name}/runs/skip",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -11269,32 +11239,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def stop_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ) -> None:  # noqa: E501
         """Stop runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.stop_runs(owner, project, body, async_req=True)
+        >>> thread = api.stop_runs(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -11305,40 +11273,36 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
-        return self.stop_runs_with_http_info(
-            owner, project, body, **kwargs
-        )  # noqa: E501
+        return self.stop_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
     def stop_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1Uuids, Field(..., description="Uuids of the entities")],
         **kwargs
     ):  # noqa: E501
         """Stop runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.stop_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.stop_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Uuids of the entities (required)
         :type body: V1Uuids
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -11359,15 +11323,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -11388,16 +11352,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -11425,15 +11389,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/stop",
+            "/api/v1/{owner}/{name}/runs/stop",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -11625,32 +11589,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def tag_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1EntitiesTags, Field(..., description="Data")],
         **kwargs
     ) -> None:  # noqa: E501
         """Tag runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.tag_runs(owner, project, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Data (required)
         :type body: V1EntitiesTags
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -11661,40 +11623,36 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
-        return self.tag_runs_with_http_info(
-            owner, project, body, **kwargs
-        )  # noqa: E501
+        return self.tag_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
     def tag_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1EntitiesTags, Field(..., description="Data")],
         **kwargs
     ):  # noqa: E501
         """Tag runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.tag_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.tag_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Data (required)
         :type body: V1EntitiesTags
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -11715,15 +11673,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -11744,16 +11702,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -11781,15 +11739,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/tag",
+            "/api/v1/{owner}/{name}/runs/tag",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -11989,32 +11947,30 @@
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
     def transfer_runs(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1EntitiesTransfer, Field(..., description="Data")],
         **kwargs
     ) -> None:  # noqa: E501
         """Transfer runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.transfer_runs(owner, project, body, async_req=True)
+        >>> thread = api.transfer_runs(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Data (required)
         :type body: V1EntitiesTransfer
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -12026,39 +11982,37 @@
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
         return self.transfer_runs_with_http_info(
-            owner, project, body, **kwargs
+            owner, name, body, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def transfer_runs_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        project: Annotated[
-            StrictStr, Field(..., description="Project under namesapce")
-        ],
+        name: Annotated[StrictStr, Field(..., description="Entity under namespace")],
         body: Annotated[V1EntitiesTransfer, Field(..., description="Data")],
         **kwargs
     ):  # noqa: E501
         """Transfer runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.transfer_runs_with_http_info(owner, project, body, async_req=True)
+        >>> thread = api.transfer_runs_with_http_info(owner, name, body, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
-        :param project: Project under namesapce (required)
-        :type project: str
+        :param name: Entity under namespace (required)
+        :type name: str
         :param body: Data (required)
         :type body: V1EntitiesTransfer
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -12079,15 +12033,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "project", "body"]
+        _all_params = ["owner", "name", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -12108,16 +12062,16 @@
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["owner"]:
             _path_params["owner"] = _params["owner"]
-        if _params["project"]:
-            _path_params["project"] = _params["project"]
+        if _params["name"]:
+            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
 
@@ -12145,15 +12099,15 @@
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/{owner}/{project}/runs/transfer",
+            "/api/v1/{owner}/{name}/runs/transfer",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
```

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/searches_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/searches_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/service_accounts_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/service_accounts_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1304,15 +1304,15 @@
 
     @validate_arguments
     def list_service_account_tokens(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         entity: Annotated[
-            Optional[StrictStr], Field(description="Entity name under namesapce.")
+            Optional[StrictStr], Field(description="Entity name under namespace.")
         ] = None,
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
             Optional[StrictStr], Field(description="Sort to order the search.")
@@ -1331,15 +1331,15 @@
         >>> thread = api.list_service_account_tokens(owner, uuid, entity, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
-        :param entity: Entity name under namesapce.
+        :param entity: Entity name under namespace.
         :type entity: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
         :param sort: Sort to order the search.
         :type sort: str
@@ -1369,15 +1369,15 @@
 
     @validate_arguments
     def list_service_account_tokens_with_http_info(
         self,
         owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         uuid: Annotated[StrictStr, Field(..., description="SubEntity uuid")],
         entity: Annotated[
-            Optional[StrictStr], Field(description="Entity name under namesapce.")
+            Optional[StrictStr], Field(description="Entity name under namespace.")
         ] = None,
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
             Optional[StrictStr], Field(description="Sort to order the search.")
@@ -1396,15 +1396,15 @@
         >>> thread = api.list_service_account_tokens_with_http_info(owner, uuid, entity, offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
         :param owner: Owner of the namespace (required)
         :type owner: str
         :param uuid: SubEntity uuid (required)
         :type uuid: str
-        :param entity: Entity name under namesapce.
+        :param entity: Entity name under namespace.
         :type entity: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
         :param sort: Sort to order the search.
         :type sort: str
```

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/tags_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/tags_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/teams_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/users_v1_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,256 +1,67 @@
 from typing import Optional
 from typing_extensions import Annotated
 
 from clipped.compact.pydantic import Field, StrictInt, StrictStr, validate_arguments
 
 from polyaxon._sdk.base_api import BaseApi
-from polyaxon._sdk.schemas.v1_list_team_members_response import (
-    V1ListTeamMembersResponse,
-)
-from polyaxon._sdk.schemas.v1_list_teams_response import V1ListTeamsResponse
-from polyaxon._sdk.schemas.v1_team import V1Team
-from polyaxon._sdk.schemas.v1_team_member import V1TeamMember
+from polyaxon._sdk.schemas.v1_list_activities_response import V1ListActivitiesResponse
+from polyaxon._sdk.schemas.v1_list_token_response import V1ListTokenResponse
+from polyaxon._sdk.schemas.v1_token import V1Token
+from polyaxon._sdk.schemas.v1_user import V1User
 from polyaxon.exceptions import ApiTypeError
 
 
-class TeamsV1Api(BaseApi):
+class UsersV1Api(BaseApi):
     @validate_arguments
-    def create_team(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        body: Annotated[V1Team, Field(..., description="Team body")],
-        **kwargs
-    ) -> V1Team:
-        """Create team
+    def create_token(
+        self, body: Annotated[V1Token, Field(..., description="Token body")], **kwargs
+    ) -> V1Token:  # noqa: E501
+        """Create token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_team(owner, body, async_req=True)
+        >>> thread = api.create_token(body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param body: Team body (required)
-        :type body: V1Team
+        :param body: Token body (required)
+        :type body: V1Token
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1Team
+        :rtype: V1Token
         """
         kwargs["_return_http_data_only"] = True
-        return self.create_team_with_http_info(owner, body, **kwargs)
+        return self.create_token_with_http_info(body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_team_with_http_info(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        body: Annotated[V1Team, Field(..., description="Team body")],
-        **kwargs
-    ):
-        """Create team
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_team_with_http_info(owner, body, async_req=True)
-        >>> result = thread.get()
-
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param body: Team body (required)
-        :type body: V1Team
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(V1Team, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = ["owner", "body"]
-        _all_params.extend(
-            [
-                "async_req",
-                "_return_http_data_only",
-                "_preload_content",
-                "_request_timeout",
-                "_request_auth",
-                "_content_type",
-                "_headers",
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params["kwargs"].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method create_team" % _key
-                )
-            _params[_key] = _val
-        del _params["kwargs"]
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-
-        # process the query parameters
-        _query_params = []
-
-        # process the header parameters
-        _header_params = dict(_params.get("_headers", {}))
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-
-        # process the body parameter
-        _body_params = None
-        if _params["body"]:
-            _body_params = _params["body"]
-
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(
-            ["application/json"]
-        )
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get(
-            "_content_type",
-            self.api_client.select_header_content_type(["application/json"]),
-        )
-        if _content_types_list:
-            _header_params["Content-Type"] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ["ApiKey"]
-
-        _response_types_map = {
-            "200": "V1Team",
-            "204": "object",
-            "403": "object",
-            "404": "object",
-        }
-
-        return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams",
-            "POST",
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get("async_req"),
-            _return_http_data_only=_params.get("_return_http_data_only"),
-            _preload_content=_params.get("_preload_content", True),
-            _request_timeout=_params.get("_request_timeout"),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get("_request_auth"),
-        )
-
-    @validate_arguments
-    def create_team_member(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team")],
-        body: Annotated[V1TeamMember, Field(..., description="Team body")],
-        **kwargs
-    ) -> V1TeamMember:  # noqa: E501
-        """Create team member  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_team_member(owner, team, body, async_req=True)
-        >>> result = thread.get()
-
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team (required)
-        :type team: str
-        :param body: Team body (required)
-        :type body: V1TeamMember
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: V1TeamMember
-        """
-        kwargs["_return_http_data_only"] = True
-        return self.create_team_member_with_http_info(
-            owner, team, body, **kwargs
-        )  # noqa: E501
-
-    @validate_arguments
-    def create_team_member_with_http_info(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team")],
-        body: Annotated[V1TeamMember, Field(..., description="Team body")],
-        **kwargs
+    def create_token_with_http_info(
+        self, body: Annotated[V1Token, Field(..., description="Token body")], **kwargs
     ):  # noqa: E501
-        """Create team member  # noqa: E501
+        """Create token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_team_member_with_http_info(owner, team, body, async_req=True)
+        >>> thread = api.create_token_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team (required)
-        :type team: str
-        :param body: Team body (required)
-        :type body: V1TeamMember
+        :param body: Token body (required)
+        :type body: V1Token
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -264,20 +75,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1TeamMember, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1Token, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["owner", "team", "body"]
+        _all_params = ["body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -287,38 +98,31 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_team_member" % _key
+                    " to method create_token" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["team"]:
-            _path_params["team"] = _params["team"]
 
         # process the query parameters
         _query_params = []
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
         if _params["body"]:
             _body_params = _params["body"]
 
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
@@ -333,22 +137,22 @@
         if _content_types_list:
             _header_params["Content-Type"] = _content_types_list
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1TeamMember",
+            "200": "V1Token",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{team}/members",
+            "/api/v1/users/tokens",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -359,32 +163,29 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def delete_team(
+    def delete_token(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        uuid: Annotated[StrictStr, Field(..., description="UUid of the namespace")],
         **kwargs
     ) -> None:  # noqa: E501
-        """Delete team  # noqa: E501
+        """Delete token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_team(owner, name, async_req=True)
+        >>> thread = api.delete_token(uuid, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param name: Component under namesapce (required)
-        :type name: str
+        :param uuid: UUid of the namespace (required)
+        :type uuid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -393,35 +194,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs["_return_http_data_only"] = True
-        return self.delete_team_with_http_info(owner, name, **kwargs)  # noqa: E501
+        return self.delete_token_with_http_info(uuid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_team_with_http_info(
+    def delete_token_with_http_info(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        uuid: Annotated[StrictStr, Field(..., description="UUid of the namespace")],
         **kwargs
     ):  # noqa: E501
-        """Delete team  # noqa: E501
+        """Delete token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_team_with_http_info(owner, name, async_req=True)
+        >>> thread = api.delete_token_with_http_info(uuid, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param name: Component under namesapce (required)
-        :type name: str
+        :param uuid: UUid of the namespace (required)
+        :type uuid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -440,15 +238,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["owner", "name"]
+        _all_params = ["uuid"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -458,53 +256,47 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_team" % _key
+                    " to method delete_token" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["name"]:
-            _path_params["name"] = _params["name"]
+        if _params["uuid"]:
+            _path_params["uuid"] = _params["uuid"]
 
         # process the query parameters
         _query_params = []
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
-
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
             ["application/json"]
         )  # noqa: E501
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{name}",
+            "/api/v1/users/tokens/{uuid}",
             "DELETE",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -515,77 +307,101 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def delete_team_member(
+    def get_history(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team under namesapce")],
-        user: Annotated[StrictStr, Field(..., description="Member under team")],
+        offset: Annotated[
+            Optional[StrictInt], Field(description="Pagination offset.")
+        ] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
+        sort: Annotated[
+            Optional[StrictStr], Field(description="Sort to order the search.")
+        ] = None,
+        query: Annotated[
+            Optional[StrictStr], Field(description="Query filter the search.")
+        ] = None,
+        no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
         **kwargs
-    ) -> None:  # noqa: E501
-        """Delete team member details  # noqa: E501
+    ) -> V1ListActivitiesResponse:  # noqa: E501
+        """User History  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_team_member(owner, team, user, async_req=True)
+        >>> thread = api.get_history(offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team under namesapce (required)
-        :type team: str
-        :param user: Member under team (required)
-        :type user: str
+        :param offset: Pagination offset.
+        :type offset: int
+        :param limit: Limit size.
+        :type limit: int
+        :param sort: Sort to order the search.
+        :type sort: str
+        :param query: Query filter the search.
+        :type query: str
+        :param no_page: No pagination.
+        :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: V1ListActivitiesResponse
         """
         kwargs["_return_http_data_only"] = True
-        return self.delete_team_member_with_http_info(
-            owner, team, user, **kwargs
+        return self.get_history_with_http_info(
+            offset, limit, sort, query, no_page, **kwargs
         )  # noqa: E501
 
     @validate_arguments
-    def delete_team_member_with_http_info(
+    def get_history_with_http_info(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team under namesapce")],
-        user: Annotated[StrictStr, Field(..., description="Member under team")],
+        offset: Annotated[
+            Optional[StrictInt], Field(description="Pagination offset.")
+        ] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
+        sort: Annotated[
+            Optional[StrictStr], Field(description="Sort to order the search.")
+        ] = None,
+        query: Annotated[
+            Optional[StrictStr], Field(description="Query filter the search.")
+        ] = None,
+        no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
         **kwargs
     ):  # noqa: E501
-        """Delete team member details  # noqa: E501
+        """User History  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_team_member_with_http_info(owner, team, user, async_req=True)
+        >>> thread = api.get_history_with_http_info(offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team under namesapce (required)
-        :type team: str
-        :param user: Member under team (required)
-        :type user: str
+        :param offset: Pagination offset.
+        :type offset: int
+        :param limit: Limit size.
+        :type limit: int
+        :param sort: Sort to order the search.
+        :type sort: str
+        :param query: Query filter the search.
+        :type query: str
+        :param no_page: No pagination.
+        :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -599,20 +415,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(V1ListActivitiesResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["owner", "team", "user"]
+        _all_params = ["offset", "limit", "sort", "query", "no_page"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -622,56 +438,66 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_team_member" % _key
+                    " to method get_history" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["team"]:
-            _path_params["team"] = _params["team"]
-        if _params["user"]:
-            _path_params["user"] = _params["user"]
 
         # process the query parameters
         _query_params = []
+        if _params.get("offset") is not None:  # noqa: E501
+            _query_params.append(("offset", _params["offset"]))
+
+        if _params.get("limit") is not None:  # noqa: E501
+            _query_params.append(("limit", _params["limit"]))
+
+        if _params.get("sort") is not None:  # noqa: E501
+            _query_params.append(("sort", _params["sort"]))
+
+        if _params.get("query") is not None:  # noqa: E501
+            _query_params.append(("query", _params["query"]))
+
+        if _params.get("no_page") is not None:  # noqa: E501
+            _query_params.append(("no_page", _params["no_page"]))
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
-
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
             ["application/json"]
         )  # noqa: E501
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            "200": "V1ListActivitiesResponse",
+            "204": "object",
+            "403": "object",
+            "404": "object",
+        }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{team}/members/{user}",
-            "DELETE",
+            "/api/v1/users/history",
+            "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -681,69 +507,101 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def get_team(
+    def get_suggestions(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        offset: Annotated[
+            Optional[StrictInt], Field(description="Pagination offset.")
+        ] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
+        sort: Annotated[
+            Optional[StrictStr], Field(description="Sort to order the search.")
+        ] = None,
+        query: Annotated[
+            Optional[StrictStr], Field(description="Query filter the search.")
+        ] = None,
+        no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
         **kwargs
-    ) -> V1Team:  # noqa: E501
-        """Get team  # noqa: E501
+    ) -> object:  # noqa: E501
+        """User suggestions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_team(owner, name, async_req=True)
+        >>> thread = api.get_suggestions(offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param name: Component under namesapce (required)
-        :type name: str
+        :param offset: Pagination offset.
+        :type offset: int
+        :param limit: Limit size.
+        :type limit: int
+        :param sort: Sort to order the search.
+        :type sort: str
+        :param query: Query filter the search.
+        :type query: str
+        :param no_page: No pagination.
+        :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1Team
+        :rtype: object
         """
         kwargs["_return_http_data_only"] = True
-        return self.get_team_with_http_info(owner, name, **kwargs)  # noqa: E501
+        return self.get_suggestions_with_http_info(
+            offset, limit, sort, query, no_page, **kwargs
+        )  # noqa: E501
 
     @validate_arguments
-    def get_team_with_http_info(
+    def get_suggestions_with_http_info(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[StrictStr, Field(..., description="Component under namesapce")],
+        offset: Annotated[
+            Optional[StrictInt], Field(description="Pagination offset.")
+        ] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
+        sort: Annotated[
+            Optional[StrictStr], Field(description="Sort to order the search.")
+        ] = None,
+        query: Annotated[
+            Optional[StrictStr], Field(description="Query filter the search.")
+        ] = None,
+        no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
         **kwargs
     ):  # noqa: E501
-        """Get team  # noqa: E501
+        """User suggestions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_team_with_http_info(owner, name, async_req=True)
+        >>> thread = api.get_suggestions_with_http_info(offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param name: Component under namesapce (required)
-        :type name: str
+        :param offset: Pagination offset.
+        :type offset: int
+        :param limit: Limit size.
+        :type limit: int
+        :param sort: Sort to order the search.
+        :type sort: str
+        :param query: Query filter the search.
+        :type query: str
+        :param no_page: No pagination.
+        :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -757,20 +615,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1Team, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["owner", "name"]
+        _all_params = ["offset", "limit", "sort", "query", "no_page"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -780,58 +638,65 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_team" % _key
+                    " to method get_suggestions" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["name"]:
-            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
+        if _params.get("offset") is not None:  # noqa: E501
+            _query_params.append(("offset", _params["offset"]))
+
+        if _params.get("limit") is not None:  # noqa: E501
+            _query_params.append(("limit", _params["limit"]))
+
+        if _params.get("sort") is not None:  # noqa: E501
+            _query_params.append(("sort", _params["sort"]))
+
+        if _params.get("query") is not None:  # noqa: E501
+            _query_params.append(("query", _params["query"]))
+
+        if _params.get("no_page") is not None:  # noqa: E501
+            _query_params.append(("no_page", _params["no_page"]))
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
-
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
             ["application/json"]
         )  # noqa: E501
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1Team",
+            "200": "object",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{name}",
+            "/api/v1/users/suggestions",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -842,77 +707,63 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def get_team_member(
+    def get_token(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team under namesapce")],
-        user: Annotated[StrictStr, Field(..., description="Member under team")],
+        uuid: Annotated[StrictStr, Field(..., description="UUid of the namespace")],
         **kwargs
-    ) -> V1TeamMember:  # noqa: E501
-        """Get team member details  # noqa: E501
+    ) -> V1Token:  # noqa: E501
+        """Get token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_team_member(owner, team, user, async_req=True)
+        >>> thread = api.get_token(uuid, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team under namesapce (required)
-        :type team: str
-        :param user: Member under team (required)
-        :type user: str
+        :param uuid: UUid of the namespace (required)
+        :type uuid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1TeamMember
+        :rtype: V1Token
         """
         kwargs["_return_http_data_only"] = True
-        return self.get_team_member_with_http_info(
-            owner, team, user, **kwargs
-        )  # noqa: E501
+        return self.get_token_with_http_info(uuid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_team_member_with_http_info(
+    def get_token_with_http_info(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team under namesapce")],
-        user: Annotated[StrictStr, Field(..., description="Member under team")],
+        uuid: Annotated[StrictStr, Field(..., description="UUid of the namespace")],
         **kwargs
     ):  # noqa: E501
-        """Get team member details  # noqa: E501
+        """Get token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_team_member_with_http_info(owner, team, user, async_req=True)
+        >>> thread = api.get_token_with_http_info(uuid, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team under namesapce (required)
-        :type team: str
-        :param user: Member under team (required)
-        :type user: str
+        :param uuid: UUid of the namespace (required)
+        :type uuid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -926,20 +777,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1TeamMember, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1Token, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["owner", "team", "user"]
+        _all_params = ["uuid"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -949,60 +800,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_team_member" % _key
+                    " to method get_token" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["team"]:
-            _path_params["team"] = _params["team"]
-        if _params["user"]:
-            _path_params["user"] = _params["user"]
+        if _params["uuid"]:
+            _path_params["uuid"] = _params["uuid"]
 
         # process the query parameters
         _query_params = []
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
-
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
             ["application/json"]
         )  # noqa: E501
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1TeamMember",
+            "200": "V1Token",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{team}/members/{user}",
+            "/api/v1/users/tokens/{uuid}",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -1013,137 +856,51 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def list_team_members(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[
-            StrictStr, Field(..., description="Entity managing the resource")
-        ],
-        offset: Annotated[
-            Optional[StrictInt], Field(description="Pagination offset.")
-        ] = None,
-        limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
-        sort: Annotated[
-            Optional[StrictStr], Field(description="Sort to order the search.")
-        ] = None,
-        query: Annotated[
-            Optional[StrictStr], Field(description="Query filter the search.")
-        ] = None,
-        bookmarks: Annotated[
-            Optional[bool], Field(description="Filter by bookmarks.")
-        ] = None,
-        mode: Annotated[
-            Optional[StrictStr], Field(description="Mode of the search.")
-        ] = None,
-        no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
-        **kwargs
-    ) -> V1ListTeamMembersResponse:  # noqa: E501
-        """Get team members  # noqa: E501
+    def get_user(self, **kwargs) -> V1User:  # noqa: E501
+        """Get current user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_team_members(owner, name, offset, limit, sort, query, bookmarks, mode, no_page, async_req=True)
+        >>> thread = api.get_user(async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param name: Entity managing the resource (required)
-        :type name: str
-        :param offset: Pagination offset.
-        :type offset: int
-        :param limit: Limit size.
-        :type limit: int
-        :param sort: Sort to order the search.
-        :type sort: str
-        :param query: Query filter the search.
-        :type query: str
-        :param bookmarks: Filter by bookmarks.
-        :type bookmarks: bool
-        :param mode: Mode of the search.
-        :type mode: str
-        :param no_page: No pagination.
-        :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1ListTeamMembersResponse
+        :rtype: V1User
         """
         kwargs["_return_http_data_only"] = True
-        return self.list_team_members_with_http_info(
-            owner, name, offset, limit, sort, query, bookmarks, mode, no_page, **kwargs
-        )  # noqa: E501
+        return self.get_user_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_team_members_with_http_info(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        name: Annotated[
-            StrictStr, Field(..., description="Entity managing the resource")
-        ],
-        offset: Annotated[
-            Optional[StrictInt], Field(description="Pagination offset.")
-        ] = None,
-        limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
-        sort: Annotated[
-            Optional[StrictStr], Field(description="Sort to order the search.")
-        ] = None,
-        query: Annotated[
-            Optional[StrictStr], Field(description="Query filter the search.")
-        ] = None,
-        bookmarks: Annotated[
-            Optional[bool], Field(description="Filter by bookmarks.")
-        ] = None,
-        mode: Annotated[
-            Optional[StrictStr], Field(description="Mode of the search.")
-        ] = None,
-        no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
-        **kwargs
-    ):  # noqa: E501
-        """Get team members  # noqa: E501
+    def get_user_with_http_info(self, **kwargs):  # noqa: E501
+        """Get current user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_team_members_with_http_info(owner, name, offset, limit, sort, query, bookmarks, mode, no_page, async_req=True)
+        >>> thread = api.get_user_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param name: Entity managing the resource (required)
-        :type name: str
-        :param offset: Pagination offset.
-        :type offset: int
-        :param limit: Limit size.
-        :type limit: int
-        :param sort: Sort to order the search.
-        :type sort: str
-        :param query: Query filter the search.
-        :type query: str
-        :param bookmarks: Filter by bookmarks.
-        :type bookmarks: bool
-        :param mode: Mode of the search.
-        :type mode: str
-        :param no_page: No pagination.
-        :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1157,30 +914,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1ListTeamMembersResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1User, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = [
-            "owner",
-            "name",
-            "offset",
-            "limit",
-            "sort",
-            "query",
-            "bookmarks",
-            "mode",
-            "no_page",
-        ]
+        _all_params = []
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -1190,72 +937,50 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_team_members" % _key
+                    " to method get_user" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["name"]:
-            _path_params["name"] = _params["name"]
 
         # process the query parameters
         _query_params = []
-        if _params.get("offset") is not None:  # noqa: E501
-            _query_params.append(("offset", _params["offset"]))
-        if _params.get("limit") is not None:  # noqa: E501
-            _query_params.append(("limit", _params["limit"]))
-        if _params.get("sort") is not None:  # noqa: E501
-            _query_params.append(("sort", _params["sort"]))
-        if _params.get("query") is not None:  # noqa: E501
-            _query_params.append(("query", _params["query"]))
-        if _params.get("bookmarks") is not None:  # noqa: E501
-            _query_params.append(("bookmarks", _params["bookmarks"]))
-        if _params.get("mode") is not None:  # noqa: E501
-            _query_params.append(("mode", _params["mode"]))
-        if _params.get("no_page") is not None:  # noqa: E501
-            _query_params.append(("no_page", _params["no_page"]))
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
-
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
             ["application/json"]
         )  # noqa: E501
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1ListTeamMembersResponse",
+            "200": "V1User",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{name}/members",
+            "/api/v1/users",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -1266,58 +991,45 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def list_team_names(
+    def get_workspaces(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
             Optional[StrictStr], Field(description="Sort to order the search.")
         ] = None,
         query: Annotated[
             Optional[StrictStr], Field(description="Query filter the search.")
         ] = None,
-        bookmarks: Annotated[
-            Optional[bool], Field(description="Filter by bookmarks.")
-        ] = None,
-        mode: Annotated[
-            Optional[StrictStr], Field(description="Mode of the search.")
-        ] = None,
         no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
         **kwargs
-    ) -> V1ListTeamsResponse:  # noqa: E501
-        """List teams names  # noqa: E501
+    ) -> object:  # noqa: E501
+        """User workspaces  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_team_names(owner, offset, limit, sort, query, bookmarks, mode, no_page, async_req=True)
+        >>> thread = api.get_workspaces(offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
         :param sort: Sort to order the search.
         :type sort: str
         :param query: Query filter the search.
         :type query: str
-        :param bookmarks: Filter by bookmarks.
-        :type bookmarks: bool
-        :param mode: Mode of the search.
-        :type mode: str
         :param no_page: No pagination.
         :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1325,66 +1037,53 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1ListTeamsResponse
+        :rtype: object
         """
         kwargs["_return_http_data_only"] = True
-        return self.list_team_names_with_http_info(
-            owner, offset, limit, sort, query, bookmarks, mode, no_page, **kwargs
+        return self.get_workspaces_with_http_info(
+            offset, limit, sort, query, no_page, **kwargs
         )  # noqa: E501
 
     @validate_arguments
-    def list_team_names_with_http_info(
+    def get_workspaces_with_http_info(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
             Optional[StrictStr], Field(description="Sort to order the search.")
         ] = None,
         query: Annotated[
             Optional[StrictStr], Field(description="Query filter the search.")
         ] = None,
-        bookmarks: Annotated[
-            Optional[bool], Field(description="Filter by bookmarks.")
-        ] = None,
-        mode: Annotated[
-            Optional[StrictStr], Field(description="Mode of the search.")
-        ] = None,
         no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
         **kwargs
     ):  # noqa: E501
-        """List teams names  # noqa: E501
+        """User workspaces  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_team_names_with_http_info(owner, offset, limit, sort, query, bookmarks, mode, no_page, async_req=True)
+        >>> thread = api.get_workspaces_with_http_info(offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
         :param sort: Sort to order the search.
         :type sort: str
         :param query: Query filter the search.
         :type query: str
-        :param bookmarks: Filter by bookmarks.
-        :type bookmarks: bool
-        :param mode: Mode of the search.
-        :type mode: str
         :param no_page: No pagination.
         :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1400,29 +1099,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1ListTeamsResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = [
-            "owner",
-            "offset",
-            "limit",
-            "sort",
-            "query",
-            "bookmarks",
-            "mode",
-            "no_page",
-        ]
+        _all_params = ["offset", "limit", "sort", "query", "no_page"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -1432,70 +1122,65 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_team_names" % _key
+                    " to method get_workspaces" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
 
         # process the query parameters
         _query_params = []
         if _params.get("offset") is not None:  # noqa: E501
             _query_params.append(("offset", _params["offset"]))
+
         if _params.get("limit") is not None:  # noqa: E501
             _query_params.append(("limit", _params["limit"]))
+
         if _params.get("sort") is not None:  # noqa: E501
             _query_params.append(("sort", _params["sort"]))
+
         if _params.get("query") is not None:  # noqa: E501
             _query_params.append(("query", _params["query"]))
-        if _params.get("bookmarks") is not None:  # noqa: E501
-            _query_params.append(("bookmarks", _params["bookmarks"]))
-        if _params.get("mode") is not None:  # noqa: E501
-            _query_params.append(("mode", _params["mode"]))
+
         if _params.get("no_page") is not None:  # noqa: E501
             _query_params.append(("no_page", _params["no_page"]))
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
-
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
             ["application/json"]
         )  # noqa: E501
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1ListTeamsResponse",
+            "200": "object",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/names",
+            "/api/v1/users/workspaces",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -1506,58 +1191,45 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def list_teams(
+    def list_tokens(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
             Optional[StrictStr], Field(description="Sort to order the search.")
         ] = None,
         query: Annotated[
             Optional[StrictStr], Field(description="Query filter the search.")
         ] = None,
-        bookmarks: Annotated[
-            Optional[bool], Field(description="Filter by bookmarks.")
-        ] = None,
-        mode: Annotated[
-            Optional[StrictStr], Field(description="Mode of the search.")
-        ] = None,
         no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
         **kwargs
-    ) -> V1ListTeamsResponse:  # noqa: E501
-        """List teams  # noqa: E501
+    ) -> V1ListTokenResponse:  # noqa: E501
+        """List tokens  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_teams(owner, offset, limit, sort, query, bookmarks, mode, no_page, async_req=True)
+        >>> thread = api.list_tokens(offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
         :param sort: Sort to order the search.
         :type sort: str
         :param query: Query filter the search.
         :type query: str
-        :param bookmarks: Filter by bookmarks.
-        :type bookmarks: bool
-        :param mode: Mode of the search.
-        :type mode: str
         :param no_page: No pagination.
         :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1565,66 +1237,53 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1ListTeamsResponse
+        :rtype: V1ListTokenResponse
         """
         kwargs["_return_http_data_only"] = True
-        return self.list_teams_with_http_info(
-            owner, offset, limit, sort, query, bookmarks, mode, no_page, **kwargs
+        return self.list_tokens_with_http_info(
+            offset, limit, sort, query, no_page, **kwargs
         )  # noqa: E501
 
     @validate_arguments
-    def list_teams_with_http_info(
+    def list_tokens_with_http_info(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
         offset: Annotated[
             Optional[StrictInt], Field(description="Pagination offset.")
         ] = None,
         limit: Annotated[Optional[StrictInt], Field(description="Limit size.")] = None,
         sort: Annotated[
             Optional[StrictStr], Field(description="Sort to order the search.")
         ] = None,
         query: Annotated[
             Optional[StrictStr], Field(description="Query filter the search.")
         ] = None,
-        bookmarks: Annotated[
-            Optional[bool], Field(description="Filter by bookmarks.")
-        ] = None,
-        mode: Annotated[
-            Optional[StrictStr], Field(description="Mode of the search.")
-        ] = None,
         no_page: Annotated[Optional[bool], Field(description="No pagination.")] = None,
         **kwargs
     ):  # noqa: E501
-        """List teams  # noqa: E501
+        """List tokens  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_teams_with_http_info(owner, offset, limit, sort, query, bookmarks, mode, no_page, async_req=True)
+        >>> thread = api.list_tokens_with_http_info(offset, limit, sort, query, no_page, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
         :param offset: Pagination offset.
         :type offset: int
         :param limit: Limit size.
         :type limit: int
         :param sort: Sort to order the search.
         :type sort: str
         :param query: Query filter the search.
         :type query: str
-        :param bookmarks: Filter by bookmarks.
-        :type bookmarks: bool
-        :param mode: Mode of the search.
-        :type mode: str
         :param no_page: No pagination.
         :type no_page: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1640,29 +1299,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1ListTeamsResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1ListTokenResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = [
-            "owner",
-            "offset",
-            "limit",
-            "sort",
-            "query",
-            "bookmarks",
-            "mode",
-            "no_page",
-        ]
+        _all_params = ["offset", "limit", "sort", "query", "no_page"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -1672,70 +1322,65 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_teams" % _key
+                    " to method list_tokens" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
 
         # process the query parameters
         _query_params = []
         if _params.get("offset") is not None:  # noqa: E501
             _query_params.append(("offset", _params["offset"]))
+
         if _params.get("limit") is not None:  # noqa: E501
             _query_params.append(("limit", _params["limit"]))
+
         if _params.get("sort") is not None:  # noqa: E501
             _query_params.append(("sort", _params["sort"]))
+
         if _params.get("query") is not None:  # noqa: E501
             _query_params.append(("query", _params["query"]))
-        if _params.get("bookmarks") is not None:  # noqa: E501
-            _query_params.append(("bookmarks", _params["bookmarks"]))
-        if _params.get("mode") is not None:  # noqa: E501
-            _query_params.append(("mode", _params["mode"]))
+
         if _params.get("no_page") is not None:  # noqa: E501
             _query_params.append(("no_page", _params["no_page"]))
 
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
-
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
             ["application/json"]
         )  # noqa: E501
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1ListTeamsResponse",
+            "200": "V1ListTokenResponse",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams",
+            "/api/v1/users/tokens",
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -1746,77 +1391,69 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def patch_team(
+    def patch_token(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team_name: Annotated[StrictStr, Field(..., description="Name")],
-        body: Annotated[V1Team, Field(..., description="Team body")],
+        token_uuid: Annotated[StrictStr, Field(..., description="UUID")],
+        body: Annotated[V1Token, Field(..., description="Token body")],
         **kwargs
-    ) -> V1Team:  # noqa: E501
-        """Patch team  # noqa: E501
+    ) -> V1Token:  # noqa: E501
+        """Patch token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.patch_team(owner, team_name, body, async_req=True)
+        >>> thread = api.patch_token(token_uuid, body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team_name: Name (required)
-        :type team_name: str
-        :param body: Team body (required)
-        :type body: V1Team
+        :param token_uuid: UUID (required)
+        :type token_uuid: str
+        :param body: Token body (required)
+        :type body: V1Token
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1Team
+        :rtype: V1Token
         """
         kwargs["_return_http_data_only"] = True
-        return self.patch_team_with_http_info(
-            owner, team_name, body, **kwargs
-        )  # noqa: E501
+        return self.patch_token_with_http_info(token_uuid, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def patch_team_with_http_info(
+    def patch_token_with_http_info(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team_name: Annotated[StrictStr, Field(..., description="Name")],
-        body: Annotated[V1Team, Field(..., description="Team body")],
+        token_uuid: Annotated[StrictStr, Field(..., description="UUID")],
+        body: Annotated[V1Token, Field(..., description="Token body")],
         **kwargs
     ):  # noqa: E501
-        """Patch team  # noqa: E501
+        """Patch token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.patch_team_with_http_info(owner, team_name, body, async_req=True)
+        >>> thread = api.patch_token_with_http_info(token_uuid, body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team_name: Name (required)
-        :type team_name: str
-        :param body: Team body (required)
-        :type body: V1Team
+        :param token_uuid: UUID (required)
+        :type token_uuid: str
+        :param body: Token body (required)
+        :type body: V1Token
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1830,20 +1467,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1Team, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1Token, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["owner", "team_name", "body"]
+        _all_params = ["token_uuid", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -1853,38 +1490,33 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method patch_team" % _key
+                    " to method patch_token" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["team_name"]:
-            _path_params["team.name"] = _params["team_name"]
+        if _params["token_uuid"]:
+            _path_params["token.uuid"] = _params["token_uuid"]
 
         # process the query parameters
         _query_params = []
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
         if _params["body"]:
             _body_params = _params["body"]
 
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
@@ -1899,22 +1531,22 @@
         if _content_types_list:
             _header_params["Content-Type"] = _content_types_list
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1Team",
+            "200": "V1Token",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{team.name}",
+            "/api/v1/users/tokens/{token.uuid}",
             "PATCH",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -1925,83 +1557,55 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def patch_team_member(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team")],
-        member_user: Annotated[StrictStr, Field(..., description="User")],
-        body: Annotated[V1TeamMember, Field(..., description="Team body")],
-        **kwargs
-    ) -> V1TeamMember:  # noqa: E501
-        """Patch team member  # noqa: E501
+    def patch_user(self, body: V1User, **kwargs) -> V1User:  # noqa: E501
+        """Patch current user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.patch_team_member(owner, team, member_user, body, async_req=True)
+        >>> thread = api.patch_user(body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team (required)
-        :type team: str
-        :param member_user: User (required)
-        :type member_user: str
-        :param body: Team body (required)
-        :type body: V1TeamMember
+        :param body: (required)
+        :type body: V1User
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1TeamMember
+        :rtype: V1User
         """
         kwargs["_return_http_data_only"] = True
-        return self.patch_team_member_with_http_info(
-            owner, team, member_user, body, **kwargs
-        )  # noqa: E501
+        return self.patch_user_with_http_info(body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def patch_team_member_with_http_info(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team")],
-        member_user: Annotated[StrictStr, Field(..., description="User")],
-        body: Annotated[V1TeamMember, Field(..., description="Team body")],
-        **kwargs
-    ):  # noqa: E501
-        """Patch team member  # noqa: E501
+    def patch_user_with_http_info(self, body: V1User, **kwargs):  # noqa: E501
+        """Patch current user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.patch_team_member_with_http_info(owner, team, member_user, body, async_req=True)
+        >>> thread = api.patch_user_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team (required)
-        :type team: str
-        :param member_user: User (required)
-        :type member_user: str
-        :param body: Team body (required)
-        :type body: V1TeamMember
+        :param body: (required)
+        :type body: V1User
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2015,20 +1619,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1TeamMember, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1User, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["owner", "team", "member_user", "body"]
+        _all_params = ["body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -2038,40 +1642,31 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method patch_team_member" % _key
+                    " to method patch_user" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["team"]:
-            _path_params["team"] = _params["team"]
-        if _params["member_user"]:
-            _path_params["member.user"] = _params["member_user"]
 
         # process the query parameters
         _query_params = []
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
         if _params["body"]:
             _body_params = _params["body"]
 
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
@@ -2086,22 +1681,22 @@
         if _content_types_list:
             _header_params["Content-Type"] = _content_types_list
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1TeamMember",
+            "200": "V1User",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{team}/members/{member.user}",
+            "/api/v1/users",
             "PATCH",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -2112,77 +1707,71 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def update_team(
+    def update_token(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team_name: Annotated[StrictStr, Field(..., description="Name")],
-        body: Annotated[V1Team, Field(..., description="Team body")],
+        token_uuid: Annotated[StrictStr, Field(..., description="UUID")],
+        body: Annotated[V1Token, Field(..., description="Token body")],
         **kwargs
-    ) -> V1Team:  # noqa: E501
-        """Update team  # noqa: E501
+    ) -> V1Token:  # noqa: E501
+        """Update token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_team(owner, team_name, body, async_req=True)
+        >>> thread = api.update_token(token_uuid, body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team_name: Name (required)
-        :type team_name: str
-        :param body: Team body (required)
-        :type body: V1Team
+        :param token_uuid: UUID (required)
+        :type token_uuid: str
+        :param body: Token body (required)
+        :type body: V1Token
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1Team
+        :rtype: V1Token
         """
         kwargs["_return_http_data_only"] = True
-        return self.update_team_with_http_info(
-            owner, team_name, body, **kwargs
+        return self.update_token_with_http_info(
+            token_uuid, body, **kwargs
         )  # noqa: E501
 
     @validate_arguments
-    def update_team_with_http_info(
+    def update_token_with_http_info(
         self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team_name: Annotated[StrictStr, Field(..., description="Name")],
-        body: Annotated[V1Team, Field(..., description="Team body")],
+        token_uuid: Annotated[StrictStr, Field(..., description="UUID")],
+        body: Annotated[V1Token, Field(..., description="Token body")],
         **kwargs
     ):  # noqa: E501
-        """Update team  # noqa: E501
+        """Update token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_team_with_http_info(owner, team_name, body, async_req=True)
+        >>> thread = api.update_token_with_http_info(token_uuid, body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team_name: Name (required)
-        :type team_name: str
-        :param body: Team body (required)
-        :type body: V1Team
+        :param token_uuid: UUID (required)
+        :type token_uuid: str
+        :param body: Token body (required)
+        :type body: V1Token
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2196,20 +1785,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1Team, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1Token, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["owner", "team_name", "body"]
+        _all_params = ["token_uuid", "body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -2219,38 +1808,33 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_team" % _key
+                    " to method update_token" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["team_name"]:
-            _path_params["team.name"] = _params["team_name"]
+        if _params["token_uuid"]:
+            _path_params["token.uuid"] = _params["token_uuid"]
 
         # process the query parameters
         _query_params = []
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
         if _params["body"]:
             _body_params = _params["body"]
 
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
@@ -2265,22 +1849,22 @@
         if _content_types_list:
             _header_params["Content-Type"] = _content_types_list
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1Team",
+            "200": "V1Token",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{team.name}",
+            "/api/v1/users/tokens/{token.uuid}",
             "PUT",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -2291,83 +1875,55 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def update_team_member(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team")],
-        member_user: Annotated[StrictStr, Field(..., description="User")],
-        body: Annotated[V1TeamMember, Field(..., description="Team body")],
-        **kwargs
-    ) -> V1TeamMember:  # noqa: E501
-        """Update team member  # noqa: E501
+    def update_user(self, body: V1User, **kwargs) -> V1User:  # noqa: E501
+        """Update current user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_team_member(owner, team, member_user, body, async_req=True)
+        >>> thread = api.update_user(body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team (required)
-        :type team: str
-        :param member_user: User (required)
-        :type member_user: str
-        :param body: Team body (required)
-        :type body: V1TeamMember
+        :param body: (required)
+        :type body: V1User
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1TeamMember
+        :rtype: V1User
         """
         kwargs["_return_http_data_only"] = True
-        return self.update_team_member_with_http_info(
-            owner, team, member_user, body, **kwargs
-        )  # noqa: E501
+        return self.update_user_with_http_info(body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_team_member_with_http_info(
-        self,
-        owner: Annotated[StrictStr, Field(..., description="Owner of the namespace")],
-        team: Annotated[StrictStr, Field(..., description="Team")],
-        member_user: Annotated[StrictStr, Field(..., description="User")],
-        body: Annotated[V1TeamMember, Field(..., description="Team body")],
-        **kwargs
-    ):  # noqa: E501
-        """Update team member  # noqa: E501
+    def update_user_with_http_info(self, body: V1User, **kwargs):  # noqa: E501
+        """Update current user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_team_member_with_http_info(owner, team, member_user, body, async_req=True)
+        >>> thread = api.update_user_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team (required)
-        :type team: str
-        :param member_user: User (required)
-        :type member_user: str
-        :param body: Team body (required)
-        :type body: V1TeamMember
+        :param body: (required)
+        :type body: V1User
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2381,20 +1937,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1TeamMember, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1User, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["owner", "team", "member_user", "body"]
+        _all_params = ["body"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -2404,40 +1960,31 @@
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_team_member" % _key
+                    " to method update_user" % _key
                 )
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["owner"]:
-            _path_params["owner"] = _params["owner"]
-        if _params["team"]:
-            _path_params["team"] = _params["team"]
-        if _params["member_user"]:
-            _path_params["member.user"] = _params["member_user"]
 
         # process the query parameters
         _query_params = []
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
-
         # process the form parameters
         _form_params = []
         _files = {}
-
         # process the body parameter
         _body_params = None
         if _params["body"]:
             _body_params = _params["body"]
 
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(
@@ -2452,22 +1999,22 @@
         if _content_types_list:
             _header_params["Content-Type"] = _content_types_list
 
         # authentication setting
         _auth_settings = ["ApiKey"]  # noqa: E501
 
         _response_types_map = {
-            "200": "V1TeamMember",
+            "200": "V1User",
             "204": "object",
             "403": "object",
             "404": "object",
         }
 
         return self.api_client.call_api(
-            "/api/v1/orgs/{owner}/teams/{team}/members/{member.user}",
+            "/api/v1/users",
             "PUT",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
```

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/api/versions_v1_api.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/api/versions_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/async_client/api_client.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/async_client/api_client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/async_client/rest.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/async_client/rest.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/configuration.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_activity.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_activity.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_agent.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_connection_response.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_connection_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_dashboard.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_dashboard.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_entity_notification_body.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_entity_notification_body.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_operation_body.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_operation_body.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_organization.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_organization.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_preset.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_preset.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_project.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_project.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_project_settings.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_project_settings.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_project_version.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_project_version.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_queue.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_queue.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_run_settings.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_run_settings.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_search.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_search.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_search_spec.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_search_spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_section_spec.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_section_spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_service_account.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_service_account.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_team.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_team.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from clipped.types.uuids import UUIDStr
 
 from polyaxon._sdk.schemas.v1_team_settings import V1TeamSettings
 
 
 class V1Team(BaseAllowSchemaModel):
     uuid: Optional[UUIDStr]
+    owner: Optional[StrictStr]
     name: Optional[StrictStr]
     projects: Optional[List[StrictStr]]
     component_hubs: Optional[List[StrictStr]]
     model_registries: Optional[List[StrictStr]]
     settings: Optional[V1TeamSettings]
+    role: Optional[StrictStr]
     created_at: Optional[datetime.datetime]
     updated_at: Optional[datetime.datetime]
```

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/schemas/v1_token.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/schemas/v1_token.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/sync_client/api_client.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/sync_client/api_client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sdk/sync_client/rest.py` & `polyaxon-2.2.0rc0/polyaxon/_sdk/sync_client/rest.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_services/headers.py` & `polyaxon-2.2.0rc0/polyaxon/_services/headers.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_services/values.py` & `polyaxon-2.2.0rc0/polyaxon/_services/values.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sidecar/container/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_sidecar/container/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sidecar/container/monitors/artifacts.py` & `polyaxon-2.2.0rc0/polyaxon/_sidecar/container/monitors/artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sidecar/container/monitors/logs.py` & `polyaxon-2.2.0rc0/polyaxon/_sidecar/container/monitors/logs.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sidecar/container/monitors/spec.py` & `polyaxon-2.2.0rc0/polyaxon/_sidecar/container/monitors/spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_sidecar/processor.py` & `polyaxon-2.2.0rc0/polyaxon/_sidecar/processor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/cache.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/cache.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/cli_constants.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/cli_constants.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/__init__.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/backfill.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/backfill.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/bo.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/bo.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/grid.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/grid.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/jobs.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/jobs.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/mapping.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/mapping.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/pipelines.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/pipelines.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/schedule.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/schedule.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fixtures/services.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fixtures/services.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/formatting.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/fqn_utils.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/fqn_utils.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/test_utils.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_utils/urls_utils.py` & `polyaxon-2.2.0rc0/polyaxon/_utils/urls_utils.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/_vendor/shell_pty.py` & `polyaxon-2.2.0rc0/polyaxon/_vendor/shell_pty.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/api.py` & `polyaxon-2.2.0rc0/polyaxon/api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/cli.py` & `polyaxon-2.2.0rc0/polyaxon/cli.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/client.py` & `polyaxon-2.2.0rc0/polyaxon/client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/exceptions.py` & `polyaxon-2.2.0rc0/polyaxon/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/k8s.py` & `polyaxon-2.2.0rc0/polyaxon/k8s.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/logger.py` & `polyaxon-2.2.0rc0/polyaxon/logger.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/schemas.py` & `polyaxon-2.2.0rc0/polyaxon/schemas.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/settings.py` & `polyaxon-2.2.0rc0/polyaxon/settings.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon/types.py` & `polyaxon-2.2.0rc0/polyaxon/types.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/polyaxon.egg-info/PKG-INFO` & `polyaxon-2.2.0rc0/polyaxon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyaxon
-Version: 2.1.8
+Version: 2.2.0rc0
 Summary: Command Line Interface (CLI) and client to interact with Polyaxon API.
 Home-page: https://github.com/polyaxon/polyaxon
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
@@ -47,15 +47,15 @@
 Provides-Extra: sandbox
 
 [![License: Apache 2](https://img.shields.io/badge/License-apache2-blue.svg?style=flat&longCache=true)](LICENSE)
 [![Polyaxon API](https://img.shields.io/docker/pulls/polyaxon/polyaxon-api)](https://hub.docker.com/r/polyaxon/polyaxon-api)
 [![Slack](https://img.shields.io/badge/Slack-1.5k%20members-blue.svg?style=flat&logo=slack&longCache=true)](https://polyaxon.com/slack/)
 
 [![Docs](https://img.shields.io/badge/docs-stable-brightgreen.svg?style=flat&longCache=true)](https://polyaxon.com/docs/)
-[![Release](https://img.shields.io/badge/release-v2.1.8-brightgreen.svg?longCache=true)](https://polyaxon.com/docs/releases/2-1/)
+[![Release](https://img.shields.io/badge/release-v2.2.0-brightgreen.svg?longCache=true)](https://polyaxon.com/docs/releases/2-1/)
 [![GitHub](https://img.shields.io/badge/issue_tracker-github-blue?style=flat&logo=github&longCache=true)](https://github.com/polyaxon/polyaxon/issues)
 [![GitHub](https://img.shields.io/badge/roadmap-github-blue?style=flat&logo=github&longCache=true)](https://github.com/orgs/polyaxon/projects/5)
 
 [![CLI](https://github.com/polyaxon/cli/actions/workflows/cli.yml/badge.svg)](https://github.com/polyaxon/cli/actions/workflows/cli.yml)
 [![Polyaxon](https://github.com/polyaxon/polyaxon/actions/workflows/cli.yml/badge.svg)](https://github.com/polyaxon/polyaxon/actions/workflows/cli.yml)
 [![Haupt](https://github.com/polyaxon/polyaxon/actions/workflows/haupt.yml/badge.svg)](https://github.com/polyaxon/polyaxon/actions/workflows/haupt.yml)
 [![Hypertune](https://github.com/polyaxon/polyaxon/actions/workflows/hypertune.yml/badge.svg)](https://github.com/polyaxon/polyaxon/actions/workflows/hypertune.yml)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polyaxon Version: 2.1.8 Summary: Command Line
+Metadata-Version: 2.1 Name: polyaxon Version: 2.2.0rc0 Summary: Command Line
 Interface (CLI) and client to interact with Polyaxon API. Home-page: https://
 github.com/polyaxon/polyaxon Author: Polyaxon, Inc. Author-email:
 contact@polyaxon.com Maintainer: Polyaxon, Inc. Maintainer-email:
 contact@polyaxon.com License: Apache 2.0 Keywords:
 polyaxon,aws,s3,microsoft,azure,google cloud storage,gcs,deep-learning,machine-
 learning,data-science,neural-networks,artificial-intelligence,ai,reinforcement-
 learning,kubernetes,aws,microsoft,azure,google cloud,tensorFlow,pytorch
@@ -28,15 +28,15 @@
 img.shields.io/badge/License-apache2-blue.svg?style=flat&longCache=true)]
 (LICENSE) [![Polyaxon API](https://img.shields.io/docker/pulls/polyaxon/
 polyaxon-api)](https://hub.docker.com/r/polyaxon/polyaxon-api) [![Slack](https:
 //img.shields.io/badge/Slack-1.5k%20members-
 blue.svg?style=flat&logo=slack&longCache=true)](https://polyaxon.com/slack/) [!
 [Docs](https://img.shields.io/badge/docs-stable-
 brightgreen.svg?style=flat&longCache=true)](https://polyaxon.com/docs/) [!
-[Release](https://img.shields.io/badge/release-v2.1.8-
+[Release](https://img.shields.io/badge/release-v2.2.0-
 brightgreen.svg?longCache=true)](https://polyaxon.com/docs/releases/2-1/) [!
 [GitHub](https://img.shields.io/badge/issue_tracker-github-
 blue?style=flat&logo=github&longCache=true)](https://github.com/polyaxon/
 polyaxon/issues) [![GitHub](https://img.shields.io/badge/roadmap-github-
 blue?style=flat&logo=github&longCache=true)](https://github.com/orgs/polyaxon/
 projects/5) [![CLI](https://github.com/polyaxon/cli/actions/workflows/cli.yml/
 badge.svg)](https://github.com/polyaxon/cli/actions/workflows/cli.yml) [!
```

### Comparing `polyaxon-2.1.8/polyaxon.egg-info/SOURCES.txt` & `polyaxon-2.2.0rc0/polyaxon.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -356,14 +356,30 @@
 polyaxon/_k8s/logging/__init__.py
 polyaxon/_k8s/logging/async_monitor.py
 polyaxon/_k8s/logging/monitor.py
 polyaxon/_k8s/manager/__init__.py
 polyaxon/_k8s/manager/async_manager.py
 polyaxon/_k8s/manager/base.py
 polyaxon/_k8s/manager/manager.py
+polyaxon/_local_process/__init__.py
+polyaxon/_local_process/agent.py
+polyaxon/_local_process/executor.py
+polyaxon/_local_process/process_types.py
+polyaxon/_local_process/converter/__init__.py
+polyaxon/_local_process/converter/mixins.py
+polyaxon/_local_process/converter/base/__init__.py
+polyaxon/_local_process/converter/base/base.py
+polyaxon/_local_process/converter/base/containers.py
+polyaxon/_local_process/converter/base/env_vars.py
+polyaxon/_local_process/converter/base/init.py
+polyaxon/_local_process/converter/base/main.py
+polyaxon/_local_process/converter/base/mounts.py
+polyaxon/_local_process/converter/converters/__init__.py
+polyaxon/_local_process/converter/converters/job.py
+polyaxon/_local_process/converter/converters/service.py
 polyaxon/_managers/__init__.py
 polyaxon/_managers/agent.py
 polyaxon/_managers/auth.py
 polyaxon/_managers/cli.py
 polyaxon/_managers/client.py
 polyaxon/_managers/compose.py
 polyaxon/_managers/deploy.py
```

### Comparing `polyaxon-2.1.8/polyaxon.egg-info/requires.txt` & `polyaxon-2.2.0rc0/polyaxon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/setup.cfg` & `polyaxon-2.2.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `polyaxon-2.1.8/setup.py` & `polyaxon-2.2.0rc0/setup.py`

 * *Files identical despite different names*

