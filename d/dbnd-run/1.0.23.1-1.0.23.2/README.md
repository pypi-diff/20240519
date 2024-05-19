# Comparing `tmp/dbnd-run-1.0.23.1.tar.gz` & `tmp/dbnd-run-1.0.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-run-1.0.23.1.tar", last modified: Thu May 16 10:18:01 2024, max compression
+gzip compressed data, was "dbnd-run-1.0.23.2.tar", last modified: Sun May 19 17:24:57 2024, max compression
```

## Comparing `dbnd-run-1.0.23.1.tar` & `dbnd-run-1.0.23.2.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.461700 dbnd-run-1.0.23.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5514 2024-05-16 10:18:01.461700 dbnd-run-1.0.23.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4056 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2125 2024-05-16 10:18:01.464701 dbnd-run-1.0.23.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.423697 dbnd-run-1.0.23.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.429698 dbnd-run-1.0.23.1/src/databand/
--rwxrwxrwx   0 root         (0) root         (0)     1087 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/databand/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/databand/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/databand/commands.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/databand/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     2181 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/databand/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.429698 dbnd-run-1.0.23.1/src/databand/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/databand/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.429698 dbnd-run-1.0.23.1/src/databand/tasks/basics/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/databand/tasks/basics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.429698 dbnd-run-1.0.23.1/src/dbnd_run/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.431698 dbnd-run-1.0.23.1/src/dbnd_run/_vendor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:17:48.000000 dbnd-run-1.0.23.1/src/dbnd_run/_vendor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4690 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/_vendor/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/_vendor/kubernetes_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.432698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.433698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_extensions/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_extensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_extensions/dal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.433698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:17:48.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.434698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:17:48.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/airflow_windows_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/getuser.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/timeout.py
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.435698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/
--rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/airflow_multi_version_shim.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/cli_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/dbnd_task_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/kubernetes_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3768 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/config.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/db_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.437698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/README.md
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_aws.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_azure.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_gcp.py
--rw-rw-rw-   0 root         (0) root         (0)     3673 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/dbnd_airflow_default_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3128 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/dbnd_operator.py
--rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/docker_operator.py
--rw-rw-rw-   0 root         (0) root         (0)     2706 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/kubernetes_metrics_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/mng_connections.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/safe_hostname_name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.437698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2500 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/utils/system_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.438698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2512 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/airflow_operator_as_dbnd.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/airflow_operators_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/converters.py
--rw-rw-rw-   0 root         (0) root         (0)     5920 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/dbnd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)    19192 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/dbnd_task_executor_via_airflow.py
--rw-rw-rw-   0 root         (0) root         (0)     1821 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/dbnd_task_to_airflow_operator.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/optimized_trigger_rule_dep.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/task_instance_state_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.439699 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.440698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8415 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7636 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_runtime_zombies_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    31748 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    11937 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_watcher.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     8224 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/simple_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.440698 dbnd-run-1.0.23.1/src/dbnd_run/airflow/functional/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.441699 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/dbnd_airflow_webserver_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/dbnd_airflow_webserver_plugin_linkable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.441699 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/loadable_plugins/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/loadable_plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.441699 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/loadable_plugins/patched_versioned_bag/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/loadable_plugins/patched_versioned_bag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/loadable_plugins/patched_versioned_bag/dbnd_versioned_dagbag_autoload.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/setup_plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.443699 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dagrun_zombies.py
--rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dagrun_zombies_clean_job.py
--rw-rw-rw-   0 root         (0) root         (0)     4587 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dags_provider_from_databand.py
--rw-rw-rw-   0 root         (0) root         (0)     8920 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dags_provider_from_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dbnd_cmd_operators.py
--rw-rw-rw-   0 root         (0) root         (0)     3503 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/scheduler_dags_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    42534 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/single_dag_run_job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.443699 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2879 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/utils/generate_partitioned_dags.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/utils/partitioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.444699 dbnd-run-1.0.23.1/src/dbnd_run/airflow/testing/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/testing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/testing/testing_shims.py
--rw-rw-rw-   0 root         (0) root         (0)     2119 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/testing/unittest_env.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.445699 dbnd-run-1.0.23.1/src/dbnd_run/airflow/web/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3807 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/web/airflow_app_with_versioned_dagbag.py
--rw-rw-rw-   0 root         (0) root         (0)     6488 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/web/databand_versioned_dagbag.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/airflow/web/single_job_run_support.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.447699 dbnd-run-1.0.23.1/src/dbnd_run/cli/
--rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4347 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_heartbeat.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_project.py
--rw-rw-rw-   0 root         (0) root         (0)    14658 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_run.py
--rw-rw-rw-   0 root         (0) root         (0)     6204 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_scheduler_management.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_show.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6020 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/service_auto_completer.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.448699 dbnd-run-1.0.23.1/src/dbnd_run/conf/
--rw-rw-rw-   0 root         (0) root         (0)     3475 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/conf/dbnd-run.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/conf/kubernetes-pod-tensorflow.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/conf/kubernetes-pod.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.448699 dbnd-run-1.0.23.1/src/dbnd_run/conf/project_init/
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/conf/project_init/project.cfg
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/current.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.449699 dbnd-run-1.0.23.1/src/dbnd_run/errors/
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/errors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/errors/execute_engine.py
--rw-rw-rw-   0 root         (0) root         (0)     3973 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/errors/executor_k8s.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/errors/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     4970 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/errors/task_execution.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/errors/versioned_dagbag.py
--rw-rw-rw-   0 root         (0) root         (0)     3243 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/orchestration_bootstrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.449699 dbnd-run-1.0.23.1/src/dbnd_run/orchestration_tracking/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/orchestration_tracking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.450699 dbnd-run-1.0.23.1/src/dbnd_run/orchestration_tracking/backends/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/orchestration_tracking/backends/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9456 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/orchestration_tracking/backends/tracking_store_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.450699 dbnd-run-1.0.23.1/src/dbnd_run/plugin/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/plugin/dbnd_plugin_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/plugin/dbnd_plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.451700 dbnd-run-1.0.23.1/src/dbnd_run/run_executor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_executor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5339 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_executor/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5670 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_executor/heartbeat_sender.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_executor/results_view.py
--rw-rw-rw-   0 root         (0) root         (0)    35172 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_executor/run_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7496 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_executor/task_runs_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.452700 dbnd-run-1.0.23.1/src/dbnd_run/run_executor_engine/
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_executor_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5295 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_executor_engine/local_task_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.453700 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/
--rw-rw-rw-   0 root         (0) root         (0)     3776 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      727 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/describe.py
--rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/engine.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/env.py
--rw-rw-rw-   0 root         (0) root         (0)     1623 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/git.py
--rw-rw-rw-   0 root         (0) root         (0)    13117 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/log.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/output.py
--rw-rw-rw-   0 root         (0) root         (0)     8176 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/run.py
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/run_settings/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.455700 dbnd-run-1.0.23.1/src/dbnd_run/task/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task/data_source_task.py
--rw-rw-rw-   0 root         (0) root         (0)     9452 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task/decorated_callable_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task/pipeline_task.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task/python_task.py
--rw-rw-rw-   0 root         (0) root         (0)    20107 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task/task.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task/utils_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.457700 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/
--rw-rw-rw-   0 root         (0) root         (0)      723 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4810 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_dag_describe.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_output_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    13094 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_relations.py
--rw-rw-rw-   0 root         (0) root         (0)     4225 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_repr.py
--rw-rw-rw-   0 root         (0) root         (0)    10438 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_run_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     4392 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_run_orchestration_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_run_sync_local.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_sub_engine_policy_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     3655 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_sync_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.457700 dbnd-run-1.0.23.1/src/dbnd_run/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.458700 dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/
--rw-rw-rw-   0 root         (0) root         (0)      384 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2492 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/export.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/publish.py
--rw-rw-rw-   0 root         (0) root         (0)     1651 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/sanity.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/shell.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/simplest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.459700 dbnd-run-1.0.23.1/src/dbnd_run/tasks/py_distribution/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/py_distribution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/py_distribution/build_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     2704 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tasks/py_distribution/fat_wheel_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.459700 dbnd-run-1.0.23.1/src/dbnd_run/testing/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/testing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/testing/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/testing/pytest_dbnd_run_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.460700 dbnd-run-1.0.23.1/src/dbnd_run/tools/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tools/ipython.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.460700 dbnd-run-1.0.23.1/src/dbnd_run/tools/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tools/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/tools/jupyter/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.460700 dbnd-run-1.0.23.1/src/dbnd_run/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/utils/dbnd_run_module.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 10:17:47.000000 dbnd-run-1.0.23.1/src/dbnd_run/utils/user_code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:01.431698 dbnd-run-1.0.23.1/src/dbnd_run.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5514 2024-05-16 10:18:01.000000 dbnd-run-1.0.23.1/src/dbnd_run.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8288 2024-05-16 10:18:01.000000 dbnd-run-1.0.23.1/src/dbnd_run.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 10:18:01.000000 dbnd-run-1.0.23.1/src/dbnd_run.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      128 2024-05-16 10:18:01.000000 dbnd-run-1.0.23.1/src/dbnd_run.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 10:18:01.000000 dbnd-run-1.0.23.1/src/dbnd_run.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      367 2024-05-16 10:18:01.000000 dbnd-run-1.0.23.1/src/dbnd_run.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-16 10:18:01.000000 dbnd-run-1.0.23.1/src/dbnd_run.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.304772 dbnd-run-1.0.23.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-05-19 17:24:57.304772 dbnd-run-1.0.23.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2024-05-19 17:24:57.305772 dbnd-run-1.0.23.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.260767 dbnd-run-1.0.23.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.266768 dbnd-run-1.0.23.2/src/databand/
+-rwxrwxrwx   0 root         (0) root         (0)     1087 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/databand/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/databand/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/databand/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/databand/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/databand/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.266768 dbnd-run-1.0.23.2/src/databand/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/databand/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.266768 dbnd-run-1.0.23.2/src/databand/tasks/basics/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/databand/tasks/basics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.267768 dbnd-run-1.0.23.2/src/dbnd_run/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.269768 dbnd-run-1.0.23.2/src/dbnd_run/_vendor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 17:24:44.000000 dbnd-run-1.0.23.2/src/dbnd_run/_vendor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4690 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/_vendor/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/_vendor/kubernetes_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.270768 dbnd-run-1.0.23.2/src/dbnd_run/airflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.270768 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_extensions/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_extensions/dal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.271768 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 17:24:44.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.272768 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 17:24:44.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/airflow_windows_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/getuser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/timeout.py
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.273769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/airflow_multi_version_shim.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/cli_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/dbnd_task_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/kubernetes_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3768 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/config.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/db_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.277769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_aws.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_azure.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/dbnd_airflow_default_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3128 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/dbnd_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/docker_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/kubernetes_metrics_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/mng_connections.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/safe_hostname_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.278769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2500 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/utils/system_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.280769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2512 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/airflow_operator_as_dbnd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/airflow_operators_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/converters.py
+-rw-rw-rw-   0 root         (0) root         (0)     5920 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/dbnd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)    19192 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/dbnd_task_executor_via_airflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/dbnd_task_to_airflow_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/optimized_trigger_rule_dep.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/task_instance_state_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.280769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.281769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8415 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7636 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_runtime_zombies_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    31748 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    11937 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_watcher.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8224 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/simple_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.282769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/functional/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.283769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/dbnd_airflow_webserver_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/dbnd_airflow_webserver_plugin_linkable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.283769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/loadable_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/loadable_plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.283769 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/loadable_plugins/patched_versioned_bag/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/loadable_plugins/patched_versioned_bag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/loadable_plugins/patched_versioned_bag/dbnd_versioned_dagbag_autoload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/setup_plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.285770 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dagrun_zombies.py
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dagrun_zombies_clean_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dags_provider_from_databand.py
+-rw-rw-rw-   0 root         (0) root         (0)     8920 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dags_provider_from_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dbnd_cmd_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3503 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/scheduler_dags_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    42534 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/single_dag_run_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.285770 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2879 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/utils/generate_partitioned_dags.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/utils/partitioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.286770 dbnd-run-1.0.23.2/src/dbnd_run/airflow/testing/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/testing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/testing/testing_shims.py
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/testing/unittest_env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.287770 dbnd-run-1.0.23.2/src/dbnd_run/airflow/web/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3807 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/web/airflow_app_with_versioned_dagbag.py
+-rw-rw-rw-   0 root         (0) root         (0)     6488 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/web/databand_versioned_dagbag.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/airflow/web/single_job_run_support.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.289770 dbnd-run-1.0.23.2/src/dbnd_run/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4347 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_heartbeat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_project.py
+-rw-rw-rw-   0 root         (0) root         (0)    14658 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     6204 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_scheduler_management.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_show.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6020 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/service_auto_completer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.289770 dbnd-run-1.0.23.2/src/dbnd_run/conf/
+-rw-rw-rw-   0 root         (0) root         (0)     3475 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/conf/dbnd-run.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/conf/kubernetes-pod-tensorflow.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/conf/kubernetes-pod.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.289770 dbnd-run-1.0.23.2/src/dbnd_run/conf/project_init/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/conf/project_init/project.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/current.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.290770 dbnd-run-1.0.23.2/src/dbnd_run/errors/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/errors/execute_engine.py
+-rw-rw-rw-   0 root         (0) root         (0)     3973 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/errors/executor_k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/errors/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/errors/task_execution.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/errors/versioned_dagbag.py
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/orchestration_bootstrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.291770 dbnd-run-1.0.23.2/src/dbnd_run/orchestration_tracking/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/orchestration_tracking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.291770 dbnd-run-1.0.23.2/src/dbnd_run/orchestration_tracking/backends/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/orchestration_tracking/backends/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9456 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/orchestration_tracking/backends/tracking_store_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.292770 dbnd-run-1.0.23.2/src/dbnd_run/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/plugin/dbnd_plugin_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/plugin/dbnd_plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.293770 dbnd-run-1.0.23.2/src/dbnd_run/run_executor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_executor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5339 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_executor/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5670 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_executor/heartbeat_sender.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_executor/results_view.py
+-rw-rw-rw-   0 root         (0) root         (0)    35172 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_executor/run_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7496 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_executor/task_runs_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.293770 dbnd-run-1.0.23.2/src/dbnd_run/run_executor_engine/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_executor_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5295 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_executor_engine/local_task_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.295771 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/
+-rw-rw-rw-   0 root         (0) root         (0)     3776 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      727 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/describe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1623 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/git.py
+-rw-rw-rw-   0 root         (0) root         (0)    13117 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     8176 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/run_settings/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.297771 dbnd-run-1.0.23.2/src/dbnd_run/task/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task/data_source_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     9452 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task/decorated_callable_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task/pipeline_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task/python_task.py
+-rw-rw-rw-   0 root         (0) root         (0)    20107 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task/utils_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.300771 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/
+-rw-rw-rw-   0 root         (0) root         (0)      723 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_dag_describe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_output_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    13094 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4225 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_repr.py
+-rw-rw-rw-   0 root         (0) root         (0)    10438 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_run_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4392 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_run_orchestration_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_run_sync_local.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_sub_engine_policy_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_sync_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.300771 dbnd-run-1.0.23.2/src/dbnd_run/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.301771 dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/sanity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/simplest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.302771 dbnd-run-1.0.23.2/src/dbnd_run/tasks/py_distribution/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/py_distribution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/py_distribution/build_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2704 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tasks/py_distribution/fat_wheel_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.302771 dbnd-run-1.0.23.2/src/dbnd_run/testing/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/testing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/testing/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2745 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/testing/pytest_dbnd_run_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.303771 dbnd-run-1.0.23.2/src/dbnd_run/tools/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tools/ipython.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.303771 dbnd-run-1.0.23.2/src/dbnd_run/tools/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tools/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/tools/jupyter/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.304772 dbnd-run-1.0.23.2/src/dbnd_run/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/utils/dbnd_run_module.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-19 17:24:43.000000 dbnd-run-1.0.23.2/src/dbnd_run/utils/user_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:24:57.268768 dbnd-run-1.0.23.2/src/dbnd_run.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-05-19 17:24:57.000000 dbnd-run-1.0.23.2/src/dbnd_run.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8288 2024-05-19 17:24:57.000000 dbnd-run-1.0.23.2/src/dbnd_run.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 17:24:57.000000 dbnd-run-1.0.23.2/src/dbnd_run.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-19 17:24:57.000000 dbnd-run-1.0.23.2/src/dbnd_run.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 17:24:57.000000 dbnd-run-1.0.23.2/src/dbnd_run.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-19 17:24:57.000000 dbnd-run-1.0.23.2/src/dbnd_run.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-19 17:24:57.000000 dbnd-run-1.0.23.2/src/dbnd_run.egg-info/top_level.txt
```

### Comparing `dbnd-run-1.0.23.1/LICENSE` & `dbnd-run-1.0.23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/MANIFEST.in` & `dbnd-run-1.0.23.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/PKG-INFO` & `dbnd-run-1.0.23.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-run
-Version: 1.0.23.1
+Version: 1.0.23.2
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 Project-URL: Documentation, https://dbnd.readme.io/
```

### Comparing `dbnd-run-1.0.23.1/README.md` & `dbnd-run-1.0.23.2/README.md`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/setup.cfg` & `dbnd-run-1.0.23.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.23.1
+version = 1.0.23.2
 license_file = LICENSE
 description = Machine Learning Orchestration
 long_description_content_type = text/markdown
 long_description = file: README.md
 platforms = any
 author = Evgeny Shulman
 author_email = evgeny.shulman@databand.ai
```

### Comparing `dbnd-run-1.0.23.1/setup.py` & `dbnd-run-1.0.23.2/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/databand/__init__.py` & `dbnd-run-1.0.23.2/src/databand/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/databand/parameters.py` & `dbnd-run-1.0.23.2/src/databand/parameters.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/_vendor/database.py` & `dbnd-run-1.0.23.2/src/dbnd_run/_vendor/database.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/_vendor/kubernetes_utils.py` & `dbnd-run-1.0.23.2/src/dbnd_run/_vendor/kubernetes_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_env.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_env.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_extensions/dal.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_extensions/dal.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/__init__.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/configuration.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/configuration.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/timeout.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_override/dbnd_airflow_windows/timeout.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/airflow_utils.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/__init__.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/airflow_multi_version_shim.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/airflow_multi_version_shim.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/dbnd_task_runner.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/dbnd_task_runner.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/compat/kubernetes_executor.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/compat/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/config.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/config.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/db_utils.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/db_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_azure.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_azure.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_gcp.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/credentials_helper_gcp.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/dbnd_airflow_default_logger.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/dbnd_airflow_default_logger.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/dbnd_operator.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/dbnd_operator.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/docker_operator.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/docker_operator.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/kubernetes_metrics_logger.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/kubernetes_metrics_logger.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/mng_connections.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/mng_connections.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_airflow_contrib/utils/system_utils.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_airflow_contrib/utils/system_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/airflow_operator_as_dbnd.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/airflow_operator_as_dbnd.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/airflow_operators_catcher.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/airflow_operators_catcher.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/converters.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/converters.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/dbnd_execute.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/dbnd_execute.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/dbnd_task_executor_via_airflow.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/dbnd_task_executor_via_airflow.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/dbnd_task_to_airflow_operator.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/dbnd_task_to_airflow_operator.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/optimized_trigger_rule_dep.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/optimized_trigger_rule_dep.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/dbnd_task_executor/task_instance_state_manager.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/dbnd_task_executor/task_instance_state_manager.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_executor.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_runtime_zombies_cleaner.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_runtime_zombies_cleaner.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_scheduler.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_scheduler.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_watcher.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/kubernetes_watcher.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/kubernetes_executor/utils.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/kubernetes_executor/utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/executors/simple_executor.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/executors/simple_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/dbnd_airflow_webserver_plugin.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/dbnd_airflow_webserver_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/dbnd_airflow_webserver_plugin_linkable.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/dbnd_airflow_webserver_plugin_linkable.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/loadable_plugins/patched_versioned_bag/dbnd_versioned_dagbag_autoload.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/loadable_plugins/patched_versioned_bag/dbnd_versioned_dagbag_autoload.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/plugins/setup_plugins.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/plugins/setup_plugins.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dagrun_zombies.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dagrun_zombies.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dagrun_zombies_clean_job.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dagrun_zombies_clean_job.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dags_provider_from_databand.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dags_provider_from_databand.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dags_provider_from_file.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dags_provider_from_file.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/dbnd_cmd_operators.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/dbnd_cmd_operators.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/scheduler_dags_provider.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/scheduler_dags_provider.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/single_dag_run_job.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/single_dag_run_job.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/scheduler/utils/generate_partitioned_dags.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/scheduler/utils/generate_partitioned_dags.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/testing/testing_shims.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/testing/testing_shims.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/testing/unittest_env.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/testing/unittest_env.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/utils.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/web/airflow_app_with_versioned_dagbag.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/web/airflow_app_with_versioned_dagbag.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/web/databand_versioned_dagbag.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/web/databand_versioned_dagbag.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/airflow/web/single_job_run_support.py` & `dbnd-run-1.0.23.2/src/dbnd_run/airflow/web/single_job_run_support.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/__init__.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_execute.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_execute.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_heartbeat.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_heartbeat.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_project.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_project.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_run.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_run.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_scheduler_management.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_scheduler_management.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_show.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_show.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/cmd_utils.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/service_auto_completer.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/service_auto_completer.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/cli/utils.py` & `dbnd-run-1.0.23.2/src/dbnd_run/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/conf/dbnd-run.cfg` & `dbnd-run-1.0.23.2/src/dbnd_run/conf/dbnd-run.cfg`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/conf/kubernetes-pod-tensorflow.yaml` & `dbnd-run-1.0.23.2/src/dbnd_run/conf/kubernetes-pod-tensorflow.yaml`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/current.py` & `dbnd-run-1.0.23.2/src/dbnd_run/current.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/errors/execute_engine.py` & `dbnd-run-1.0.23.2/src/dbnd_run/errors/execute_engine.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/errors/executor_k8s.py` & `dbnd-run-1.0.23.2/src/dbnd_run/errors/executor_k8s.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/errors/graph.py` & `dbnd-run-1.0.23.2/src/dbnd_run/errors/graph.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/errors/task_execution.py` & `dbnd-run-1.0.23.2/src/dbnd_run/errors/task_execution.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/orchestration_bootstrap.py` & `dbnd-run-1.0.23.2/src/dbnd_run/orchestration_bootstrap.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/orchestration_tracking/backends/tracking_store_file.py` & `dbnd-run-1.0.23.2/src/dbnd_run/orchestration_tracking/backends/tracking_store_file.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/plugin/dbnd_plugin_spec.py` & `dbnd-run-1.0.23.2/src/dbnd_run/plugin/dbnd_plugin_spec.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/plugin/dbnd_plugins.py` & `dbnd-run-1.0.23.2/src/dbnd_run/plugin/dbnd_plugins.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_executor/factory.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_executor/factory.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_executor/heartbeat_sender.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_executor/heartbeat_sender.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_executor/results_view.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_executor/results_view.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_executor/run_executor.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_executor/run_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_executor/task_runs_builder.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_executor/task_runs_builder.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_executor_engine/__init__.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_executor_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_executor_engine/local_task_executor.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_executor_engine/local_task_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/__init__.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/describe.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/describe.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/engine.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/engine.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/env.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/env.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/git.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/git.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/log.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/log.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/output.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/output.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/run.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/run.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/run_settings/scheduler.py` & `dbnd-run-1.0.23.2/src/dbnd_run/run_settings/scheduler.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task/data_source_task.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task/data_source_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task/decorated_callable_task.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task/decorated_callable_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task/pipeline_task.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task/pipeline_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task/task.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task/task.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/__init__.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_dag_describe.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_dag_describe.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_namespace.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_namespace.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_output_builder.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_output_builder.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_relations.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_relations.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_repr.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_repr.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_run_executor.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_run_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_run_orchestration_logging.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_run_orchestration_logging.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_run_sync_local.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_run_sync_local.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_sub_engine_policy_ctrl.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_sub_engine_policy_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_sync_ctrl.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_sync_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_validator.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_validator.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/task_ctrl/task_visualizer.py` & `dbnd-run-1.0.23.2/src/dbnd_run/task_ctrl/task_visualizer.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/export.py` & `dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/export.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/publish.py` & `dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/publish.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/sanity.py` & `dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/sanity.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/shell.py` & `dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/shell.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/tasks/basics/simplest.py` & `dbnd-run-1.0.23.2/src/dbnd_run/tasks/basics/simplest.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/tasks/py_distribution/build_distribution.py` & `dbnd-run-1.0.23.2/src/dbnd_run/tasks/py_distribution/build_distribution.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/tasks/py_distribution/fat_wheel_tasks.py` & `dbnd-run-1.0.23.2/src/dbnd_run/tasks/py_distribution/fat_wheel_tasks.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/testing/helpers.py` & `dbnd-run-1.0.23.2/src/dbnd_run/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/testing/pytest_dbnd_run_plugin.py` & `dbnd-run-1.0.23.2/src/dbnd_run/testing/pytest_dbnd_run_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run/utils/user_code.py` & `dbnd-run-1.0.23.2/src/dbnd_run/utils/user_code.py`

 * *Files identical despite different names*

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run.egg-info/PKG-INFO` & `dbnd-run-1.0.23.2/src/dbnd_run.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-run
-Version: 1.0.23.1
+Version: 1.0.23.2
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 Project-URL: Documentation, https://dbnd.readme.io/
```

### Comparing `dbnd-run-1.0.23.1/src/dbnd_run.egg-info/SOURCES.txt` & `dbnd-run-1.0.23.2/src/dbnd_run.egg-info/SOURCES.txt`

 * *Files identical despite different names*

