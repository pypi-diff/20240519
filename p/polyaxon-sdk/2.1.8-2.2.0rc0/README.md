# Comparing `tmp/polyaxon-sdk-2.1.8.tar.gz` & `tmp/polyaxon-sdk-2.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyaxon-sdk-2.1.8.tar", last modified: Sat Apr 20 12:26:13 2024, max compression
+gzip compressed data, was "polyaxon-sdk-2.2.0rc0.tar", last modified: Sun May 19 19:30:44 2024, max compression
```

## Comparing `polyaxon-sdk-2.1.8.tar` & `polyaxon-sdk-2.2.0rc0.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:13.874328 polyaxon-sdk-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 12:26:13.874328 polyaxon-sdk-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    55502 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:13.826328 polyaxon-sdk-2.1.8/polyaxon_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:13.834328 polyaxon-sdk-2.1.8/polyaxon_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   159743 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/agents_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/artifacts_stores_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36537 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/auth_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53577 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/connections_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53190 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/dashboards_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   295153 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/organizations_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54090 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/policies_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54174 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/presets_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    64020 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/project_dashboards_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    63600 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/project_searches_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   238667 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/projects_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    75088 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/queues_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   502862 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/runs_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/schemas_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    52784 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/searches_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    98980 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/service_accounts_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    59180 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/tags_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    97653 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/teams_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    72548 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/users_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19587 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api/versions_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29604 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:13.874328 polyaxon-sdk-2.1.8/polyaxon_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/agent_state_response_agent_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/mx_job_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/runtime_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/search_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_agent_reconcile_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_agent_state_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_agent_status_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_analytics_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_artifact_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_artifact_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_artifacts_mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_artifacts_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_auth_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_average_stopping_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_bucket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_claim_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_clean_pod_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_cloning_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_compiled_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_cron_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dag_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dashboard_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dask_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dask_replica.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_date_time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_diff_stopping_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dockerfile_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entities_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entities_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entity_notification_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entity_stage_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entity_status_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_chart_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_curve_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_span.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_span_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_events_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_failure_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_gcs_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_git_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_git_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_grid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_host_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_host_path_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_date_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_date_time_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_geom_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_lin_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_log_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_log_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_log_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_p_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_q_log_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_q_log_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_q_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_q_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hub_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hyperband.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hyperopt_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_installation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_interval_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_join_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_kf_replica.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_activities_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_bookmarks_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_dashboards_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_organization_members_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_organizations_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_policies_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_presets_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_project_versions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_queues_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_run_artifacts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_run_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_run_edges_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_searches_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_service_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_team_members_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_teams_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_managed_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_matrix_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_median_stopping_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_metric_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_multi_events_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_mx_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_operation_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_optimization_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_optimization_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_organization_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_paddle_elastic_polic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_password_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_patch_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_path_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_pipeline_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_polyaxon_init_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_polyaxon_sidecar_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_project_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_project_version_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_pytorch_elastic_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_pytorch_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_random_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_ray_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_ray_replica.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_edge_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_edge_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_edges_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_pending.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_reference_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_s3_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_schedule_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_search_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_section_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_settings_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_stage_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_status_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_team_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_team_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_tensorboard_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_termination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_tf_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_trial_start.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_trigger_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_truncation_stopping_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_uri_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_url_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_user_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_user_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_user_singup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_uuids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_wasb_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_xg_boost_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/polyaxon_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:13.830328 polyaxon-sdk-2.1.8/polyaxon_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 12:26:13.000000 polyaxon-sdk-2.1.8/polyaxon_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-20 12:26:13.000000 polyaxon-sdk-2.1.8/polyaxon_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:13.000000 polyaxon-sdk-2.1.8/polyaxon_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 12:26:13.000000 polyaxon-sdk-2.1.8/polyaxon_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 12:26:13.000000 polyaxon-sdk-2.1.8/polyaxon_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 12:26:13.874328 polyaxon-sdk-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-20 12:26:03.000000 polyaxon-sdk-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:44.807820 polyaxon-sdk-2.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-19 19:30:44.807820 polyaxon-sdk-2.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    58270 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:44.755820 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)    16991 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:44.763820 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   159747 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/agents_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/artifacts_stores_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36541 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/auth_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53581 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/connections_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53194 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/dashboards_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295157 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/organizations_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54094 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/policies_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54178 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/presets_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64024 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/project_dashboards_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63604 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/project_searches_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   245680 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/projects_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75092 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/queues_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   502406 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/runs_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/schemas_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52788 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/searches_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98984 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/service_accounts_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59184 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/tags_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   214158 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/teams_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80358 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/users_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/versions_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29612 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:44.807820 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/agent_state_response_agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/mx_job_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/runtime_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/search_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_agent_reconcile_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_agent_state_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_agent_status_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_analytics_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_artifact_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_artifact_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_artifacts_mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_artifacts_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_auth_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_average_stopping_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_bucket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_claim_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_clean_pod_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_cloning_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_compiled_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_cron_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dag_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dashboard_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dask_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dask_replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_date_time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_diff_stopping_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dockerfile_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entities_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entities_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entity_notification_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entity_stage_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entity_status_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_chart_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_curve_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_span_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_failure_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_gcs_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_git_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_git_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_host_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_host_path_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_date_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_date_time_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_geom_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_lin_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_log_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_log_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_log_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_p_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_q_log_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_q_log_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_q_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_q_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hub_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hyperopt_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_interval_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_join_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_kf_replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_activities_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_bookmarks_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_dashboards_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_organization_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_organizations_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_policies_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_presets_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_project_versions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_queues_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_run_artifacts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_run_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_run_edges_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_searches_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_service_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_team_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_teams_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_managed_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_matrix_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_median_stopping_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_metric_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_multi_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_operation_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_optimization_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_optimization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_paddle_elastic_polic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_password_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_patch_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_path_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_pipeline_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_polyaxon_init_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_polyaxon_sidecar_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_project_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_project_version_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_pytorch_elastic_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_pytorch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_random_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_ray_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_ray_replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_edge_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_edge_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_edges_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_pending.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_reference_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_s3_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_schedule_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11599 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_search_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_section_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_settings_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_stage_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_status_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_team_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_tensorboard_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_termination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_trial_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_trigger_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_truncation_stopping_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_uri_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_url_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_user_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_user_singup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_wasb_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_xg_boost_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:44.755820 polyaxon-sdk-2.2.0rc0/polyaxon_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-19 19:30:44.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-19 19:30:44.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:44.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 19:30:44.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 19:30:44.000000 polyaxon-sdk-2.2.0rc0/polyaxon_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 19:30:44.807820 polyaxon-sdk-2.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-19 19:30:36.000000 polyaxon-sdk-2.2.0rc0/setup.py
```

### Comparing `polyaxon-sdk-2.1.8/README.md` & `polyaxon-sdk-2.2.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # polyaxon-sdk
    
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.1.8
-- Package version: 2.1.8
+- API version: 2.2.0-rc0
+- Package version: 2.2.0-rc0
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://github.com/polyaxon/polyaxon](https://github.com/polyaxon/polyaxon)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -210,14 +210,15 @@
 *ProjectSearchesV1Api* | [**list_project_searches**](docs/ProjectSearchesV1Api.md#list_project_searches) | **GET** /api/v1/{owner}/{name}/searches | List project searches
 *ProjectSearchesV1Api* | [**patch_project_search**](docs/ProjectSearchesV1Api.md#patch_project_search) | **PATCH** /api/v1/{owner}/{project}/searches/{search.uuid} | Patch project search
 *ProjectSearchesV1Api* | [**promote_project_search**](docs/ProjectSearchesV1Api.md#promote_project_search) | **POST** /api/v1/{owner}/{entity}/searches/{uuid}/promote | Promote project search
 *ProjectSearchesV1Api* | [**update_project_search**](docs/ProjectSearchesV1Api.md#update_project_search) | **PUT** /api/v1/{owner}/{project}/searches/{search.uuid} | Update project search
 *ProjectsV1Api* | [**archive_project**](docs/ProjectsV1Api.md#archive_project) | **POST** /api/v1/{owner}/{name}/archive | Archive project
 *ProjectsV1Api* | [**bookmark_project**](docs/ProjectsV1Api.md#bookmark_project) | **POST** /api/v1/{owner}/{name}/bookmark | Bookmark project
 *ProjectsV1Api* | [**create_project**](docs/ProjectsV1Api.md#create_project) | **POST** /api/v1/{owner}/projects/create | Create new project
+*ProjectsV1Api* | [**create_team_project**](docs/ProjectsV1Api.md#create_team_project) | **POST** /api/v1/{owner}/{team}/projects/create | Create new project via team space
 *ProjectsV1Api* | [**create_version**](docs/ProjectsV1Api.md#create_version) | **POST** /api/v1/{owner}/{project}/versions/{version.kind} | Create version
 *ProjectsV1Api* | [**create_version_stage**](docs/ProjectsV1Api.md#create_version_stage) | **POST** /api/v1/{owner}/{entity}/versions/{kind}/{name}/stages | Create new artifact version stage
 *ProjectsV1Api* | [**delete_project**](docs/ProjectsV1Api.md#delete_project) | **DELETE** /api/v1/{owner}/{name} | Delete project
 *ProjectsV1Api* | [**delete_version**](docs/ProjectsV1Api.md#delete_version) | **DELETE** /api/v1/{owner}/{entity}/versions/{kind}/{name} | Delete version
 *ProjectsV1Api* | [**disable_project_ci**](docs/ProjectsV1Api.md#disable_project_ci) | **DELETE** /api/v1/{owner}/{name}/ci | Disbale project CI
 *ProjectsV1Api* | [**enable_project_ci**](docs/ProjectsV1Api.md#enable_project_ci) | **POST** /api/v1/{owner}/{name}/ci | Enable project CI
 *ProjectsV1Api* | [**get_project**](docs/ProjectsV1Api.md#get_project) | **GET** /api/v1/{owner}/{name} | Get project
@@ -248,29 +249,29 @@
 *QueuesV1Api* | [**list_organization_queue_names**](docs/QueuesV1Api.md#list_organization_queue_names) | **GET** /api/v1/orgs/{owner}/queues/names | List organization level queues names
 *QueuesV1Api* | [**list_organization_queues**](docs/QueuesV1Api.md#list_organization_queues) | **GET** /api/v1/orgs/{owner}/queues | List organization level queues
 *QueuesV1Api* | [**list_queue_names**](docs/QueuesV1Api.md#list_queue_names) | **GET** /api/v1/orgs/{owner}/agents/{name}/queues/names | List queues names
 *QueuesV1Api* | [**list_queues**](docs/QueuesV1Api.md#list_queues) | **GET** /api/v1/orgs/{owner}/agents/{name}/queues | List queues
 *QueuesV1Api* | [**patch_queue**](docs/QueuesV1Api.md#patch_queue) | **PATCH** /api/v1/orgs/{owner}/agents/{agent}/queues/{queue.uuid} | Patch queue
 *QueuesV1Api* | [**update_queue**](docs/QueuesV1Api.md#update_queue) | **PUT** /api/v1/orgs/{owner}/agents/{agent}/queues/{queue.uuid} | Update queue
 *RunsV1Api* | [**approve_run**](docs/RunsV1Api.md#approve_run) | **POST** /api/v1/{owner}/{entity}/runs/{uuid}/approve | Approve run
-*RunsV1Api* | [**approve_runs**](docs/RunsV1Api.md#approve_runs) | **POST** /api/v1/{owner}/{project}/runs/approve | Approve runs
+*RunsV1Api* | [**approve_runs**](docs/RunsV1Api.md#approve_runs) | **POST** /api/v1/{owner}/{name}/runs/approve | Approve runs
 *RunsV1Api* | [**archive_run**](docs/RunsV1Api.md#archive_run) | **POST** /api/v1/{owner}/{entity}/runs/{uuid}/archive | Archive run
-*RunsV1Api* | [**archive_runs**](docs/RunsV1Api.md#archive_runs) | **POST** /api/v1/{owner}/{project}/runs/archive | Archive runs
+*RunsV1Api* | [**archive_runs**](docs/RunsV1Api.md#archive_runs) | **POST** /api/v1/{owner}/{name}/runs/archive | Archive runs
 *RunsV1Api* | [**bookmark_run**](docs/RunsV1Api.md#bookmark_run) | **POST** /api/v1/{owner}/{entity}/runs/{uuid}/bookmark | Bookmark run
-*RunsV1Api* | [**bookmark_runs**](docs/RunsV1Api.md#bookmark_runs) | **POST** /api/v1/{owner}/{project}/runs/bookmark | Bookmark runs
+*RunsV1Api* | [**bookmark_runs**](docs/RunsV1Api.md#bookmark_runs) | **POST** /api/v1/{owner}/{name}/runs/bookmark | Bookmark runs
 *RunsV1Api* | [**collect_run_logs**](docs/RunsV1Api.md#collect_run_logs) | **POST** /internal/v1/{namespace}/{owner}/{project}/runs/{uuid}/{kind}/logs | Internal API to collect run logs
 *RunsV1Api* | [**copy_run**](docs/RunsV1Api.md#copy_run) | **POST** /api/v1/{owner}/{project}/runs/{run.uuid}/copy | Restart run with copy
 *RunsV1Api* | [**create_run**](docs/RunsV1Api.md#create_run) | **POST** /api/v1/{owner}/{project}/runs | Create new run
 *RunsV1Api* | [**create_run_artifacts_lineage**](docs/RunsV1Api.md#create_run_artifacts_lineage) | **POST** /api/v1/{owner}/{project}/runs/{uuid}/lineage/artifacts | Create bulk run artifacts lineage
 *RunsV1Api* | [**create_run_status**](docs/RunsV1Api.md#create_run_status) | **POST** /api/v1/{owner}/{project}/runs/{uuid}/statuses | Create new run status
 *RunsV1Api* | [**delete_run**](docs/RunsV1Api.md#delete_run) | **DELETE** /api/v1/{owner}/{entity}/runs/{uuid} | Delete run
 *RunsV1Api* | [**delete_run_artifact**](docs/RunsV1Api.md#delete_run_artifact) | **DELETE** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/artifact | Delete run artifact
 *RunsV1Api* | [**delete_run_artifact_lineage**](docs/RunsV1Api.md#delete_run_artifact_lineage) | **DELETE** /api/v1/{owner}/{project}/runs/{uuid}/lineage/artifacts/{name} | Delete run artifact lineage
 *RunsV1Api* | [**delete_run_artifacts**](docs/RunsV1Api.md#delete_run_artifacts) | **DELETE** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/artifacts | Delete run artifacts
-*RunsV1Api* | [**delete_runs**](docs/RunsV1Api.md#delete_runs) | **DELETE** /api/v1/{owner}/{project}/runs/delete | Delete runs
+*RunsV1Api* | [**delete_runs**](docs/RunsV1Api.md#delete_runs) | **DELETE** /api/v1/{owner}/{name}/runs/delete | Delete runs
 *RunsV1Api* | [**get_multi_run_events**](docs/RunsV1Api.md#get_multi_run_events) | **GET** /streams/v1/{namespace}/{owner}/{project}/runs/multi/events/{kind} | Get multi runs events
 *RunsV1Api* | [**get_multi_run_importance**](docs/RunsV1Api.md#get_multi_run_importance) | **POST** /streams/v1/{namespace}/{owner}/{project}/runs/multi/importance | Get multi run importance
 *RunsV1Api* | [**get_run**](docs/RunsV1Api.md#get_run) | **GET** /api/v1/{owner}/{entity}/runs/{uuid} | Get run
 *RunsV1Api* | [**get_run_artifact**](docs/RunsV1Api.md#get_run_artifact) | **GET** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/artifact | Get run artifact
 *RunsV1Api* | [**get_run_artifact_lineage**](docs/RunsV1Api.md#get_run_artifact_lineage) | **GET** /api/v1/{owner}/{project}/runs/{uuid}/lineage/artifacts/{name} | Get run artifacts lineage
 *RunsV1Api* | [**get_run_artifacts**](docs/RunsV1Api.md#get_run_artifacts) | **GET** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/artifacts | Get run artifacts
 *RunsV1Api* | [**get_run_artifacts_lineage**](docs/RunsV1Api.md#get_run_artifacts_lineage) | **GET** /api/v1/{owner}/{entity}/runs/{uuid}/lineage/artifacts | Get run artifacts lineage
@@ -287,33 +288,33 @@
 *RunsV1Api* | [**get_run_stats**](docs/RunsV1Api.md#get_run_stats) | **GET** /api/v1/{owner}/{entity}/runs/{uuid}/stats | Get run stats
 *RunsV1Api* | [**get_run_statuses**](docs/RunsV1Api.md#get_run_statuses) | **GET** /api/v1/{owner}/{entity}/runs/{uuid}/statuses | Get run statuses
 *RunsV1Api* | [**get_run_upstream_lineage**](docs/RunsV1Api.md#get_run_upstream_lineage) | **GET** /api/v1/{owner}/{entity}/runs/{uuid}/lineage/upstream | Get run upstream lineage
 *RunsV1Api* | [**get_runs_artifacts_lineage**](docs/RunsV1Api.md#get_runs_artifacts_lineage) | **GET** /api/v1/{owner}/{name}/runs/lineage/artifacts | Get runs artifacts lineage
 *RunsV1Api* | [**impersonate_token**](docs/RunsV1Api.md#impersonate_token) | **POST** /api/v1/{owner}/{entity}/runs/{uuid}/impersonate | Impersonate run token
 *RunsV1Api* | [**inspect_run**](docs/RunsV1Api.md#inspect_run) | **GET** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/k8s_inspect | Inspect an active run full conditions
 *RunsV1Api* | [**invalidate_run**](docs/RunsV1Api.md#invalidate_run) | **POST** /api/v1/{owner}/{entity}/runs/{uuid}/invalidate | Invalidate run
-*RunsV1Api* | [**invalidate_runs**](docs/RunsV1Api.md#invalidate_runs) | **POST** /api/v1/{owner}/{project}/runs/invalidate | Invalidate runs
+*RunsV1Api* | [**invalidate_runs**](docs/RunsV1Api.md#invalidate_runs) | **POST** /api/v1/{owner}/{name}/runs/invalidate | Invalidate runs
 *RunsV1Api* | [**list_archived_runs**](docs/RunsV1Api.md#list_archived_runs) | **GET** /api/v1/archives/{user}/runs | List archived runs for user
 *RunsV1Api* | [**list_bookmarked_runs**](docs/RunsV1Api.md#list_bookmarked_runs) | **GET** /api/v1/bookmarks/{user}/runs | List bookmarked runs for user
 *RunsV1Api* | [**list_runs**](docs/RunsV1Api.md#list_runs) | **GET** /api/v1/{owner}/{name}/runs | List runs
 *RunsV1Api* | [**notify_run_status**](docs/RunsV1Api.md#notify_run_status) | **POST** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/notify | Notify run status
 *RunsV1Api* | [**patch_run**](docs/RunsV1Api.md#patch_run) | **PATCH** /api/v1/{owner}/{project}/runs/{run.uuid} | Patch run
 *RunsV1Api* | [**restart_run**](docs/RunsV1Api.md#restart_run) | **POST** /api/v1/{owner}/{project}/runs/{run.uuid}/restart | Restart run
 *RunsV1Api* | [**restore_run**](docs/RunsV1Api.md#restore_run) | **POST** /api/v1/{owner}/{entity}/runs/{uuid}/restore | Restore run
-*RunsV1Api* | [**restore_runs**](docs/RunsV1Api.md#restore_runs) | **POST** /api/v1/{owner}/{project}/runs/restore | Restore runs
+*RunsV1Api* | [**restore_runs**](docs/RunsV1Api.md#restore_runs) | **POST** /api/v1/{owner}/{name}/runs/restore | Restore runs
 *RunsV1Api* | [**resume_run**](docs/RunsV1Api.md#resume_run) | **POST** /api/v1/{owner}/{project}/runs/{run.uuid}/resume | Resume run
 *RunsV1Api* | [**set_run_edges_lineage**](docs/RunsV1Api.md#set_run_edges_lineage) | **POST** /api/v1/{owner}/{project}/runs/{uuid}/lineage/edges | Set run edges graph lineage
 *RunsV1Api* | [**skip_run**](docs/RunsV1Api.md#skip_run) | **POST** /api/v1/{owner}/{entity}/runs/{uuid}/skip | Skip run
-*RunsV1Api* | [**skip_runs**](docs/RunsV1Api.md#skip_runs) | **POST** /api/v1/{owner}/{project}/runs/skip | Skip runs
+*RunsV1Api* | [**skip_runs**](docs/RunsV1Api.md#skip_runs) | **POST** /api/v1/{owner}/{name}/runs/skip | Skip runs
 *RunsV1Api* | [**stop_run**](docs/RunsV1Api.md#stop_run) | **POST** /api/v1/{owner}/{entity}/runs/{uuid}/stop | Stop run
-*RunsV1Api* | [**stop_runs**](docs/RunsV1Api.md#stop_runs) | **POST** /api/v1/{owner}/{project}/runs/stop | Stop runs
+*RunsV1Api* | [**stop_runs**](docs/RunsV1Api.md#stop_runs) | **POST** /api/v1/{owner}/{name}/runs/stop | Stop runs
 *RunsV1Api* | [**sync_run**](docs/RunsV1Api.md#sync_run) | **POST** /api/v1/{owner}/{project}/runs/sync | Sync offline run
-*RunsV1Api* | [**tag_runs**](docs/RunsV1Api.md#tag_runs) | **POST** /api/v1/{owner}/{project}/runs/tag | Tag runs
+*RunsV1Api* | [**tag_runs**](docs/RunsV1Api.md#tag_runs) | **POST** /api/v1/{owner}/{name}/runs/tag | Tag runs
 *RunsV1Api* | [**transfer_run**](docs/RunsV1Api.md#transfer_run) | **POST** /api/v1/{owner}/{project}/runs/{run.uuid}/transfer | Transfer run
-*RunsV1Api* | [**transfer_runs**](docs/RunsV1Api.md#transfer_runs) | **POST** /api/v1/{owner}/{project}/runs/transfer | Transfer runs
+*RunsV1Api* | [**transfer_runs**](docs/RunsV1Api.md#transfer_runs) | **POST** /api/v1/{owner}/{name}/runs/transfer | Transfer runs
 *RunsV1Api* | [**unbookmark_run**](docs/RunsV1Api.md#unbookmark_run) | **DELETE** /api/v1/{owner}/{entity}/runs/{uuid}/unbookmark | Unbookmark run
 *RunsV1Api* | [**update_run**](docs/RunsV1Api.md#update_run) | **PUT** /api/v1/{owner}/{project}/runs/{run.uuid} | Update run
 *RunsV1Api* | [**upload_run_artifact**](docs/RunsV1Api.md#upload_run_artifact) | **POST** /api/v1/{owner}/{project}/runs/{uuid}/artifacts/upload | Upload an artifact file to a store via run access
 *RunsV1Api* | [**upload_run_logs**](docs/RunsV1Api.md#upload_run_logs) | **POST** /api/v1/{owner}/{project}/runs/{uuid}/logs/upload | Upload a logs file to a store via run access
 *SchemasV1Api* | [**no_op**](docs/SchemasV1Api.md#no_op) | **GET** /schemas | NoOp
 *SearchesV1Api* | [**create_search**](docs/SearchesV1Api.md#create_search) | **POST** /api/v1/orgs/{owner}/searches | Create search
 *SearchesV1Api* | [**delete_search**](docs/SearchesV1Api.md#delete_search) | **DELETE** /api/v1/orgs/{owner}/searches/{uuid} | Delete search
@@ -339,33 +340,49 @@
 *TagsV1Api* | [**delete_tag**](docs/TagsV1Api.md#delete_tag) | **DELETE** /api/v1/orgs/{owner}/tags/{uuid} | Delete tag
 *TagsV1Api* | [**get_tag**](docs/TagsV1Api.md#get_tag) | **GET** /api/v1/orgs/{owner}/tags/{uuid} | Get tag
 *TagsV1Api* | [**list_tags**](docs/TagsV1Api.md#list_tags) | **GET** /api/v1/orgs/{owner}/tags | List tags
 *TagsV1Api* | [**load_tags**](docs/TagsV1Api.md#load_tags) | **GET** /api/v1/orgs/{owner}/tags/load | Load tags
 *TagsV1Api* | [**patch_tag**](docs/TagsV1Api.md#patch_tag) | **PATCH** /api/v1/orgs/{owner}/tags/{tag.uuid} | Patch tag
 *TagsV1Api* | [**sync_tags**](docs/TagsV1Api.md#sync_tags) | **POST** /api/v1/orgs/{owner}/tags/sync | Sync tags
 *TagsV1Api* | [**update_tag**](docs/TagsV1Api.md#update_tag) | **PUT** /api/v1/orgs/{owner}/tags/{tag.uuid} | Update tag
+*TeamsV1Api* | [**approve_team_runs**](docs/TeamsV1Api.md#approve_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/approve | Approve cross-project runs selection
+*TeamsV1Api* | [**archive_team_runs**](docs/TeamsV1Api.md#archive_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/archive | Archive cross-project runs selection
+*TeamsV1Api* | [**bookmark_team_runs**](docs/TeamsV1Api.md#bookmark_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/bookmark | Bookmark cross-project runs selection
 *TeamsV1Api* | [**create_team**](docs/TeamsV1Api.md#create_team) | **POST** /api/v1/orgs/{owner}/teams | Create team
 *TeamsV1Api* | [**create_team_member**](docs/TeamsV1Api.md#create_team_member) | **POST** /api/v1/orgs/{owner}/teams/{team}/members | Create team member
 *TeamsV1Api* | [**delete_team**](docs/TeamsV1Api.md#delete_team) | **DELETE** /api/v1/orgs/{owner}/teams/{name} | Delete team
 *TeamsV1Api* | [**delete_team_member**](docs/TeamsV1Api.md#delete_team_member) | **DELETE** /api/v1/orgs/{owner}/teams/{team}/members/{user} | Delete team member details
+*TeamsV1Api* | [**delete_team_runs**](docs/TeamsV1Api.md#delete_team_runs) | **DELETE** /api/v1/orgs/{owner}/teams/{name}/runs/delete | Delete cross-project runs selection
 *TeamsV1Api* | [**get_team**](docs/TeamsV1Api.md#get_team) | **GET** /api/v1/orgs/{owner}/teams/{name} | Get team
+*TeamsV1Api* | [**get_team_activities**](docs/TeamsV1Api.md#get_team_activities) | **GET** /api/v1/orgs/{owner}/teams/{name}/activities | Get organization activities
 *TeamsV1Api* | [**get_team_member**](docs/TeamsV1Api.md#get_team_member) | **GET** /api/v1/orgs/{owner}/teams/{team}/members/{user} | Get team member details
+*TeamsV1Api* | [**get_team_run**](docs/TeamsV1Api.md#get_team_run) | **GET** /api/v1/orgs/{owner}/teams/{entity}/runs/{uuid} | Get a run in a team
+*TeamsV1Api* | [**get_team_runs**](docs/TeamsV1Api.md#get_team_runs) | **GET** /api/v1/orgs/{owner}/teams/{name}/runs | Get all runs in a team
+*TeamsV1Api* | [**get_team_stats**](docs/TeamsV1Api.md#get_team_stats) | **GET** /api/v1/orgs/{owner}/teams/{name}/stats | Get team stats
+*TeamsV1Api* | [**get_team_versions**](docs/TeamsV1Api.md#get_team_versions) | **GET** /api/v1/orgs/{owner}/teams/{entity}/versions/{kind} | Get all runs in a team
+*TeamsV1Api* | [**invalidate_team_runs**](docs/TeamsV1Api.md#invalidate_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/invalidate | Invalidate cross-project runs selection
 *TeamsV1Api* | [**list_team_members**](docs/TeamsV1Api.md#list_team_members) | **GET** /api/v1/orgs/{owner}/teams/{name}/members | Get team members
 *TeamsV1Api* | [**list_team_names**](docs/TeamsV1Api.md#list_team_names) | **GET** /api/v1/orgs/{owner}/teams/names | List teams names
 *TeamsV1Api* | [**list_teams**](docs/TeamsV1Api.md#list_teams) | **GET** /api/v1/orgs/{owner}/teams | List teams
 *TeamsV1Api* | [**patch_team**](docs/TeamsV1Api.md#patch_team) | **PATCH** /api/v1/orgs/{owner}/teams/{team.name} | Patch team
 *TeamsV1Api* | [**patch_team_member**](docs/TeamsV1Api.md#patch_team_member) | **PATCH** /api/v1/orgs/{owner}/teams/{team}/members/{member.user} | Patch team member
+*TeamsV1Api* | [**restore_team_runs**](docs/TeamsV1Api.md#restore_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/restore | Restore cross-project runs selection
+*TeamsV1Api* | [**skip_team_runs**](docs/TeamsV1Api.md#skip_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/Skip | Skip cross-project runs selection
+*TeamsV1Api* | [**stop_team_runs**](docs/TeamsV1Api.md#stop_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/stop | Stop cross-project runs selection
+*TeamsV1Api* | [**tag_team_runs**](docs/TeamsV1Api.md#tag_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/tag | Tag cross-project runs selection
+*TeamsV1Api* | [**transfer_team_runs**](docs/TeamsV1Api.md#transfer_team_runs) | **POST** /api/v1/orgs/{owner}/teams/{name}/runs/transfer | Transfer cross-project runs selection to a new project
 *TeamsV1Api* | [**update_team**](docs/TeamsV1Api.md#update_team) | **PUT** /api/v1/orgs/{owner}/teams/{team.name} | Update team
 *TeamsV1Api* | [**update_team_member**](docs/TeamsV1Api.md#update_team_member) | **PUT** /api/v1/orgs/{owner}/teams/{team}/members/{member.user} | Update team member
 *UsersV1Api* | [**create_token**](docs/UsersV1Api.md#create_token) | **POST** /api/v1/users/tokens | Create token
 *UsersV1Api* | [**delete_token**](docs/UsersV1Api.md#delete_token) | **DELETE** /api/v1/users/tokens/{uuid} | Delete token
 *UsersV1Api* | [**get_history**](docs/UsersV1Api.md#get_history) | **GET** /api/v1/users/history | User History
 *UsersV1Api* | [**get_suggestions**](docs/UsersV1Api.md#get_suggestions) | **GET** /api/v1/users/suggestions | User suggestions
 *UsersV1Api* | [**get_token**](docs/UsersV1Api.md#get_token) | **GET** /api/v1/users/tokens/{uuid} | Get token
 *UsersV1Api* | [**get_user**](docs/UsersV1Api.md#get_user) | **GET** /api/v1/users | Get current user
+*UsersV1Api* | [**get_workspaces**](docs/UsersV1Api.md#get_workspaces) | **GET** /api/v1/users/workspaces | User workspaces
 *UsersV1Api* | [**list_tokens**](docs/UsersV1Api.md#list_tokens) | **GET** /api/v1/users/tokens | List tokens
 *UsersV1Api* | [**patch_token**](docs/UsersV1Api.md#patch_token) | **PATCH** /api/v1/users/tokens/{token.uuid} | Patch token
 *UsersV1Api* | [**patch_user**](docs/UsersV1Api.md#patch_user) | **PATCH** /api/v1/users | Patch current user
 *UsersV1Api* | [**update_token**](docs/UsersV1Api.md#update_token) | **PUT** /api/v1/users/tokens/{token.uuid} | Update token
 *UsersV1Api* | [**update_user**](docs/UsersV1Api.md#update_user) | **PUT** /api/v1/users | Update current user
 *VersionsV1Api* | [**get_compatibility**](docs/VersionsV1Api.md#get_compatibility) | **GET** /api/v1/compatibility/{uuid}/{version}/{service} | Get compatibility versions
 *VersionsV1Api* | [**get_installation**](docs/VersionsV1Api.md#get_installation) | **GET** /api/v1/installation | Get installation versions
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/__init__.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "2.1.8"
+__version__ = "2.2.0-rc0"
 
 # import apis into sdk package
 from polyaxon_sdk.api.agents_v1_api import AgentsV1Api
 from polyaxon_sdk.api.artifacts_stores_v1_api import ArtifactsStoresV1Api
 from polyaxon_sdk.api.auth_v1_api import AuthV1Api
 from polyaxon_sdk.api.connections_v1_api import ConnectionsV1Api
 from polyaxon_sdk.api.dashboards_v1_api import DashboardsV1Api
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/__init__.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/agents_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/agents_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/artifacts_stores_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/artifacts_stores_v1_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/auth_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/auth_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/connections_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/connections_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/dashboards_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/dashboards_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/organizations_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/organizations_v1_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -1159,26 +1159,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_organization_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
+    def delete_organization_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> None:  # noqa: E501
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
@@ -1191,26 +1191,26 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.delete_organization_member_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_organization_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def delete_organization_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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
@@ -2003,26 +2003,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_organization_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> V1OrganizationMember:  # noqa: E501
+    def get_organization_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> V1OrganizationMember:  # noqa: E501
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
@@ -2035,26 +2035,26 @@
                  returns the request thread.
         :rtype: V1OrganizationMember
         """
         kwargs['_return_http_data_only'] = True
         return self.get_organization_member_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_organization_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def get_organization_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/policies_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/policies_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/presets_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/presets_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/project_dashboards_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/project_dashboards_v1_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -41,26 +41,26 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_project_dashboard(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs) -> V1Dashboard:  # noqa: E501
+    def create_project_dashboard(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs) -> V1Dashboard:  # noqa: E501
         """Create project dashboard  # noqa: E501
 
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
@@ -75,26 +75,26 @@
                  returns the request thread.
         :rtype: V1Dashboard
         """
         kwargs['_return_http_data_only'] = True
         return self.create_project_dashboard_with_http_info(owner, project, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_project_dashboard_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs):  # noqa: E501
+    def create_project_dashboard_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs):  # noqa: E501
         """Create project dashboard  # noqa: E501
 
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
@@ -924,26 +924,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def patch_project_dashboard(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], dashboard_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs) -> V1Dashboard:  # noqa: E501
+    def patch_project_dashboard(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], dashboard_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs) -> V1Dashboard:  # noqa: E501
         """Patch project dashboard  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -960,26 +960,26 @@
                  returns the request thread.
         :rtype: V1Dashboard
         """
         kwargs['_return_http_data_only'] = True
         return self.patch_project_dashboard_with_http_info(owner, project, dashboard_uuid, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def patch_project_dashboard_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], dashboard_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs):  # noqa: E501
+    def patch_project_dashboard_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], dashboard_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs):  # noqa: E501
         """Patch project dashboard  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -1248,26 +1248,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_project_dashboard(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], dashboard_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs) -> V1Dashboard:  # noqa: E501
+    def update_project_dashboard(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], dashboard_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs) -> V1Dashboard:  # noqa: E501
         """Update project dashboard  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -1284,26 +1284,26 @@
                  returns the request thread.
         :rtype: V1Dashboard
         """
         kwargs['_return_http_data_only'] = True
         return self.update_project_dashboard_with_http_info(owner, project, dashboard_uuid, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_project_dashboard_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], dashboard_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs):  # noqa: E501
+    def update_project_dashboard_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], dashboard_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Dashboard, Field(..., description="Dashboard body")], **kwargs):  # noqa: E501
         """Update project dashboard  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/project_searches_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/project_searches_v1_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -41,26 +41,26 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_project_search(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs) -> V1Search:  # noqa: E501
+    def create_project_search(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs) -> V1Search:  # noqa: E501
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
@@ -75,26 +75,26 @@
                  returns the request thread.
         :rtype: V1Search
         """
         kwargs['_return_http_data_only'] = True
         return self.create_project_search_with_http_info(owner, project, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_project_search_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs):  # noqa: E501
+    def create_project_search_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs):  # noqa: E501
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
@@ -924,26 +924,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def patch_project_search(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], search_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs) -> V1Search:  # noqa: E501
+    def patch_project_search(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], search_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs) -> V1Search:  # noqa: E501
         """Patch project search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -960,26 +960,26 @@
                  returns the request thread.
         :rtype: V1Search
         """
         kwargs['_return_http_data_only'] = True
         return self.patch_project_search_with_http_info(owner, project, search_uuid, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def patch_project_search_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], search_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs):  # noqa: E501
+    def patch_project_search_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], search_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs):  # noqa: E501
         """Patch project search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -1248,26 +1248,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_project_search(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], search_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs) -> V1Search:  # noqa: E501
+    def update_project_search(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], search_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs) -> V1Search:  # noqa: E501
         """Update project search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -1284,26 +1284,26 @@
                  returns the request thread.
         :rtype: V1Search
         """
         kwargs['_return_http_data_only'] = True
         return self.update_project_search_with_http_info(owner, project, search_uuid, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_project_search_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], search_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs):  # noqa: E501
+    def update_project_search_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namespace")], search_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Search, Field(..., description="Search body")], **kwargs):  # noqa: E501
         """Update project search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/projects_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/projects_v1_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -48,26 +48,26 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def archive_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
+    def archive_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> None:  # noqa: E501
         """Archive project  # noqa: E501
 
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
@@ -80,26 +80,26 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.archive_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def archive_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def archive_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
         """Archive project  # noqa: E501
 
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
@@ -192,26 +192,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def bookmark_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
+    def bookmark_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> None:  # noqa: E501
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
@@ -224,26 +224,26 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.bookmark_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def bookmark_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def bookmark_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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
@@ -492,14 +492,178 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def create_team_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team")], body : Annotated[V1Project, Field(..., description="Project body")], **kwargs) -> V1Project:  # noqa: E501
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
+        kwargs['_return_http_data_only'] = True
+        return self.create_team_project_with_http_info(owner, team, body, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def create_team_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team")], body : Annotated[V1Project, Field(..., description="Project body")], **kwargs):  # noqa: E501
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
+        _all_params = [
+            'owner',
+            'team',
+            'body'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_team_project" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['owner']:
+            _path_params['owner'] = _params['owner']
+
+        if _params['team']:
+            _path_params['team'] = _params['team']
+
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['body']:
+            _body_params = _params['body']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKey']  # noqa: E501
+
+        _response_types_map = {
+            '200': "V1Project",
+            '204': "object",
+            '403': "object",
+            '404': "object",
+        }
+
+        return self.api_client.call_api(
+            '/api/v1/{owner}/{team}/projects/create', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def create_version(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project name")], version_kind : Annotated[StrictStr, Field(..., description="Optional kind to tell the kind of this version")], body : Annotated[V1ProjectVersion, Field(..., description="Project version body")], **kwargs) -> V1ProjectVersion:  # noqa: E501
         """Create version  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_version(owner, project, version_kind, body, async_req=True)
@@ -844,26 +1008,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
+    def delete_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> None:  # noqa: E501
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
@@ -876,26 +1040,26 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.delete_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def delete_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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
@@ -1148,26 +1312,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def disable_project_ci(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
+    def disable_project_ci(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> None:  # noqa: E501
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
@@ -1180,26 +1344,26 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.disable_project_ci_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def disable_project_ci_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def disable_project_ci_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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
@@ -1292,26 +1456,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def enable_project_ci(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
+    def enable_project_ci(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> None:  # noqa: E501
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
@@ -1324,26 +1488,26 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.enable_project_ci_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def enable_project_ci_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def enable_project_ci_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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
@@ -1436,26 +1600,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> V1Project:  # noqa: E501
+    def get_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> V1Project:  # noqa: E501
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
@@ -1468,26 +1632,26 @@
                  returns the request thread.
         :rtype: V1Project
         """
         kwargs['_return_http_data_only'] = True
         return self.get_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def get_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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
@@ -1790,26 +1954,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_project_settings(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> V1ProjectSettings:  # noqa: E501
+    def get_project_settings(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> V1ProjectSettings:  # noqa: E501
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
@@ -1822,26 +1986,26 @@
                  returns the request thread.
         :rtype: V1ProjectSettings
         """
         kwargs['_return_http_data_only'] = True
         return self.get_project_settings_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_project_settings_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def get_project_settings_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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
@@ -3254,26 +3418,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_version_names(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], kind : Annotated[StrictStr, Field(..., description="Version Kind")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListProjectVersionsResponse:  # noqa: E501
+    def list_version_names(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], kind : Annotated[StrictStr, Field(..., description="Version Kind")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListProjectVersionsResponse:  # noqa: E501
         """List versions names  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -3298,26 +3462,26 @@
                  returns the request thread.
         :rtype: V1ListProjectVersionsResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.list_version_names_with_http_info(owner, entity, kind, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_version_names_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], kind : Annotated[StrictStr, Field(..., description="Version Kind")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def list_version_names_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], kind : Annotated[StrictStr, Field(..., description="Version Kind")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """List versions names  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -3451,26 +3615,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_versions(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], kind : Annotated[StrictStr, Field(..., description="Version Kind")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListProjectVersionsResponse:  # noqa: E501
+    def list_versions(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], kind : Annotated[StrictStr, Field(..., description="Version Kind")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListProjectVersionsResponse:  # noqa: E501
         """List versions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -3495,26 +3659,26 @@
                  returns the request thread.
         :rtype: V1ListProjectVersionsResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.list_versions_with_http_info(owner, entity, kind, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_versions_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], kind : Annotated[StrictStr, Field(..., description="Version Kind")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def list_versions_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], kind : Annotated[StrictStr, Field(..., description="Version Kind")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """List versions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -4156,26 +4320,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def restore_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
+    def restore_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> None:  # noqa: E501
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
@@ -4188,26 +4352,26 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.restore_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def restore_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def restore_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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
@@ -4475,26 +4639,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def unbookmark_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
+    def unbookmark_project(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs) -> None:  # noqa: E501
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
@@ -4507,26 +4671,26 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.unbookmark_project_with_http_info(owner, name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def unbookmark_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
+    def unbookmark_project_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namespace")], **kwargs):  # noqa: E501
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

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/queues_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/queues_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/runs_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/runs_v1_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -215,27 +215,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def approve_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
+    def approve_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
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
@@ -246,30 +246,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.approve_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.approve_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def approve_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
+    def approve_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
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
@@ -292,15 +292,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -324,16 +324,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -357,15 +357,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/approve', 'POST',
+            '/api/v1/{owner}/{name}/runs/approve', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -526,27 +526,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def archive_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
+    def archive_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
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
@@ -557,30 +557,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.archive_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.archive_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def archive_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
+    def archive_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
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
@@ -603,15 +603,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -635,16 +635,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -668,15 +668,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/archive', 'POST',
+            '/api/v1/{owner}/{name}/runs/archive', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -837,27 +837,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def bookmark_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
+    def bookmark_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
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
@@ -868,30 +868,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.bookmark_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.bookmark_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def bookmark_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
+    def bookmark_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
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
@@ -914,15 +914,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -946,16 +946,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -979,15 +979,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/bookmark', 'POST',
+            '/api/v1/{owner}/{name}/runs/bookmark', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2511,27 +2511,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
+    def delete_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
         """Delete runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_runs(owner, project, body, async_req=True)
+        >>> thread = api.delete_runs(owner, name, body, async_req=True)
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
@@ -2542,30 +2542,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.delete_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
+    def delete_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
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
@@ -2588,15 +2588,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -2620,16 +2620,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -2653,15 +2653,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/delete', 'DELETE',
+            '/api/v1/{owner}/{name}/runs/delete', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -3779,26 +3779,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_run_artifacts_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunArtifactsResponse:  # noqa: E501
+    def get_run_artifacts_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunArtifactsResponse:  # noqa: E501
         """Get run artifacts lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -3823,26 +3823,26 @@
                  returns the request thread.
         :rtype: V1ListRunArtifactsResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.get_run_artifacts_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_run_artifacts_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def get_run_artifacts_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """Get run artifacts lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -3976,26 +3976,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_run_artifacts_lineage_names(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunArtifactsResponse:  # noqa: E501
+    def get_run_artifacts_lineage_names(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunArtifactsResponse:  # noqa: E501
         """Get run artifacts lineage names  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -4020,26 +4020,26 @@
                  returns the request thread.
         :rtype: V1ListRunArtifactsResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.get_run_artifacts_lineage_names_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_run_artifacts_lineage_names_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def get_run_artifacts_lineage_names_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """Get run artifacts lineage names  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -4354,26 +4354,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_run_clones_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunsResponse:  # noqa: E501
+    def get_run_clones_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunsResponse:  # noqa: E501
         """Get run clones lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -4398,26 +4398,26 @@
                  returns the request thread.
         :rtype: V1ListRunsResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.get_run_clones_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_run_clones_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def get_run_clones_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """Get run clones lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -4551,26 +4551,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_run_connections_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunConnectionsResponse:  # noqa: E501
+    def get_run_connections_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunConnectionsResponse:  # noqa: E501
         """Get run connections lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -4595,26 +4595,26 @@
                  returns the request thread.
         :rtype: V1ListRunConnectionsResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.get_run_connections_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_run_connections_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def get_run_connections_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """Get run connections lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -4748,26 +4748,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_run_downstream_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunEdgesResponse:  # noqa: E501
+    def get_run_downstream_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunEdgesResponse:  # noqa: E501
         """Get run downstream lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -4792,26 +4792,26 @@
                  returns the request thread.
         :rtype: V1ListRunEdgesResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.get_run_downstream_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_run_downstream_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def get_run_downstream_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """Get run downstream lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -5893,26 +5893,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_run_stats(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Stats Mode.")] = None, kind : Annotated[Optional[StrictStr], Field(description="Stats Kind.")] = None, aggregate : Annotated[Optional[StrictStr], Field(description="Stats aggregate.")] = None, groupby : Annotated[Optional[StrictStr], Field(description="Stats group.")] = None, trunc : Annotated[Optional[StrictStr], Field(description="Stats trunc.")] = None, **kwargs) -> object:  # noqa: E501
+    def get_run_stats(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Stats Mode.")] = None, kind : Annotated[Optional[StrictStr], Field(description="Stats Kind.")] = None, aggregate : Annotated[Optional[StrictStr], Field(description="Stats aggregate.")] = None, groupby : Annotated[Optional[StrictStr], Field(description="Stats group.")] = None, trunc : Annotated[Optional[StrictStr], Field(description="Stats trunc.")] = None, **kwargs) -> object:  # noqa: E501
         """Get run stats  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -5947,26 +5947,26 @@
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
         return self.get_run_stats_with_http_info(owner, entity, uuid, offset, limit, sort, query, bookmarks, mode, kind, aggregate, groupby, trunc, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_run_stats_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Stats Mode.")] = None, kind : Annotated[Optional[StrictStr], Field(description="Stats Kind.")] = None, aggregate : Annotated[Optional[StrictStr], Field(description="Stats aggregate.")] = None, groupby : Annotated[Optional[StrictStr], Field(description="Stats group.")] = None, trunc : Annotated[Optional[StrictStr], Field(description="Stats trunc.")] = None, **kwargs):  # noqa: E501
+    def get_run_stats_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Stats Mode.")] = None, kind : Annotated[Optional[StrictStr], Field(description="Stats Kind.")] = None, aggregate : Annotated[Optional[StrictStr], Field(description="Stats aggregate.")] = None, groupby : Annotated[Optional[StrictStr], Field(description="Stats group.")] = None, trunc : Annotated[Optional[StrictStr], Field(description="Stats trunc.")] = None, **kwargs):  # noqa: E501
         """Get run stats  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -6287,26 +6287,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_run_upstream_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunEdgesResponse:  # noqa: E501
+    def get_run_upstream_lineage(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListRunEdgesResponse:  # noqa: E501
         """Get run upstream lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -6331,26 +6331,26 @@
                  returns the request thread.
         :rtype: V1ListRunEdgesResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.get_run_upstream_lineage_with_http_info(owner, entity, uuid, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_run_upstream_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namesapce")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def get_run_upstream_lineage_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], entity : Annotated[StrictStr, Field(..., description="Entity name under namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """Get run upstream lineage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
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
@@ -7211,27 +7211,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def invalidate_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
+    def invalidate_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
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
@@ -7242,30 +7242,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.invalidate_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.invalidate_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def invalidate_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
+    def invalidate_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
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
@@ -7288,15 +7288,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -7320,16 +7320,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -7353,15 +7353,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/invalidate', 'POST',
+            '/api/v1/{owner}/{name}/runs/invalidate', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -8608,27 +8608,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def restore_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
+    def restore_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
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
@@ -8639,30 +8639,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.restore_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.restore_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def restore_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
+    def restore_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
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
@@ -8685,15 +8685,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -8717,16 +8717,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -8750,15 +8750,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/restore', 'POST',
+            '/api/v1/{owner}/{name}/runs/restore', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -9258,27 +9258,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def skip_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
+    def skip_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
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
@@ -9289,30 +9289,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.skip_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.skip_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def skip_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
+    def skip_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
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
@@ -9335,15 +9335,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -9367,16 +9367,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -9400,15 +9400,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/skip', 'POST',
+            '/api/v1/{owner}/{name}/runs/skip', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -9569,27 +9569,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def stop_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
+    def stop_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs) -> None:  # noqa: E501
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
@@ -9600,30 +9600,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.stop_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.stop_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def stop_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
+    def stop_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1Uuids, Field(..., description="Uuids of the entities")], **kwargs):  # noqa: E501
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
@@ -9646,15 +9646,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -9678,16 +9678,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -9711,15 +9711,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/stop', 'POST',
+            '/api/v1/{owner}/{name}/runs/stop', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -9887,27 +9887,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def tag_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1EntitiesTags, Field(..., description="Data")], **kwargs) -> None:  # noqa: E501
+    def tag_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1EntitiesTags, Field(..., description="Data")], **kwargs) -> None:  # noqa: E501
         """Tag runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.tag_runs(owner, project, body, async_req=True)
+        >>> thread = api.tag_runs(owner, name, body, async_req=True)
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
@@ -9918,30 +9918,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.tag_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.tag_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def tag_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1EntitiesTags, Field(..., description="Data")], **kwargs):  # noqa: E501
+    def tag_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1EntitiesTags, Field(..., description="Data")], **kwargs):  # noqa: E501
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
@@ -9964,15 +9964,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -9996,16 +9996,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -10029,15 +10029,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/tag', 'POST',
+            '/api/v1/{owner}/{name}/runs/tag', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -10213,27 +10213,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def transfer_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1EntitiesTransfer, Field(..., description="Data")], **kwargs) -> None:  # noqa: E501
+    def transfer_runs(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1EntitiesTransfer, Field(..., description="Data")], **kwargs) -> None:  # noqa: E501
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
@@ -10244,30 +10244,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.transfer_runs_with_http_info(owner, project, body, **kwargs)  # noqa: E501
+        return self.transfer_runs_with_http_info(owner, name, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def transfer_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project under namesapce")], body : Annotated[V1EntitiesTransfer, Field(..., description="Data")], **kwargs):  # noqa: E501
+    def transfer_runs_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity under namespace")], body : Annotated[V1EntitiesTransfer, Field(..., description="Data")], **kwargs):  # noqa: E501
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
@@ -10290,15 +10290,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'owner',
-            'project',
+            'name',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -10322,16 +10322,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['owner']:
             _path_params['owner'] = _params['owner']
 
-        if _params['project']:
-            _path_params['project'] = _params['project']
+        if _params['name']:
+            _path_params['name'] = _params['name']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -10355,15 +10355,15 @@
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/{owner}/{project}/runs/transfer', 'POST',
+            '/api/v1/{owner}/{name}/runs/transfer', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/schemas_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/schemas_v1_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/searches_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/searches_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/service_accounts_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/service_accounts_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -1162,28 +1162,28 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_service_account_tokens(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], entity : Annotated[Optional[StrictStr], Field(description="Entity name under namesapce.")] = None, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListTokenResponse:  # noqa: E501
+    def list_service_account_tokens(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], entity : Annotated[Optional[StrictStr], Field(description="Entity name under namespace.")] = None, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListTokenResponse:  # noqa: E501
         """List service account tokens  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
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
@@ -1206,28 +1206,28 @@
                  returns the request thread.
         :rtype: V1ListTokenResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.list_service_account_tokens_with_http_info(owner, uuid, entity, offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_service_account_tokens_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], entity : Annotated[Optional[StrictStr], Field(description="Entity name under namesapce.")] = None, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+    def list_service_account_tokens_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], uuid : Annotated[StrictStr, Field(..., description="SubEntity uuid")], entity : Annotated[Optional[StrictStr], Field(description="Entity name under namespace.")] = None, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
         """List service account tokens  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
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

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/tags_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/tags_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/teams_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/users_v1_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,97 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr
 
-from typing import Optional
+from typing import Any, Dict, Optional
 
-from polyaxon_sdk.models.v1_list_team_members_response import V1ListTeamMembersResponse
-from polyaxon_sdk.models.v1_list_teams_response import V1ListTeamsResponse
-from polyaxon_sdk.models.v1_team import V1Team
-from polyaxon_sdk.models.v1_team_member import V1TeamMember
+from polyaxon_sdk.models.v1_list_activities_response import V1ListActivitiesResponse
+from polyaxon_sdk.models.v1_list_token_response import V1ListTokenResponse
+from polyaxon_sdk.models.v1_token import V1Token
+from polyaxon_sdk.models.v1_user import V1User
 
 from polyaxon_sdk.api_client import ApiClient
 from polyaxon_sdk.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class TeamsV1Api(object):
+class UsersV1Api(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_team(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], body : Annotated[V1Team, Field(..., description="Team body")], **kwargs) -> V1Team:  # noqa: E501
-        """Create team  # noqa: E501
+    def create_token(self, body : Annotated[V1Token, Field(..., description="Token body")], **kwargs) -> V1Token:  # noqa: E501
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
         kwargs['_return_http_data_only'] = True
-        return self.create_team_with_http_info(owner, body, **kwargs)  # noqa: E501
+        return self.create_token_with_http_info(body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_team_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], body : Annotated[V1Team, Field(..., description="Team body")], **kwargs):  # noqa: E501
-        """Create team  # noqa: E501
+    def create_token_with_http_info(self, body : Annotated[V1Token, Field(..., description="Token body")], **kwargs):  # noqa: E501
+        """Create token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_team_with_http_info(owner, body, async_req=True)
+        >>> thread = api.create_token_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param body: Team body (required)
-        :type body: V1Team
+        :param body: Token body (required)
+        :type body: V1Token
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -109,21 +105,20 @@
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
 
         _all_params = [
-            'owner',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -135,26 +130,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_team" % _key
+                    " to method create_token" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
@@ -175,22 +167,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1Team",
+            '200': "V1Token",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams', 'POST',
+            '/api/v1/users/tokens', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -199,63 +191,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_team_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team")], body : Annotated[V1TeamMember, Field(..., description="Team body")], **kwargs) -> V1TeamMember:  # noqa: E501
-        """Create team member  # noqa: E501
+    def delete_token(self, uuid : Annotated[StrictStr, Field(..., description="UUid of the namespace")], **kwargs) -> None:  # noqa: E501
+        """Delete token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_team_member(owner, team, body, async_req=True)
+        >>> thread = api.delete_token(uuid, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team (required)
-        :type team: str
-        :param body: Team body (required)
-        :type body: V1TeamMember
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
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_team_member_with_http_info(owner, team, body, **kwargs)  # noqa: E501
+        return self.delete_token_with_http_info(uuid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_team_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team")], body : Annotated[V1TeamMember, Field(..., description="Team body")], **kwargs):  # noqa: E501
-        """Create team member  # noqa: E501
+    def delete_token_with_http_info(self, uuid : Annotated[StrictStr, Field(..., description="UUid of the namespace")], **kwargs):  # noqa: E501
+        """Delete token  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_team_member_with_http_info(owner, team, body, async_req=True)
+        >>> thread = api.delete_token_with_http_info(uuid, async_req=True)
         >>> result = thread.get()
 
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team (required)
-        :type team: str
-        :param body: Team body (required)
-        :type body: V1TeamMember
+        :param uuid: UUid of the namespace (required)
+        :type uuid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -269,23 +253,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1TeamMember, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'owner',
-            'team',
-            'body'
+            'uuid'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -296,65 +278,47 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_team_member" % _key
+                    " to method delete_token" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['team']:
-            _path_params['team'] = _params['team']
+        if _params['uuid']:
+            _path_params['uuid'] = _params['uuid']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['body']:
-            _body_params = _params['body']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
-        _response_types_map = {
-            '200': "V1TeamMember",
-            '204': "object",
-            '403': "object",
-            '404': "object",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{team}/members', 'POST',
+            '/api/v1/users/tokens/{uuid}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -363,59 +327,71 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_team(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> None:  # noqa: E501
-        """Delete team  # noqa: E501
+    def get_history(self, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListActivitiesResponse:  # noqa: E501
+        """User History  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_team(owner, name, async_req=True)
+        >>> thread = api.get_history(offset, limit, sort, query, no_page, async_req=True)
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
-        :rtype: None
+        :rtype: V1ListActivitiesResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_team_with_http_info(owner, name, **kwargs)  # noqa: E501
+        return self.get_history_with_http_info(offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_team_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
-        """Delete team  # noqa: E501
+    def get_history_with_http_info(self, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
+        """User History  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_team_with_http_info(owner, name, async_req=True)
+        >>> thread = api.get_history_with_http_info(offset, limit, sort, query, no_page, async_req=True)
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
@@ -429,22 +405,25 @@
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
 
         _all_params = [
-            'owner',
-            'name'
+            'offset',
+            'limit',
+            'sort',
+            'query',
+            'no_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -455,202 +434,64 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_team" % _key
+                    " to method get_history" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['name']:
-            _path_params['name'] = _params['name']
-
 
         # process the query parameters
         _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['ApiKey']  # noqa: E501
-
-        _response_types_map = {}
-
-        return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{name}', 'DELETE',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def delete_team_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team under namesapce")], user : Annotated[StrictStr, Field(..., description="Member under team")], **kwargs) -> None:  # noqa: E501
-        """Delete team member details  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.delete_team_member(owner, team, user, async_req=True)
-        >>> result = thread.get()
-
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team under namesapce (required)
-        :type team: str
-        :param user: Member under team (required)
-        :type user: str
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
-        :rtype: None
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.delete_team_member_with_http_info(owner, team, user, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def delete_team_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team under namesapce")], user : Annotated[StrictStr, Field(..., description="Member under team")], **kwargs):  # noqa: E501
-        """Delete team member details  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.delete_team_member_with_http_info(owner, team, user, async_req=True)
-        >>> result = thread.get()
-
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param team: Team under namesapce (required)
-        :type team: str
-        :param user: Member under team (required)
-        :type user: str
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
-        :rtype: None
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'owner',
-            'team',
-            'user'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method delete_team_member" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
+        if _params.get('offset') is not None:  # noqa: E501
+            _query_params.append(('offset', _params['offset']))
 
-        # process the path parameters
-        _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
+        if _params.get('limit') is not None:  # noqa: E501
+            _query_params.append(('limit', _params['limit']))
 
-        if _params['team']:
-            _path_params['team'] = _params['team']
+        if _params.get('sort') is not None:  # noqa: E501
+            _query_params.append(('sort', _params['sort']))
 
-        if _params['user']:
-            _path_params['user'] = _params['user']
+        if _params.get('query') is not None:  # noqa: E501
+            _query_params.append(('query', _params['query']))
 
+        if _params.get('no_page') is not None:  # noqa: E501
+            _query_params.append(('no_page', _params['no_page']))
 
-        # process the query parameters
-        _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "V1ListActivitiesResponse",
+            '204': "object",
+            '403': "object",
+            '404': "object",
+        }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{team}/members/{user}', 'DELETE',
+            '/api/v1/users/history', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -659,59 +500,71 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_team(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs) -> V1Team:  # noqa: E501
-        """Get team  # noqa: E501
+    def get_suggestions(self, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> object:  # noqa: E501
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
         kwargs['_return_http_data_only'] = True
-        return self.get_team_with_http_info(owner, name, **kwargs)  # noqa: E501
+        return self.get_suggestions_with_http_info(offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_team_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Component under namesapce")], **kwargs):  # noqa: E501
-        """Get team  # noqa: E501
+    def get_suggestions_with_http_info(self, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
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
@@ -725,22 +578,25 @@
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
 
         _all_params = [
-            'owner',
-            'name'
+            'offset',
+            'limit',
+            'sort',
+            'query',
+            'no_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -751,32 +607,41 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_team" % _key
+                    " to method get_suggestions" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['name']:
-            _path_params['name'] = _params['name']
-
 
         # process the query parameters
         _query_params = []
+        if _params.get('offset') is not None:  # noqa: E501
+            _query_params.append(('offset', _params['offset']))
+
+        if _params.get('limit') is not None:  # noqa: E501
+            _query_params.append(('limit', _params['limit']))
+
+        if _params.get('sort') is not None:  # noqa: E501
+            _query_params.append(('sort', _params['sort']))
+
+        if _params.get('query') is not None:  # noqa: E501
+            _query_params.append(('query', _params['query']))
+
+        if _params.get('no_page') is not None:  # noqa: E501
+            _query_params.append(('no_page', _params['no_page']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -784,22 +649,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1Team",
+            '200': "object",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{name}', 'GET',
+            '/api/v1/users/suggestions', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -808,63 +673,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_team_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team under namesapce")], user : Annotated[StrictStr, Field(..., description="Member under team")], **kwargs) -> V1TeamMember:  # noqa: E501
-        """Get team member details  # noqa: E501
+    def get_token(self, uuid : Annotated[StrictStr, Field(..., description="UUid of the namespace")], **kwargs) -> V1Token:  # noqa: E501
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
         kwargs['_return_http_data_only'] = True
-        return self.get_team_member_with_http_info(owner, team, user, **kwargs)  # noqa: E501
+        return self.get_token_with_http_info(uuid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_team_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team under namesapce")], user : Annotated[StrictStr, Field(..., description="Member under team")], **kwargs):  # noqa: E501
-        """Get team member details  # noqa: E501
+    def get_token_with_http_info(self, uuid : Annotated[StrictStr, Field(..., description="UUid of the namespace")], **kwargs):  # noqa: E501
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
@@ -878,23 +735,21 @@
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
 
         _all_params = [
-            'owner',
-            'team',
-            'user'
+            'uuid'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -905,31 +760,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_team_member" % _key
+                    " to method get_token" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['team']:
-            _path_params['team'] = _params['team']
-
-        if _params['user']:
-            _path_params['user'] = _params['user']
+        if _params['uuid']:
+            _path_params['uuid'] = _params['uuid']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -941,22 +790,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1TeamMember",
+            '200': "V1Token",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{team}/members/{user}', 'GET',
+            '/api/v1/users/tokens/{uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -965,87 +814,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_team_members(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity managing the resource")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Mode of the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListTeamMembersResponse:  # noqa: E501
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
         kwargs['_return_http_data_only'] = True
-        return self.list_team_members_with_http_info(owner, name, offset, limit, sort, query, bookmarks, mode, no_page, **kwargs)  # noqa: E501
+        return self.get_user_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_team_members_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], name : Annotated[StrictStr, Field(..., description="Entity managing the resource")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Mode of the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
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
@@ -1059,29 +872,20 @@
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
 
         _all_params = [
-            'owner',
-            'name',
-            'offset',
-            'limit',
-            'sort',
-            'query',
-            'bookmarks',
-            'mode',
-            'no_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1092,53 +896,26 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_team_members" % _key
+                    " to method get_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['name']:
-            _path_params['name'] = _params['name']
-
 
         # process the query parameters
         _query_params = []
-        if _params.get('offset') is not None:  # noqa: E501
-            _query_params.append(('offset', _params['offset']))
-
-        if _params.get('limit') is not None:  # noqa: E501
-            _query_params.append(('limit', _params['limit']))
-
-        if _params.get('sort') is not None:  # noqa: E501
-            _query_params.append(('sort', _params['sort']))
-
-        if _params.get('query') is not None:  # noqa: E501
-            _query_params.append(('query', _params['query']))
-
-        if _params.get('bookmarks') is not None:  # noqa: E501
-            _query_params.append(('bookmarks', _params['bookmarks']))
-
-        if _params.get('mode') is not None:  # noqa: E501
-            _query_params.append(('mode', _params['mode']))
-
-        if _params.get('no_page') is not None:  # noqa: E501
-            _query_params.append(('no_page', _params['no_page']))
-
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -1146,22 +923,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1ListTeamMembersResponse",
+            '200': "V1User",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{name}/members', 'GET',
+            '/api/v1/users', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1170,37 +947,31 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_team_names(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Mode of the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListTeamsResponse:  # noqa: E501
-        """List teams names  # noqa: E501
+    def get_workspaces(self, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> object:  # noqa: E501
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
@@ -1208,43 +979,37 @@
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
         kwargs['_return_http_data_only'] = True
-        return self.list_team_names_with_http_info(owner, offset, limit, sort, query, bookmarks, mode, no_page, **kwargs)  # noqa: E501
+        return self.get_workspaces_with_http_info(offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_team_names_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Mode of the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
-        """List teams names  # noqa: E501
+    def get_workspaces_with_http_info(self, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
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
@@ -1260,27 +1025,24 @@
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
 
         _all_params = [
-            'owner',
             'offset',
             'limit',
             'sort',
             'query',
-            'bookmarks',
-            'mode',
             'no_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1292,26 +1054,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_team_names" % _key
+                    " to method get_workspaces" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
 
         # process the query parameters
         _query_params = []
         if _params.get('offset') is not None:  # noqa: E501
             _query_params.append(('offset', _params['offset']))
 
         if _params.get('limit') is not None:  # noqa: E501
@@ -1319,20 +1078,14 @@
 
         if _params.get('sort') is not None:  # noqa: E501
             _query_params.append(('sort', _params['sort']))
 
         if _params.get('query') is not None:  # noqa: E501
             _query_params.append(('query', _params['query']))
 
-        if _params.get('bookmarks') is not None:  # noqa: E501
-            _query_params.append(('bookmarks', _params['bookmarks']))
-
-        if _params.get('mode') is not None:  # noqa: E501
-            _query_params.append(('mode', _params['mode']))
-
         if _params.get('no_page') is not None:  # noqa: E501
             _query_params.append(('no_page', _params['no_page']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
@@ -1343,22 +1096,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1ListTeamsResponse",
+            '200': "object",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/names', 'GET',
+            '/api/v1/users/workspaces', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1367,37 +1120,31 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_teams(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Mode of the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListTeamsResponse:  # noqa: E501
-        """List teams  # noqa: E501
+    def list_tokens(self, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs) -> V1ListTokenResponse:  # noqa: E501
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
@@ -1405,43 +1152,37 @@
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
         kwargs['_return_http_data_only'] = True
-        return self.list_teams_with_http_info(owner, offset, limit, sort, query, bookmarks, mode, no_page, **kwargs)  # noqa: E501
+        return self.list_tokens_with_http_info(offset, limit, sort, query, no_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_teams_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, bookmarks : Annotated[Optional[StrictBool], Field(description="Filter by bookmarks.")] = None, mode : Annotated[Optional[StrictStr], Field(description="Mode of the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
-        """List teams  # noqa: E501
+    def list_tokens_with_http_info(self, offset : Annotated[Optional[StrictInt], Field(description="Pagination offset.")] = None, limit : Annotated[Optional[StrictInt], Field(description="Limit size.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort to order the search.")] = None, query : Annotated[Optional[StrictStr], Field(description="Query filter the search.")] = None, no_page : Annotated[Optional[StrictBool], Field(description="No pagination.")] = None, **kwargs):  # noqa: E501
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
@@ -1457,27 +1198,24 @@
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
 
         _all_params = [
-            'owner',
             'offset',
             'limit',
             'sort',
             'query',
-            'bookmarks',
-            'mode',
             'no_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1489,26 +1227,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_teams" % _key
+                    " to method list_tokens" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
 
         # process the query parameters
         _query_params = []
         if _params.get('offset') is not None:  # noqa: E501
             _query_params.append(('offset', _params['offset']))
 
         if _params.get('limit') is not None:  # noqa: E501
@@ -1516,20 +1251,14 @@
 
         if _params.get('sort') is not None:  # noqa: E501
             _query_params.append(('sort', _params['sort']))
 
         if _params.get('query') is not None:  # noqa: E501
             _query_params.append(('query', _params['query']))
 
-        if _params.get('bookmarks') is not None:  # noqa: E501
-            _query_params.append(('bookmarks', _params['bookmarks']))
-
-        if _params.get('mode') is not None:  # noqa: E501
-            _query_params.append(('mode', _params['mode']))
-
         if _params.get('no_page') is not None:  # noqa: E501
             _query_params.append(('no_page', _params['no_page']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
@@ -1540,22 +1269,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1ListTeamsResponse",
+            '200': "V1ListTokenResponse",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams', 'GET',
+            '/api/v1/users/tokens', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1564,63 +1293,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def patch_team(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team_name : Annotated[StrictStr, Field(..., description="Name")], body : Annotated[V1Team, Field(..., description="Team body")], **kwargs) -> V1Team:  # noqa: E501
-        """Patch team  # noqa: E501
+    def patch_token(self, token_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Token, Field(..., description="Token body")], **kwargs) -> V1Token:  # noqa: E501
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
         kwargs['_return_http_data_only'] = True
-        return self.patch_team_with_http_info(owner, team_name, body, **kwargs)  # noqa: E501
+        return self.patch_token_with_http_info(token_uuid, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def patch_team_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team_name : Annotated[StrictStr, Field(..., description="Name")], body : Annotated[V1Team, Field(..., description="Team body")], **kwargs):  # noqa: E501
-        """Patch team  # noqa: E501
+    def patch_token_with_http_info(self, token_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Token, Field(..., description="Token body")], **kwargs):  # noqa: E501
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
@@ -1634,22 +1359,21 @@
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
 
         _all_params = [
-            'owner',
-            'team_name',
+            'token_uuid',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1661,28 +1385,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method patch_team" % _key
+                    " to method patch_token" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['team_name']:
-            _path_params['team.name'] = _params['team_name']
+        if _params['token_uuid']:
+            _path_params['token.uuid'] = _params['token_uuid']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -1704,22 +1425,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1Team",
+            '200': "V1Token",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{team.name}', 'PATCH',
+            '/api/v1/users/tokens/{token.uuid}', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1728,67 +1449,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def patch_team_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team")], member_user : Annotated[StrictStr, Field(..., description="User")], body : Annotated[V1TeamMember, Field(..., description="Team body")], **kwargs) -> V1TeamMember:  # noqa: E501
-        """Patch team member  # noqa: E501
+    def patch_user(self, body : V1User, **kwargs) -> V1User:  # noqa: E501
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
         kwargs['_return_http_data_only'] = True
-        return self.patch_team_member_with_http_info(owner, team, member_user, body, **kwargs)  # noqa: E501
+        return self.patch_user_with_http_info(body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def patch_team_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team")], member_user : Annotated[StrictStr, Field(..., description="User")], body : Annotated[V1TeamMember, Field(..., description="Team body")], **kwargs):  # noqa: E501
-        """Patch team member  # noqa: E501
+    def patch_user_with_http_info(self, body : V1User, **kwargs):  # noqa: E501
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
@@ -1802,23 +1511,20 @@
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
 
         _all_params = [
-            'owner',
-            'team',
-            'member_user',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1830,32 +1536,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method patch_team_member" % _key
+                    " to method patch_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['team']:
-            _path_params['team'] = _params['team']
-
-        if _params['member_user']:
-            _path_params['member.user'] = _params['member_user']
-
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
@@ -1876,22 +1573,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1TeamMember",
+            '200': "V1User",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{team}/members/{member.user}', 'PATCH',
+            '/api/v1/users', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1900,63 +1597,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_team(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team_name : Annotated[StrictStr, Field(..., description="Name")], body : Annotated[V1Team, Field(..., description="Team body")], **kwargs) -> V1Team:  # noqa: E501
-        """Update team  # noqa: E501
+    def update_token(self, token_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Token, Field(..., description="Token body")], **kwargs) -> V1Token:  # noqa: E501
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
         kwargs['_return_http_data_only'] = True
-        return self.update_team_with_http_info(owner, team_name, body, **kwargs)  # noqa: E501
+        return self.update_token_with_http_info(token_uuid, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_team_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team_name : Annotated[StrictStr, Field(..., description="Name")], body : Annotated[V1Team, Field(..., description="Team body")], **kwargs):  # noqa: E501
-        """Update team  # noqa: E501
+    def update_token_with_http_info(self, token_uuid : Annotated[StrictStr, Field(..., description="UUID")], body : Annotated[V1Token, Field(..., description="Token body")], **kwargs):  # noqa: E501
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
@@ -1970,22 +1663,21 @@
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
 
         _all_params = [
-            'owner',
-            'team_name',
+            'token_uuid',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1997,28 +1689,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_team" % _key
+                    " to method update_token" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['team_name']:
-            _path_params['team.name'] = _params['team_name']
+        if _params['token_uuid']:
+            _path_params['token.uuid'] = _params['token_uuid']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -2040,22 +1729,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1Team",
+            '200': "V1Token",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{team.name}', 'PUT',
+            '/api/v1/users/tokens/{token.uuid}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2064,67 +1753,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_team_member(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team")], member_user : Annotated[StrictStr, Field(..., description="User")], body : Annotated[V1TeamMember, Field(..., description="Team body")], **kwargs) -> V1TeamMember:  # noqa: E501
-        """Update team member  # noqa: E501
+    def update_user(self, body : V1User, **kwargs) -> V1User:  # noqa: E501
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
         kwargs['_return_http_data_only'] = True
-        return self.update_team_member_with_http_info(owner, team, member_user, body, **kwargs)  # noqa: E501
+        return self.update_user_with_http_info(body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_team_member_with_http_info(self, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], team : Annotated[StrictStr, Field(..., description="Team")], member_user : Annotated[StrictStr, Field(..., description="User")], body : Annotated[V1TeamMember, Field(..., description="Team body")], **kwargs):  # noqa: E501
-        """Update team member  # noqa: E501
+    def update_user_with_http_info(self, body : V1User, **kwargs):  # noqa: E501
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
@@ -2138,23 +1815,20 @@
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
 
         _all_params = [
-            'owner',
-            'team',
-            'member_user',
             'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -2166,32 +1840,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_team_member" % _key
+                    " to method update_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['team']:
-            _path_params['team'] = _params['team']
-
-        if _params['member_user']:
-            _path_params['member.user'] = _params['member_user']
-
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
@@ -2212,22 +1877,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['ApiKey']  # noqa: E501
 
         _response_types_map = {
-            '200': "V1TeamMember",
+            '200': "V1User",
             '204': "object",
             '403': "object",
             '404': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/orgs/{owner}/teams/{team}/members/{member.user}', 'PUT',
+            '/api/v1/users', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api/versions_v1_api.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api/versions_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/api_client.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.1.8/python'
+        self.user_agent = 'OpenAPI-Generator/2.2.0-rc0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/configuration.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -389,16 +389,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.1.8\n"\
-               "SDK Package Version: 2.1.8".\
+               "Version of the API: 2.2.0-rc0\n"\
+               "SDK Package Version: 2.2.0-rc0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/exceptions.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/__init__.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/agent_state_response_agent_state.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/agent_state_response_agent_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/mx_job_mode.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_pending.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,18 +18,20 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MXJobMode(str, Enum):
+class V1RunPending(str, Enum):
     """
-    MXJobMode
+    V1RunPending
     """
 
     """
     allowed enum values
     """
-    MXTRAIN = 'MXTrain'
-    MXTUNE = 'MXTune'
+    APPROVAL = 'approval'
+    UPLOAD = 'upload'
+    CACHE = 'cache'
+    BUILD = 'build'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/protobuf_any.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/protobuf_any.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/protobuf_null_value.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_project_version_kind.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,17 +18,19 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ProtobufNullValue(str, Enum):
+class V1ProjectVersionKind(str, Enum):
     """
-    `NullValue` is a singleton enumeration to represent the null value for the `Value` type union.   The JSON representation for `NullValue` is JSON `null`.   - NULL_VALUE: Null value.
+    V1ProjectVersionKind
     """
 
     """
     allowed enum values
     """
-    NULL_VALUE = 'NULL_VALUE'
+    COMPONENT = 'component'
+    MODEL = 'model'
+    ARTIFACT = 'artifact'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/runtime_error.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/runtime_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/search_view.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/search_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_activity.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_agent.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_agent_reconcile_body_request.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_agent_reconcile_body_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_agent_state_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_agent_state_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_agent_status_body_request.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_agent_status_body_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_analytics_spec.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_analytics_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_artifact_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_artifact_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_artifact_tree.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_artifact_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_artifacts_mount.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_artifacts_mount.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_artifacts_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_artifacts_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_auth.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_auth_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_auth_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_average_stopping_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_average_stopping_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_bayes.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_bayes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_bucket_connection.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_bucket_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_build.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_cache.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_claim_connection.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_claim_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_clean_pod_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/mx_job_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,19 +18,18 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1CleanPodPolicy(str, Enum):
+class MXJobMode(str, Enum):
     """
-    V1CleanPodPolicy
+    MXJobMode
     """
 
     """
     allowed enum values
     """
-    ALL = 'All'
-    RUNNING = 'Running'
-    NONE = 'None'
+    MXTRAIN = 'MXTrain'
+    MXTUNE = 'MXTune'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_cloning.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_cloning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_cloning_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_pipeline_kind.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,19 +18,18 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1CloningKind(str, Enum):
+class V1PipelineKind(str, Enum):
     """
-    V1CloningKind
+    V1PipelineKind
     """
 
     """
     allowed enum values
     """
-    COPY = 'copy'
-    RESTART = 'restart'
-    CACHE = 'cache'
+    DAG = 'dag'
+    MATRIX = 'matrix'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_compatibility.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_compiled_operation.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_compiled_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_component.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_resource.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_schema.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_connection_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_connection_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_credentials.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_cron_schedule.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_cron_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dag.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dag_ref.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dag_ref.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dashboard.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dashboard_spec.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dashboard_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dask_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dask_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dask_replica.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dask_replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_date_time_schedule.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_date_time_schedule.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_diff_stopping_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_diff_stopping_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_dockerfile_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_dockerfile_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_early_stopping.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_early_stopping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entities_tags.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entities_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entities_transfer.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entities_transfer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entity_notification_body.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entity_notification_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entity_stage_body_request.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entity_stage_body_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_entity_status_body_request.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_entity_status_body_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_environment.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_artifact.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_artifact.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_audio.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_chart.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_chart_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_chart_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_confusion_matrix.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_confusion_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_curve.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_curve_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_curve_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_dataframe.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_histogram.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_histogram.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_image.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_model.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_span.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_span.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_span_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_schedule_kind.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,22 +18,19 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1EventSpanKind(str, Enum):
+class V1ScheduleKind(str, Enum):
     """
-    V1EventSpanKind
+    V1ScheduleKind
     """
 
     """
     allowed enum values
     """
-    LLM = 'llm'
-    CHAIN = 'chain'
-    AGENT = 'agent'
-    TOOL = 'tool'
-    EMBEDDING = 'embedding'
-    RETRIEVER = 'retriever'
+    CRON = 'cron'
+    INTERVAL = 'interval'
+    DATETIME = 'datetime'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_trigger.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_trigger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_event_video.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_video.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_events_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_events_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_failure_early_stopping.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_failure_early_stopping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_file_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_file_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_gcs_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_gcs_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_git_connection.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_git_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_git_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_git_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_grid_search.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_grid_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hook.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_host_connection.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_host_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_host_path_connection.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_host_path_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_choice.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_choice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_date_range.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_date_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_date_time_range.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_date_time_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_geom_space.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_geom_space.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_lin_space.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_lin_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_log_normal.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_log_normal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_log_space.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_log_space.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_log_uniform.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_log_uniform.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_normal.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_normal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_p_choice.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_p_choice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_params.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_q_log_normal.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_q_log_normal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_q_log_uniform.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_uniform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -19,19 +19,19 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
 from pydantic import BaseModel, StrictStr
 
-class V1HpQLogUniform(BaseModel):
+class V1HpUniform(BaseModel):
     """
-    V1HpQLogUniform
+    V1HpUniform
     """
-    kind: Optional[StrictStr] = 'qloguniform'
+    kind: Optional[StrictStr] = 'uniform'
     value: Optional[Dict[str, Any]] = None
     __properties = ["kind", "value"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -40,34 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1HpQLogUniform:
-        """Create an instance of V1HpQLogUniform from a JSON string"""
+    def from_json(cls, json_str: str) -> V1HpUniform:
+        """Create an instance of V1HpUniform from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1HpQLogUniform:
-        """Create an instance of V1HpQLogUniform from a dict"""
+    def from_dict(cls, obj: dict) -> V1HpUniform:
+        """Create an instance of V1HpUniform from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1HpQLogUniform.parse_obj(obj)
+            return V1HpUniform.parse_obj(obj)
 
-        _obj = V1HpQLogUniform.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'qloguniform',
+        _obj = V1HpUniform.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'uniform',
             "value": obj.get("value")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_q_normal.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_q_normal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_q_uniform.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_q_uniform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_range.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_range.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hp_uniform.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_path_ref.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
+from typing import Optional
 from pydantic import BaseModel, StrictStr
 
-class V1HpUniform(BaseModel):
+class V1PathRef(BaseModel):
     """
-    V1HpUniform
+    V1PathRef
     """
-    kind: Optional[StrictStr] = 'uniform'
-    value: Optional[Dict[str, Any]] = None
-    __properties = ["kind", "value"]
+    kind: Optional[StrictStr] = 'path_ref'
+    path: Optional[StrictStr] = None
+    __properties = ["kind", "path"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1HpUniform:
-        """Create an instance of V1HpUniform from a JSON string"""
+    def from_json(cls, json_str: str) -> V1PathRef:
+        """Create an instance of V1PathRef from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1HpUniform:
-        """Create an instance of V1HpUniform from a dict"""
+    def from_dict(cls, obj: dict) -> V1PathRef:
+        """Create an instance of V1PathRef from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1HpUniform.parse_obj(obj)
+            return V1PathRef.parse_obj(obj)
 
-        _obj = V1HpUniform.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'uniform',
-            "value": obj.get("value")
+        _obj = V1PathRef.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'path_ref',
+            "path": obj.get("path")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hub_ref.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hub_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hyperband.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hyperband.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hyperopt.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hyperopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_hyperopt_algorithms.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hyperopt_algorithms.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_init.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_installation.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_installation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_interval_schedule.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_interval_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_io.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_iterative.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_iterative.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_join.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_join.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_join_param.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_join_param.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_kf_replica.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_kf_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_activities_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_activities_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_agents_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_agents_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_bookmarks_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_bookmarks_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_connections_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_connections_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_dashboards_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_dashboards_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_organization_members_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_organization_members_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_organizations_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_organizations_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_policies_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_policies_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_presets_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_presets_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_project_versions_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_project_versions_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_projects_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_projects_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_queues_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_queues_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_run_artifacts_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_run_artifacts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_run_connections_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_run_connections_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_run_edges_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_run_edges_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_runs_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_runs_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_searches_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_searches_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_service_accounts_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_service_accounts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_tags_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_tags_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_team_members_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_team_members_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_teams_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_teams_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_list_token_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_list_token_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_log.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_log_handler.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_log_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_logs.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_managed_by.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_managed_by.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_mapping.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_matrix.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_matrix_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_matrix_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_median_stopping_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_median_stopping_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_metric_early_stopping.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_metric_early_stopping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_mpi_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_mpi_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_multi_events_response.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_multi_events_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_mx_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_mx_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_notification.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_notification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_operation.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_operation_body.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_operation_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_optimization.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_optimization_metric.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_optimization_metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_optimization_resource.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_optimization_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_organization.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_organization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_organization_member.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_organization_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_paddle_elastic_polic.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_paddle_elastic_polic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_paddle_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_paddle_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_param.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_param.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_password_change.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_password_change.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_patch_strategy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_patch_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_path_ref.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_uri_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -17,57 +17,59 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictBool, StrictStr
 
-class V1PathRef(BaseModel):
+class V1UriType(BaseModel):
     """
-    V1PathRef
+    V1UriType
     """
-    kind: Optional[StrictStr] = 'path_ref'
-    path: Optional[StrictStr] = None
-    __properties = ["kind", "path"]
+    user: Optional[StrictStr] = None
+    password: Optional[StrictStr] = None
+    host: Optional[StrictBool] = None
+    __properties = ["user", "password", "host"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1PathRef:
-        """Create an instance of V1PathRef from a JSON string"""
+    def from_json(cls, json_str: str) -> V1UriType:
+        """Create an instance of V1UriType from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1PathRef:
-        """Create an instance of V1PathRef from a dict"""
+    def from_dict(cls, obj: dict) -> V1UriType:
+        """Create an instance of V1UriType from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1PathRef.parse_obj(obj)
+            return V1UriType.parse_obj(obj)
 
-        _obj = V1PathRef.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'path_ref',
-            "path": obj.get("path")
+        _obj = V1UriType.parse_obj({
+            "user": obj.get("user"),
+            "password": obj.get("password"),
+            "host": obj.get("host")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_pipeline.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_pipeline_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_stages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,18 +18,20 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1PipelineKind(str, Enum):
+class V1Stages(str, Enum):
     """
-    V1PipelineKind
+    V1Stages
     """
 
     """
     allowed enum values
     """
-    DAG = 'dag'
-    MATRIX = 'matrix'
+    TESTING = 'testing'
+    STAGING = 'staging'
+    PRODUCTION = 'production'
+    DISABLED = 'disabled'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_plugins.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_polyaxon_init_container.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_polyaxon_init_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_polyaxon_sidecar_container.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_polyaxon_sidecar_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_preset.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_preset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_project.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_project_settings.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_project_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_project_version.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_project_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_project_version_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_cloning_kind.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,19 +18,19 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1ProjectVersionKind(str, Enum):
+class V1CloningKind(str, Enum):
     """
-    V1ProjectVersionKind
+    V1CloningKind
     """
 
     """
     allowed enum values
     """
-    COMPONENT = 'component'
-    MODEL = 'model'
-    ARTIFACT = 'artifact'
+    COPY = 'copy'
+    RESTART = 'restart'
+    CACHE = 'cache'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_pytorch_elastic_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_pytorch_elastic_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_pytorch_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_pytorch_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_queue.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_random_search.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_random_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_ray_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_ray_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_ray_replica.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_ray_replica.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_reference.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_resource_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_resource_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_artifact.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_artifact.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_artifacts.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_artifacts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_connection.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_edge.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_edge_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_edge_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_edge_lineage.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_edge_lineage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_edges_graph.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_edges_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_pending.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_clean_pod_policy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,20 +18,19 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1RunPending(str, Enum):
+class V1CleanPodPolicy(str, Enum):
     """
-    V1RunPending
+    V1CleanPodPolicy
     """
 
     """
     allowed enum values
     """
-    APPROVAL = 'approval'
-    UPLOAD = 'upload'
-    CACHE = 'cache'
-    BUILD = 'build'
+    ALL = 'All'
+    RUNNING = 'Running'
+    NONE = 'None'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_reference_catalog.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_reference_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_resources.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_schema.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_run_settings.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_run_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_s3_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_s3_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_schedule.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_schedule_kind.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_event_span_kind.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,19 +18,22 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1ScheduleKind(str, Enum):
+class V1EventSpanKind(str, Enum):
     """
-    V1ScheduleKind
+    V1EventSpanKind
     """
 
     """
     allowed enum values
     """
-    CRON = 'cron'
-    INTERVAL = 'interval'
-    DATETIME = 'datetime'
+    LLM = 'llm'
+    CHAIN = 'chain'
+    AGENT = 'agent'
+    TOOL = 'tool'
+    EMBEDDING = 'embedding'
+    RETRIEVER = 'retriever'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_scheduling_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_scheduling_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_schemas.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_search.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_search_spec.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_search_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_section_spec.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_section_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_service.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_service_account.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_service_account.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_settings_catalog.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_settings_catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_stage.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_stage_condition.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_stage_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_stages.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/protobuf_null_value.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,20 +18,17 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1Stages(str, Enum):
+class ProtobufNullValue(str, Enum):
     """
-    V1Stages
+    `NullValue` is a singleton enumeration to represent the null value for the `Value` type union.   The JSON representation for `NullValue` is JSON `null`.   - NULL_VALUE: Null value.
     """
 
     """
     allowed enum values
     """
-    TESTING = 'testing'
-    STAGING = 'staging'
-    PRODUCTION = 'production'
-    DISABLED = 'disabled'
+    NULL_VALUE = 'NULL_VALUE'
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_status.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_status_condition.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_status_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_statuses.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_statuses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_tag.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_team.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_team.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -25,22 +25,24 @@
 from polyaxon_sdk.models.v1_team_settings import V1TeamSettings
 
 class V1Team(BaseModel):
     """
     V1Team
     """
     uuid: Optional[StrictStr] = None
+    owner: Optional[StrictStr] = None
     name: Optional[StrictStr] = None
     projects: Optional[conlist(StrictStr)] = None
     component_hubs: Optional[conlist(StrictStr)] = None
     model_registries: Optional[conlist(StrictStr)] = None
     settings: Optional[V1TeamSettings] = None
+    role: Optional[StrictStr] = None
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
-    __properties = ["uuid", "name", "projects", "component_hubs", "model_registries", "settings", "created_at", "updated_at"]
+    __properties = ["uuid", "owner", "name", "projects", "component_hubs", "model_registries", "settings", "role", "created_at", "updated_at"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -73,17 +75,19 @@
             return None
 
         if type(obj) is not dict:
             return V1Team.parse_obj(obj)
 
         _obj = V1Team.parse_obj({
             "uuid": obj.get("uuid"),
+            "owner": obj.get("owner"),
             "name": obj.get("name"),
             "projects": obj.get("projects"),
             "component_hubs": obj.get("component_hubs"),
             "model_registries": obj.get("model_registries"),
             "settings": V1TeamSettings.from_dict(obj.get("settings")) if obj.get("settings") is not None else None,
+            "role": obj.get("role"),
             "created_at": obj.get("created_at"),
             "updated_at": obj.get("updated_at")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_team_member.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_team_member.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_team_settings.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_team_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_template.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_tensorboard_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_tensorboard_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_termination.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_termination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_tf_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_tf_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_token.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_trial_start.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_trial_start.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_trigger_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_trigger_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_truncation_stopping_policy.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_truncation_stopping_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_tuner.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_tuner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_uri_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_uuids.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictBool, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, StrictStr, conlist
 
-class V1UriType(BaseModel):
+class V1Uuids(BaseModel):
     """
-    V1UriType
+    V1Uuids
     """
-    user: Optional[StrictStr] = None
-    password: Optional[StrictStr] = None
-    host: Optional[StrictBool] = None
-    __properties = ["user", "password", "host"]
+    uuids: Optional[conlist(StrictStr)] = None
+    __properties = ["uuids"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1UriType:
-        """Create an instance of V1UriType from a JSON string"""
+    def from_json(cls, json_str: str) -> V1Uuids:
+        """Create an instance of V1Uuids from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1UriType:
-        """Create an instance of V1UriType from a dict"""
+    def from_dict(cls, obj: dict) -> V1Uuids:
+        """Create an instance of V1Uuids from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1UriType.parse_obj(obj)
+            return V1Uuids.parse_obj(obj)
 
-        _obj = V1UriType.parse_obj({
-            "user": obj.get("user"),
-            "password": obj.get("password"),
-            "host": obj.get("host")
+        _obj = V1Uuids.parse_obj({
+            "uuids": obj.get("uuids")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_url_ref.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_url_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_user.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_user_access.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_user_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_user_email.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_user_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_user_singup.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_user_singup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_uuids.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, StrictStr, conlist
+from typing import Optional
+from pydantic import BaseModel, StrictStr
 
-class V1Uuids(BaseModel):
+class V1Version(BaseModel):
     """
-    V1Uuids
+    V1Version
     """
-    uuids: Optional[conlist(StrictStr)] = None
-    __properties = ["uuids"]
+    min: Optional[StrictStr] = None
+    latest: Optional[StrictStr] = None
+    __properties = ["min", "latest"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1Uuids:
-        """Create an instance of V1Uuids from a JSON string"""
+    def from_json(cls, json_str: str) -> V1Version:
+        """Create an instance of V1Version from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1Uuids:
-        """Create an instance of V1Uuids from a dict"""
+    def from_dict(cls, obj: dict) -> V1Version:
+        """Create an instance of V1Version from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1Uuids.parse_obj(obj)
+            return V1Version.parse_obj(obj)
 
-        _obj = V1Uuids.parse_obj({
-            "uuids": obj.get("uuids")
+        _obj = V1Version.parse_obj({
+            "min": obj.get("min"),
+            "latest": obj.get("latest")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_validation.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_version.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_hp_q_log_uniform.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Any, Dict, Optional
 from pydantic import BaseModel, StrictStr
 
-class V1Version(BaseModel):
+class V1HpQLogUniform(BaseModel):
     """
-    V1Version
+    V1HpQLogUniform
     """
-    min: Optional[StrictStr] = None
-    latest: Optional[StrictStr] = None
-    __properties = ["min", "latest"]
+    kind: Optional[StrictStr] = 'qloguniform'
+    value: Optional[Dict[str, Any]] = None
+    __properties = ["kind", "value"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1Version:
-        """Create an instance of V1Version from a JSON string"""
+    def from_json(cls, json_str: str) -> V1HpQLogUniform:
+        """Create an instance of V1HpQLogUniform from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1Version:
-        """Create an instance of V1Version from a dict"""
+    def from_dict(cls, obj: dict) -> V1HpQLogUniform:
+        """Create an instance of V1HpQLogUniform from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1Version.parse_obj(obj)
+            return V1HpQLogUniform.parse_obj(obj)
 
-        _obj = V1Version.parse_obj({
-            "min": obj.get("min"),
-            "latest": obj.get("latest")
+        _obj = V1HpQLogUniform.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'qloguniform',
+            "value": obj.get("value")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_wasb_type.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_wasb_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/models/v1_xg_boost_job.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/models/v1_xg_boost_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk/rest.py` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.1.8/polyaxon_sdk.egg-info/SOURCES.txt` & `polyaxon-sdk-2.2.0rc0/polyaxon_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyaxon-sdk-2.1.8/pyproject.toml` & `polyaxon-sdk-2.2.0rc0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyaxon_sdk"
-version = "2.1.8"
+version = "2.2.0-rc0"
 description = "Polyaxon SDKs and REST API specification."
 authors = ["contact@polyaxon.com"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_REPO_ID/GIT_USER_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Polyaxon SDKs and REST API specification."]
```

### Comparing `polyaxon-sdk-2.1.8/setup.py` & `polyaxon-sdk-2.2.0rc0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
          # noqa: E501
 
-    The version of the OpenAPI document: 2.1.8
+    The version of the OpenAPI document: 2.2.0-rc0
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "polyaxon-sdk"
-VERSION = "2.1.8"
+VERSION = "2.2.0-rc0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic",
     "aenum"
 ]
```

