# Comparing `tmp/types-influxdb-client-1.42.0.20240423.tar.gz` & `tmp/types-influxdb-client-1.42.0.20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-influxdb-client-1.42.0.20240423.tar", last modified: Tue Apr 23 02:19:56 2024, max compression
+gzip compressed data, was "types-influxdb-client-1.42.0.20240425.tar", last modified: Thu Apr 25 02:19:25 2024, max compression
```

## Comparing `types-influxdb-client-1.42.0.20240423.tar` & `types-influxdb-client-1.42.0.20240425.tar`

### file list

```diff
@@ -1,427 +1,427 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.664501 types-influxdb-client-1.42.0.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-23 02:19:56.664501 types-influxdb-client-1.42.0.20240423/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.608501 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    34856 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.608501 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_async/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_async/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_async/api_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_async/rest.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.608501 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_sync/api_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_sync/rest.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.612501 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/authorizations_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/bucket_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/delete_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/delete_api_async.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/flux_csv_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/flux_table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/influxdb_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/influxdb_client_async.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/invokable_scripts_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/labels_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/logging_handler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/organizations_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/query_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/query_api_async.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/tasks_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/users_api.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.612501 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/util/date_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/util/date_utils_pandas.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/util/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/util/multiprocessing_helper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/warnings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.612501 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/dataframe_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/point.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write_api_async.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/configuration.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.656501 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/
--rw-r--r--   0 runner    (1001) docker     (127)    30203 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/add_resource_member_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/analyze_query_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/analyze_query_response_errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/array_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/ast_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/authorization.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/authorization_post_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/authorization_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/authorizations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/axes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/axis.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/axis_scale.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bad_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/band_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/binary_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/block.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/boolean_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket_metadata_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket_retention_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket_shard_mapping.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/buckets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builder_aggregate_function_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builder_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builder_config_aggregate_window.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builder_functions_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builder_tags_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builtin_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/call_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/cell_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/cell_update.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/cell_with_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_base_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_discriminator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_patch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_status_level.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/column_data_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/column_semantic_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/conditional_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/constant_variable_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/create_cell.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/create_dashboard_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/custom_check.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboard.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboard_color.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboard_query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboard_with_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/date_time_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dbr_ps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dbrp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dbrp_create.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dbrp_get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dbrp_update.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/deadman_check.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/decimal_places.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/delete_predicate_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dialect.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dict_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dict_item.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/duration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/duration_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/expression_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/field.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/file.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/float_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/flux_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/flux_suggestion.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/flux_suggestions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/function_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/gauge_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/greater_threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/health_check.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/heatmap_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/histogram_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/http_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/http_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/http_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/identifier.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/import_declaration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/index_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/integer_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/is_onboarding.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label_mapping.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label_update.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/labels_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/language_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/legacy_authorization_post_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/lesser_threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/line_plus_single_stat_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/line_protocol_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/line_protocol_length_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/list_stacks_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/log_event.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/logical_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/logs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/map_variable_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/markdown_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/measurement_schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/measurement_schema_column.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/measurement_schema_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/measurement_schema_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/measurement_schema_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/member_assignment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/member_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/metadata_backup.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/model_property.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/mosaic_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/node.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_base_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_discriminator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_update.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule_base_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule_discriminator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule_update.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/object_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/onboarding_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/onboarding_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/option_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/organization.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/organization_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/organizations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/package.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/package_clause.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pager_duty_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pager_duty_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pager_duty_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/paren_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/password_reset_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_bucket_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_dashboard_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_organization_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_retention_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_stack_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_stack_request_additional_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/permission.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/permission_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pipe_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pipe_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_bucket_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_check.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_organization_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_restore_kv_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_stack_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/property_key.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/query_edit_mode.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/query_variable_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/query_variable_properties_values.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/range_threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/ready.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/regexp_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/remote_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/remote_connection_creation_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/remote_connection_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/remote_connections.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/renamable_field.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/replication.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/replication_creation_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/replication_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/replications.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_member.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_members.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_members_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_owner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_owners.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/restored_bucket_mappings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/retention_policy_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/return_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/routes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/routes_external.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/routes_query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/routes_system.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/rule_status_level.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/run.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/run_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/run_manually.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/runs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/scatter_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/schema_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/scraper_target_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/scraper_target_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/scraper_target_responses.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/script.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/script_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/script_invocation_params.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/script_language.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/script_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/secret_keys.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/secret_keys_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/shard_group_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/shard_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/shard_owner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/simple_table_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/single_stat_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/slack_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/slack_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/slack_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/smtp_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/smtp_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/source.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/source_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/sources.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack_associations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/statement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/static_legend.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/status_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/string_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/subscription_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/table_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/table_view_properties_table_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/tag_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task_status_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_plugin_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_plugin_request_plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_request_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegrafs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegram_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegram_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegram_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_apply.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_apply_remotes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_apply_template.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_id.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_id_org_ids.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_id_resource_filters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_id_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_name.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_name_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_kind.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_buckets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_buckets_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_dashboards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_dashboards_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_label_mappings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_labels.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_labels_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_notification_endpoints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_notification_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_notification_rules_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_tasks_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_telegraf_configs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_variables.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_variables_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_label.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_label_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_buckets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_dashboards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_label_mappings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_notification_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_status_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_tag_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_variables.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/test_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/threshold_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/threshold_check.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/unary_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/unsigned_integer_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/user.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/user_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/user_response_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/users.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/variable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/variable_assignment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/variable_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/variable_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/variables.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/view.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/view_links.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/views.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/write_precision.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/xy_geom.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/xy_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/extras.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/rest.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.660501 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/_base_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/authorizations_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/backup_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/bucket_schemas_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/buckets_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/cells_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/checks_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/config_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/dashboards_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/dbr_ps_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/delete_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/health_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/invokable_scripts_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/labels_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/legacy_authorizations_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/metrics_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/notification_endpoints_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/notification_rules_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/organizations_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/ping_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/query_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/ready_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/remote_connections_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/replications_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/resources_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/restore_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/routes_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/rules_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/scraper_targets_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/secrets_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/setup_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/signin_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/signout_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/sources_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/tasks_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/telegraf_plugins_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/telegrafs_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/templates_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/users_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/variables_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/views_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/write_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 02:18:48.000000 types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:56.664501 types-influxdb-client-1.42.0.20240423/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    15590 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:56.664501 types-influxdb-client-1.42.0.20240423/types_influxdb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/types_influxdb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21298 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/types_influxdb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/types_influxdb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/types_influxdb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 02:19:56.000000 types-influxdb-client-1.42.0.20240423/types_influxdb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.998968 types-influxdb-client-1.42.0.20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-25 02:19:24.998968 types-influxdb-client-1.42.0.20240425/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.938969 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    34856 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.938969 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_async/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_async/api_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_async/rest.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.942969 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_sync/api_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_sync/rest.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.942969 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/authorizations_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/bucket_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/delete_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/delete_api_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/flux_csv_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/flux_table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/influxdb_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/influxdb_client_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/invokable_scripts_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/labels_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/logging_handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/organizations_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/query_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/query_api_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/tasks_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/users_api.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.942969 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/util/date_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/util/date_utils_pandas.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/util/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/util/multiprocessing_helper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/warnings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.946969 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/dataframe_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/point.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write_api_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/configuration.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.990968 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)    30203 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/add_resource_member_request_body.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/analyze_query_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/analyze_query_response_errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/array_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/ast_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/authorization.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/authorization_post_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/authorization_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/authorizations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/axes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/axis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/axis_scale.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bad_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/band_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/binary_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/block.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/boolean_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket_metadata_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket_retention_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket_shard_mapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/buckets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builder_aggregate_function_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builder_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builder_config_aggregate_window.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builder_functions_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builder_tags_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builtin_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/call_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/cell_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/cell_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/cell_with_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_base_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_discriminator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_patch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_status_level.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/column_data_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/column_semantic_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/conditional_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/constant_variable_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/create_cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/create_dashboard_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/custom_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboard.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboard_color.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboard_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboard_with_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/date_time_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dbr_ps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dbrp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dbrp_create.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dbrp_get.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dbrp_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/deadman_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/decimal_places.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/delete_predicate_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dialect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dict_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dict_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/duration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/duration_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/expression_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/field.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/float_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/flux_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/flux_suggestion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/flux_suggestions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/function_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/gauge_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/greater_threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/health_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/heatmap_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/histogram_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/http_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/http_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/http_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/identifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/import_declaration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/index_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/integer_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/is_onboarding.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label_create_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label_mapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/labels_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/language_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/legacy_authorization_post_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/lesser_threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/line_plus_single_stat_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/line_protocol_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/line_protocol_length_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/list_stacks_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/log_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/logical_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/logs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/map_variable_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/markdown_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/measurement_schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/measurement_schema_column.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/measurement_schema_create_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/measurement_schema_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/measurement_schema_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/member_assignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/member_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/metadata_backup.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/model_property.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/mosaic_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_base_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_discriminator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule_base_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule_discriminator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/object_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/onboarding_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/onboarding_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/option_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/organization.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/organization_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/organizations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/package.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/package_clause.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pager_duty_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pager_duty_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pager_duty_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/paren_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/password_reset_body.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_bucket_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_dashboard_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_organization_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_retention_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_stack_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_stack_request_additional_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/permission.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/permission_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pipe_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pipe_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_bucket_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_organization_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_restore_kv_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_stack_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/property_key.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/query_edit_mode.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/query_variable_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/query_variable_properties_values.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/range_threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/ready.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/regexp_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/remote_connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/remote_connection_creation_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/remote_connection_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/remote_connections.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/renamable_field.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/replication.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/replication_creation_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/replication_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/replications.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_member.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_members.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_members_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_owner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_owners.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/restored_bucket_mappings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/retention_policy_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/return_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/routes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/routes_external.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/routes_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/routes_system.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/rule_status_level.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/run.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/run_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/run_manually.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/runs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/scatter_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/schema_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/scraper_target_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/scraper_target_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/scraper_target_responses.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/script.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/script_create_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/script_invocation_params.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/script_language.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/script_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/secret_keys.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/secret_keys_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/shard_group_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/shard_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/shard_owner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/simple_table_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/single_stat_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/slack_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/slack_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/slack_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/smtp_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/smtp_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/source.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/source_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/sources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack_associations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/static_legend.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/status_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/string_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/subscription_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/table_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/table_view_properties_table_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/tag_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task_create_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task_status_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_plugin_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_plugin_request_plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_request_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegrafs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegram_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegram_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegram_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_apply.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_apply_remotes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_apply_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_id.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_id_org_ids.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_id_resource_filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_id_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_name.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_name_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_kind.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_buckets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_buckets_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_dashboards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_dashboards_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_label_mappings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_labels.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_labels_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_notification_endpoints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_notification_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_notification_rules_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_tasks_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_telegraf_configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_variables.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_variables_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_label.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_label_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_buckets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_dashboards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_label_mappings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_notification_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_status_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_tag_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_variables.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/test_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/threshold_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/threshold_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/unary_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/unsigned_integer_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/user_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/user_response_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/users.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/variable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/variable_assignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/variable_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/variable_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/variables.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/view.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/view_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/write_precision.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/xy_geom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/xy_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/extras.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/rest.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.998968 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/_base_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/authorizations_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/backup_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/bucket_schemas_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/buckets_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/cells_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/checks_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/config_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/dashboards_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/dbr_ps_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/delete_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/health_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/invokable_scripts_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/labels_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/legacy_authorizations_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/metrics_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/notification_endpoints_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/notification_rules_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/organizations_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/ping_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/query_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/ready_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/remote_connections_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/replications_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/resources_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/restore_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/routes_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/rules_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/scraper_targets_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/secrets_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/setup_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/signin_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/signout_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/sources_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/tasks_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/telegraf_plugins_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/telegrafs_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/templates_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/users_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/variables_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/views_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/write_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 02:18:23.000000 types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:19:24.998968 types-influxdb-client-1.42.0.20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:24.998968 types-influxdb-client-1.42.0.20240425/types_influxdb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/types_influxdb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21298 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/types_influxdb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/types_influxdb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/types_influxdb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 02:19:24.000000 types-influxdb-client-1.42.0.20240425/types_influxdb_client.egg-info/top_level.txt
```

### Comparing `types-influxdb-client-1.42.0.20240423/CHANGELOG.md` & `types-influxdb-client-1.42.0.20240425/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.42.0.20240425 (2024-04-25)
+
+Introduce SupportsContainsAndGetItem (#11827)
+
 ## 1.42.0.20240423 (2024-04-23)
 
 Add precise values for enum members where possible (#11299)
 
 Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
 Co-authored-by: Alex Waygood <alex.waygood@gmail.com>
```

### Comparing `types-influxdb-client-1.42.0.20240423/PKG-INFO` & `types-influxdb-client-1.42.0.20240425/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-influxdb-client
-Version: 1.42.0.20240423
+Version: 1.42.0.20240425
 Summary: Typing stubs for influxdb-client
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/influxdb-client.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -30,10 +30,10 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/influxdb-client. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-influxdb-client` has required `urllib3>=2` since v1.37.0.1. If you need to install `types-influxdb-client` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-influxdb-client<1.37.0.1`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/METADATA.toml` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/METADATA.toml`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/__init__.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_async/api_client.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_async/api_client.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_async/rest.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_async/rest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_sync/api_client.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_sync/api_client.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/_sync/rest.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/_sync/rest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/__init__.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/authorizations_api.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/authorizations_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/bucket_api.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/bucket_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/flux_csv_parser.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/flux_csv_parser.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/flux_table.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/flux_table.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/influxdb_client.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/influxdb_client.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/influxdb_client_async.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/influxdb_client_async.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/invokable_scripts_api.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/invokable_scripts_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/labels_api.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/labels_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/query_api.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/query_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/query_api_async.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/query_api_async.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/tasks_api.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/tasks_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/util/date_utils.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/util/date_utils.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/util/multiprocessing_helper.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/util/multiprocessing_helper.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/__init__.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/dataframe_serializer.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/dataframe_serializer.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/point.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/point.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 DEFAULT_WRITE_PRECISION: _WritePrecision
 
 class Point:
     @staticmethod
     def measurement(measurement: str) -> Point: ...
     @staticmethod
     def from_dict(
-        dictionary: SupportsGetItem[str, Any],
+        dictionary: SupportsGetItem[str, Any],  # TODO: Use SupportsContainsAndGetItem
         write_precision: _WritePrecision = "ns",
         *,
         record_measurement_name: str | None = ...,
         record_measurement_key: str = ...,
         record_tag_keys: Iterable[str] | None = ...,
         record_field_keys: Iterable[str] | None = ...,
         record_time_key: str = ...,
```

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write/retry.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write/retry.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write_api.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/client/write_api_async.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/client/write_api_async.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/configuration.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/configuration.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/__init__.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/add_resource_member_request_body.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/add_resource_member_request_body.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/analyze_query_response_errors.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/analyze_query_response_errors.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/array_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/array_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/authorization.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/authorization.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/authorization_post_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/authorization_post_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/authorization_update_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/authorization_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/authorizations.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/authorizations.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/axis.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/axis.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bad_statement.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bad_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/band_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/band_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/binary_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/binary_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/block.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/block.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/boolean_literal.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/boolean_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket_metadata_manifest.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket_metadata_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket_retention_rules.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket_retention_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/bucket_shard_mapping.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/bucket_shard_mapping.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/buckets.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/buckets.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builder_config.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builder_config.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builder_config_aggregate_window.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builder_config_aggregate_window.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builder_tags_type.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builder_tags_type.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/builtin_statement.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/builtin_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/call_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/call_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/cell.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/cell_update.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/cell_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/cell_with_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/cell_with_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_base_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_base_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_discriminator.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_discriminator.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_patch.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_patch.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/check_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/check_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/checks.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/checks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/conditional_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/conditional_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/constant_variable_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/constant_variable_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/create_cell.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/create_cell.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/create_dashboard_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/create_dashboard_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/custom_check.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/custom_check.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboard.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboard.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboard_color.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboard_color.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboard_query.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboard_query.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboard_with_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboard_with_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dashboards.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dashboards.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/date_time_literal.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/date_time_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dbrp.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dbrp.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dbrp_create.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dbrp_create.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dbrp_update.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dbrp_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/deadman_check.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/deadman_check.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/decimal_places.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/decimal_places.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/delete_predicate_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/delete_predicate_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dialect.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dialect.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dict_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dict_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/dict_item.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/dict_item.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/duration.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/duration.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/duration_literal.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/duration_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/error.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/error.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/expression_statement.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/expression_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/field.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/field.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/file.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/file.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/float_literal.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/float_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/flux_suggestion.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/flux_suggestion.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/function_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/function_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/gauge_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/gauge_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/greater_threshold.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/greater_threshold.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/health_check.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/health_check.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/heatmap_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/heatmap_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/histogram_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/histogram_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/http_notification_endpoint.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/http_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/http_notification_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/http_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/http_notification_rule_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/http_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/identifier.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/identifier.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/import_declaration.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/import_declaration.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/index_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/index_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/integer_literal.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/integer_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label_create_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label_create_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label_response.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/label_update.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/label_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/labels_response.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/labels_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/legacy_authorization_post_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/legacy_authorization_post_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/lesser_threshold.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/lesser_threshold.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/line_plus_single_stat_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/line_plus_single_stat_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/line_protocol_error.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/line_protocol_error.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/line_protocol_length_error.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/line_protocol_length_error.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/log_event.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/log_event.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/logical_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/logical_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/map_variable_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/map_variable_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/markdown_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/markdown_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/measurement_schema.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/measurement_schema.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/measurement_schema_column.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/measurement_schema_column.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/measurement_schema_create_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/measurement_schema_create_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/member_assignment.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/member_assignment.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/member_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/member_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/metadata_backup.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/metadata_backup.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/model_property.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/model_property.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/mosaic_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/mosaic_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_base_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_base_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_discriminator.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_discriminator.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoint_update.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoint_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_endpoints.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule_base_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule_base_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule_discriminator.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule_discriminator.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rule_update.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rule_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/notification_rules.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/notification_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/object_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/object_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/onboarding_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/onboarding_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/onboarding_response.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/onboarding_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/option_statement.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/option_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/organization.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/organization.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/organization_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/organization_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/organizations.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/organizations.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/package.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/package.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/package_clause.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/package_clause.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pager_duty_notification_endpoint.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pager_duty_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pager_duty_notification_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pager_duty_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pager_duty_notification_rule_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pager_duty_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/paren_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/paren_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_bucket_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_bucket_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_dashboard_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_dashboard_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_organization_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_organization_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_retention_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_retention_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_stack_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_stack_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/patch_stack_request_additional_resources.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/patch_stack_request_additional_resources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/permission.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/permission.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/permission_resource.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/permission_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/pipe_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/pipe_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_bucket_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_bucket_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_notification_endpoint.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_notification_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_organization_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_organization_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/post_stack_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/post_stack_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/query.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/query.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/query_variable_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/query_variable_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/query_variable_properties_values.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/query_variable_properties_values.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/range_threshold.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/range_threshold.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/ready.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/ready.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/regexp_literal.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/regexp_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/remote_connection.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/remote_connection.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/remote_connection_creation_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/remote_connection_creation_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/remote_connection_update_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/remote_connection_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/renamable_field.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/renamable_field.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/replication.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/replication.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/replication_creation_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/replication_creation_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/replication_update_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/replication_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_member.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_member.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_members.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_members.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_owner.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_owner.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/resource_owners.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/resource_owners.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/restored_bucket_mappings.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/restored_bucket_mappings.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/retention_policy_manifest.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/retention_policy_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/return_statement.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/return_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/routes.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/routes.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/routes_query.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/routes_query.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/routes_system.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/routes_system.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/run.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/run.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/run_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/run_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/runs.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/runs.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/scatter_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/scatter_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/scraper_target_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/scraper_target_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/scraper_target_response.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/scraper_target_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/script.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/script.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/script_create_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/script_create_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/script_update_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/script_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/secret_keys_response.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/secret_keys_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/shard_group_manifest.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/shard_group_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/shard_manifest.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/shard_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/simple_table_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/simple_table_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/single_stat_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/single_stat_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/slack_notification_endpoint.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/slack_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/slack_notification_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/slack_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/slack_notification_rule_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/slack_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/smtp_notification_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/smtp_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/smtp_notification_rule_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/smtp_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/source.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/source.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/source_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/source_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/sources.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/sources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack_associations.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack_associations.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack_events.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack_events.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/stack_resources.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/stack_resources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/static_legend.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/static_legend.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/status_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/status_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/string_literal.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/string_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/subscription_manifest.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/subscription_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/table_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/table_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/table_view_properties_table_options.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/table_view_properties_table_options.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/tag_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/tag_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task_create_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task_create_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/task_update_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/task_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/tasks.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/tasks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_plugin.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_plugin_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_plugin_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_plugin_request_plugins.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_plugin_request_plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_plugins.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegraf_request.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegraf_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegram_notification_endpoint.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegram_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegram_notification_rule.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegram_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/telegram_notification_rule_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/telegram_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_apply.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_apply.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_apply_remotes.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_apply_remotes.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_apply_template.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_apply_template.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_chart.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_id.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_id.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_id_org_ids.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_id_org_ids.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_id_resource_filters.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_id_resource_filters.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_id_resources.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_id_resources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_name.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_name.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_export_by_name_resources.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_export_by_name_resources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_kind.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_kind.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_buckets.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_buckets.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_buckets_new_old.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_buckets_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_checks.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_checks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_dashboards.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_dashboards.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_dashboards_new_old.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_dashboards_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_label_mappings.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_label_mappings.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_labels.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_labels.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_labels_new_old.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_labels_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_notification_endpoints.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_notification_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_notification_rules.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_notification_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_notification_rules_new_old.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_notification_rules_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_tasks.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_tasks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_tasks_new_old.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_tasks_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_telegraf_configs.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_telegraf_configs.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_variables.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_variables.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_diff_variables_new_old.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_diff_variables_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_errors.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_errors.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_label.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_label.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_label_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_label_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_buckets.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_buckets.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_dashboards.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_dashboards.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_label_mappings.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_label_mappings.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_notification_rules.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_notification_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_status_rules.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_status_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_tag_rules.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_tag_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_tasks.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_tasks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/template_summary_summary_variables.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/template_summary_summary_variables.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/test_statement.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/test_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/threshold_base.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/threshold_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/threshold_check.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/threshold_check.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/unary_expression.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/unary_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/unsigned_integer_literal.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/unsigned_integer_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/user.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/user.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/user_response.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/user_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/users.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/users.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/variable.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/variable.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/variable_assignment.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/variable_assignment.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/variable_links.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/variable_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/view.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/view.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/views.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/views.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/write_precision.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/write_precision.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/domain/xy_view_properties.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/domain/xy_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/rest.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/rest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/__init__.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/authorizations_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/authorizations_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/backup_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/backup_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/bucket_schemas_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/bucket_schemas_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/buckets_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/buckets_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/cells_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/cells_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/checks_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/checks_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/dashboards_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/dashboards_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/dbr_ps_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/dbr_ps_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/invokable_scripts_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/invokable_scripts_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/labels_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/labels_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/legacy_authorizations_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/legacy_authorizations_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/notification_endpoints_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/notification_endpoints_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/notification_rules_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/notification_rules_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/organizations_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/organizations_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/query_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/query_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/remote_connections_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/remote_connections_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/replications_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/replications_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/restore_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/restore_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/scraper_targets_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/scraper_targets_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/secrets_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/secrets_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/setup_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/setup_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/sources_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/sources_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/tasks_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/tasks_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/telegrafs_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/telegrafs_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/templates_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/templates_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/users_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/users_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/variables_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/variables_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/influxdb_client-stubs/service/views_service.pyi` & `types-influxdb-client-1.42.0.20240425/influxdb_client-stubs/service/views_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.42.0.20240423/setup.py` & `types-influxdb-client-1.42.0.20240425/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/influxdb-client. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-influxdb-client` has required `urllib3>=2` since v1.37.0.1. If you need to install `types-influxdb-client` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-influxdb-client<1.37.0.1`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="1.42.0.20240423",
+      version="1.42.0.20240425",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/influxdb-client.md",
```

### Comparing `types-influxdb-client-1.42.0.20240423/types_influxdb_client.egg-info/PKG-INFO` & `types-influxdb-client-1.42.0.20240425/types_influxdb_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-influxdb-client
-Version: 1.42.0.20240423
+Version: 1.42.0.20240425
 Summary: Typing stubs for influxdb-client
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/influxdb-client.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -30,10 +30,10 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/influxdb-client. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-influxdb-client` has required `urllib3>=2` since v1.37.0.1. If you need to install `types-influxdb-client` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-influxdb-client<1.37.0.1`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-influxdb-client-1.42.0.20240423/types_influxdb_client.egg-info/SOURCES.txt` & `types-influxdb-client-1.42.0.20240425/types_influxdb_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

