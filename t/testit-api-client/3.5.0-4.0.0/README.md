# Comparing `tmp/testit-api-client-3.5.0.tar.gz` & `tmp/testit_api_client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-api-client-3.5.0.tar", last modified: Mon Mar  4 17:22:09 2024, max compression
+gzip compressed data, was "testit_api_client-4.0.0.tar", last modified: Sun May 19 21:36:09 2024, max compression
```

## Comparing `testit-api-client-3.5.0.tar` & `testit_api_client-4.0.0.tar`

### file list

```diff
@@ -1,482 +1,488 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:22:09.024491 testit-api-client-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    54620 2024-03-04 17:22:09.024491 testit-api-client-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-04 17:22:09.024491 testit-api-client-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:22:08.924490 testit-api-client-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:22:08.924490 testit-api-client-3.5.0/src/testit_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:22:08.936490 testit-api-client-3.5.0/src/testit_api_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   127065 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/auto_tests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28466 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/background_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    64692 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46729 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/custom_attribute_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28447 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/custom_attributes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29117 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    83810 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/parameters_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20109 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_attribute_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37070 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_attributes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31167 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_export_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_sections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31265 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_test_plan_attributes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39098 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_test_plans_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36093 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/project_work_items_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   164670 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    45572 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/sections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    38895 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   170702 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/test_plans_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/test_points_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    68830 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/test_results_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    87361 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/test_runs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    71988 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/test_suites_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    42999 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/webhooks_logs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   145599 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/work_items_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api/work_items_comments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39271 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:22:08.936490 testit-api-client-3.5.0/src/testit_api_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:22:09.024491 testit-api-client-3.5.0/src/testit_api_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/action_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_attachments_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_auto_tests_flaky_bulk_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_auto_tests_id_test_results_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14289 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_auto_tests_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_background_jobs_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_configurations_create_by_parameters_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14578 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_configurations_purge_bulk_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_configurations_put_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_configurations_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_global_id_put_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15628 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_global_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16104 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14288 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_templates_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14470 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_templates_put_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_templates_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14707 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_notifications_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_parameters_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_attributes_templates_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_test_plans_delete_bulk_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_test_plans_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14708 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_work_items_search_grouped_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_work_items_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_restore_bulk_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17975 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14159 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_search_global_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_tags_delete_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_tags_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_tags_put_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_plans_id_export_test_points_xlsx_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14420 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_plans_id_test_points_tester_user_id_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_plans_id_test_runs_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    23549 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_points_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_results_id_put_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_results_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_runs_id_statistics_filter_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_runs_id_test_results_bulk_put_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18847 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_runs_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_runs_update_multiple_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_suites_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_suites_put_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17518 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_webhooks_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15749 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_webhooks_search_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_webhooks_test_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13926 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_comments_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_comments_put_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_move_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_shared_step_id_references_sections_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_shared_step_id_references_work_items_post_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/attachment_change_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/attachment_change_view_model_array_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/attachment_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/attachment_model_auto_test_step_results_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/attachment_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15072 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/attachment_put_model_auto_test_step_results_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_average_duration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_change_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_change_view_model_array_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16288 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_model_v2_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_namespace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17540 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_related_to_test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    18905 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_results_for_test_run_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/auto_test_step_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18379 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_filter_model_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_filter_model_modified_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_filter_model_stability_percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)    13525 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_historical_result_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_result_historical_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_result_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_result_reason_sub_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_select_model_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20832 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotest_select_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotests_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotests_extraction_model_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotests_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20835 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotests_select_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/autotests_select_model_includes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/available_test_result_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/background_job_attachment_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/background_job_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/background_job_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/background_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/background_job_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/boolean_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/boolean_nullable_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_by_parameters_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13969 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_extraction_model_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_extraction_model_project_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_select_model_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/configuration_select_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_and_fill_by_auto_tests_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_and_fill_by_configurations_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_and_fill_by_work_items_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_auto_test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_configuration_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15260 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_empty_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_parameter_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_projects_attribute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_section_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16475 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_test_plan_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/create_work_item_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_change_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_option_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_option_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13586 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_search_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_template_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_template_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_template_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_template_search_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_test_plan_project_relation_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_types_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/date_time_range_selector_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/deletion_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/export_project_json_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14391 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/export_project_with_test_plans_json_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/external_link_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/failure_category_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/failure_class_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/failure_class_regex_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13886 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21728 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/filter_model_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/flaky_bulk_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14350 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/flaky_bulk_model_autotest_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/get_xlsx_test_points_by_test_plan_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/global_custom_attribute_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/global_custom_attribute_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/global_search_item_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/global_search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/global_search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/guid_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/guid_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/image_resize_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/int32_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/int32_range_selector_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/int64_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/int64_range_selector_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/iteration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/iteration_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/label_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/label_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/last_test_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13888 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/link_auto_test_to_work_item_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/link_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/link_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/link_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/link_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/link_sub_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/move_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/no_content_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/notification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/notification_query_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/notification_type_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/parameter_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/parameter_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/parameter_iteration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/parameter_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/parameter_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/parameter_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/period_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/period_view_model_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_attributes_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_custom_attribute_template_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_custom_attributes_templates_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_export_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_export_with_test_plans_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_shortest_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/project_test_plans_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_autotests_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_checklists_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_shared_steps_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_test_cases_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    12788 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/public_test_point_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/public_test_run_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/rename_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/request_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/request_type_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/search_attributes_in_project_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/search_auto_tests_query_includes_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12933 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/search_custom_attribute_template_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/search_webhooks_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    23936 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/search_work_items_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/section_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/section_move_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/section_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/section_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/section_rename_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/section_shared_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/section_with_steps_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/set_of_attachment_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/set_of_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_change_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16721 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_section_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model_modified_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    16489 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_references_query_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/shared_step_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/short_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/step_comment_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/step_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/step_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/step_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/step_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/string_array_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/string_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/string_changed_field_with_diffs_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/tag_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/tag_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/tag_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/tag_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/tag_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/tags_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/tags_filter_model_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_change_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19670 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_change_model_test_plan_changed_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    17147 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_changed_fields_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_group_by_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_group_by_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_group_by_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_group_by_tester_and_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    17817 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18377 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_with_analytic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_with_analytic_model_analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_plan_with_test_suite_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_analytic_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_by_test_suite_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_change_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_change_view_model_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21072 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_modified_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    14012 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_work_item_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_work_item_median_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_work_item_modified_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_related_to_test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    23026 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_short_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15233 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_short_get_model_last_test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12295 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    17986 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_point_with_last_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_points_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_points_extraction_model_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_change_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_change_view_model_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_chronology_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20720 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_history_report_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)    16114 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_short_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_step_comment_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_v2_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16587 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_result_v2_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15835 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_results_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_results_filter_model_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_results_filter_model_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13429 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_results_local_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_results_statistics_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_results_statistics_get_model_failure_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_results_statistics_get_model_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_analytic_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_extraction_model_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_fill_by_auto_tests_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_fill_by_configurations_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_fill_by_work_items_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model_auto_tests_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model_completed_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model_started_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_group_by_failure_class_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_group_by_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14653 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_model_analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13124 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_search_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_select_model_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14357 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_selection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14880 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_short_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_short_get_model_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_statistics_error_categories_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_statistics_statuses_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_partial_bulk_set_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_partial_bulk_set_model_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_select_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_select_model_test_result_ids_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_update_multiple_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16328 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_v2_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_v2_post_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12883 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_run_v2_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_change_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_change_view_model_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_v2_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_v2_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_v2_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_v2_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_with_children_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21469 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_work_items_search_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_work_items_search_model_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13978 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/test_suite_work_items_search_model_median_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_attachment_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_auto_test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_custom_attribute_test_plan_project_relations_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15171 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_empty_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_link_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_parameter_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14496 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_project_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_projects_attribute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_section_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_test_plan_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17901 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/update_work_item_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12938 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/user_rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/user_with_rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/user_with_rank_model_user_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/validate_anti_forgery_token_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/validation_problem_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    14500 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/web_hook_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    14515 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/web_hook_event_type_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15943 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/web_hook_log_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/web_hook_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16519 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/web_hook_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/web_hook_test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/webhook_variables_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_change_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21486 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_change_model_work_item_changed_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_attribute_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20781 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_auto_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_global_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    13887 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_is_deleted.py
--rw-r--r--   0 runner    (1001) docker     (127)    14498 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_project_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    14863 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_comment_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_comment_model_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_comment_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_comment_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_extraction_model_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_extraction_model_section_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_group_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_group_get_model_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_group_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_identifier_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_like_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_link_change_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_link_change_view_model_array_changed_field_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_local_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_local_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15001 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_local_select_model_extraction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21412 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_local_select_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    21058 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_move_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_post_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_priority_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_put_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_search_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_select_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_select_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19136 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_short_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_states.py
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_step_change_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_step_change_view_model_array_changed_field_with_diffs_view_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14335 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_step_change_view_model_work_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model/work_item_version_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    82623 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:22:09.024491 testit-api-client-3.5.0/src/testit_api_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    40322 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-03-04 17:22:02.000000 testit-api-client-3.5.0/src/testit_api_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:22:09.024491 testit-api-client-3.5.0/src/testit_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    54620 2024-03-04 17:22:08.000000 testit-api-client-3.5.0/src/testit_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28406 2024-03-04 17:22:08.000000 testit-api-client-3.5.0/src/testit_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 17:22:08.000000 testit-api-client-3.5.0/src/testit_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-04 17:22:08.000000 testit-api-client-3.5.0/src/testit_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-04 17:22:08.000000 testit-api-client-3.5.0/src/testit_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:36:09.966636 testit_api_client-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    55718 2024-05-19 21:36:09.966636 testit_api_client-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    55351 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 21:36:09.966636 testit_api_client-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:36:09.874634 testit_api_client-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:36:09.878635 testit_api_client-4.0.0/src/testit_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:36:09.886635 testit_api_client-4.0.0/src/testit_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127065 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/auto_tests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28466 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/background_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64692 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46729 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/custom_attribute_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28447 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/custom_attributes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29117 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83810 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/parameters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20109 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_attribute_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37070 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_attributes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31167 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_export_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31265 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_test_plan_attributes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39098 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36114 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/project_work_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164670 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45572 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38895 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   170702 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/test_points_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68830 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/test_results_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118404 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/test_runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71988 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/test_suites_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/webhooks_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145599 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/work_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api/work_items_comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39271 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:36:09.886635 testit_api_client-4.0.0/src/testit_api_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:36:09.966636 testit_api_client-4.0.0/src/testit_api_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/action_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_attachments_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_auto_tests_flaky_bulk_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_auto_tests_id_test_results_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14289 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_auto_tests_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_background_jobs_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_configurations_create_by_parameters_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14578 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_configurations_purge_bulk_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_configurations_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_configurations_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_global_id_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15628 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_global_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16104 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14288 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_templates_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14470 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_templates_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_templates_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14707 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_notifications_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_parameters_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_attributes_templates_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_test_plans_delete_bulk_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_test_plans_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14708 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_work_items_search_grouped_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_work_items_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_restore_bulk_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17975 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14159 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_search_global_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_tags_delete_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_tags_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_tags_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_plans_id_export_test_points_xlsx_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14420 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_plans_id_test_points_tester_user_id_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_plans_id_test_runs_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23549 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_points_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_results_id_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19828 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_results_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_delete_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_id_statistics_filter_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_id_test_results_bulk_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18847 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_update_multiple_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_suites_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_suites_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17518 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_webhooks_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15749 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_webhooks_search_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_webhooks_test_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13926 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_comments_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_comments_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_move_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_shared_step_id_references_sections_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_shared_step_id_references_work_items_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/attachment_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/attachment_change_view_model_array_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/attachment_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/attachment_model_auto_test_step_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/attachment_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15072 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/attachment_put_model_auto_test_step_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_average_duration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_change_view_model_array_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16288 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_model_v2_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_namespace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17540 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_related_to_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18905 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_results_for_test_run_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/auto_test_step_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18379 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_filter_model_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_filter_model_modified_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_filter_model_stability_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13525 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_historical_result_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_result_historical_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_result_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_result_reason_sub_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_select_model_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20832 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotest_select_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotests_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotests_extraction_model_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotests_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20835 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotests_select_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/autotests_select_model_includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/available_test_result_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/background_job_attachment_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/background_job_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/background_job_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/background_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/background_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/boolean_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/boolean_nullable_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_by_parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13969 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_extraction_model_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_extraction_model_project_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_select_model_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/configuration_select_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16659 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_and_fill_by_auto_tests_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_and_fill_by_configurations_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_and_fill_by_work_items_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_auto_test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_configuration_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15260 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_empty_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_parameter_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_projects_attribute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16475 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_test_plan_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/create_work_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_option_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_option_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13586 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_search_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_template_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_template_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_template_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_template_search_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_test_plan_project_relation_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_types_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/date_time_range_selector_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/deletion_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/export_project_json_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14391 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/export_project_with_test_plans_json_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/external_link_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/failure_category_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/failure_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/failure_class_regex_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13886 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21728 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/filter_model_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/flaky_bulk_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14350 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/flaky_bulk_model_autotest_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/get_xlsx_test_points_by_test_plan_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/global_custom_attribute_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/global_custom_attribute_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/global_search_item_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/global_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/global_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/guid_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/guid_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/image_resize_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/int32_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/int32_range_selector_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/int64_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/int64_range_selector_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/iteration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/iteration_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/label_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/label_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/last_test_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13888 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/link_auto_test_to_work_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/link_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/link_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/link_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/link_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/link_sub_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/move_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/named_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/no_content_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/notification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/notification_query_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/notification_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/parameter_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/parameter_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/parameter_iteration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/parameter_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/parameter_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/parameter_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/period_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/period_view_model_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_attributes_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_custom_attribute_template_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_custom_attributes_templates_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_export_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_export_with_test_plans_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_shortest_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/project_test_plans_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_autotests_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_checklists_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_shared_steps_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_test_cases_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/public_test_point_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/public_test_run_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/rename_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/request_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/search_attributes_in_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/search_auto_tests_query_includes_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12933 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/search_custom_attribute_template_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/search_webhooks_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23936 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/search_work_items_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/section_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/section_move_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/section_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/section_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/section_rename_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/section_shared_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/section_with_steps_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/set_of_attachment_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/set_of_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16721 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_section_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model_modified_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16489 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_references_query_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/shared_step_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/short_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/step_comment_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/step_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/step_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/step_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/string_array_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/string_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/string_changed_field_with_diffs_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/tag_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/tag_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/tag_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/tag_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/tag_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/tag_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/tags_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/tags_filter_model_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19670 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_change_model_test_plan_changed_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17147 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_changed_fields_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_group_by_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_group_by_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_group_by_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_group_by_tester_and_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17817 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18377 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_with_analytic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_with_analytic_model_analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_plan_with_test_suite_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_analytic_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_by_test_suite_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_change_view_model_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21072 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_modified_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14012 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_work_item_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_work_item_median_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_work_item_modified_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_related_to_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23896 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_short_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15233 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_short_get_model_last_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12295 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17986 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_point_with_last_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_points_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_points_extraction_model_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_change_view_model_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_chronology_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20720 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_history_report_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17598 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_short_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_step_comment_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_v2_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16587 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_result_v2_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model_completed_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13997 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model_modified_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model_started_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13429 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_local_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_statistics_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_statistics_get_model_failure_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_results_statistics_get_model_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_analytic_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_extraction_model_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_fill_by_auto_tests_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_fill_by_configurations_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_fill_by_work_items_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model_auto_tests_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model_completed_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model_started_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_group_by_failure_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_group_by_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14653 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_model_analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13124 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_search_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_select_model_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14357 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_selection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14880 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_short_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_short_get_model_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_statistics_error_categories_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_statistics_statuses_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_partial_bulk_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_partial_bulk_set_model_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_select_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_select_model_test_result_ids_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_update_multiple_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17041 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_v2_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_v2_post_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12883 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_run_v2_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_change_view_model_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_v2_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_v2_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_v2_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_v2_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_with_children_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21469 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_work_items_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_work_items_search_model_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13978 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/test_suite_work_items_search_model_median_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_attachment_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_auto_test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_custom_attribute_test_plan_project_relations_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15171 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_empty_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_link_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_parameter_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14496 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_projects_attribute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_test_plan_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17901 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/update_work_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13305 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/user_rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/user_with_rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/user_with_rank_model_user_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/validate_anti_forgery_token_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/validation_problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14500 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/web_hook_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14515 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/web_hook_event_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15943 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/web_hook_log_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/web_hook_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16519 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/web_hook_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/web_hook_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/webhook_variables_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21486 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_change_model_work_item_changed_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_attribute_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20781 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_auto_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_global_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13887 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_is_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14498 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_project_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14863 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_comment_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_comment_model_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_comment_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_comment_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_extraction_model_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_extraction_model_section_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_group_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_group_get_model_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_group_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_identifier_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_like_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_link_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_link_change_view_model_array_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_local_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_local_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15001 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_local_select_model_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21412 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_local_select_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21058 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_move_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_priority_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_search_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_select_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19485 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_step_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_step_change_view_model_array_changed_field_with_diffs_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14335 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_step_change_view_model_work_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model/work_item_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82623 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:36:09.966636 testit_api_client-4.0.0/src/testit_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    40888 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-05-19 21:36:05.000000 testit_api_client-4.0.0/src/testit_api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:36:09.966636 testit_api_client-4.0.0/src/testit_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55718 2024-05-19 21:36:09.000000 testit_api_client-4.0.0/src/testit_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28779 2024-05-19 21:36:09.000000 testit_api_client-4.0.0/src/testit_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:36:09.000000 testit_api_client-4.0.0/src/testit_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-19 21:36:09.000000 testit_api_client-4.0.0/src/testit_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 21:36:09.000000 testit_api_client-4.0.0/src/testit_api_client.egg-info/top_level.txt
```

### Comparing `testit-api-client-3.5.0/LICENSE.md` & `testit_api_client-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/PKG-INFO` & `testit_api_client-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-api-client
-Version: 3.5.0
+Version: 4.0.0
 Summary: API-client for Test IT
 Home-page: https://pypi.org/project/testit-api-client/
 Author: Integration team
 Author-email: integrations@testit.software
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -28,14 +28,15 @@
 | 3.5     | 2.0.4      |
 | 4.0     | 3.0.0      |
 | 4.2     | 3.1.0      |
 | 4.3     | 3.2.0      |
 | 4.4     | 3.3.0      |
 | 4.5     | 3.4.0      |
 | 4.6     | 3.5.0      |
+| 5.0     | 4.0.0      |
 
 ## Installation & Usage
 ### pip install
 
 ```sh
 pip install testit-api-client
 ```
@@ -278,18 +279,24 @@
 *TestResultsApi* | [**api_v2_test_results_search_post**](docs/TestResultsApi.md#api_v2_test_results_search_post) | **POST** /api/v2/testResults/search | Search for test results
 *TestResultsApi* | [**api_v2_test_results_statistics_filter_post**](docs/TestResultsApi.md#api_v2_test_results_statistics_filter_post) | **POST** /api/v2/testResults/statistics/filter | Search for test results and extract statistics
 *TestResultsApi* | [**create_attachment**](docs/TestResultsApi.md#create_attachment) | **POST** /api/v2/testResults/{id}/attachments | Upload and link attachment to TestResult
 *TestResultsApi* | [**delete_attachment**](docs/TestResultsApi.md#delete_attachment) | **DELETE** /api/v2/testResults/{id}/attachments/{attachmentId} | Remove attachment and unlink from TestResult
 *TestResultsApi* | [**download_attachment**](docs/TestResultsApi.md#download_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId} | Get attachment of TestResult
 *TestResultsApi* | [**get_attachment**](docs/TestResultsApi.md#get_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId}/info | Get Metadata of TestResult&#39;s attachment
 *TestResultsApi* | [**get_attachments**](docs/TestResultsApi.md#get_attachments) | **GET** /api/v2/testResults/{id}/attachments | Get all attachments of TestResult
+*TestRunsApi* | [**api_v2_test_runs_delete**](docs/TestRunsApi.md#api_v2_test_runs_delete) | **DELETE** /api/v2/testRuns | Delete multiple test runs
+*TestRunsApi* | [**api_v2_test_runs_id_delete**](docs/TestRunsApi.md#api_v2_test_runs_id_delete) | **DELETE** /api/v2/testRuns/{id} | Delete test run
+*TestRunsApi* | [**api_v2_test_runs_id_purge_post**](docs/TestRunsApi.md#api_v2_test_runs_id_purge_post) | **POST** /api/v2/testRuns/{id}/purge | Permanently delete test run from archive
+*TestRunsApi* | [**api_v2_test_runs_id_restore_post**](docs/TestRunsApi.md#api_v2_test_runs_id_restore_post) | **POST** /api/v2/testRuns/{id}/restore | Restore test run from the archive
 *TestRunsApi* | [**api_v2_test_runs_id_statistics_filter_post**](docs/TestRunsApi.md#api_v2_test_runs_id_statistics_filter_post) | **POST** /api/v2/testRuns/{id}/statistics/filter | Search for the test run test results and build statistics
 *TestRunsApi* | [**api_v2_test_runs_id_test_points_results_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_points_results_get) | **GET** /api/v2/testRuns/{id}/testPoints/results | Get test results from the test run grouped by test points
 *TestRunsApi* | [**api_v2_test_runs_id_test_results_bulk_put**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_bulk_put) | **PUT** /api/v2/testRuns/{id}/testResults/bulk | Partial edit of multiple test results in the test run
 *TestRunsApi* | [**api_v2_test_runs_id_test_results_last_modified_modification_date_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_last_modified_modification_date_get) | **GET** /api/v2/testRuns/{id}/testResults/lastModified/modificationDate | Get modification date of last test result of the test run
+*TestRunsApi* | [**api_v2_test_runs_purge_bulk_post**](docs/TestRunsApi.md#api_v2_test_runs_purge_bulk_post) | **POST** /api/v2/testRuns/purge/bulk | Permanently delete multiple test runs from archive
+*TestRunsApi* | [**api_v2_test_runs_restore_bulk_post**](docs/TestRunsApi.md#api_v2_test_runs_restore_bulk_post) | **POST** /api/v2/testRuns/restore/bulk | Restore multiple test runs from the archive
 *TestRunsApi* | [**api_v2_test_runs_search_post**](docs/TestRunsApi.md#api_v2_test_runs_search_post) | **POST** /api/v2/testRuns/search | Search for test runs
 *TestRunsApi* | [**api_v2_test_runs_update_multiple_post**](docs/TestRunsApi.md#api_v2_test_runs_update_multiple_post) | **POST** /api/v2/testRuns/updateMultiple | Update multiple test runs
 *TestRunsApi* | [**complete_test_run**](docs/TestRunsApi.md#complete_test_run) | **POST** /api/v2/testRuns/{id}/complete | Complete TestRun
 *TestRunsApi* | [**create_and_fill_by_auto_tests**](docs/TestRunsApi.md#create_and_fill_by_auto_tests) | **POST** /api/v2/testRuns/byAutoTests | Create test runs based on autotests and configurations
 *TestRunsApi* | [**create_and_fill_by_configurations**](docs/TestRunsApi.md#create_and_fill_by_configurations) | **POST** /api/v2/testRuns/byConfigurations | Create test runs picking the needed test points
 *TestRunsApi* | [**create_and_fill_by_work_items**](docs/TestRunsApi.md#create_and_fill_by_work_items) | **POST** /api/v2/testRuns/byWorkItems | Create test run based on configurations and work items
 *TestRunsApi* | [**create_empty**](docs/TestRunsApi.md#create_empty) | **POST** /api/v2/testRuns | Create empty TestRun
```

### Comparing `testit-api-client-3.5.0/README.md` & `testit_api_client-4.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 | 3.5     | 2.0.4      |
 | 4.0     | 3.0.0      |
 | 4.2     | 3.1.0      |
 | 4.3     | 3.2.0      |
 | 4.4     | 3.3.0      |
 | 4.5     | 3.4.0      |
 | 4.6     | 3.5.0      |
+| 5.0     | 4.0.0      |
 
 ## Installation & Usage
 ### pip install
 
 ```sh
 pip install testit-api-client
 ```
@@ -265,18 +266,24 @@
 *TestResultsApi* | [**api_v2_test_results_search_post**](docs/TestResultsApi.md#api_v2_test_results_search_post) | **POST** /api/v2/testResults/search | Search for test results
 *TestResultsApi* | [**api_v2_test_results_statistics_filter_post**](docs/TestResultsApi.md#api_v2_test_results_statistics_filter_post) | **POST** /api/v2/testResults/statistics/filter | Search for test results and extract statistics
 *TestResultsApi* | [**create_attachment**](docs/TestResultsApi.md#create_attachment) | **POST** /api/v2/testResults/{id}/attachments | Upload and link attachment to TestResult
 *TestResultsApi* | [**delete_attachment**](docs/TestResultsApi.md#delete_attachment) | **DELETE** /api/v2/testResults/{id}/attachments/{attachmentId} | Remove attachment and unlink from TestResult
 *TestResultsApi* | [**download_attachment**](docs/TestResultsApi.md#download_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId} | Get attachment of TestResult
 *TestResultsApi* | [**get_attachment**](docs/TestResultsApi.md#get_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId}/info | Get Metadata of TestResult&#39;s attachment
 *TestResultsApi* | [**get_attachments**](docs/TestResultsApi.md#get_attachments) | **GET** /api/v2/testResults/{id}/attachments | Get all attachments of TestResult
+*TestRunsApi* | [**api_v2_test_runs_delete**](docs/TestRunsApi.md#api_v2_test_runs_delete) | **DELETE** /api/v2/testRuns | Delete multiple test runs
+*TestRunsApi* | [**api_v2_test_runs_id_delete**](docs/TestRunsApi.md#api_v2_test_runs_id_delete) | **DELETE** /api/v2/testRuns/{id} | Delete test run
+*TestRunsApi* | [**api_v2_test_runs_id_purge_post**](docs/TestRunsApi.md#api_v2_test_runs_id_purge_post) | **POST** /api/v2/testRuns/{id}/purge | Permanently delete test run from archive
+*TestRunsApi* | [**api_v2_test_runs_id_restore_post**](docs/TestRunsApi.md#api_v2_test_runs_id_restore_post) | **POST** /api/v2/testRuns/{id}/restore | Restore test run from the archive
 *TestRunsApi* | [**api_v2_test_runs_id_statistics_filter_post**](docs/TestRunsApi.md#api_v2_test_runs_id_statistics_filter_post) | **POST** /api/v2/testRuns/{id}/statistics/filter | Search for the test run test results and build statistics
 *TestRunsApi* | [**api_v2_test_runs_id_test_points_results_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_points_results_get) | **GET** /api/v2/testRuns/{id}/testPoints/results | Get test results from the test run grouped by test points
 *TestRunsApi* | [**api_v2_test_runs_id_test_results_bulk_put**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_bulk_put) | **PUT** /api/v2/testRuns/{id}/testResults/bulk | Partial edit of multiple test results in the test run
 *TestRunsApi* | [**api_v2_test_runs_id_test_results_last_modified_modification_date_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_last_modified_modification_date_get) | **GET** /api/v2/testRuns/{id}/testResults/lastModified/modificationDate | Get modification date of last test result of the test run
+*TestRunsApi* | [**api_v2_test_runs_purge_bulk_post**](docs/TestRunsApi.md#api_v2_test_runs_purge_bulk_post) | **POST** /api/v2/testRuns/purge/bulk | Permanently delete multiple test runs from archive
+*TestRunsApi* | [**api_v2_test_runs_restore_bulk_post**](docs/TestRunsApi.md#api_v2_test_runs_restore_bulk_post) | **POST** /api/v2/testRuns/restore/bulk | Restore multiple test runs from the archive
 *TestRunsApi* | [**api_v2_test_runs_search_post**](docs/TestRunsApi.md#api_v2_test_runs_search_post) | **POST** /api/v2/testRuns/search | Search for test runs
 *TestRunsApi* | [**api_v2_test_runs_update_multiple_post**](docs/TestRunsApi.md#api_v2_test_runs_update_multiple_post) | **POST** /api/v2/testRuns/updateMultiple | Update multiple test runs
 *TestRunsApi* | [**complete_test_run**](docs/TestRunsApi.md#complete_test_run) | **POST** /api/v2/testRuns/{id}/complete | Complete TestRun
 *TestRunsApi* | [**create_and_fill_by_auto_tests**](docs/TestRunsApi.md#create_and_fill_by_auto_tests) | **POST** /api/v2/testRuns/byAutoTests | Create test runs based on autotests and configurations
 *TestRunsApi* | [**create_and_fill_by_configurations**](docs/TestRunsApi.md#create_and_fill_by_configurations) | **POST** /api/v2/testRuns/byConfigurations | Create test runs picking the needed test points
 *TestRunsApi* | [**create_and_fill_by_work_items**](docs/TestRunsApi.md#create_and_fill_by_work_items) | **POST** /api/v2/testRuns/byWorkItems | Create test run based on configurations and work items
 *TestRunsApi* | [**create_empty**](docs/TestRunsApi.md#create_empty) | **POST** /api/v2/testRuns | Create empty TestRun
```

### Comparing `testit-api-client-3.5.0/setup.py` & `testit_api_client-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "testit-api-client"
 
-VERSION = "3.5.0"
+VERSION = "4.0.0"
 
 REQUIRES = [
   "urllib3 >= 1.25.3",
   "python-dateutil",
 ]
 
 setup(
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/__init__.py` & `testit_api_client-4.0.0/src/testit_api_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: v2.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "3.5.0"
+__version__ = "3.6.0"
 
 # import ApiClient
 from testit_api_client.api_client import ApiClient
 
 # import Configuration
 from testit_api_client.configuration import Configuration
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/attachments_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/auto_tests_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/auto_tests_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/background_jobs_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/background_jobs_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/configurations_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/configurations_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/custom_attribute_templates_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/custom_attribute_templates_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/custom_attributes_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/custom_attributes_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/notifications_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/parameters_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/parameters_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_attribute_templates_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_attribute_templates_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_attributes_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_attributes_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_configurations_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_configurations_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_export_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_export_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_import_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_import_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_sections_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_sections_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_test_plan_attributes_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_test_plan_attributes_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_test_plans_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_test_plans_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/project_work_items_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/project_work_items_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     file_type,
     none_type,
     validate_and_convert_types
 )
 from testit_api_client.model.api_v2_projects_project_id_work_items_search_grouped_post_request import ApiV2ProjectsProjectIdWorkItemsSearchGroupedPostRequest
 from testit_api_client.model.api_v2_projects_project_id_work_items_search_post_request import ApiV2ProjectsProjectIdWorkItemsSearchPostRequest
 from testit_api_client.model.problem_details import ProblemDetails
-from testit_api_client.model.tag_model import TagModel
+from testit_api_client.model.tag_short_model import TagShortModel
 from testit_api_client.model.work_item_group_model import WorkItemGroupModel
 from testit_api_client.model.work_item_short_model import WorkItemShortModel
 
 
 class ProjectWorkItemsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -284,15 +284,15 @@
                     'application/json'
                 ]
             },
             api_client=api_client
         )
         self.api_v2_projects_project_id_work_items_tags_get_endpoint = _Endpoint(
             settings={
-                'response_type': ([TagModel],),
+                'response_type': ([TagShortModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/projects/{projectId}/workItems/tags',
                 'operation_id': 'api_v2_projects_project_id_work_items_tags_get',
                 'http_method': 'GET',
                 'servers': None,
@@ -746,15 +746,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            [TagModel]
+            [TagShortModel]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/projects_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/search_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/sections_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/sections_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/tags_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/test_plans_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/test_plans_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/test_points_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/test_points_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/test_results_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/test_results_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/test_runs_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/test_suites_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,58 +17,54 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from testit_api_client.model.api_v2_test_runs_id_statistics_filter_post_request import ApiV2TestRunsIdStatisticsFilterPostRequest
-from testit_api_client.model.api_v2_test_runs_id_test_results_bulk_put_request import ApiV2TestRunsIdTestResultsBulkPutRequest
-from testit_api_client.model.api_v2_test_runs_search_post_request import ApiV2TestRunsSearchPostRequest
-from testit_api_client.model.api_v2_test_runs_update_multiple_post_request import ApiV2TestRunsUpdateMultiplePostRequest
-from testit_api_client.model.auto_test_results_for_test_run_model import AutoTestResultsForTestRunModel
-from testit_api_client.model.create_and_fill_by_auto_tests_request import CreateAndFillByAutoTestsRequest
-from testit_api_client.model.create_and_fill_by_configurations_request import CreateAndFillByConfigurationsRequest
-from testit_api_client.model.create_and_fill_by_work_items_request import CreateAndFillByWorkItemsRequest
-from testit_api_client.model.create_empty_request import CreateEmptyRequest
+from testit_api_client.model.api_v2_projects_project_id_work_items_search_post_request import ApiV2ProjectsProjectIdWorkItemsSearchPostRequest
+from testit_api_client.model.api_v2_test_suites_post_request import ApiV2TestSuitesPostRequest
+from testit_api_client.model.api_v2_test_suites_put_request import ApiV2TestSuitesPutRequest
+from testit_api_client.model.configuration_model import ConfigurationModel
+from testit_api_client.model.operation import Operation
 from testit_api_client.model.problem_details import ProblemDetails
-from testit_api_client.model.test_point_result_model import TestPointResultModel
-from testit_api_client.model.test_results_statistics_get_model import TestResultsStatisticsGetModel
-from testit_api_client.model.test_run_short_get_model import TestRunShortGetModel
-from testit_api_client.model.test_run_v2_get_model import TestRunV2GetModel
-from testit_api_client.model.update_empty_request import UpdateEmptyRequest
+from testit_api_client.model.search_work_items_request import SearchWorkItemsRequest
+from testit_api_client.model.test_point_by_test_suite_model import TestPointByTestSuiteModel
+from testit_api_client.model.test_result_v2_short_model import TestResultV2ShortModel
+from testit_api_client.model.test_suite_v2_get_model import TestSuiteV2GetModel
 from testit_api_client.model.validation_problem_details import ValidationProblemDetails
+from testit_api_client.model.work_item_short_model import WorkItemShortModel
 
 
-class TestRunsApi(object):
+class TestSuitesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.api_v2_test_runs_id_statistics_filter_post_endpoint = _Endpoint(
+        self.add_test_points_to_test_suite_endpoint = _Endpoint(
             settings={
-                'response_type': (TestResultsStatisticsGetModel,),
+                'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}/statistics/filter',
-                'operation_id': 'api_v2_test_runs_id_statistics_filter_post',
+                'endpoint_path': '/api/v2/testSuites/{id}/test-points',
+                'operation_id': 'add_test_points_to_test_suite',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'api_v2_test_runs_id_statistics_filter_post_request',
+                    'api_v2_projects_project_id_work_items_search_post_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -80,51 +76,52 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
-                    'api_v2_test_runs_id_statistics_filter_post_request':
-                        (ApiV2TestRunsIdStatisticsFilterPostRequest,),
+                    'api_v2_projects_project_id_work_items_search_post_request':
+                        (ApiV2ProjectsProjectIdWorkItemsSearchPostRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'api_v2_test_runs_id_statistics_filter_post_request': 'body',
+                    'api_v2_projects_project_id_work_items_search_post_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.api_v2_test_runs_id_test_points_results_get_endpoint = _Endpoint(
+        self.api_v2_test_suites_id_patch_endpoint = _Endpoint(
             settings={
-                'response_type': ([TestPointResultModel],),
+                'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}/testPoints/results',
-                'operation_id': 'api_v2_test_runs_id_test_points_results_get',
-                'http_method': 'GET',
+                'endpoint_path': '/api/v2/testSuites/{id}',
+                'operation_id': 'api_v2_test_suites_id_patch',
+                'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'operation',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -136,47 +133,51 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
+                    'operation':
+                        ([Operation],),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
+                    'operation': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.api_v2_test_runs_id_test_results_bulk_put_endpoint = _Endpoint(
+        self.api_v2_test_suites_id_refresh_post_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}/testResults/bulk',
-                'operation_id': 'api_v2_test_runs_id_test_results_bulk_put',
-                'http_method': 'PUT',
+                'endpoint_path': '/api/v2/testSuites/{id}/refresh',
+                'operation_id': 'api_v2_test_suites_id_refresh_post',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'api_v2_test_runs_id_test_results_bulk_put_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -188,107 +189,107 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
-                    'api_v2_test_runs_id_test_results_bulk_put_request':
-                        (ApiV2TestRunsIdTestResultsBulkPutRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'api_v2_test_runs_id_test_results_bulk_put_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.api_v2_test_runs_id_test_results_last_modified_modification_date_get_endpoint = _Endpoint(
+        self.api_v2_test_suites_id_work_items_post_endpoint = _Endpoint(
             settings={
-                'response_type': (datetime,),
+                'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}/testResults/lastModified/modificationDate',
-                'operation_id': 'api_v2_test_runs_id_test_results_last_modified_modification_date_get',
-                'http_method': 'GET',
+                'endpoint_path': '/api/v2/testSuites/{id}/workItems',
+                'operation_id': 'api_v2_test_suites_id_work_items_post',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'request_body',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
+                    'request_body',
                 ]
             },
             root_map={
                 'validations': {
+                    ('request_body',): {
+
+                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
+                    'request_body':
+                        ([str],),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
+                    'request_body': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.api_v2_test_runs_search_post_endpoint = _Endpoint(
+        self.api_v2_test_suites_post_endpoint = _Endpoint(
             settings={
-                'response_type': ([TestRunShortGetModel],),
+                'response_type': (TestSuiteV2GetModel,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/search',
-                'operation_id': 'api_v2_test_runs_search_post',
+                'endpoint_path': '/api/v2/testSuites',
+                'operation_id': 'api_v2_test_suites_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'skip',
-                    'take',
-                    'order_by',
-                    'search_field',
-                    'search_value',
-                    'api_v2_test_runs_search_post_request',
+                    'api_v2_test_suites_post_request',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -296,69 +297,49 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'skip':
-                        (int,),
-                    'take':
-                        (int,),
-                    'order_by':
-                        (str,),
-                    'search_field':
-                        (str,),
-                    'search_value':
-                        (str,),
-                    'api_v2_test_runs_search_post_request':
-                        (ApiV2TestRunsSearchPostRequest,),
+                    'api_v2_test_suites_post_request':
+                        (ApiV2TestSuitesPostRequest,),
                 },
                 'attribute_map': {
-                    'skip': 'Skip',
-                    'take': 'Take',
-                    'order_by': 'OrderBy',
-                    'search_field': 'SearchField',
-                    'search_value': 'SearchValue',
                 },
                 'location_map': {
-                    'skip': 'query',
-                    'take': 'query',
-                    'order_by': 'query',
-                    'search_field': 'query',
-                    'search_value': 'query',
-                    'api_v2_test_runs_search_post_request': 'body',
+                    'api_v2_test_suites_post_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.api_v2_test_runs_update_multiple_post_endpoint = _Endpoint(
+        self.api_v2_test_suites_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/updateMultiple',
-                'operation_id': 'api_v2_test_runs_update_multiple_post',
-                'http_method': 'POST',
+                'endpoint_path': '/api/v2/testSuites',
+                'operation_id': 'api_v2_test_suites_put',
+                'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'api_v2_test_runs_update_multiple_post_request',
+                    'api_v2_test_suites_put_request',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -366,42 +347,44 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'api_v2_test_runs_update_multiple_post_request':
-                        (ApiV2TestRunsUpdateMultiplePostRequest,),
+                    'api_v2_test_suites_put_request':
+                        (ApiV2TestSuitesPutRequest,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'api_v2_test_runs_update_multiple_post_request': 'body',
+                    'api_v2_test_suites_put_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/json'
+                ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.complete_test_run_endpoint = _Endpoint(
+        self.delete_test_suite_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}/complete',
-                'operation_id': 'complete_test_run',
-                'http_method': 'POST',
+                'endpoint_path': '/api/v2/testSuites/{id}',
+                'operation_id': 'delete_test_suite',
+                'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                 ],
                 'required': [
@@ -436,222 +419,124 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.create_and_fill_by_auto_tests_endpoint = _Endpoint(
+        self.get_configurations_by_test_suite_id_endpoint = _Endpoint(
             settings={
-                'response_type': (TestRunV2GetModel,),
+                'response_type': ([ConfigurationModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/byAutoTests',
-                'operation_id': 'create_and_fill_by_auto_tests',
-                'http_method': 'POST',
+                'endpoint_path': '/api/v2/testSuites/{id}/configurations',
+                'operation_id': 'get_configurations_by_test_suite_id',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'create_and_fill_by_auto_tests_request',
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'create_and_fill_by_auto_tests_request':
-                        (CreateAndFillByAutoTestsRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'create_and_fill_by_auto_tests_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-        self.create_and_fill_by_configurations_endpoint = _Endpoint(
-            settings={
-                'response_type': (TestRunV2GetModel,),
-                'auth': [
-                    'Bearer or PrivateToken'
+                    'id',
                 ],
-                'endpoint_path': '/api/v2/testRuns/byConfigurations',
-                'operation_id': 'create_and_fill_by_configurations',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'create_and_fill_by_configurations_request',
+                'required': [
+                    'id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'create_and_fill_by_configurations_request':
-                        (CreateAndFillByConfigurationsRequest,),
+                    'id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'id': 'id',
                 },
                 'location_map': {
-                    'create_and_fill_by_configurations_request': 'body',
+                    'id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.create_and_fill_by_work_items_endpoint = _Endpoint(
+        self.get_test_points_by_id_endpoint = _Endpoint(
             settings={
-                'response_type': (TestRunV2GetModel,),
+                'response_type': ([TestPointByTestSuiteModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/byWorkItems',
-                'operation_id': 'create_and_fill_by_work_items',
-                'http_method': 'POST',
+                'endpoint_path': '/api/v2/testSuites/{id}/testPoints',
+                'operation_id': 'get_test_points_by_id',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'create_and_fill_by_work_items_request',
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'create_and_fill_by_work_items_request':
-                        (CreateAndFillByWorkItemsRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'create_and_fill_by_work_items_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-        self.create_empty_endpoint = _Endpoint(
-            settings={
-                'response_type': (TestRunV2GetModel,),
-                'auth': [
-                    'Bearer or PrivateToken'
+                    'id',
                 ],
-                'endpoint_path': '/api/v2/testRuns',
-                'operation_id': 'create_empty',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'create_empty_request',
+                'required': [
+                    'id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'create_empty_request':
-                        (CreateEmptyRequest,),
+                    'id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'id': 'id',
                 },
                 'location_map': {
-                    'create_empty_request': 'body',
+                    'id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.get_test_run_by_id_endpoint = _Endpoint(
+        self.get_test_results_by_id_endpoint = _Endpoint(
             settings={
-                'response_type': (TestRunV2GetModel,),
+                'response_type': ([TestResultV2ShortModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}',
-                'operation_id': 'get_test_run_by_id',
+                'endpoint_path': '/api/v2/testSuites/{id}/testResults',
+                'operation_id': 'get_test_results_by_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                 ],
@@ -687,29 +572,28 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.set_auto_test_results_for_test_run_endpoint = _Endpoint(
+        self.get_test_suite_by_id_endpoint = _Endpoint(
             settings={
-                'response_type': ([str],),
+                'response_type': (TestSuiteV2GetModel,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}/testResults',
-                'operation_id': 'set_auto_test_results_for_test_run',
-                'http_method': 'POST',
+                'endpoint_path': '/api/v2/testSuites/{id}',
+                'operation_id': 'get_test_suite_by_id',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'auto_test_results_for_test_run_model',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -721,51 +605,52 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
-                    'auto_test_results_for_test_run_model':
-                        ([AutoTestResultsForTestRunModel],),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'auto_test_results_for_test_run_model': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.start_test_run_endpoint = _Endpoint(
+        self.search_work_items_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': ([WorkItemShortModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}/start',
-                'operation_id': 'start_test_run',
+                'endpoint_path': '/api/v2/testSuites/{id}/workItems/search',
+                'operation_id': 'search_work_items',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'skip',
+                    'take',
+                    'order_by',
+                    'search_field',
+                    'search_value',
+                    'search_work_items_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -777,119 +662,104 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
+                    'skip':
+                        (int,),
+                    'take':
+                        (int,),
+                    'order_by':
+                        (str,),
+                    'search_field':
+                        (str,),
+                    'search_value':
+                        (str,),
+                    'search_work_items_request':
+                        (SearchWorkItemsRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
+                    'skip': 'Skip',
+                    'take': 'Take',
+                    'order_by': 'OrderBy',
+                    'search_field': 'SearchField',
+                    'search_value': 'SearchValue',
                 },
                 'location_map': {
                     'id': 'path',
+                    'skip': 'query',
+                    'take': 'query',
+                    'order_by': 'query',
+                    'search_field': 'query',
+                    'search_value': 'query',
+                    'search_work_items_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.stop_test_run_endpoint = _Endpoint(
+        self.set_configurations_by_test_suite_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testRuns/{id}/stop',
-                'operation_id': 'stop_test_run',
+                'endpoint_path': '/api/v2/testSuites/{id}/configurations',
+                'operation_id': 'set_configurations_by_test_suite_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'request_body',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
+                    'request_body',
                 ]
             },
             root_map={
                 'validations': {
+                    ('request_body',): {
+
+                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
+                    'request_body':
+                        ([str],),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.update_empty_endpoint = _Endpoint(
-            settings={
-                'response_type': None,
-                'auth': [
-                    'Bearer or PrivateToken'
-                ],
-                'endpoint_path': '/api/v2/testRuns',
-                'operation_id': 'update_empty',
-                'http_method': 'PUT',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'update_empty_request',
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'update_empty_request':
-                        (UpdateEmptyRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'update_empty_request': 'body',
+                    'request_body': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -897,32 +767,32 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
-    def api_v2_test_runs_id_statistics_filter_post(
+    def add_test_points_to_test_suite(
         self,
         id,
         **kwargs
     ):
-        """Search for the test run test results and build statistics  # noqa: E501
+        """Add test-points to test suite  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_runs_id_statistics_filter_post(id, async_req=True)
+        >>> thread = api.add_test_points_to_test_suite(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test run unique ID
+            id (str): Test suite internal identifier
 
         Keyword Args:
-            api_v2_test_runs_id_statistics_filter_post_request (ApiV2TestRunsIdStatisticsFilterPostRequest): [optional]
+            api_v2_projects_project_id_work_items_search_post_request (ApiV2ProjectsProjectIdWorkItemsSearchPostRequest): Filter object to retrieve work items for test-suite's project. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -947,15 +817,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TestResultsStatisticsGetModel
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -978,33 +848,35 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.api_v2_test_runs_id_statistics_filter_post_endpoint.call_with_http_info(**kwargs)
+        return self.add_test_points_to_test_suite_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_runs_id_test_points_results_get(
+    def api_v2_test_suites_id_patch(
         self,
         id,
         **kwargs
     ):
-        """Get test results from the test run grouped by test points  # noqa: E501
+        """Patch test suite  # noqa: E501
 
+        See <a href=\"https://www.rfc-editor.org/rfc/rfc6902\" target=\"_blank\">RFC 6902: JavaScript Object Notation (JSON) Patch</a> for details  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_runs_id_test_points_results_get(id, async_req=True)
+        >>> thread = api.api_v2_test_suites_id_patch(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test run unique ID
+            id (str): Test Suite internal (UUID) identifier
 
         Keyword Args:
+            operation ([Operation]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1029,15 +901,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            [TestPointResultModel]
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1060,34 +932,33 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.api_v2_test_runs_id_test_points_results_get_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_suites_id_patch_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_runs_id_test_results_bulk_put(
+    def api_v2_test_suites_id_refresh_post(
         self,
         id,
         **kwargs
     ):
-        """Partial edit of multiple test results in the test run  # noqa: E501
+        """Refresh test suite. Only dynamic test suites are supported by this method  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_runs_id_test_results_bulk_put(id, async_req=True)
+        >>> thread = api.api_v2_test_suites_id_refresh_post(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test run unique ID
+            id (str): Test Suite internal (UUID) identifier
 
         Keyword Args:
-            api_v2_test_runs_id_test_results_bulk_put_request (ApiV2TestRunsIdTestResultsBulkPutRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1143,33 +1014,34 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.api_v2_test_runs_id_test_results_bulk_put_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_suites_id_refresh_post_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_runs_id_test_results_last_modified_modification_date_get(
+    def api_v2_test_suites_id_work_items_post(
         self,
         id,
         **kwargs
     ):
-        """Get modification date of last test result of the test run  # noqa: E501
+        """Set work items for test suite  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_runs_id_test_results_last_modified_modification_date_get(id, async_req=True)
+        >>> thread = api.api_v2_test_suites_id_work_items_post(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test run unique ID
+            id (str): Unique ID of the test suite
 
         Keyword Args:
+            request_body ([str]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1194,15 +1066,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            datetime
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1225,36 +1097,31 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.api_v2_test_runs_id_test_results_last_modified_modification_date_get_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_suites_id_work_items_post_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_runs_search_post(
+    def api_v2_test_suites_post(
         self,
         **kwargs
     ):
-        """Search for test runs  # noqa: E501
+        """Create test suite  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_runs_search_post(async_req=True)
+        >>> thread = api.api_v2_test_suites_post(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            skip (int): Amount of items to be skipped (offset). [optional]
-            take (int): Amount of items to be taken (limit). [optional]
-            order_by (str): SQL-like  ORDER BY statement (column1 ASC|DESC , column2 ASC|DESC). [optional]
-            search_field (str): Property name for searching. [optional]
-            search_value (str): Value for searching. [optional]
-            api_v2_test_runs_search_post_request (ApiV2TestRunsSearchPostRequest): [optional]
+            api_v2_test_suites_post_request (ApiV2TestSuitesPostRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1279,15 +1146,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            [TestRunShortGetModel]
+            TestSuiteV2GetModel
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1308,31 +1175,31 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.api_v2_test_runs_search_post_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_suites_post_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_runs_update_multiple_post(
+    def api_v2_test_suites_put(
         self,
         **kwargs
     ):
-        """Update multiple test runs  # noqa: E501
+        """Edit test suite  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_runs_update_multiple_post(async_req=True)
+        >>> thread = api.api_v2_test_suites_put(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            api_v2_test_runs_update_multiple_post_request (ApiV2TestRunsUpdateMultiplePostRequest): [optional]
+            api_v2_test_suites_put_request (ApiV2TestSuitesPutRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1386,32 +1253,32 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.api_v2_test_runs_update_multiple_post_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_suites_put_endpoint.call_with_http_info(**kwargs)
 
-    def complete_test_run(
+    def delete_test_suite(
         self,
         id,
         **kwargs
     ):
-        """Complete TestRun  # noqa: E501
+        """Delete TestSuite  # noqa: E501
 
-        <br>Use case  <br>User sets test run identifier  <br>User runs method execution  <br>System completes test run  <br>System returns no content response  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System deletes test suite  <br>System returns no content response  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.complete_test_run(id, async_req=True)
+        >>> thread = api.delete_test_suite(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test Run internal identifier (GUID format)
+            id (str): Test suite internal (guid format) identifier\"
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1469,269 +1336,34 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.complete_test_run_endpoint.call_with_http_info(**kwargs)
-
-    def create_and_fill_by_auto_tests(
-        self,
-        **kwargs
-    ):
-        """Create test runs based on autotests and configurations  # noqa: E501
-
-        This method creates a test run based on an autotest and a configuration.  The difference between the `POST /api/v2/testRuns/byWorkItems` and `POST /api/v2/testRuns/byConfigurations` methods is  that in this method there is no need to create a test plan and work items (test cases and checklists).  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_and_fill_by_auto_tests(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            create_and_fill_by_auto_tests_request (CreateAndFillByAutoTestsRequest): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            TestRunV2GetModel
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.create_and_fill_by_auto_tests_endpoint.call_with_http_info(**kwargs)
+        return self.delete_test_suite_endpoint.call_with_http_info(**kwargs)
 
-    def create_and_fill_by_configurations(
-        self,
-        **kwargs
-    ):
-        """Create test runs picking the needed test points  # noqa: E501
-
-        This method creates a test run based on a combination of a configuration and a work item(test case or checklist).  Before you create a test run using this method, make sure to create a test plan. Work items must be automated.  This method is different from the `POST /api/v2/testRuns/byWorkItems` method because of the ability to send a  jagged array within the \"<b>testPointSelectors</b>\" parameter.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_and_fill_by_configurations(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            create_and_fill_by_configurations_request (CreateAndFillByConfigurationsRequest): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            TestRunV2GetModel
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.create_and_fill_by_configurations_endpoint.call_with_http_info(**kwargs)
-
-    def create_and_fill_by_work_items(
-        self,
-        **kwargs
-    ):
-        """Create test run based on configurations and work items  # noqa: E501
-
-        This method creates a test run based on a combination of configuration and work item (test case or checklist).  Before you create a test run using this method, make sure to create a test plan.  Work items must be automated.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_and_fill_by_work_items(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            create_and_fill_by_work_items_request (CreateAndFillByWorkItemsRequest): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            TestRunV2GetModel
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.create_and_fill_by_work_items_endpoint.call_with_http_info(**kwargs)
-
-    def create_empty(
+    def get_configurations_by_test_suite_id(
         self,
+        id,
         **kwargs
     ):
-        """Create empty TestRun  # noqa: E501
+        """Get Configurations By Id  # noqa: E501
 
-        <br>Use case  <br>User sets test run model (listed in the request example)  <br>User runs method execution  <br>System creates test run  <br>System returns test run model  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search configurations related to the test points  <br>System returns configurations array  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_empty(async_req=True)
+        >>> thread = api.get_configurations_by_test_suite_id(id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            id (str): Test suite internal (guid format) identifier\"
 
         Keyword Args:
-            create_empty_request (CreateEmptyRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1756,15 +1388,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TestRunV2GetModel
+            [ConfigurationModel]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1785,32 +1417,34 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.create_empty_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = \
+            id
+        return self.get_configurations_by_test_suite_id_endpoint.call_with_http_info(**kwargs)
 
-    def get_test_run_by_id(
+    def get_test_points_by_id(
         self,
         id,
         **kwargs
     ):
-        """Get TestRun by Id  # noqa: E501
+        """Get TestPoints By Id  # noqa: E501
 
-        <br>Use case  <br>User sets test run identifier  <br>User runs method execution  <br>System finds test run  <br>System returns test run  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System returns test points array  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_test_run_by_id(id, async_req=True)
+        >>> thread = api.get_test_points_by_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test Run internal identifier (GUID format)
+            id (str): Test suite internal (guid format) identifier\"
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1837,15 +1471,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TestRunV2GetModel
+            [TestPointByTestSuiteModel]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1868,35 +1502,34 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.get_test_run_by_id_endpoint.call_with_http_info(**kwargs)
+        return self.get_test_points_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def set_auto_test_results_for_test_run(
+    def get_test_results_by_id(
         self,
         id,
         **kwargs
     ):
-        """Send test results to the test runs in the system  # noqa: E501
+        """Get TestResults By Id  # noqa: E501
 
-        This method sends test results to the test management system.  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search test results related to the test points  <br>System returns test results array  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.set_auto_test_results_for_test_run(id, async_req=True)
+        >>> thread = api.get_test_results_by_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test Run internal identifier (GUID format)
+            id (str): Test suite internal (guid format) identifier\"
 
         Keyword Args:
-            auto_test_results_for_test_run_model ([AutoTestResultsForTestRunModel]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1921,15 +1554,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            [str]
+            [TestResultV2ShortModel]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1952,32 +1585,32 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.set_auto_test_results_for_test_run_endpoint.call_with_http_info(**kwargs)
+        return self.get_test_results_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def start_test_run(
+    def get_test_suite_by_id(
         self,
         id,
         **kwargs
     ):
-        """Start TestRun  # noqa: E501
+        """Get TestSuite by Id  # noqa: E501
 
-        <br>Use case  <br>User sets test run identifier  <br>User runs method execution  <br>System starts test run  <br>System returns no content response  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System returns test suite  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.start_test_run(id, async_req=True)
+        >>> thread = api.get_test_suite_by_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test Run internal identifier (GUID format)
+            id (str): Test suite internal (guid format) identifier\"
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -2004,15 +1637,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            TestSuiteV2GetModel
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -2035,34 +1668,40 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.start_test_run_endpoint.call_with_http_info(**kwargs)
+        return self.get_test_suite_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def stop_test_run(
+    def search_work_items(
         self,
         id,
         **kwargs
     ):
-        """Stop TestRun  # noqa: E501
+        """Search WorkItems  # noqa: E501
 
-        <br>Use case  <br>User sets test run identifier  <br>User runs method execution  <br>System stops test run  <br>System returns no content response  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>[Optional] User sets filter  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search work items related to the test points  <br>                      [Optional] User sets filter, system applies filter                    <br>System returns work items array  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.stop_test_run(id, async_req=True)
+        >>> thread = api.search_work_items(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test Run internal identifier (GUID format)
+            id (str): Test suite internal (guid format) identifier\"
 
         Keyword Args:
+            skip (int): Amount of items to be skipped (offset). [optional]
+            take (int): Amount of items to be taken (limit). [optional]
+            order_by (str): SQL-like  ORDER BY statement (column1 ASC|DESC , column2 ASC|DESC). [optional]
+            search_field (str): Property name for searching. [optional]
+            search_value (str): Value for searching. [optional]
+            search_work_items_request (SearchWorkItemsRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2087,15 +1726,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            [WorkItemShortModel]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -2118,32 +1757,35 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.stop_test_run_endpoint.call_with_http_info(**kwargs)
+        return self.search_work_items_endpoint.call_with_http_info(**kwargs)
 
-    def update_empty(
+    def set_configurations_by_test_suite_id(
         self,
+        id,
         **kwargs
     ):
-        """Update empty TestRun  # noqa: E501
+        """Set Configurations By TestSuite Id  # noqa: E501
 
-        <br>Use case  <br>User sets test run properties (listed in the request example)  <br>User runs method execution  <br>System updates test run  <br>System returns returns no content response  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>User sets collection of configuration identifiers  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search configuration  <br>System restores(if exist) or creates test points with listed configuration  <br>System returns no content response  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_empty(async_req=True)
+        >>> thread = api.set_configurations_by_test_suite_id(id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            id (str): Test suite internal (guid format) identifier\"
 
         Keyword Args:
-            update_empty_request (UpdateEmptyRequest): [optional]
+            request_body ([str]): Collection of configuration identifiers\". [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2197,9 +1839,11 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.update_empty_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = \
+            id
+        return self.set_configurations_by_test_suite_id_endpoint.call_with_http_info(**kwargs)
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/test_suites_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/test_runs_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,54 +17,108 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from testit_api_client.model.api_v2_projects_project_id_work_items_search_post_request import ApiV2ProjectsProjectIdWorkItemsSearchPostRequest
-from testit_api_client.model.api_v2_test_suites_post_request import ApiV2TestSuitesPostRequest
-from testit_api_client.model.api_v2_test_suites_put_request import ApiV2TestSuitesPutRequest
-from testit_api_client.model.configuration_model import ConfigurationModel
-from testit_api_client.model.operation import Operation
+from testit_api_client.model.api_v2_test_runs_delete_request import ApiV2TestRunsDeleteRequest
+from testit_api_client.model.api_v2_test_runs_id_statistics_filter_post_request import ApiV2TestRunsIdStatisticsFilterPostRequest
+from testit_api_client.model.api_v2_test_runs_id_test_results_bulk_put_request import ApiV2TestRunsIdTestResultsBulkPutRequest
+from testit_api_client.model.api_v2_test_runs_search_post_request import ApiV2TestRunsSearchPostRequest
+from testit_api_client.model.api_v2_test_runs_update_multiple_post_request import ApiV2TestRunsUpdateMultiplePostRequest
+from testit_api_client.model.auto_test_results_for_test_run_model import AutoTestResultsForTestRunModel
+from testit_api_client.model.create_and_fill_by_auto_tests_request import CreateAndFillByAutoTestsRequest
+from testit_api_client.model.create_and_fill_by_configurations_request import CreateAndFillByConfigurationsRequest
+from testit_api_client.model.create_and_fill_by_work_items_request import CreateAndFillByWorkItemsRequest
+from testit_api_client.model.create_empty_request import CreateEmptyRequest
 from testit_api_client.model.problem_details import ProblemDetails
-from testit_api_client.model.search_work_items_request import SearchWorkItemsRequest
-from testit_api_client.model.test_point_by_test_suite_model import TestPointByTestSuiteModel
-from testit_api_client.model.test_result_v2_short_model import TestResultV2ShortModel
-from testit_api_client.model.test_suite_v2_get_model import TestSuiteV2GetModel
+from testit_api_client.model.test_point_result_model import TestPointResultModel
+from testit_api_client.model.test_results_statistics_get_model import TestResultsStatisticsGetModel
+from testit_api_client.model.test_run_short_get_model import TestRunShortGetModel
+from testit_api_client.model.test_run_v2_get_model import TestRunV2GetModel
+from testit_api_client.model.update_empty_request import UpdateEmptyRequest
 from testit_api_client.model.validation_problem_details import ValidationProblemDetails
-from testit_api_client.model.work_item_short_model import WorkItemShortModel
 
 
-class TestSuitesApi(object):
+class TestRunsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.add_test_points_to_test_suite_endpoint = _Endpoint(
+        self.api_v2_test_runs_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': (int,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns',
+                'operation_id': 'api_v2_test_runs_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'api_v2_test_runs_delete_request',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'api_v2_test_runs_delete_request':
+                        (ApiV2TestRunsDeleteRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'api_v2_test_runs_delete_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_v2_test_runs_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}/test-points',
-                'operation_id': 'add_test_points_to_test_suite',
-                'http_method': 'POST',
+                'endpoint_path': '/api/v2/testRuns/{id}',
+                'operation_id': 'api_v2_test_runs_id_delete',
+                'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'api_v2_projects_project_id_work_items_search_post_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -76,52 +130,46 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
-                    'api_v2_projects_project_id_work_items_search_post_request':
-                        (ApiV2ProjectsProjectIdWorkItemsSearchPostRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'api_v2_projects_project_id_work_items_search_post_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.api_v2_test_suites_id_patch_endpoint = _Endpoint(
+        self.api_v2_test_runs_id_purge_post_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}',
-                'operation_id': 'api_v2_test_suites_id_patch',
-                'http_method': 'PATCH',
+                'endpoint_path': '/api/v2/testRuns/{id}/purge',
+                'operation_id': 'api_v2_test_runs_id_purge_post',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'operation',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -133,45 +181,40 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
-                    'operation':
-                        ([Operation],),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'operation': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.api_v2_test_suites_id_refresh_post_endpoint = _Endpoint(
+        self.api_v2_test_runs_id_restore_post_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}/refresh',
-                'operation_id': 'api_v2_test_suites_id_refresh_post',
+                'endpoint_path': '/api/v2/testRuns/{id}/restore',
+                'operation_id': 'api_v2_test_runs_id_restore_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                 ],
@@ -207,184 +250,188 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.api_v2_test_suites_id_work_items_post_endpoint = _Endpoint(
+        self.api_v2_test_runs_id_statistics_filter_post_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (TestResultsStatisticsGetModel,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}/workItems',
-                'operation_id': 'api_v2_test_suites_id_work_items_post',
+                'endpoint_path': '/api/v2/testRuns/{id}/statistics/filter',
+                'operation_id': 'api_v2_test_runs_id_statistics_filter_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'request_body',
+                    'api_v2_test_runs_id_statistics_filter_post_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
-                    'request_body',
                 ]
             },
             root_map={
                 'validations': {
-                    ('request_body',): {
-
-                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
-                    'request_body':
-                        ([str],),
+                    'api_v2_test_runs_id_statistics_filter_post_request':
+                        (ApiV2TestRunsIdStatisticsFilterPostRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'request_body': 'body',
+                    'api_v2_test_runs_id_statistics_filter_post_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.api_v2_test_suites_post_endpoint = _Endpoint(
+        self.api_v2_test_runs_id_test_points_results_get_endpoint = _Endpoint(
             settings={
-                'response_type': (TestSuiteV2GetModel,),
+                'response_type': ([TestPointResultModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites',
-                'operation_id': 'api_v2_test_suites_post',
-                'http_method': 'POST',
+                'endpoint_path': '/api/v2/testRuns/{id}/testPoints/results',
+                'operation_id': 'api_v2_test_runs_id_test_points_results_get',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'api_v2_test_suites_post_request',
+                    'id',
+                ],
+                'required': [
+                    'id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'api_v2_test_suites_post_request':
-                        (ApiV2TestSuitesPostRequest,),
+                    'id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'id': 'id',
                 },
                 'location_map': {
-                    'api_v2_test_suites_post_request': 'body',
+                    'id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.api_v2_test_suites_put_endpoint = _Endpoint(
+        self.api_v2_test_runs_id_test_results_bulk_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites',
-                'operation_id': 'api_v2_test_suites_put',
+                'endpoint_path': '/api/v2/testRuns/{id}/testResults/bulk',
+                'operation_id': 'api_v2_test_runs_id_test_results_bulk_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'api_v2_test_suites_put_request',
+                    'id',
+                    'api_v2_test_runs_id_test_results_bulk_put_request',
+                ],
+                'required': [
+                    'id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'api_v2_test_suites_put_request':
-                        (ApiV2TestSuitesPutRequest,),
+                    'id':
+                        (str,),
+                    'api_v2_test_runs_id_test_results_bulk_put_request':
+                        (ApiV2TestRunsIdTestResultsBulkPutRequest,),
                 },
                 'attribute_map': {
+                    'id': 'id',
                 },
                 'location_map': {
-                    'api_v2_test_suites_put_request': 'body',
+                    'id': 'path',
+                    'api_v2_test_runs_id_test_results_bulk_put_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.delete_test_suite_endpoint = _Endpoint(
+        self.api_v2_test_runs_id_test_results_last_modified_modification_date_get_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (datetime,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}',
-                'operation_id': 'delete_test_suite',
-                'http_method': 'DELETE',
+                'endpoint_path': '/api/v2/testRuns/{id}/testResults/lastModified/modificationDate',
+                'operation_id': 'api_v2_test_runs_id_test_results_last_modified_modification_date_get',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                 ],
                 'required': [
@@ -419,74 +466,246 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_configurations_by_test_suite_id_endpoint = _Endpoint(
+        self.api_v2_test_runs_purge_bulk_post_endpoint = _Endpoint(
             settings={
-                'response_type': ([ConfigurationModel],),
+                'response_type': (int,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}/configurations',
-                'operation_id': 'get_configurations_by_test_suite_id',
-                'http_method': 'GET',
+                'endpoint_path': '/api/v2/testRuns/purge/bulk',
+                'operation_id': 'api_v2_test_runs_purge_bulk_post',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id',
+                    'api_v2_test_runs_delete_request',
                 ],
-                'required': [
-                    'id',
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
                 ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'api_v2_test_runs_delete_request':
+                        (ApiV2TestRunsDeleteRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'api_v2_test_runs_delete_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_v2_test_runs_restore_bulk_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (int,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns/restore/bulk',
+                'operation_id': 'api_v2_test_runs_restore_bulk_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'api_v2_test_runs_delete_request',
+                ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id':
+                    'api_v2_test_runs_delete_request':
+                        (ApiV2TestRunsDeleteRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'api_v2_test_runs_delete_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_v2_test_runs_search_post_endpoint = _Endpoint(
+            settings={
+                'response_type': ([TestRunShortGetModel],),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns/search',
+                'operation_id': 'api_v2_test_runs_search_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'skip',
+                    'take',
+                    'order_by',
+                    'search_field',
+                    'search_value',
+                    'api_v2_test_runs_search_post_request',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'skip':
+                        (int,),
+                    'take':
+                        (int,),
+                    'order_by':
                         (str,),
+                    'search_field':
+                        (str,),
+                    'search_value':
+                        (str,),
+                    'api_v2_test_runs_search_post_request':
+                        (ApiV2TestRunsSearchPostRequest,),
                 },
                 'attribute_map': {
-                    'id': 'id',
+                    'skip': 'Skip',
+                    'take': 'Take',
+                    'order_by': 'OrderBy',
+                    'search_field': 'SearchField',
+                    'search_value': 'SearchValue',
                 },
                 'location_map': {
-                    'id': 'path',
+                    'skip': 'query',
+                    'take': 'query',
+                    'order_by': 'query',
+                    'search_field': 'query',
+                    'search_value': 'query',
+                    'api_v2_test_runs_search_post_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.get_test_points_by_id_endpoint = _Endpoint(
+        self.api_v2_test_runs_update_multiple_post_endpoint = _Endpoint(
             settings={
-                'response_type': ([TestPointByTestSuiteModel],),
+                'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}/testPoints',
-                'operation_id': 'get_test_points_by_id',
-                'http_method': 'GET',
+                'endpoint_path': '/api/v2/testRuns/updateMultiple',
+                'operation_id': 'api_v2_test_runs_update_multiple_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'api_v2_test_runs_update_multiple_post_request',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'api_v2_test_runs_update_multiple_post_request':
+                        (ApiV2TestRunsUpdateMultiplePostRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'api_v2_test_runs_update_multiple_post_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.complete_test_run_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns/{id}/complete',
+                'operation_id': 'complete_test_run',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                 ],
                 'required': [
@@ -521,22 +740,222 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_test_results_by_id_endpoint = _Endpoint(
+        self.create_and_fill_by_auto_tests_endpoint = _Endpoint(
+            settings={
+                'response_type': (TestRunV2GetModel,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns/byAutoTests',
+                'operation_id': 'create_and_fill_by_auto_tests',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'create_and_fill_by_auto_tests_request',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'create_and_fill_by_auto_tests_request':
+                        (CreateAndFillByAutoTestsRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'create_and_fill_by_auto_tests_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.create_and_fill_by_configurations_endpoint = _Endpoint(
+            settings={
+                'response_type': (TestRunV2GetModel,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns/byConfigurations',
+                'operation_id': 'create_and_fill_by_configurations',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'create_and_fill_by_configurations_request',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'create_and_fill_by_configurations_request':
+                        (CreateAndFillByConfigurationsRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'create_and_fill_by_configurations_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.create_and_fill_by_work_items_endpoint = _Endpoint(
+            settings={
+                'response_type': (TestRunV2GetModel,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns/byWorkItems',
+                'operation_id': 'create_and_fill_by_work_items',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'create_and_fill_by_work_items_request',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'create_and_fill_by_work_items_request':
+                        (CreateAndFillByWorkItemsRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'create_and_fill_by_work_items_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.create_empty_endpoint = _Endpoint(
             settings={
-                'response_type': ([TestResultV2ShortModel],),
+                'response_type': (TestRunV2GetModel,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}/testResults',
-                'operation_id': 'get_test_results_by_id',
+                'endpoint_path': '/api/v2/testRuns',
+                'operation_id': 'create_empty',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'create_empty_request',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'create_empty_request':
+                        (CreateEmptyRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'create_empty_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.get_test_run_by_id_endpoint = _Endpoint(
+            settings={
+                'response_type': (TestRunV2GetModel,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns/{id}',
+                'operation_id': 'get_test_run_by_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                 ],
@@ -572,28 +991,29 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_test_suite_by_id_endpoint = _Endpoint(
+        self.set_auto_test_results_for_test_run_endpoint = _Endpoint(
             settings={
-                'response_type': (TestSuiteV2GetModel,),
+                'response_type': ([str],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}',
-                'operation_id': 'get_test_suite_by_id',
-                'http_method': 'GET',
+                'endpoint_path': '/api/v2/testRuns/{id}/testResults',
+                'operation_id': 'set_auto_test_results_for_test_run',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'auto_test_results_for_test_run_model',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -605,52 +1025,51 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
+                    'auto_test_results_for_test_run_model':
+                        ([AutoTestResultsForTestRunModel],),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
+                    'auto_test_results_for_test_run_model': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.search_work_items_endpoint = _Endpoint(
+        self.start_test_run_endpoint = _Endpoint(
             settings={
-                'response_type': ([WorkItemShortModel],),
+                'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}/workItems/search',
-                'operation_id': 'search_work_items',
+                'endpoint_path': '/api/v2/testRuns/{id}/start',
+                'operation_id': 'start_test_run',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'skip',
-                    'take',
-                    'order_by',
-                    'search_field',
-                    'search_value',
-                    'search_work_items_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -662,104 +1081,119 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
-                    'skip':
-                        (int,),
-                    'take':
-                        (int,),
-                    'order_by':
-                        (str,),
-                    'search_field':
-                        (str,),
-                    'search_value':
-                        (str,),
-                    'search_work_items_request':
-                        (SearchWorkItemsRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'skip': 'Skip',
-                    'take': 'Take',
-                    'order_by': 'OrderBy',
-                    'search_field': 'SearchField',
-                    'search_value': 'SearchValue',
                 },
                 'location_map': {
                     'id': 'path',
-                    'skip': 'query',
-                    'take': 'query',
-                    'order_by': 'query',
-                    'search_field': 'query',
-                    'search_value': 'query',
-                    'search_work_items_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.set_configurations_by_test_suite_id_endpoint = _Endpoint(
+        self.stop_test_run_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
-                'endpoint_path': '/api/v2/testSuites/{id}/configurations',
-                'operation_id': 'set_configurations_by_test_suite_id',
+                'endpoint_path': '/api/v2/testRuns/{id}/stop',
+                'operation_id': 'stop_test_run',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'request_body',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
-                    'request_body',
                 ]
             },
             root_map={
                 'validations': {
-                    ('request_body',): {
-
-                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
-                    'request_body':
-                        ([str],),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'request_body': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.update_empty_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testRuns',
+                'operation_id': 'update_empty',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'update_empty_request',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'update_empty_request':
+                        (UpdateEmptyRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'update_empty_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -767,32 +1201,30 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
-    def add_test_points_to_test_suite(
+    def api_v2_test_runs_delete(
         self,
-        id,
         **kwargs
     ):
-        """Add test-points to test suite  # noqa: E501
+        """Delete multiple test runs  # noqa: E501
 
+        <br>Use case  <br>User sets selection parameters of test runs  <br>System search and delete collection of test runs  <br>System returns the number of deleted test runs  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.add_test_points_to_test_suite(id, async_req=True)
+        >>> thread = api.api_v2_test_runs_delete(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            id (str): Test suite internal identifier
 
         Keyword Args:
-            api_v2_projects_project_id_work_items_search_post_request (ApiV2ProjectsProjectIdWorkItemsSearchPostRequest): Filter object to retrieve work items for test-suite's project. [optional]
+            api_v2_test_runs_delete_request (ApiV2TestRunsDeleteRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -817,15 +1249,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            int
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -846,37 +1278,34 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['id'] = \
-            id
-        return self.add_test_points_to_test_suite_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_runs_delete_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_suites_id_patch(
+    def api_v2_test_runs_id_delete(
         self,
         id,
         **kwargs
     ):
-        """Patch test suite  # noqa: E501
+        """Delete test run  # noqa: E501
 
-        See <a href=\"https://www.rfc-editor.org/rfc/rfc6902\" target=\"_blank\">RFC 6902: JavaScript Object Notation (JSON) Patch</a> for details  # noqa: E501
+        <br>Use case  <br>User sets test run internal (guid format) identifier  <br>System search and delete test run  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_suites_id_patch(id, async_req=True)
+        >>> thread = api.api_v2_test_runs_id_delete(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test Suite internal (UUID) identifier
+            id (str): Test run internal (UUID) identifier
 
         Keyword Args:
-            operation ([Operation]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -932,31 +1361,32 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.api_v2_test_suites_id_patch_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_runs_id_delete_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_suites_id_refresh_post(
+    def api_v2_test_runs_id_purge_post(
         self,
         id,
         **kwargs
     ):
-        """Refresh test suite. Only dynamic test suites are supported by this method  # noqa: E501
+        """Permanently delete test run from archive  # noqa: E501
 
+        <br>Use case  <br>User sets archived test run internal (guid format) identifier  <br>System search and purge archived test run  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_suites_id_refresh_post(id, async_req=True)
+        >>> thread = api.api_v2_test_runs_id_purge_post(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test Suite internal (UUID) identifier
+            id (str): Test run internal (UUID) identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1014,34 +1444,34 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.api_v2_test_suites_id_refresh_post_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_runs_id_purge_post_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_suites_id_work_items_post(
+    def api_v2_test_runs_id_restore_post(
         self,
         id,
         **kwargs
     ):
-        """Set work items for test suite  # noqa: E501
+        """Restore test run from the archive  # noqa: E501
 
+        <br>Use case  <br>User sets archived test run internal (guid format) identifier  <br>System search and restore test run  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_suites_id_work_items_post(id, async_req=True)
+        >>> thread = api.api_v2_test_runs_id_restore_post(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Unique ID of the test suite
+            id (str): Unique ID of the test run
 
         Keyword Args:
-            request_body ([str]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1097,31 +1527,34 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.api_v2_test_suites_id_work_items_post_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_runs_id_restore_post_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_suites_post(
+    def api_v2_test_runs_id_statistics_filter_post(
         self,
+        id,
         **kwargs
     ):
-        """Create test suite  # noqa: E501
+        """Search for the test run test results and build statistics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_suites_post(async_req=True)
+        >>> thread = api.api_v2_test_runs_id_statistics_filter_post(id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            id (str): Test run unique ID
 
         Keyword Args:
-            api_v2_test_suites_post_request (ApiV2TestSuitesPostRequest): [optional]
+            api_v2_test_runs_id_statistics_filter_post_request (ApiV2TestRunsIdStatisticsFilterPostRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1146,15 +1579,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TestSuiteV2GetModel
+            TestResultsStatisticsGetModel
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1175,31 +1608,35 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.api_v2_test_suites_post_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = \
+            id
+        return self.api_v2_test_runs_id_statistics_filter_post_endpoint.call_with_http_info(**kwargs)
 
-    def api_v2_test_suites_put(
+    def api_v2_test_runs_id_test_points_results_get(
         self,
+        id,
         **kwargs
     ):
-        """Edit test suite  # noqa: E501
+        """Get test results from the test run grouped by test points  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_v2_test_suites_put(async_req=True)
+        >>> thread = api.api_v2_test_runs_id_test_points_results_get(id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            id (str): Test run unique ID
 
         Keyword Args:
-            api_v2_test_suites_put_request (ApiV2TestSuitesPutRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1224,15 +1661,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            [TestPointResultModel]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1253,34 +1690,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.api_v2_test_suites_put_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = \
+            id
+        return self.api_v2_test_runs_id_test_points_results_get_endpoint.call_with_http_info(**kwargs)
 
-    def delete_test_suite(
+    def api_v2_test_runs_id_test_results_bulk_put(
         self,
         id,
         **kwargs
     ):
-        """Delete TestSuite  # noqa: E501
+        """Partial edit of multiple test results in the test run  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System deletes test suite  <br>System returns no content response  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_test_suite(id, async_req=True)
+        >>> thread = api.api_v2_test_runs_id_test_results_bulk_put(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test suite internal (guid format) identifier\"
+            id (str): Test run unique ID
 
         Keyword Args:
+            api_v2_test_runs_id_test_results_bulk_put_request (ApiV2TestRunsIdTestResultsBulkPutRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1336,32 +1775,31 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.delete_test_suite_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_runs_id_test_results_bulk_put_endpoint.call_with_http_info(**kwargs)
 
-    def get_configurations_by_test_suite_id(
+    def api_v2_test_runs_id_test_results_last_modified_modification_date_get(
         self,
         id,
         **kwargs
     ):
-        """Get Configurations By Id  # noqa: E501
+        """Get modification date of last test result of the test run  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search configurations related to the test points  <br>System returns configurations array  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_configurations_by_test_suite_id(id, async_req=True)
+        >>> thread = api.api_v2_test_runs_id_test_results_last_modified_modification_date_get(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test suite internal (guid format) identifier\"
+            id (str): Test run unique ID
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1388,15 +1826,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            [ConfigurationModel]
+            datetime
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1419,32 +1857,351 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.get_configurations_by_test_suite_id_endpoint.call_with_http_info(**kwargs)
+        return self.api_v2_test_runs_id_test_results_last_modified_modification_date_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_v2_test_runs_purge_bulk_post(
+        self,
+        **kwargs
+    ):
+        """Permanently delete multiple test runs from archive  # noqa: E501
+
+        <br>Use case  <br>User sets selection parameters of archived test runs  <br>System search and delete collection of archived test runs  <br>System returns the number of deleted archived test runs  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_runs_purge_bulk_post(async_req=True)
+        >>> result = thread.get()
 
-    def get_test_points_by_id(
+
+        Keyword Args:
+            api_v2_test_runs_delete_request (ApiV2TestRunsDeleteRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            int
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.api_v2_test_runs_purge_bulk_post_endpoint.call_with_http_info(**kwargs)
+
+    def api_v2_test_runs_restore_bulk_post(
+        self,
+        **kwargs
+    ):
+        """Restore multiple test runs from the archive  # noqa: E501
+
+        <br>Use case  <br>User sets selection parameters of archived test runs  <br>System search and restore collection of archived test runs  <br>System returns the number of restored test runs  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_runs_restore_bulk_post(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            api_v2_test_runs_delete_request (ApiV2TestRunsDeleteRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            int
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.api_v2_test_runs_restore_bulk_post_endpoint.call_with_http_info(**kwargs)
+
+    def api_v2_test_runs_search_post(
+        self,
+        **kwargs
+    ):
+        """Search for test runs  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_runs_search_post(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            skip (int): Amount of items to be skipped (offset). [optional]
+            take (int): Amount of items to be taken (limit). [optional]
+            order_by (str): SQL-like  ORDER BY statement (column1 ASC|DESC , column2 ASC|DESC). [optional]
+            search_field (str): Property name for searching. [optional]
+            search_value (str): Value for searching. [optional]
+            api_v2_test_runs_search_post_request (ApiV2TestRunsSearchPostRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [TestRunShortGetModel]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.api_v2_test_runs_search_post_endpoint.call_with_http_info(**kwargs)
+
+    def api_v2_test_runs_update_multiple_post(
+        self,
+        **kwargs
+    ):
+        """Update multiple test runs  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_runs_update_multiple_post(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            api_v2_test_runs_update_multiple_post_request (ApiV2TestRunsUpdateMultiplePostRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.api_v2_test_runs_update_multiple_post_endpoint.call_with_http_info(**kwargs)
+
+    def complete_test_run(
         self,
         id,
         **kwargs
     ):
-        """Get TestPoints By Id  # noqa: E501
+        """Complete TestRun  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System returns test points array  # noqa: E501
+        <br>Use case  <br>User sets test run identifier  <br>User runs method execution  <br>System completes test run  <br>System returns no content response  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_test_points_by_id(id, async_req=True)
+        >>> thread = api.complete_test_run(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test suite internal (guid format) identifier\"
+            id (str): Test Run internal identifier (GUID format)
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1471,15 +2228,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            [TestPointByTestSuiteModel]
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1502,32 +2259,348 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.get_test_points_by_id_endpoint.call_with_http_info(**kwargs)
+        return self.complete_test_run_endpoint.call_with_http_info(**kwargs)
+
+    def create_and_fill_by_auto_tests(
+        self,
+        **kwargs
+    ):
+        """Create test runs based on autotests and configurations  # noqa: E501
+
+        This method creates a test run based on an autotest and a configuration.  The difference between the `POST /api/v2/testRuns/byWorkItems` and `POST /api/v2/testRuns/byConfigurations` methods is  that in this method there is no need to create a test plan and work items (test cases and checklists).  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_and_fill_by_auto_tests(async_req=True)
+        >>> result = thread.get()
+
 
-    def get_test_results_by_id(
+        Keyword Args:
+            create_and_fill_by_auto_tests_request (CreateAndFillByAutoTestsRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            TestRunV2GetModel
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.create_and_fill_by_auto_tests_endpoint.call_with_http_info(**kwargs)
+
+    def create_and_fill_by_configurations(
+        self,
+        **kwargs
+    ):
+        """Create test runs picking the needed test points  # noqa: E501
+
+        This method creates a test run based on a combination of a configuration and a work item(test case or checklist).  Before you create a test run using this method, make sure to create a test plan. Work items must be automated.  This method is different from the `POST /api/v2/testRuns/byWorkItems` method because of the ability to send a  jagged array within the \"<b>testPointSelectors</b>\" parameter.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_and_fill_by_configurations(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            create_and_fill_by_configurations_request (CreateAndFillByConfigurationsRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            TestRunV2GetModel
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.create_and_fill_by_configurations_endpoint.call_with_http_info(**kwargs)
+
+    def create_and_fill_by_work_items(
+        self,
+        **kwargs
+    ):
+        """Create test run based on configurations and work items  # noqa: E501
+
+        This method creates a test run based on a combination of configuration and work item (test case or checklist).  Before you create a test run using this method, make sure to create a test plan.  Work items must be automated.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_and_fill_by_work_items(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            create_and_fill_by_work_items_request (CreateAndFillByWorkItemsRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            TestRunV2GetModel
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.create_and_fill_by_work_items_endpoint.call_with_http_info(**kwargs)
+
+    def create_empty(
+        self,
+        **kwargs
+    ):
+        """Create empty TestRun  # noqa: E501
+
+        <br>Use case  <br>User sets test run model (listed in the request example)  <br>User runs method execution  <br>System creates test run  <br>System returns test run model  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_empty(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            create_empty_request (CreateEmptyRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            TestRunV2GetModel
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.create_empty_endpoint.call_with_http_info(**kwargs)
+
+    def get_test_run_by_id(
         self,
         id,
         **kwargs
     ):
-        """Get TestResults By Id  # noqa: E501
+        """Get TestRun by Id  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search test results related to the test points  <br>System returns test results array  # noqa: E501
+        <br>Use case  <br>User sets test run identifier  <br>User runs method execution  <br>System finds test run  <br>System returns test run  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_test_results_by_id(id, async_req=True)
+        >>> thread = api.get_test_run_by_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test suite internal (guid format) identifier\"
+            id (str): Test Run internal identifier (GUID format)
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1554,15 +2627,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            [TestResultV2ShortModel]
+            TestRunV2GetModel
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1585,34 +2658,35 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.get_test_results_by_id_endpoint.call_with_http_info(**kwargs)
+        return self.get_test_run_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def get_test_suite_by_id(
+    def set_auto_test_results_for_test_run(
         self,
         id,
         **kwargs
     ):
-        """Get TestSuite by Id  # noqa: E501
+        """Send test results to the test runs in the system  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>User runs method execution  <br>System search test suite by identifier  <br>System returns test suite  # noqa: E501
+        This method sends test results to the test management system.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_test_suite_by_id(id, async_req=True)
+        >>> thread = api.set_auto_test_results_for_test_run(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test suite internal (guid format) identifier\"
+            id (str): Test Run internal identifier (GUID format)
 
         Keyword Args:
+            auto_test_results_for_test_run_model ([AutoTestResultsForTestRunModel]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1637,15 +2711,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TestSuiteV2GetModel
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1668,40 +2742,34 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.get_test_suite_by_id_endpoint.call_with_http_info(**kwargs)
+        return self.set_auto_test_results_for_test_run_endpoint.call_with_http_info(**kwargs)
 
-    def search_work_items(
+    def start_test_run(
         self,
         id,
         **kwargs
     ):
-        """Search WorkItems  # noqa: E501
+        """Start TestRun  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>[Optional] User sets filter  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search work items related to the test points  <br>                      [Optional] User sets filter, system applies filter                    <br>System returns work items array  # noqa: E501
+        <br>Use case  <br>User sets test run identifier  <br>User runs method execution  <br>System starts test run  <br>System returns no content response  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.search_work_items(id, async_req=True)
+        >>> thread = api.start_test_run(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test suite internal (guid format) identifier\"
+            id (str): Test Run internal identifier (GUID format)
 
         Keyword Args:
-            skip (int): Amount of items to be skipped (offset). [optional]
-            take (int): Amount of items to be taken (limit). [optional]
-            order_by (str): SQL-like  ORDER BY statement (column1 ASC|DESC , column2 ASC|DESC). [optional]
-            search_field (str): Property name for searching. [optional]
-            search_value (str): Value for searching. [optional]
-            search_work_items_request (SearchWorkItemsRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1726,15 +2794,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            [WorkItemShortModel]
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1757,35 +2825,34 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.search_work_items_endpoint.call_with_http_info(**kwargs)
+        return self.start_test_run_endpoint.call_with_http_info(**kwargs)
 
-    def set_configurations_by_test_suite_id(
+    def stop_test_run(
         self,
         id,
         **kwargs
     ):
-        """Set Configurations By TestSuite Id  # noqa: E501
+        """Stop TestRun  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>User sets collection of configuration identifiers  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search configuration  <br>System restores(if exist) or creates test points with listed configuration  <br>System returns no content response  # noqa: E501
+        <br>Use case  <br>User sets test run identifier  <br>User runs method execution  <br>System stops test run  <br>System returns no content response  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.set_configurations_by_test_suite_id(id, async_req=True)
+        >>> thread = api.stop_test_run(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): Test suite internal (guid format) identifier\"
+            id (str): Test Run internal identifier (GUID format)
 
         Keyword Args:
-            request_body ([str]): Collection of configuration identifiers\". [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1841,9 +2908,88 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
-        return self.set_configurations_by_test_suite_id_endpoint.call_with_http_info(**kwargs)
+        return self.stop_test_run_endpoint.call_with_http_info(**kwargs)
+
+    def update_empty(
+        self,
+        **kwargs
+    ):
+        """Update empty TestRun  # noqa: E501
+
+        <br>Use case  <br>User sets test run properties (listed in the request example)  <br>User runs method execution  <br>System updates test run  <br>System returns returns no content response  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_empty(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            update_empty_request (UpdateEmptyRequest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.update_empty_endpoint.call_with_http_info(**kwargs)
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/webhooks_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/webhooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     none_type,
     validate_and_convert_types
 )
 from testit_api_client.model.api_v2_webhooks_post_request import ApiV2WebhooksPostRequest
 from testit_api_client.model.api_v2_webhooks_search_post_request import ApiV2WebhooksSearchPostRequest
 from testit_api_client.model.api_v2_webhooks_test_post_request import ApiV2WebhooksTestPostRequest
 from testit_api_client.model.problem_details import ProblemDetails
-from testit_api_client.model.request_data import RequestData
 from testit_api_client.model.web_hook_event_type import WebHookEventType
 from testit_api_client.model.web_hook_model import WebHookModel
+from testit_api_client.model.webhook_response import WebhookResponse
 from testit_api_client.model.webhook_variables_type import WebhookVariablesType
 
 
 class WebhooksApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -427,15 +427,15 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.api_v2_webhooks_test_post_endpoint = _Endpoint(
             settings={
-                'response_type': (RequestData,),
+                'response_type': (WebhookResponse,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/webhooks/test',
                 'operation_id': 'api_v2_webhooks_test_post',
                 'http_method': 'POST',
                 'servers': None,
@@ -1088,15 +1088,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            RequestData
+            WebhookResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/webhooks_logs_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/webhooks_logs_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/work_items_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/work_items_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api/work_items_comments_api.py` & `testit_api_client-4.0.0/src/testit_api_client/api/work_items_comments_api.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/api_client.py` & `testit_api_client-4.0.0/src/testit_api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.6.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/apis/__init__.py` & `testit_api_client-4.0.0/src/testit_api_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/configuration.py` & `testit_api_client-4.0.0/src/testit_api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v2.0\n"\
-               "SDK Package Version: 3.5.0".\
+               "SDK Package Version: 3.6.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/exceptions.py` & `testit_api_client-4.0.0/src/testit_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/action_update.py` & `testit_api_client-4.0.0/src/testit_api_client/model/action_update.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_attachments_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_attachments_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_auto_tests_flaky_bulk_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_auto_tests_flaky_bulk_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_auto_tests_id_test_results_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_auto_tests_id_test_results_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_auto_tests_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_auto_tests_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_background_jobs_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_background_jobs_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_configurations_create_by_parameters_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_configurations_create_by_parameters_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_configurations_purge_bulk_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_configurations_purge_bulk_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_configurations_put_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_configurations_put_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_configurations_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_configurations_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_global_id_put_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_global_id_put_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_global_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_global_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_templates_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_templates_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_templates_put_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_templates_put_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_custom_attributes_templates_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_custom_attributes_templates_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_notifications_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_notifications_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_parameters_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_parameters_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_attributes_templates_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_attributes_templates_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_test_plans_delete_bulk_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_test_plans_delete_bulk_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_test_plans_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_test_plans_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_work_items_search_grouped_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_work_items_search_grouped_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_project_id_work_items_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_project_id_work_items_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_restore_bulk_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_restore_bulk_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_projects_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_projects_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_search_global_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_search_global_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_tags_delete_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_tags_delete_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_tags_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_tags_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_tags_put_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_tags_put_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_plans_id_export_test_points_xlsx_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_plans_id_export_test_points_xlsx_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_plans_id_test_points_tester_user_id_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_plans_id_test_points_tester_user_id_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_plans_id_test_runs_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_plans_id_test_runs_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_points_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_points_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_results_id_put_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_results_id_put_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_results_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_results_search_post_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,21 +29,27 @@
 from testit_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from testit_api_client.model.failure_category_model import FailureCategoryModel
     from testit_api_client.model.test_result_outcome import TestResultOutcome
     from testit_api_client.model.test_results_filter_model import TestResultsFilterModel
+    from testit_api_client.model.test_results_filter_model_completed_on import TestResultsFilterModelCompletedOn
     from testit_api_client.model.test_results_filter_model_created_date import TestResultsFilterModelCreatedDate
     from testit_api_client.model.test_results_filter_model_duration import TestResultsFilterModelDuration
+    from testit_api_client.model.test_results_filter_model_modified_date import TestResultsFilterModelModifiedDate
+    from testit_api_client.model.test_results_filter_model_started_on import TestResultsFilterModelStartedOn
     globals()['FailureCategoryModel'] = FailureCategoryModel
     globals()['TestResultOutcome'] = TestResultOutcome
     globals()['TestResultsFilterModel'] = TestResultsFilterModel
+    globals()['TestResultsFilterModelCompletedOn'] = TestResultsFilterModelCompletedOn
     globals()['TestResultsFilterModelCreatedDate'] = TestResultsFilterModelCreatedDate
     globals()['TestResultsFilterModelDuration'] = TestResultsFilterModelDuration
+    globals()['TestResultsFilterModelModifiedDate'] = TestResultsFilterModelModifiedDate
+    globals()['TestResultsFilterModelStartedOn'] = TestResultsFilterModelStartedOn
 
 
 class ApiV2TestResultsSearchPostRequest(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -103,14 +109,17 @@
         """
         lazy_import()
         return {
             'test_run_ids': ([str], none_type,),  # noqa: E501
             'auto_test_global_ids': ([int], none_type,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'created_date': (TestResultsFilterModelCreatedDate,),  # noqa: E501
+            'modified_date': (TestResultsFilterModelModifiedDate,),  # noqa: E501
+            'started_on': (TestResultsFilterModelStartedOn,),  # noqa: E501
+            'completed_on': (TestResultsFilterModelCompletedOn,),  # noqa: E501
             'duration': (TestResultsFilterModelDuration,),  # noqa: E501
             'result_reasons': ([str], none_type,),  # noqa: E501
             'configuration_ids': ([str], none_type,),  # noqa: E501
             'outcomes': ([TestResultOutcome], none_type,),  # noqa: E501
             'failure_categories': ([FailureCategoryModel], none_type,),  # noqa: E501
             'namespace': (str, none_type,),  # noqa: E501
             'class_name': (str, none_type,),  # noqa: E501
@@ -122,14 +131,17 @@
 
 
     attribute_map = {
         'test_run_ids': 'testRunIds',  # noqa: E501
         'auto_test_global_ids': 'autoTestGlobalIds',  # noqa: E501
         'name': 'name',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
+        'modified_date': 'modifiedDate',  # noqa: E501
+        'started_on': 'startedOn',  # noqa: E501
+        'completed_on': 'completedOn',  # noqa: E501
         'duration': 'duration',  # noqa: E501
         'result_reasons': 'resultReasons',  # noqa: E501
         'configuration_ids': 'configurationIds',  # noqa: E501
         'outcomes': 'outcomes',  # noqa: E501
         'failure_categories': 'failureCategories',  # noqa: E501
         'namespace': 'namespace',  # noqa: E501
         'class_name': 'className',  # noqa: E501
@@ -174,14 +186,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             test_run_ids ([str], none_type): Specifies a test result test run IDs to search for. [optional]  # noqa: E501
             auto_test_global_ids ([int], none_type): Specifies an autotest global IDs to search results for. [optional]  # noqa: E501
             name (str, none_type): Specifies an autotest name to search results for. [optional]  # noqa: E501
             created_date (TestResultsFilterModelCreatedDate): [optional]  # noqa: E501
+            modified_date (TestResultsFilterModelModifiedDate): [optional]  # noqa: E501
+            started_on (TestResultsFilterModelStartedOn): [optional]  # noqa: E501
+            completed_on (TestResultsFilterModelCompletedOn): [optional]  # noqa: E501
             duration (TestResultsFilterModelDuration): [optional]  # noqa: E501
             result_reasons ([str], none_type): Specifies result reasons for searching test results. [optional]  # noqa: E501
             configuration_ids ([str], none_type): Specifies a test result configuration IDs to search for. [optional]  # noqa: E501
             outcomes ([TestResultOutcome], none_type): Specifies a test result outcomes to search for. [optional]  # noqa: E501
             failure_categories ([FailureCategoryModel], none_type): Specifies a test result failure categories to search for. [optional]  # noqa: E501
             namespace (str, none_type): Specifies a test result namespace to search for. [optional]  # noqa: E501
             class_name (str, none_type): Specifies a test result class name to search for. [optional]  # noqa: E501
@@ -288,14 +303,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             test_run_ids ([str], none_type): Specifies a test result test run IDs to search for. [optional]  # noqa: E501
             auto_test_global_ids ([int], none_type): Specifies an autotest global IDs to search results for. [optional]  # noqa: E501
             name (str, none_type): Specifies an autotest name to search results for. [optional]  # noqa: E501
             created_date (TestResultsFilterModelCreatedDate): [optional]  # noqa: E501
+            modified_date (TestResultsFilterModelModifiedDate): [optional]  # noqa: E501
+            started_on (TestResultsFilterModelStartedOn): [optional]  # noqa: E501
+            completed_on (TestResultsFilterModelCompletedOn): [optional]  # noqa: E501
             duration (TestResultsFilterModelDuration): [optional]  # noqa: E501
             result_reasons ([str], none_type): Specifies result reasons for searching test results. [optional]  # noqa: E501
             configuration_ids ([str], none_type): Specifies a test result configuration IDs to search for. [optional]  # noqa: E501
             outcomes ([TestResultOutcome], none_type): Specifies a test result outcomes to search for. [optional]  # noqa: E501
             failure_categories ([FailureCategoryModel], none_type): Specifies a test result failure categories to search for. [optional]  # noqa: E501
             namespace (str, none_type): Specifies a test result namespace to search for. [optional]  # noqa: E501
             class_name (str, none_type): Specifies a test result class name to search for. [optional]  # noqa: E501
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_runs_id_statistics_filter_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_id_statistics_filter_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_runs_id_test_results_bulk_put_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_id_test_results_bulk_put_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_runs_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_runs_update_multiple_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_runs_update_multiple_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_suites_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_suites_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_test_suites_put_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_test_suites_put_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_webhooks_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_webhooks_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_webhooks_search_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_webhooks_search_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_webhooks_test_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_webhooks_test_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_comments_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_comments_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_comments_put_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_comments_put_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_move_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_move_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_shared_step_id_references_sections_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_shared_step_id_references_sections_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/api_v2_work_items_shared_step_id_references_work_items_post_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/api_v2_work_items_shared_step_id_references_work_items_post_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/attachment_change_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/attachment_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/attachment_change_view_model_array_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/attachment_change_view_model_array_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/attachment_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/attachment_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/attachment_model_auto_test_step_results_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/attachment_model_auto_test_step_results_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/attachment_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/attachment_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/attachment_put_model_auto_test_step_results_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/attachment_put_model_auto_test_step_results_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_average_duration_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_average_duration_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_change_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_change_view_model_array_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_change_view_model_array_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_id_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_id_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_model_v2_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_model_v2_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_namespace_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_namespace_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_related_to_test_result.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_related_to_test_result.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_results_for_test_run_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_results_for_test_run_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/auto_test_step_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/auto_test_step_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_filter_model_created_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_filter_model_created_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_filter_model_modified_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_filter_model_modified_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_filter_model_stability_percentage.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_filter_model_stability_percentage.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_historical_result_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_historical_result_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_result_historical_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_result_historical_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_result_outcome.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_result_outcome.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_result_reason_sub_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_result_reason_sub_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_select_model_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_select_model_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotest_select_model_filter.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotest_select_model_filter.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotests_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotests_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotests_extraction_model_ids.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotests_extraction_model_ids.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotests_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotests_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotests_select_model_filter.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotests_select_model_filter.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/autotests_select_model_includes.py` & `testit_api_client-4.0.0/src/testit_api_client/model/autotests_select_model_includes.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/available_test_result_outcome.py` & `testit_api_client-4.0.0/src/testit_api_client/model/available_test_result_outcome.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/background_job_attachment_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/background_job_attachment_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/background_job_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/background_job_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/background_job_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/background_job_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/background_job_state.py` & `testit_api_client-4.0.0/src/testit_api_client/model/background_job_state.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/background_job_type.py` & `testit_api_client-4.0.0/src/testit_api_client/model/background_job_type.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/boolean_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/boolean_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/boolean_nullable_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/boolean_nullable_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_by_parameters_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_by_parameters_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_extraction_model_ids.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_extraction_model_ids.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_extraction_model_project_ids.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_extraction_model_project_ids.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_select_model_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_select_model_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/configuration_select_model_filter.py` & `testit_api_client-4.0.0/src/testit_api_client/model/configuration_select_model_filter.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_and_fill_by_auto_tests_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_and_fill_by_auto_tests_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,17 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('configuration_ids',): {
+            'min_items': 1,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_and_fill_by_configurations_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_and_fill_by_configurations_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_and_fill_by_work_items_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_and_fill_by_work_items_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_auto_test_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_auto_test_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_configuration_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_configuration_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_empty_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_empty_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_parameter_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_parameter_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_project_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_project_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_projects_attribute_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_projects_attribute_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_section_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_section_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_test_plan_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_test_plan_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/create_work_item_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/create_work_item_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_change_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_change_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_put_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def lazy_import():
     from testit_api_client.model.custom_attribute_option_model import CustomAttributeOptionModel
     from testit_api_client.model.custom_attribute_types_enum import CustomAttributeTypesEnum
     globals()['CustomAttributeOptionModel'] = CustomAttributeOptionModel
     globals()['CustomAttributeTypesEnum'] = CustomAttributeTypesEnum
 
 
-class CustomAttributeModel(ModelNormal):
+class CustomAttributePutModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -116,20 +116,20 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, type, is_deleted, name, is_enabled, is_required, is_global, *args, **kwargs):  # noqa: E501
-        """CustomAttributeModel - a model defined in OpenAPI
+        """CustomAttributePutModel - a model defined in OpenAPI
 
         Args:
             id (str): Unique ID of the attribute
             type (CustomAttributeTypesEnum):
-            is_deleted (bool): Indicates if the attribute is deleted
+            is_deleted (bool): Indicates if the entity is deleted
             name (str): Name of the attribute
             is_enabled (bool): Indicates if the attribute is enabled
             is_required (bool): Indicates if the attribute value is mandatory to specify
             is_global (bool): Indicates if the attribute is available across all projects
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -218,20 +218,20 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, type, is_deleted, name, is_enabled, is_required, is_global, *args, **kwargs):  # noqa: E501
-        """CustomAttributeModel - a model defined in OpenAPI
+        """CustomAttributePutModel - a model defined in OpenAPI
 
         Args:
             id (str): Unique ID of the attribute
             type (CustomAttributeTypesEnum):
-            is_deleted (bool): Indicates if the attribute is deleted
+            is_deleted (bool): Indicates if the entity is deleted
             name (str): Name of the attribute
             is_enabled (bool): Indicates if the attribute is enabled
             is_required (bool): Indicates if the attribute value is mandatory to specify
             is_global (bool): Indicates if the attribute is available across all projects
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_option_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_option_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_option_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_option_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def lazy_import():
     from testit_api_client.model.custom_attribute_option_model import CustomAttributeOptionModel
     from testit_api_client.model.custom_attribute_types_enum import CustomAttributeTypesEnum
     globals()['CustomAttributeOptionModel'] = CustomAttributeOptionModel
     globals()['CustomAttributeTypesEnum'] = CustomAttributeTypesEnum
 
 
-class CustomAttributePutModel(ModelNormal):
+class CustomAttributeModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,53 +83,54 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
+            'options': ([CustomAttributeOptionModel],),  # noqa: E501
             'type': (CustomAttributeTypesEnum,),  # noqa: E501
             'is_deleted': (bool,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'is_enabled': (bool,),  # noqa: E501
             'is_required': (bool,),  # noqa: E501
             'is_global': (bool,),  # noqa: E501
-            'options': ([CustomAttributeOptionModel], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
+        'options': 'options',  # noqa: E501
         'type': 'type',  # noqa: E501
         'is_deleted': 'isDeleted',  # noqa: E501
         'name': 'name',  # noqa: E501
         'is_enabled': 'isEnabled',  # noqa: E501
         'is_required': 'isRequired',  # noqa: E501
         'is_global': 'isGlobal',  # noqa: E501
-        'options': 'options',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, type, is_deleted, name, is_enabled, is_required, is_global, *args, **kwargs):  # noqa: E501
-        """CustomAttributePutModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, options, type, is_deleted, name, is_enabled, is_required, is_global, *args, **kwargs):  # noqa: E501
+        """CustomAttributeModel - a model defined in OpenAPI
 
         Args:
             id (str): Unique ID of the attribute
+            options ([CustomAttributeOptionModel]): Collection of the attribute options  <br />  Available for attributes of type `options` and `multiple options` only
             type (CustomAttributeTypesEnum):
-            is_deleted (bool): Indicates if the entity is deleted
+            is_deleted (bool): Indicates if the attribute is deleted
             name (str): Name of the attribute
             is_enabled (bool): Indicates if the attribute is enabled
             is_required (bool): Indicates if the attribute value is mandatory to specify
             is_global (bool): Indicates if the attribute is available across all projects
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -158,15 +159,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            options ([CustomAttributeOptionModel], none_type): Collection of the attribute options  <br />  Available for attributes of type `options` and `multiple options` only. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,14 +191,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
+        self.options = options
         self.type = type
         self.is_deleted = is_deleted
         self.name = name
         self.is_enabled = is_enabled
         self.is_required = is_required
         self.is_global = is_global
         for var_name, var_value in kwargs.items():
@@ -217,21 +218,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, type, is_deleted, name, is_enabled, is_required, is_global, *args, **kwargs):  # noqa: E501
-        """CustomAttributePutModel - a model defined in OpenAPI
+    def __init__(self, id, options, type, is_deleted, name, is_enabled, is_required, is_global, *args, **kwargs):  # noqa: E501
+        """CustomAttributeModel - a model defined in OpenAPI
 
         Args:
             id (str): Unique ID of the attribute
+            options ([CustomAttributeOptionModel]): Collection of the attribute options  <br />  Available for attributes of type `options` and `multiple options` only
             type (CustomAttributeTypesEnum):
-            is_deleted (bool): Indicates if the entity is deleted
+            is_deleted (bool): Indicates if the attribute is deleted
             name (str): Name of the attribute
             is_enabled (bool): Indicates if the attribute is enabled
             is_required (bool): Indicates if the attribute value is mandatory to specify
             is_global (bool): Indicates if the attribute is available across all projects
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -260,15 +262,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            options ([CustomAttributeOptionModel], none_type): Collection of the attribute options  <br />  Available for attributes of type `options` and `multiple options` only. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -291,14 +292,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
+        self.options = options
         self.type = type
         self.is_deleted = is_deleted
         self.name = name
         self.is_enabled = is_enabled
         self.is_required = is_required
         self.is_global = is_global
         for var_name, var_value in kwargs.items():
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_search_query_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_search_query_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_template_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_template_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_template_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_template_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_template_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_template_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_template_search_query_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_template_search_query_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_test_plan_project_relation_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_test_plan_project_relation_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/custom_attribute_types_enum.py` & `testit_api_client-4.0.0/src/testit_api_client/model/custom_attribute_types_enum.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/date_time_range_selector_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/date_time_range_selector_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/deletion_state.py` & `testit_api_client-4.0.0/src/testit_api_client/model/deletion_state.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/export_project_json_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/export_project_json_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/export_project_with_test_plans_json_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/export_project_with_test_plans_json_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/external_link_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/external_link_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/failure_category_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/failure_category_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/failure_class_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/failure_class_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/failure_class_regex_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/failure_class_regex_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/filter_model_data.py` & `testit_api_client-4.0.0/src/testit_api_client/model/filter_model_data.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/flaky_bulk_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/flaky_bulk_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/flaky_bulk_model_autotest_select.py` & `testit_api_client-4.0.0/src/testit_api_client/model/flaky_bulk_model_autotest_select.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/get_xlsx_test_points_by_test_plan_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/get_xlsx_test_points_by_test_plan_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/global_custom_attribute_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/global_custom_attribute_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/global_custom_attribute_update_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/global_custom_attribute_update_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/global_search_item_result.py` & `testit_api_client-4.0.0/src/testit_api_client/model/global_search_item_result.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/global_search_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/global_search_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/global_search_response.py` & `testit_api_client-4.0.0/src/testit_api_client/model/global_search_response.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/guid_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/guid_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/guid_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/guid_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/image_resize_type.py` & `testit_api_client-4.0.0/src/testit_api_client/model/image_resize_type.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/int32_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/int32_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/int32_range_selector_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/int32_range_selector_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/int64_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/int64_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/int64_range_selector_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/int64_range_selector_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/iteration_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/iteration_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/iteration_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/iteration_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/label_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/label_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/label_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/label_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/last_test_result_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/last_test_result_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/link_auto_test_to_work_item_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/link_auto_test_to_work_item_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/link_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/link_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/link_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/link_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/link_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/link_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/link_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/link_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/link_sub_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/link_sub_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/link_type.py` & `testit_api_client-4.0.0/src/testit_api_client/model/link_type.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/move_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/move_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/no_content_result.py` & `testit_api_client-4.0.0/src/testit_api_client/model/no_content_result.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/notification_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/notification_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/notification_query_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/notification_query_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/notification_type_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/notification_type_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/operation.py` & `testit_api_client-4.0.0/src/testit_api_client/model/operation.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/parameter_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/parameter_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/parameter_group_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/parameter_group_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/parameter_iteration_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/parameter_iteration_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/parameter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/parameter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/parameter_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/parameter_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/parameter_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/parameter_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/parameter_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/parameter_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/period_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/period_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/period_view_model_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/period_view_model_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/problem_details.py` & `testit_api_client-4.0.0/src/testit_api_client/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_attributes_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_attributes_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_custom_attribute_template_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_custom_attribute_template_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_custom_attributes_templates_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_custom_attributes_templates_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_export_query_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_export_query_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_export_with_test_plans_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_export_with_test_plans_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_shortest_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_shortest_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/project_test_plans_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/project_test_plans_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_autotests_count.py` & `testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_autotests_count.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_checklists_count.py` & `testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_checklists_count.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_created_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_created_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_shared_steps_count.py` & `testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_shared_steps_count.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/projects_filter_model_test_cases_count.py` & `testit_api_client-4.0.0/src/testit_api_client/model/projects_filter_model_test_cases_count.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/public_test_point_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/public_test_point_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,45 +79,48 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'configuration_id': (str,),  # noqa: E501
             'configuration_global_id': (int,),  # noqa: E501
             'iteration_id': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
             'auto_test_ids': ([str], none_type,),  # noqa: E501
             'parameter_models': ([ParameterShortModel], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'configuration_id': 'configurationId',  # noqa: E501
         'configuration_global_id': 'configurationGlobalId',  # noqa: E501
         'iteration_id': 'iterationId',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'auto_test_ids': 'autoTestIds',  # noqa: E501
         'parameter_models': 'parameterModels',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, configuration_id, configuration_global_id, iteration_id, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, configuration_id, configuration_global_id, iteration_id, id, *args, **kwargs):  # noqa: E501
         """PublicTestPointModel - a model defined in OpenAPI
 
         Args:
             configuration_id (str):
             configuration_global_id (int):
             iteration_id (str):
+            id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -178,14 +181,15 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.configuration_id = configuration_id
         self.configuration_global_id = configuration_global_id
         self.iteration_id = iteration_id
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,21 +202,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, configuration_id, configuration_global_id, iteration_id, *args, **kwargs):  # noqa: E501
+    def __init__(self, configuration_id, configuration_global_id, iteration_id, id, *args, **kwargs):  # noqa: E501
         """PublicTestPointModel - a model defined in OpenAPI
 
         Args:
             configuration_id (str):
             configuration_global_id (int):
             iteration_id (str):
+            id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -271,14 +276,15 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.configuration_id = configuration_id
         self.configuration_global_id = configuration_global_id
         self.iteration_id = iteration_id
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/public_test_run_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/public_test_run_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,16 @@
             'configurations': ([ConfigurationModel],),  # noqa: E501
             'auto_tests': ([AutoTestModel],),  # noqa: E501
             'test_points': ([PublicTestPointModel],),  # noqa: E501
             'status': (str,),  # noqa: E501
             'test_plan_id': (str, none_type,),  # noqa: E501
             'product_name': (str, none_type,),  # noqa: E501
             'build': (str, none_type,),  # noqa: E501
+            'custom_parameters': ({str: (str,)}, none_type,),  # noqa: E501
+            'test_run_description': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,14 +110,16 @@
         'configurations': 'configurations',  # noqa: E501
         'auto_tests': 'autoTests',  # noqa: E501
         'test_points': 'testPoints',  # noqa: E501
         'status': 'status',  # noqa: E501
         'test_plan_id': 'testPlanId',  # noqa: E501
         'product_name': 'productName',  # noqa: E501
         'build': 'build',  # noqa: E501
+        'custom_parameters': 'customParameters',  # noqa: E501
+        'test_run_description': 'testRunDescription',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -163,14 +167,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             test_plan_id (str, none_type): [optional]  # noqa: E501
             product_name (str, none_type): [optional]  # noqa: E501
             build (str, none_type): [optional]  # noqa: E501
+            custom_parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
+            test_run_description (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,14 +273,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             test_plan_id (str, none_type): [optional]  # noqa: E501
             product_name (str, none_type): [optional]  # noqa: E501
             build (str, none_type): [optional]  # noqa: E501
+            custom_parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
+            test_run_description (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/rename_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/rename_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/request_data.py` & `testit_api_client-4.0.0/src/testit_api_client/model/webhook_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testit_api_client.exceptions import ApiAttributeError
 
 
 
-class RequestData(ModelNormal):
+class WebhookResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, status_code, request_meta, response_body, response_meta, *args, **kwargs):  # noqa: E501
-        """RequestData - a model defined in OpenAPI
+        """WebhookResponse - a model defined in OpenAPI
 
         Args:
             status_code (int):
             request_meta (str):
             response_body (str):
             response_meta (str):
 
@@ -198,15 +198,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, status_code, request_meta, response_body, response_meta, *args, **kwargs):  # noqa: E501
-        """RequestData - a model defined in OpenAPI
+        """WebhookResponse - a model defined in OpenAPI
 
         Args:
             status_code (int):
             request_meta (str):
             response_body (str):
             response_meta (str):
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/request_type_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/request_type_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/search_attributes_in_project_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/search_attributes_in_project_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/search_auto_tests_query_includes_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/search_auto_tests_query_includes_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/search_custom_attribute_template_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/search_custom_attribute_template_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/search_webhooks_query_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/search_webhooks_query_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/search_work_items_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/search_work_items_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/section_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/section_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/section_move_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/section_move_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/section_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/section_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/section_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/section_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/section_rename_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/section_rename_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/section_shared_step.py` & `testit_api_client-4.0.0/src/testit_api_client/model/section_shared_step.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/section_with_steps_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/section_with_steps_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/set_of_attachment_ids.py` & `testit_api_client-4.0.0/src/testit_api_client/model/set_of_attachment_ids.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/set_of_links.py` & `testit_api_client-4.0.0/src/testit_api_client/model/set_of_links.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_change_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_section_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_section_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model_created_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model_created_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model_modified_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_reference_sections_query_filter_model_modified_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_references_query_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_references_query_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/shared_step_result_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/shared_step_result_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/short_configuration.py` & `testit_api_client-4.0.0/src/testit_api_client/model/short_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/step_comment_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/step_comment_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/step_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/step_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/step_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/step_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/step_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/step_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/step_result_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/step_result_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/string_array_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/string_array_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/string_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/string_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/string_changed_field_with_diffs_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/string_changed_field_with_diffs_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/tag_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/tag_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/tag_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/tag_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/tag_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/tag_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/tag_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/tag_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/tag_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/tag_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/tags_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/tags_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/tags_filter_model_created_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/tags_filter_model_created_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_change_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_change_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_change_model_test_plan_changed_fields.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_change_model_test_plan_changed_fields.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_changed_fields_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_changed_fields_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_group_by_status.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_group_by_status.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_group_by_test_suite.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_group_by_test_suite.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_group_by_tester.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_group_by_tester.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_group_by_tester_and_status.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_group_by_tester_and_status.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_link.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_link.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_status_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_status_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_with_analytic_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_with_analytic_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_with_analytic_model_analytic.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_with_analytic_model_analytic.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_plan_with_test_suite_tree_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_plan_with_test_suite_tree_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_analytic_result.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_analytic_result.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_by_test_suite_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_by_test_suite_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_change_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_change_view_model_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_change_view_model_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_created_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_created_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_duration.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_duration.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_modified_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_modified_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_work_item_created_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_work_item_created_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_work_item_median_duration.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_work_item_median_duration.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_filter_model_work_item_modified_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_filter_model_work_item_modified_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_related_to_test_result.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_related_to_test_result.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_result_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_result_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_selector.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_selector.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_short_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_short_get_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,17 +89,19 @@
             'id': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'attributes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'links': ([str],),  # noqa: E501
             'test_suite_id': (str,),  # noqa: E501
+            'test_suite_name': (str,),  # noqa: E501
             'work_item_id': (str,),  # noqa: E501
             'work_item_global_id': (int,),  # noqa: E501
             'work_item_version_id': (str,),  # noqa: E501
+            'work_item_version_number': (int,),  # noqa: E501
             'status': (TestPointStatus,),  # noqa: E501
             'priority': (WorkItemPriorityModel,),  # noqa: E501
             'is_automated': (bool,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'configuration_id': (str,),  # noqa: E501
             'duration': (int,),  # noqa: E501
             'section_id': (str,),  # noqa: E501
@@ -128,17 +130,19 @@
         'id': 'id',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'links': 'links',  # noqa: E501
         'test_suite_id': 'testSuiteId',  # noqa: E501
+        'test_suite_name': 'testSuiteName',  # noqa: E501
         'work_item_id': 'workItemId',  # noqa: E501
         'work_item_global_id': 'workItemGlobalId',  # noqa: E501
         'work_item_version_id': 'workItemVersionId',  # noqa: E501
+        'work_item_version_number': 'workItemVersionNumber',  # noqa: E501
         'status': 'status',  # noqa: E501
         'priority': 'priority',  # noqa: E501
         'is_automated': 'isAutomated',  # noqa: E501
         'name': 'name',  # noqa: E501
         'configuration_id': 'configurationId',  # noqa: E501
         'duration': 'duration',  # noqa: E501
         'section_id': 'sectionId',  # noqa: E501
@@ -161,28 +165,30 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, created_date, created_by_id, attributes, tags, links, test_suite_id, work_item_id, work_item_global_id, work_item_version_id, status, priority, is_automated, name, configuration_id, duration, section_id, project_id, last_test_result, iteration_id, work_item_state, work_item_created_by_id, work_item_created_date, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, created_date, created_by_id, attributes, tags, links, test_suite_id, test_suite_name, work_item_id, work_item_global_id, work_item_version_id, work_item_version_number, status, priority, is_automated, name, configuration_id, duration, section_id, project_id, last_test_result, iteration_id, work_item_state, work_item_created_by_id, work_item_created_date, *args, **kwargs):  # noqa: E501
         """TestPointShortGetModel - a model defined in OpenAPI
 
         Args:
             id (str): Unique ID of the test point
             created_date (datetime): Creation date of the test point
             created_by_id (str): Unique ID of the test point creator
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Collection of attributes of work item the test point represents
             tags ([str]): Collection of the test point tags
             links ([str]): Collection of the test point links
             test_suite_id (str): Unique ID of test suite the test point assigned to
+            test_suite_name (str): Name of the test suite
             work_item_id (str): Unique ID of work item the test point represents
             work_item_global_id (int): Global ID of work item the test point represents
             work_item_version_id (str): Unique ID of work item version the test point represents
+            work_item_version_number (int): Number of work item version the test point represents
             status (TestPointStatus):
             priority (WorkItemPriorityModel):
             is_automated (bool): Indicates if the test point represents an autotest
             name (str): Name of the test point
             configuration_id (str): Unique ID of the test point configuration
             duration (int): Duration of the test point
             section_id (str): Unique ID of section where work item the test point represents is located
@@ -266,17 +272,19 @@
         self.id = id
         self.created_date = created_date
         self.created_by_id = created_by_id
         self.attributes = attributes
         self.tags = tags
         self.links = links
         self.test_suite_id = test_suite_id
+        self.test_suite_name = test_suite_name
         self.work_item_id = work_item_id
         self.work_item_global_id = work_item_global_id
         self.work_item_version_id = work_item_version_id
+        self.work_item_version_number = work_item_version_number
         self.status = status
         self.priority = priority
         self.is_automated = is_automated
         self.name = name
         self.configuration_id = configuration_id
         self.duration = duration
         self.section_id = section_id
@@ -302,28 +310,30 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, created_date, created_by_id, attributes, tags, links, test_suite_id, work_item_id, work_item_global_id, work_item_version_id, status, priority, is_automated, name, configuration_id, duration, section_id, project_id, last_test_result, iteration_id, work_item_state, work_item_created_by_id, work_item_created_date, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, created_date, created_by_id, attributes, tags, links, test_suite_id, test_suite_name, work_item_id, work_item_global_id, work_item_version_id, work_item_version_number, status, priority, is_automated, name, configuration_id, duration, section_id, project_id, last_test_result, iteration_id, work_item_state, work_item_created_by_id, work_item_created_date, *args, **kwargs):  # noqa: E501
         """TestPointShortGetModel - a model defined in OpenAPI
 
         Args:
             id (str): Unique ID of the test point
             created_date (datetime): Creation date of the test point
             created_by_id (str): Unique ID of the test point creator
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Collection of attributes of work item the test point represents
             tags ([str]): Collection of the test point tags
             links ([str]): Collection of the test point links
             test_suite_id (str): Unique ID of test suite the test point assigned to
+            test_suite_name (str): Name of the test suite
             work_item_id (str): Unique ID of work item the test point represents
             work_item_global_id (int): Global ID of work item the test point represents
             work_item_version_id (str): Unique ID of work item version the test point represents
+            work_item_version_number (int): Number of work item version the test point represents
             status (TestPointStatus):
             priority (WorkItemPriorityModel):
             is_automated (bool): Indicates if the test point represents an autotest
             name (str): Name of the test point
             configuration_id (str): Unique ID of the test point configuration
             duration (int): Duration of the test point
             section_id (str): Unique ID of section where work item the test point represents is located
@@ -405,17 +415,19 @@
         self.id = id
         self.created_date = created_date
         self.created_by_id = created_by_id
         self.attributes = attributes
         self.tags = tags
         self.links = links
         self.test_suite_id = test_suite_id
+        self.test_suite_name = test_suite_name
         self.work_item_id = work_item_id
         self.work_item_global_id = work_item_global_id
         self.work_item_version_id = work_item_version_id
+        self.work_item_version_number = work_item_version_number
         self.status = status
         self.priority = priority
         self.is_automated = is_automated
         self.name = name
         self.configuration_id = configuration_id
         self.duration = duration
         self.section_id = section_id
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_short_get_model_last_test_result.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_short_get_model_last_test_result.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_status.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_status.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_point_with_last_result_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_point_with_last_result_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_points_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_points_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_points_extraction_model_ids.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_points_extraction_model_ids.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_change_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_change_view_model_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_change_view_model_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_chronology_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_chronology_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_configuration.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_history_report_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_history_report_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_outcome.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_outcome.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_short_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_short_get_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,17 +89,21 @@
             'autotest_global_id': (int,),  # noqa: E501
             'test_run_id': (str,),  # noqa: E501
             'configuration_id': (str,),  # noqa: E501
             'configuration_name': (str,),  # noqa: E501
             'outcome': (str,),  # noqa: E501
             'result_reasons': ([AutotestResultReasonSubGetModel],),  # noqa: E501
             'date': (datetime,),  # noqa: E501
+            'created_date': (datetime,),  # noqa: E501
             'links': ([LinkSubGetModel],),  # noqa: E501
             'attachments': ([AttachmentModel],),  # noqa: E501
             'comment': (str, none_type,),  # noqa: E501
+            'modified_date': (datetime, none_type,),  # noqa: E501
+            'started_on': (datetime, none_type,),  # noqa: E501
+            'completed_on': (datetime, none_type,),  # noqa: E501
             'duration': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -110,40 +114,45 @@
         'autotest_global_id': 'autotestGlobalId',  # noqa: E501
         'test_run_id': 'testRunId',  # noqa: E501
         'configuration_id': 'configurationId',  # noqa: E501
         'configuration_name': 'configurationName',  # noqa: E501
         'outcome': 'outcome',  # noqa: E501
         'result_reasons': 'resultReasons',  # noqa: E501
         'date': 'date',  # noqa: E501
+        'created_date': 'createdDate',  # noqa: E501
         'links': 'links',  # noqa: E501
         'attachments': 'attachments',  # noqa: E501
         'comment': 'comment',  # noqa: E501
+        'modified_date': 'modifiedDate',  # noqa: E501
+        'started_on': 'startedOn',  # noqa: E501
+        'completed_on': 'completedOn',  # noqa: E501
         'duration': 'duration',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, autotest_global_id, test_run_id, configuration_id, configuration_name, outcome, result_reasons, date, links, attachments, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, name, autotest_global_id, test_run_id, configuration_id, configuration_name, outcome, result_reasons, date, created_date, links, attachments, *args, **kwargs):  # noqa: E501
         """TestResultShortGetModel - a model defined in OpenAPI
 
         Args:
             id (str): Unique ID of the test result
             name (str): Name of autotest represented by the test result
             autotest_global_id (int): Global ID of autotest represented by the test result
             test_run_id (str): Unique ID of test run where the test result is located
             configuration_id (str): Unique ID of configuration which the test result uses
             configuration_name (str): Name of configuration which the test result uses
             outcome (str): Outcome of the test result
             result_reasons ([AutotestResultReasonSubGetModel]): Collection of result reasons which the test result have
-            date (datetime): Date when the test result has been set
+            date (datetime): Date when the test result was completed or started or created
+            created_date (datetime): Date when the test result has been created
             links ([LinkSubGetModel]): Collection of links attached to the test result
             attachments ([AttachmentModel]): Collection of files attached to the test result
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -171,14 +180,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             comment (str, none_type): Comment to the test result. [optional]  # noqa: E501
+            modified_date (datetime, none_type): Date when the test result has been modified. [optional]  # noqa: E501
+            started_on (datetime, none_type): Date when the test result has been started. [optional]  # noqa: E501
+            completed_on (datetime, none_type): Date when the test result has been completed. [optional]  # noqa: E501
             duration (int, none_type): Time which it took to run the test. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -212,14 +224,15 @@
         self.autotest_global_id = autotest_global_id
         self.test_run_id = test_run_id
         self.configuration_id = configuration_id
         self.configuration_name = configuration_name
         self.outcome = outcome
         self.result_reasons = result_reasons
         self.date = date
+        self.created_date = created_date
         self.links = links
         self.attachments = attachments
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -234,27 +247,28 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, autotest_global_id, test_run_id, configuration_id, configuration_name, outcome, result_reasons, date, links, attachments, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, name, autotest_global_id, test_run_id, configuration_id, configuration_name, outcome, result_reasons, date, created_date, links, attachments, *args, **kwargs):  # noqa: E501
         """TestResultShortGetModel - a model defined in OpenAPI
 
         Args:
             id (str): Unique ID of the test result
             name (str): Name of autotest represented by the test result
             autotest_global_id (int): Global ID of autotest represented by the test result
             test_run_id (str): Unique ID of test run where the test result is located
             configuration_id (str): Unique ID of configuration which the test result uses
             configuration_name (str): Name of configuration which the test result uses
             outcome (str): Outcome of the test result
             result_reasons ([AutotestResultReasonSubGetModel]): Collection of result reasons which the test result have
-            date (datetime): Date when the test result has been set
+            date (datetime): Date when the test result was completed or started or created
+            created_date (datetime): Date when the test result has been created
             links ([LinkSubGetModel]): Collection of links attached to the test result
             attachments ([AttachmentModel]): Collection of files attached to the test result
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -282,14 +296,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             comment (str, none_type): Comment to the test result. [optional]  # noqa: E501
+            modified_date (datetime, none_type): Date when the test result has been modified. [optional]  # noqa: E501
+            started_on (datetime, none_type): Date when the test result has been started. [optional]  # noqa: E501
+            completed_on (datetime, none_type): Date when the test result has been completed. [optional]  # noqa: E501
             duration (int, none_type): Time which it took to run the test. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -321,14 +338,15 @@
         self.autotest_global_id = autotest_global_id
         self.test_run_id = test_run_id
         self.configuration_id = configuration_id
         self.configuration_name = configuration_name
         self.outcome = outcome
         self.result_reasons = result_reasons
         self.date = date
+        self.created_date = created_date
         self.links = links
         self.attachments = attachments
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_step_comment_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_step_comment_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_update_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_update_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_v2_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_v2_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_result_v2_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_result_v2_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_results_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,20 +28,26 @@
 )
 from testit_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from testit_api_client.model.failure_category_model import FailureCategoryModel
     from testit_api_client.model.test_result_outcome import TestResultOutcome
+    from testit_api_client.model.test_results_filter_model_completed_on import TestResultsFilterModelCompletedOn
     from testit_api_client.model.test_results_filter_model_created_date import TestResultsFilterModelCreatedDate
     from testit_api_client.model.test_results_filter_model_duration import TestResultsFilterModelDuration
+    from testit_api_client.model.test_results_filter_model_modified_date import TestResultsFilterModelModifiedDate
+    from testit_api_client.model.test_results_filter_model_started_on import TestResultsFilterModelStartedOn
     globals()['FailureCategoryModel'] = FailureCategoryModel
     globals()['TestResultOutcome'] = TestResultOutcome
+    globals()['TestResultsFilterModelCompletedOn'] = TestResultsFilterModelCompletedOn
     globals()['TestResultsFilterModelCreatedDate'] = TestResultsFilterModelCreatedDate
     globals()['TestResultsFilterModelDuration'] = TestResultsFilterModelDuration
+    globals()['TestResultsFilterModelModifiedDate'] = TestResultsFilterModelModifiedDate
+    globals()['TestResultsFilterModelStartedOn'] = TestResultsFilterModelStartedOn
 
 
 class TestResultsFilterModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -94,14 +100,17 @@
         """
         lazy_import()
         return {
             'test_run_ids': ([str], none_type,),  # noqa: E501
             'auto_test_global_ids': ([int], none_type,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'created_date': (TestResultsFilterModelCreatedDate,),  # noqa: E501
+            'modified_date': (TestResultsFilterModelModifiedDate,),  # noqa: E501
+            'started_on': (TestResultsFilterModelStartedOn,),  # noqa: E501
+            'completed_on': (TestResultsFilterModelCompletedOn,),  # noqa: E501
             'duration': (TestResultsFilterModelDuration,),  # noqa: E501
             'result_reasons': ([str], none_type,),  # noqa: E501
             'configuration_ids': ([str], none_type,),  # noqa: E501
             'outcomes': ([TestResultOutcome], none_type,),  # noqa: E501
             'failure_categories': ([FailureCategoryModel], none_type,),  # noqa: E501
             'namespace': (str, none_type,),  # noqa: E501
             'class_name': (str, none_type,),  # noqa: E501
@@ -113,14 +122,17 @@
 
 
     attribute_map = {
         'test_run_ids': 'testRunIds',  # noqa: E501
         'auto_test_global_ids': 'autoTestGlobalIds',  # noqa: E501
         'name': 'name',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
+        'modified_date': 'modifiedDate',  # noqa: E501
+        'started_on': 'startedOn',  # noqa: E501
+        'completed_on': 'completedOn',  # noqa: E501
         'duration': 'duration',  # noqa: E501
         'result_reasons': 'resultReasons',  # noqa: E501
         'configuration_ids': 'configurationIds',  # noqa: E501
         'outcomes': 'outcomes',  # noqa: E501
         'failure_categories': 'failureCategories',  # noqa: E501
         'namespace': 'namespace',  # noqa: E501
         'class_name': 'className',  # noqa: E501
@@ -167,14 +179,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             test_run_ids ([str], none_type): Specifies a test result test run IDs to search for. [optional]  # noqa: E501
             auto_test_global_ids ([int], none_type): Specifies an autotest global IDs to search results for. [optional]  # noqa: E501
             name (str, none_type): Specifies an autotest name to search results for. [optional]  # noqa: E501
             created_date (TestResultsFilterModelCreatedDate): [optional]  # noqa: E501
+            modified_date (TestResultsFilterModelModifiedDate): [optional]  # noqa: E501
+            started_on (TestResultsFilterModelStartedOn): [optional]  # noqa: E501
+            completed_on (TestResultsFilterModelCompletedOn): [optional]  # noqa: E501
             duration (TestResultsFilterModelDuration): [optional]  # noqa: E501
             result_reasons ([str], none_type): Specifies result reasons for searching test results. [optional]  # noqa: E501
             configuration_ids ([str], none_type): Specifies a test result configuration IDs to search for. [optional]  # noqa: E501
             outcomes ([TestResultOutcome], none_type): Specifies a test result outcomes to search for. [optional]  # noqa: E501
             failure_categories ([FailureCategoryModel], none_type): Specifies a test result failure categories to search for. [optional]  # noqa: E501
             namespace (str, none_type): Specifies a test result namespace to search for. [optional]  # noqa: E501
             class_name (str, none_type): Specifies a test result class name to search for. [optional]  # noqa: E501
@@ -263,14 +278,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             test_run_ids ([str], none_type): Specifies a test result test run IDs to search for. [optional]  # noqa: E501
             auto_test_global_ids ([int], none_type): Specifies an autotest global IDs to search results for. [optional]  # noqa: E501
             name (str, none_type): Specifies an autotest name to search results for. [optional]  # noqa: E501
             created_date (TestResultsFilterModelCreatedDate): [optional]  # noqa: E501
+            modified_date (TestResultsFilterModelModifiedDate): [optional]  # noqa: E501
+            started_on (TestResultsFilterModelStartedOn): [optional]  # noqa: E501
+            completed_on (TestResultsFilterModelCompletedOn): [optional]  # noqa: E501
             duration (TestResultsFilterModelDuration): [optional]  # noqa: E501
             result_reasons ([str], none_type): Specifies result reasons for searching test results. [optional]  # noqa: E501
             configuration_ids ([str], none_type): Specifies a test result configuration IDs to search for. [optional]  # noqa: E501
             outcomes ([TestResultOutcome], none_type): Specifies a test result outcomes to search for. [optional]  # noqa: E501
             failure_categories ([FailureCategoryModel], none_type): Specifies a test result failure categories to search for. [optional]  # noqa: E501
             namespace (str, none_type): Specifies a test result namespace to search for. [optional]  # noqa: E501
             class_name (str, none_type): Specifies a test result class name to search for. [optional]  # noqa: E501
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_results_filter_model_created_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model_created_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_results_filter_model_duration.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_results_filter_model_duration.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_results_local_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_results_local_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_results_statistics_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_results_statistics_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_results_statistics_get_model_failure_categories.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_results_statistics_get_model_failure_categories.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_results_statistics_get_model_statuses.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_results_statistics_get_model_statuses.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_analytic_result_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_analytic_result_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_extraction_model_ids.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_extraction_model_ids.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_fill_by_auto_tests_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_fill_by_auto_tests_post_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,17 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('configuration_ids',): {
+            'min_items': 1,
+        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_fill_by_configurations_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_fill_by_configurations_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_fill_by_work_items_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_fill_by_work_items_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model_auto_tests_count.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model_auto_tests_count.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model_completed_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model_completed_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model_created_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model_created_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_filter_model_started_date.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_filter_model_started_date.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_group_by_failure_class_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_group_by_failure_class_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_group_by_status_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_group_by_status_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_model_analytic.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_model_analytic.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_search_query_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_search_query_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_select_model_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_select_model_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_selection_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_selection_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_short_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_short_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_short_get_model_statistics.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_short_get_model_statistics.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_state.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_state.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_statistics_error_categories_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_statistics_error_categories_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_statistics_statuses_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_statistics_statuses_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_partial_bulk_set_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_partial_bulk_set_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_partial_bulk_set_model_selector.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_partial_bulk_set_model_selector.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_select_model_filter.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_select_model_filter.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_test_results_select_model_test_result_ids_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_test_results_select_model_test_result_ids_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_update_multiple_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_update_multiple_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_v2_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_v2_get_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 )
 from testit_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from testit_api_client.model.attachment_model import AttachmentModel
     from testit_api_client.model.link_model import LinkModel
+    from testit_api_client.model.named_entity_model import NamedEntityModel
     from testit_api_client.model.test_result_v2_get_model import TestResultV2GetModel
     from testit_api_client.model.test_run_state import TestRunState
     globals()['AttachmentModel'] = AttachmentModel
     globals()['LinkModel'] = LinkModel
+    globals()['NamedEntityModel'] = NamedEntityModel
     globals()['TestResultV2GetModel'] = TestResultV2GetModel
     globals()['TestRunState'] = TestRunState
 
 
 class TestRunV2GetModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -91,23 +93,25 @@
         return {
             'state_name': (TestRunState,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'attachments': ([AttachmentModel],),  # noqa: E501
             'links': ([LinkModel],),  # noqa: E501
+            'webhooks': ([NamedEntityModel],),  # noqa: E501
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'started_on': (datetime, none_type,),  # noqa: E501
             'completed_on': (datetime, none_type,),  # noqa: E501
             'test_plan_id': (str, none_type,),  # noqa: E501
             'test_results': ([TestResultV2GetModel], none_type,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'created_by_user_name': (str, none_type,),  # noqa: E501
+            'custom_parameters': ({str: (str,)}, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'launch_source': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -116,44 +120,47 @@
     attribute_map = {
         'state_name': 'stateName',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'attachments': 'attachments',  # noqa: E501
         'links': 'links',  # noqa: E501
+        'webhooks': 'webhooks',  # noqa: E501
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'started_on': 'startedOn',  # noqa: E501
         'completed_on': 'completedOn',  # noqa: E501
         'test_plan_id': 'testPlanId',  # noqa: E501
         'test_results': 'testResults',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'created_by_user_name': 'createdByUserName',  # noqa: E501
+        'custom_parameters': 'customParameters',  # noqa: E501
         'description': 'description',  # noqa: E501
         'launch_source': 'launchSource',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, state_name, project_id, created_date, created_by_id, attachments, links, id, name, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, state_name, project_id, created_date, created_by_id, attachments, links, webhooks, id, name, *args, **kwargs):  # noqa: E501
         """TestRunV2GetModel - a model defined in OpenAPI
 
         Args:
             state_name (TestRunState):
             project_id (str): This property is used to link test run with project
             created_date (datetime):
             created_by_id (str):
             attachments ([AttachmentModel]):
             links ([LinkModel]):
+            webhooks ([NamedEntityModel]):
             id (str):
             name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -187,14 +194,15 @@
             started_on (datetime, none_type): [optional]  # noqa: E501
             completed_on (datetime, none_type): [optional]  # noqa: E501
             test_plan_id (str, none_type): This property is used to link test run with test plan. [optional]  # noqa: E501
             test_results ([TestResultV2GetModel], none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             created_by_user_name (str, none_type): [optional]  # noqa: E501
+            custom_parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             launch_source (str, none_type): Once launch source is specified it cannot be updated. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -226,14 +234,15 @@
 
         self.state_name = state_name
         self.project_id = project_id
         self.created_date = created_date
         self.created_by_id = created_by_id
         self.attachments = attachments
         self.links = links
+        self.webhooks = webhooks
         self.id = id
         self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -248,24 +257,25 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, state_name, project_id, created_date, created_by_id, attachments, links, id, name, *args, **kwargs):  # noqa: E501
+    def __init__(self, state_name, project_id, created_date, created_by_id, attachments, links, webhooks, id, name, *args, **kwargs):  # noqa: E501
         """TestRunV2GetModel - a model defined in OpenAPI
 
         Args:
             state_name (TestRunState):
             project_id (str): This property is used to link test run with project
             created_date (datetime):
             created_by_id (str):
             attachments ([AttachmentModel]):
             links ([LinkModel]):
+            webhooks ([NamedEntityModel]):
             id (str):
             name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -299,14 +309,15 @@
             started_on (datetime, none_type): [optional]  # noqa: E501
             completed_on (datetime, none_type): [optional]  # noqa: E501
             test_plan_id (str, none_type): This property is used to link test run with test plan. [optional]  # noqa: E501
             test_results ([TestResultV2GetModel], none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             created_by_user_name (str, none_type): [optional]  # noqa: E501
+            custom_parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             launch_source (str, none_type): Once launch source is specified it cannot be updated. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -336,14 +347,15 @@
 
         self.state_name = state_name
         self.project_id = project_id
         self.created_date = created_date
         self.created_by_id = created_by_id
         self.attachments = attachments
         self.links = links
+        self.webhooks = webhooks
         self.id = id
         self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_v2_post_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_v2_post_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_run_v2_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_run_v2_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_change_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_change_view_model_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_change_view_model_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_type.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_type.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_v2_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_v2_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_v2_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_v2_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_v2_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_v2_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_v2_tree_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_v2_tree_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_with_children_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_with_children_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_work_items_search_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_work_items_search_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_work_items_search_model_duration.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_work_items_search_model_duration.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/test_suite_work_items_search_model_median_duration.py` & `testit_api_client-4.0.0/src/testit_api_client/model/test_suite_work_items_search_model_median_duration.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_attachment_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_attachment_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_auto_test_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_auto_test_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_custom_attribute_test_plan_project_relations_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_custom_attribute_test_plan_project_relations_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_empty_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_empty_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_link_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_link_short_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_parameter_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_parameter_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_project_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_project_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_projects_attribute_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_projects_attribute_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_section_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_section_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_test_plan_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_test_plan_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/update_work_item_request.py` & `testit_api_client-4.0.0/src/testit_api_client/model/update_work_item_request.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/user_rank_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/user_rank_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,47 +77,50 @@
         return {
             'score': (int,),  # noqa: E501
             'work_items_created': (int,),  # noqa: E501
             'passed_test_points': (int,),  # noqa: E501
             'failed_test_points': (int,),  # noqa: E501
             'skipped_test_points': (int,),  # noqa: E501
             'blocked_test_points': (int,),  # noqa: E501
+            'level_avatar_enabled': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'score': 'score',  # noqa: E501
         'work_items_created': 'workItemsCreated',  # noqa: E501
         'passed_test_points': 'passedTestPoints',  # noqa: E501
         'failed_test_points': 'failedTestPoints',  # noqa: E501
         'skipped_test_points': 'skippedTestPoints',  # noqa: E501
         'blocked_test_points': 'blockedTestPoints',  # noqa: E501
+        'level_avatar_enabled': 'levelAvatarEnabled',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, score, work_items_created, passed_test_points, failed_test_points, skipped_test_points, blocked_test_points, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, score, work_items_created, passed_test_points, failed_test_points, skipped_test_points, blocked_test_points, level_avatar_enabled, *args, **kwargs):  # noqa: E501
         """UserRankModel - a model defined in OpenAPI
 
         Args:
             score (int):
             work_items_created (int):
             passed_test_points (int):
             failed_test_points (int):
             skipped_test_points (int):
             blocked_test_points (int):
+            level_avatar_enabled (bool):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -179,14 +182,15 @@
 
         self.score = score
         self.work_items_created = work_items_created
         self.passed_test_points = passed_test_points
         self.failed_test_points = failed_test_points
         self.skipped_test_points = skipped_test_points
         self.blocked_test_points = blocked_test_points
+        self.level_avatar_enabled = level_avatar_enabled
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -199,24 +203,25 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, score, work_items_created, passed_test_points, failed_test_points, skipped_test_points, blocked_test_points, *args, **kwargs):  # noqa: E501
+    def __init__(self, score, work_items_created, passed_test_points, failed_test_points, skipped_test_points, blocked_test_points, level_avatar_enabled, *args, **kwargs):  # noqa: E501
         """UserRankModel - a model defined in OpenAPI
 
         Args:
             score (int):
             work_items_created (int):
             passed_test_points (int):
             failed_test_points (int):
             skipped_test_points (int):
             blocked_test_points (int):
+            level_avatar_enabled (bool):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -276,14 +281,15 @@
 
         self.score = score
         self.work_items_created = work_items_created
         self.passed_test_points = passed_test_points
         self.failed_test_points = failed_test_points
         self.skipped_test_points = skipped_test_points
         self.blocked_test_points = blocked_test_points
+        self.level_avatar_enabled = level_avatar_enabled
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/user_with_rank_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/user_with_rank_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/user_with_rank_model_user_rank.py` & `testit_api_client-4.0.0/src/testit_api_client/model/user_with_rank_model_user_rank.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,28 +89,30 @@
         return {
             'score': (int,),  # noqa: E501
             'work_items_created': (int,),  # noqa: E501
             'passed_test_points': (int,),  # noqa: E501
             'failed_test_points': (int,),  # noqa: E501
             'skipped_test_points': (int,),  # noqa: E501
             'blocked_test_points': (int,),  # noqa: E501
+            'level_avatar_enabled': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'score': 'score',  # noqa: E501
         'work_items_created': 'workItemsCreated',  # noqa: E501
         'passed_test_points': 'passedTestPoints',  # noqa: E501
         'failed_test_points': 'failedTestPoints',  # noqa: E501
         'skipped_test_points': 'skippedTestPoints',  # noqa: E501
         'blocked_test_points': 'blockedTestPoints',  # noqa: E501
+        'level_avatar_enabled': 'levelAvatarEnabled',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
@@ -120,14 +122,15 @@
         Keyword Args:
             score (int):
             work_items_created (int):
             passed_test_points (int):
             failed_test_points (int):
             skipped_test_points (int):
             blocked_test_points (int):
+            level_avatar_enabled (bool):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -229,14 +232,15 @@
         Keyword Args:
             score (int):
             work_items_created (int):
             passed_test_points (int):
             failed_test_points (int):
             skipped_test_points (int):
             blocked_test_points (int):
+            level_avatar_enabled (bool):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/validate_anti_forgery_token_attribute.py` & `testit_api_client-4.0.0/src/testit_api_client/model/validate_anti_forgery_token_attribute.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/validation_problem_details.py` & `testit_api_client-4.0.0/src/testit_api_client/model/validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/web_hook_event_type.py` & `testit_api_client-4.0.0/src/testit_api_client/model/web_hook_event_type.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/web_hook_event_type_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/web_hook_event_type_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/web_hook_log_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/web_hook_log_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/web_hook_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/web_hook_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/web_hook_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/web_hook_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/web_hook_test_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/web_hook_test_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/webhook_variables_type.py` & `testit_api_client-4.0.0/src/testit_api_client/model/webhook_variables_type.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_change_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_change_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_change_model_work_item_changed_fields.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_change_model_work_item_changed_fields.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_attribute_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_attribute_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_attachments.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_attachments.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_auto_tests.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_auto_tests.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_duration.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_duration.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_global_id.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_global_id.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_is_deleted.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_is_deleted.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_links.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_links.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_project_id.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_project_id.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_state.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_state.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_steps.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_steps.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_changed_fields_view_model_tags.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_changed_fields_view_model_tags.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_comment_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_comment_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_comment_model_user.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_comment_model_user.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_comment_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_comment_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_comment_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_comment_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_entity_types.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_entity_types.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_extraction_model_ids.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_extraction_model_ids.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_extraction_model_section_ids.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_extraction_model_section_ids.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_group_get_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_group_get_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_group_get_model_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_group_get_model_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_group_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_group_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_group_type.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_group_type.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_id_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_id_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_identifier_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_identifier_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_like_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_like_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_link_change_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_link_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_link_change_view_model_array_changed_field_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_link_change_view_model_array_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_local_filter_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_local_filter_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_local_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_local_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_local_select_model_extraction_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_local_select_model_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_local_select_model_filter.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_local_select_model_filter.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_move_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_move_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_post_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_post_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_priority_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_priority_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_put_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_put_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_search_query_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_search_query_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_select_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_select_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_select_model_filter.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_select_model_filter.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_short_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_short_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'version_id': (str,),  # noqa: E501
+            'version_number': (int,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'entity_type_name': (str,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'section_id': (str,),  # noqa: E501
             'section_name': (str,),  # noqa: E501
             'is_automated': (bool,),  # noqa: E501
             'global_id': (int,),  # noqa: E501
@@ -123,14 +124,15 @@
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'version_id': 'versionId',  # noqa: E501
+        'version_number': 'versionNumber',  # noqa: E501
         'name': 'name',  # noqa: E501
         'entity_type_name': 'entityTypeName',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
         'section_id': 'sectionId',  # noqa: E501
         'section_name': 'sectionName',  # noqa: E501
         'is_automated': 'isAutomated',  # noqa: E501
         'global_id': 'globalId',  # noqa: E501
@@ -152,20 +154,21 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, version_id, name, entity_type_name, project_id, section_id, section_name, is_automated, global_id, duration, created_by_id, state, priority, is_deleted, iterations, links, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, version_id, version_number, name, entity_type_name, project_id, section_id, section_name, is_automated, global_id, duration, created_by_id, state, priority, is_deleted, iterations, links, *args, **kwargs):  # noqa: E501
         """WorkItemShortModel - a model defined in OpenAPI
 
         Args:
             id (str): Work Item internal unique identifier
             version_id (str): Work Item version identifier
+            version_number (int): Work Item version number
             name (str): Work Item name
             entity_type_name (str): Work Item type. Possible values: CheckLists, SharedSteps, TestCases
             project_id (str): Project unique identifier
             section_id (str): Identifier of Section where Work Item is located
             section_name (str): Section name of Work Item
             is_automated (bool): Boolean flag determining whether Work Item is automated
             global_id (int): Work Item global identifier
@@ -243,14 +246,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.version_id = version_id
+        self.version_number = version_number
         self.name = name
         self.entity_type_name = entity_type_name
         self.project_id = project_id
         self.section_id = section_id
         self.section_name = section_name
         self.is_automated = is_automated
         self.global_id = global_id
@@ -277,20 +281,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, version_id, name, entity_type_name, project_id, section_id, section_name, is_automated, global_id, duration, created_by_id, state, priority, is_deleted, iterations, links, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, version_id, version_number, name, entity_type_name, project_id, section_id, section_name, is_automated, global_id, duration, created_by_id, state, priority, is_deleted, iterations, links, *args, **kwargs):  # noqa: E501
         """WorkItemShortModel - a model defined in OpenAPI
 
         Args:
             id (str): Work Item internal unique identifier
             version_id (str): Work Item version identifier
+            version_number (int): Work Item version number
             name (str): Work Item name
             entity_type_name (str): Work Item type. Possible values: CheckLists, SharedSteps, TestCases
             project_id (str): Project unique identifier
             section_id (str): Identifier of Section where Work Item is located
             section_name (str): Section name of Work Item
             is_automated (bool): Boolean flag determining whether Work Item is automated
             global_id (int): Work Item global identifier
@@ -366,14 +371,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.version_id = version_id
+        self.version_number = version_number
         self.name = name
         self.entity_type_name = entity_type_name
         self.project_id = project_id
         self.section_id = section_id
         self.section_name = section_name
         self.is_automated = is_automated
         self.global_id = global_id
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_state.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_state.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_states.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_states.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_step_change_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_step_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_step_change_view_model_array_changed_field_with_diffs_view_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_step_change_view_model_array_changed_field_with_diffs_view_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_step_change_view_model_work_item.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_step_change_view_model_work_item.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model/work_item_version_model.py` & `testit_api_client-4.0.0/src/testit_api_client/model/work_item_version_model.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/model_utils.py` & `testit_api_client-4.0.0/src/testit_api_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client/models/__init__.py` & `testit_api_client-4.0.0/src/testit_api_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from testit_api_client.model.api_v2_tags_put_request import ApiV2TagsPutRequest
 from testit_api_client.model.api_v2_test_plans_id_export_test_points_xlsx_post_request import ApiV2TestPlansIdExportTestPointsXlsxPostRequest
 from testit_api_client.model.api_v2_test_plans_id_test_points_tester_user_id_post_request import ApiV2TestPlansIdTestPointsTesterUserIdPostRequest
 from testit_api_client.model.api_v2_test_plans_id_test_runs_search_post_request import ApiV2TestPlansIdTestRunsSearchPostRequest
 from testit_api_client.model.api_v2_test_points_search_post_request import ApiV2TestPointsSearchPostRequest
 from testit_api_client.model.api_v2_test_results_id_put_request import ApiV2TestResultsIdPutRequest
 from testit_api_client.model.api_v2_test_results_search_post_request import ApiV2TestResultsSearchPostRequest
+from testit_api_client.model.api_v2_test_runs_delete_request import ApiV2TestRunsDeleteRequest
 from testit_api_client.model.api_v2_test_runs_id_statistics_filter_post_request import ApiV2TestRunsIdStatisticsFilterPostRequest
 from testit_api_client.model.api_v2_test_runs_id_test_results_bulk_put_request import ApiV2TestRunsIdTestResultsBulkPutRequest
 from testit_api_client.model.api_v2_test_runs_search_post_request import ApiV2TestRunsSearchPostRequest
 from testit_api_client.model.api_v2_test_runs_update_multiple_post_request import ApiV2TestRunsUpdateMultiplePostRequest
 from testit_api_client.model.api_v2_test_suites_post_request import ApiV2TestSuitesPostRequest
 from testit_api_client.model.api_v2_test_suites_put_request import ApiV2TestSuitesPutRequest
 from testit_api_client.model.api_v2_webhooks_post_request import ApiV2WebhooksPostRequest
@@ -172,14 +173,15 @@
 from testit_api_client.model.link_model import LinkModel
 from testit_api_client.model.link_post_model import LinkPostModel
 from testit_api_client.model.link_put_model import LinkPutModel
 from testit_api_client.model.link_short_model import LinkShortModel
 from testit_api_client.model.link_sub_get_model import LinkSubGetModel
 from testit_api_client.model.link_type import LinkType
 from testit_api_client.model.move_request import MoveRequest
+from testit_api_client.model.named_entity_model import NamedEntityModel
 from testit_api_client.model.no_content_result import NoContentResult
 from testit_api_client.model.notification_model import NotificationModel
 from testit_api_client.model.notification_query_filter_model import NotificationQueryFilterModel
 from testit_api_client.model.notification_type_model import NotificationTypeModel
 from testit_api_client.model.operation import Operation
 from testit_api_client.model.parameter_filter_model import ParameterFilterModel
 from testit_api_client.model.parameter_group_model import ParameterGroupModel
@@ -208,15 +210,14 @@
 from testit_api_client.model.projects_filter_model_checklists_count import ProjectsFilterModelChecklistsCount
 from testit_api_client.model.projects_filter_model_created_date import ProjectsFilterModelCreatedDate
 from testit_api_client.model.projects_filter_model_shared_steps_count import ProjectsFilterModelSharedStepsCount
 from testit_api_client.model.projects_filter_model_test_cases_count import ProjectsFilterModelTestCasesCount
 from testit_api_client.model.public_test_point_model import PublicTestPointModel
 from testit_api_client.model.public_test_run_model import PublicTestRunModel
 from testit_api_client.model.rename_request import RenameRequest
-from testit_api_client.model.request_data import RequestData
 from testit_api_client.model.request_type_model import RequestTypeModel
 from testit_api_client.model.search_attributes_in_project_request import SearchAttributesInProjectRequest
 from testit_api_client.model.search_auto_tests_query_includes_model import SearchAutoTestsQueryIncludesModel
 from testit_api_client.model.search_custom_attribute_template_get_model import SearchCustomAttributeTemplateGetModel
 from testit_api_client.model.search_webhooks_query_model import SearchWebhooksQueryModel
 from testit_api_client.model.search_work_items_request import SearchWorkItemsRequest
 from testit_api_client.model.section_model import SectionModel
@@ -247,14 +248,15 @@
 from testit_api_client.model.string_changed_field_view_model import StringChangedFieldViewModel
 from testit_api_client.model.string_changed_field_with_diffs_view_model import StringChangedFieldWithDiffsViewModel
 from testit_api_client.model.tag_extraction_model import TagExtractionModel
 from testit_api_client.model.tag_model import TagModel
 from testit_api_client.model.tag_post_model import TagPostModel
 from testit_api_client.model.tag_put_model import TagPutModel
 from testit_api_client.model.tag_select_model import TagSelectModel
+from testit_api_client.model.tag_short_model import TagShortModel
 from testit_api_client.model.tags_filter_model import TagsFilterModel
 from testit_api_client.model.tags_filter_model_created_date import TagsFilterModelCreatedDate
 from testit_api_client.model.test_plan_change_model import TestPlanChangeModel
 from testit_api_client.model.test_plan_change_model_test_plan_changed_fields import TestPlanChangeModelTestPlanChangedFields
 from testit_api_client.model.test_plan_changed_fields_view_model import TestPlanChangedFieldsViewModel
 from testit_api_client.model.test_plan_extraction_model import TestPlanExtractionModel
 from testit_api_client.model.test_plan_group_by_status import TestPlanGroupByStatus
@@ -304,16 +306,19 @@
 from testit_api_client.model.test_result_short_get_model import TestResultShortGetModel
 from testit_api_client.model.test_result_short_model import TestResultShortModel
 from testit_api_client.model.test_result_step_comment_put_model import TestResultStepCommentPutModel
 from testit_api_client.model.test_result_update_model import TestResultUpdateModel
 from testit_api_client.model.test_result_v2_get_model import TestResultV2GetModel
 from testit_api_client.model.test_result_v2_short_model import TestResultV2ShortModel
 from testit_api_client.model.test_results_filter_model import TestResultsFilterModel
+from testit_api_client.model.test_results_filter_model_completed_on import TestResultsFilterModelCompletedOn
 from testit_api_client.model.test_results_filter_model_created_date import TestResultsFilterModelCreatedDate
 from testit_api_client.model.test_results_filter_model_duration import TestResultsFilterModelDuration
+from testit_api_client.model.test_results_filter_model_modified_date import TestResultsFilterModelModifiedDate
+from testit_api_client.model.test_results_filter_model_started_on import TestResultsFilterModelStartedOn
 from testit_api_client.model.test_results_local_filter_model import TestResultsLocalFilterModel
 from testit_api_client.model.test_results_statistics_get_model import TestResultsStatisticsGetModel
 from testit_api_client.model.test_results_statistics_get_model_failure_categories import TestResultsStatisticsGetModelFailureCategories
 from testit_api_client.model.test_results_statistics_get_model_statuses import TestResultsStatisticsGetModelStatuses
 from testit_api_client.model.test_run_analytic_result_model import TestRunAnalyticResultModel
 from testit_api_client.model.test_run_extraction_model import TestRunExtractionModel
 from testit_api_client.model.test_run_extraction_model_ids import TestRunExtractionModelIds
@@ -377,14 +382,15 @@
 from testit_api_client.model.validation_problem_details import ValidationProblemDetails
 from testit_api_client.model.web_hook_event_type import WebHookEventType
 from testit_api_client.model.web_hook_event_type_model import WebHookEventTypeModel
 from testit_api_client.model.web_hook_log_model import WebHookLogModel
 from testit_api_client.model.web_hook_model import WebHookModel
 from testit_api_client.model.web_hook_post_model import WebHookPostModel
 from testit_api_client.model.web_hook_test_model import WebHookTestModel
+from testit_api_client.model.webhook_response import WebhookResponse
 from testit_api_client.model.webhook_variables_type import WebhookVariablesType
 from testit_api_client.model.work_item_change_model import WorkItemChangeModel
 from testit_api_client.model.work_item_change_model_work_item_changed_fields import WorkItemChangeModelWorkItemChangedFields
 from testit_api_client.model.work_item_changed_attribute_view_model import WorkItemChangedAttributeViewModel
 from testit_api_client.model.work_item_changed_fields_view_model import WorkItemChangedFieldsViewModel
 from testit_api_client.model.work_item_changed_fields_view_model_attachments import WorkItemChangedFieldsViewModelAttachments
 from testit_api_client.model.work_item_changed_fields_view_model_auto_tests import WorkItemChangedFieldsViewModelAutoTests
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client/rest.py` & `testit_api_client-4.0.0/src/testit_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `testit-api-client-3.5.0/src/testit_api_client.egg-info/PKG-INFO` & `testit_api_client-4.0.0/src/testit_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-api-client
-Version: 3.5.0
+Version: 4.0.0
 Summary: API-client for Test IT
 Home-page: https://pypi.org/project/testit-api-client/
 Author: Integration team
 Author-email: integrations@testit.software
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -28,14 +28,15 @@
 | 3.5     | 2.0.4      |
 | 4.0     | 3.0.0      |
 | 4.2     | 3.1.0      |
 | 4.3     | 3.2.0      |
 | 4.4     | 3.3.0      |
 | 4.5     | 3.4.0      |
 | 4.6     | 3.5.0      |
+| 5.0     | 4.0.0      |
 
 ## Installation & Usage
 ### pip install
 
 ```sh
 pip install testit-api-client
 ```
@@ -278,18 +279,24 @@
 *TestResultsApi* | [**api_v2_test_results_search_post**](docs/TestResultsApi.md#api_v2_test_results_search_post) | **POST** /api/v2/testResults/search | Search for test results
 *TestResultsApi* | [**api_v2_test_results_statistics_filter_post**](docs/TestResultsApi.md#api_v2_test_results_statistics_filter_post) | **POST** /api/v2/testResults/statistics/filter | Search for test results and extract statistics
 *TestResultsApi* | [**create_attachment**](docs/TestResultsApi.md#create_attachment) | **POST** /api/v2/testResults/{id}/attachments | Upload and link attachment to TestResult
 *TestResultsApi* | [**delete_attachment**](docs/TestResultsApi.md#delete_attachment) | **DELETE** /api/v2/testResults/{id}/attachments/{attachmentId} | Remove attachment and unlink from TestResult
 *TestResultsApi* | [**download_attachment**](docs/TestResultsApi.md#download_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId} | Get attachment of TestResult
 *TestResultsApi* | [**get_attachment**](docs/TestResultsApi.md#get_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId}/info | Get Metadata of TestResult&#39;s attachment
 *TestResultsApi* | [**get_attachments**](docs/TestResultsApi.md#get_attachments) | **GET** /api/v2/testResults/{id}/attachments | Get all attachments of TestResult
+*TestRunsApi* | [**api_v2_test_runs_delete**](docs/TestRunsApi.md#api_v2_test_runs_delete) | **DELETE** /api/v2/testRuns | Delete multiple test runs
+*TestRunsApi* | [**api_v2_test_runs_id_delete**](docs/TestRunsApi.md#api_v2_test_runs_id_delete) | **DELETE** /api/v2/testRuns/{id} | Delete test run
+*TestRunsApi* | [**api_v2_test_runs_id_purge_post**](docs/TestRunsApi.md#api_v2_test_runs_id_purge_post) | **POST** /api/v2/testRuns/{id}/purge | Permanently delete test run from archive
+*TestRunsApi* | [**api_v2_test_runs_id_restore_post**](docs/TestRunsApi.md#api_v2_test_runs_id_restore_post) | **POST** /api/v2/testRuns/{id}/restore | Restore test run from the archive
 *TestRunsApi* | [**api_v2_test_runs_id_statistics_filter_post**](docs/TestRunsApi.md#api_v2_test_runs_id_statistics_filter_post) | **POST** /api/v2/testRuns/{id}/statistics/filter | Search for the test run test results and build statistics
 *TestRunsApi* | [**api_v2_test_runs_id_test_points_results_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_points_results_get) | **GET** /api/v2/testRuns/{id}/testPoints/results | Get test results from the test run grouped by test points
 *TestRunsApi* | [**api_v2_test_runs_id_test_results_bulk_put**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_bulk_put) | **PUT** /api/v2/testRuns/{id}/testResults/bulk | Partial edit of multiple test results in the test run
 *TestRunsApi* | [**api_v2_test_runs_id_test_results_last_modified_modification_date_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_last_modified_modification_date_get) | **GET** /api/v2/testRuns/{id}/testResults/lastModified/modificationDate | Get modification date of last test result of the test run
+*TestRunsApi* | [**api_v2_test_runs_purge_bulk_post**](docs/TestRunsApi.md#api_v2_test_runs_purge_bulk_post) | **POST** /api/v2/testRuns/purge/bulk | Permanently delete multiple test runs from archive
+*TestRunsApi* | [**api_v2_test_runs_restore_bulk_post**](docs/TestRunsApi.md#api_v2_test_runs_restore_bulk_post) | **POST** /api/v2/testRuns/restore/bulk | Restore multiple test runs from the archive
 *TestRunsApi* | [**api_v2_test_runs_search_post**](docs/TestRunsApi.md#api_v2_test_runs_search_post) | **POST** /api/v2/testRuns/search | Search for test runs
 *TestRunsApi* | [**api_v2_test_runs_update_multiple_post**](docs/TestRunsApi.md#api_v2_test_runs_update_multiple_post) | **POST** /api/v2/testRuns/updateMultiple | Update multiple test runs
 *TestRunsApi* | [**complete_test_run**](docs/TestRunsApi.md#complete_test_run) | **POST** /api/v2/testRuns/{id}/complete | Complete TestRun
 *TestRunsApi* | [**create_and_fill_by_auto_tests**](docs/TestRunsApi.md#create_and_fill_by_auto_tests) | **POST** /api/v2/testRuns/byAutoTests | Create test runs based on autotests and configurations
 *TestRunsApi* | [**create_and_fill_by_configurations**](docs/TestRunsApi.md#create_and_fill_by_configurations) | **POST** /api/v2/testRuns/byConfigurations | Create test runs picking the needed test points
 *TestRunsApi* | [**create_and_fill_by_work_items**](docs/TestRunsApi.md#create_and_fill_by_work_items) | **POST** /api/v2/testRuns/byWorkItems | Create test run based on configurations and work items
 *TestRunsApi* | [**create_empty**](docs/TestRunsApi.md#create_empty) | **POST** /api/v2/testRuns | Create empty TestRun
```

### Comparing `testit-api-client-3.5.0/src/testit_api_client.egg-info/SOURCES.txt` & `testit_api_client-4.0.0/src/testit_api_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 src/testit_api_client/model/api_v2_tags_put_request.py
 src/testit_api_client/model/api_v2_test_plans_id_export_test_points_xlsx_post_request.py
 src/testit_api_client/model/api_v2_test_plans_id_test_points_tester_user_id_post_request.py
 src/testit_api_client/model/api_v2_test_plans_id_test_runs_search_post_request.py
 src/testit_api_client/model/api_v2_test_points_search_post_request.py
 src/testit_api_client/model/api_v2_test_results_id_put_request.py
 src/testit_api_client/model/api_v2_test_results_search_post_request.py
+src/testit_api_client/model/api_v2_test_runs_delete_request.py
 src/testit_api_client/model/api_v2_test_runs_id_statistics_filter_post_request.py
 src/testit_api_client/model/api_v2_test_runs_id_test_results_bulk_put_request.py
 src/testit_api_client/model/api_v2_test_runs_search_post_request.py
 src/testit_api_client/model/api_v2_test_runs_update_multiple_post_request.py
 src/testit_api_client/model/api_v2_test_suites_post_request.py
 src/testit_api_client/model/api_v2_test_suites_put_request.py
 src/testit_api_client/model/api_v2_webhooks_post_request.py
@@ -209,14 +210,15 @@
 src/testit_api_client/model/link_model.py
 src/testit_api_client/model/link_post_model.py
 src/testit_api_client/model/link_put_model.py
 src/testit_api_client/model/link_short_model.py
 src/testit_api_client/model/link_sub_get_model.py
 src/testit_api_client/model/link_type.py
 src/testit_api_client/model/move_request.py
+src/testit_api_client/model/named_entity_model.py
 src/testit_api_client/model/no_content_result.py
 src/testit_api_client/model/notification_model.py
 src/testit_api_client/model/notification_query_filter_model.py
 src/testit_api_client/model/notification_type_model.py
 src/testit_api_client/model/operation.py
 src/testit_api_client/model/parameter_filter_model.py
 src/testit_api_client/model/parameter_group_model.py
@@ -245,15 +247,14 @@
 src/testit_api_client/model/projects_filter_model_checklists_count.py
 src/testit_api_client/model/projects_filter_model_created_date.py
 src/testit_api_client/model/projects_filter_model_shared_steps_count.py
 src/testit_api_client/model/projects_filter_model_test_cases_count.py
 src/testit_api_client/model/public_test_point_model.py
 src/testit_api_client/model/public_test_run_model.py
 src/testit_api_client/model/rename_request.py
-src/testit_api_client/model/request_data.py
 src/testit_api_client/model/request_type_model.py
 src/testit_api_client/model/search_attributes_in_project_request.py
 src/testit_api_client/model/search_auto_tests_query_includes_model.py
 src/testit_api_client/model/search_custom_attribute_template_get_model.py
 src/testit_api_client/model/search_webhooks_query_model.py
 src/testit_api_client/model/search_work_items_request.py
 src/testit_api_client/model/section_model.py
@@ -284,14 +285,15 @@
 src/testit_api_client/model/string_changed_field_view_model.py
 src/testit_api_client/model/string_changed_field_with_diffs_view_model.py
 src/testit_api_client/model/tag_extraction_model.py
 src/testit_api_client/model/tag_model.py
 src/testit_api_client/model/tag_post_model.py
 src/testit_api_client/model/tag_put_model.py
 src/testit_api_client/model/tag_select_model.py
+src/testit_api_client/model/tag_short_model.py
 src/testit_api_client/model/tags_filter_model.py
 src/testit_api_client/model/tags_filter_model_created_date.py
 src/testit_api_client/model/test_plan_change_model.py
 src/testit_api_client/model/test_plan_change_model_test_plan_changed_fields.py
 src/testit_api_client/model/test_plan_changed_fields_view_model.py
 src/testit_api_client/model/test_plan_extraction_model.py
 src/testit_api_client/model/test_plan_group_by_status.py
@@ -341,16 +343,19 @@
 src/testit_api_client/model/test_result_short_get_model.py
 src/testit_api_client/model/test_result_short_model.py
 src/testit_api_client/model/test_result_step_comment_put_model.py
 src/testit_api_client/model/test_result_update_model.py
 src/testit_api_client/model/test_result_v2_get_model.py
 src/testit_api_client/model/test_result_v2_short_model.py
 src/testit_api_client/model/test_results_filter_model.py
+src/testit_api_client/model/test_results_filter_model_completed_on.py
 src/testit_api_client/model/test_results_filter_model_created_date.py
 src/testit_api_client/model/test_results_filter_model_duration.py
+src/testit_api_client/model/test_results_filter_model_modified_date.py
+src/testit_api_client/model/test_results_filter_model_started_on.py
 src/testit_api_client/model/test_results_local_filter_model.py
 src/testit_api_client/model/test_results_statistics_get_model.py
 src/testit_api_client/model/test_results_statistics_get_model_failure_categories.py
 src/testit_api_client/model/test_results_statistics_get_model_statuses.py
 src/testit_api_client/model/test_run_analytic_result_model.py
 src/testit_api_client/model/test_run_extraction_model.py
 src/testit_api_client/model/test_run_extraction_model_ids.py
@@ -414,14 +419,15 @@
 src/testit_api_client/model/validation_problem_details.py
 src/testit_api_client/model/web_hook_event_type.py
 src/testit_api_client/model/web_hook_event_type_model.py
 src/testit_api_client/model/web_hook_log_model.py
 src/testit_api_client/model/web_hook_model.py
 src/testit_api_client/model/web_hook_post_model.py
 src/testit_api_client/model/web_hook_test_model.py
+src/testit_api_client/model/webhook_response.py
 src/testit_api_client/model/webhook_variables_type.py
 src/testit_api_client/model/work_item_change_model.py
 src/testit_api_client/model/work_item_change_model_work_item_changed_fields.py
 src/testit_api_client/model/work_item_changed_attribute_view_model.py
 src/testit_api_client/model/work_item_changed_fields_view_model.py
 src/testit_api_client/model/work_item_changed_fields_view_model_attachments.py
 src/testit_api_client/model/work_item_changed_fields_view_model_auto_tests.py
```

