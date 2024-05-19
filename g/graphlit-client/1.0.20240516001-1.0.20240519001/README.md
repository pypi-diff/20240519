# Comparing `tmp/graphlit_client-1.0.20240516001.tar.gz` & `tmp/graphlit_client-1.0.20240519001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240516001.tar", last modified: Thu May 16 19:36:01 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240519001.tar", last modified: Sun May 19 19:49:20 2024, max compression
```

## Comparing `graphlit_client-1.0.20240516001.tar` & `graphlit_client-1.0.20240519001.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 19:36:01.618694 graphlit_client-1.0.20240516001/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-16 19:36:01.618694 graphlit_client-1.0.20240516001/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 19:36:01.582693 graphlit_client-1.0.20240516001/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 19:36:01.614694 graphlit_client-1.0.20240516001/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    86024 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    99668 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/count_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8595 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17547 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9869 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7098 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_share_point_consent_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5777 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8029 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    80420 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68855 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4029 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/publish_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10738 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12137 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_contents_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)      975 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_contents_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7902 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      834 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_microsoft_teams_channels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      782 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_microsoft_teams_teams.py
--rw-r--r--   0 vsts      (1001) docker     (127)      718 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_one_drive_folders.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_share_point_folders.py
--rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_share_point_libraries.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1645 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9007 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8595 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/graphlit_api/update_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 19:36:01.614694 graphlit_client-1.0.20240516001/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-16 19:36:01.000000 graphlit_client-1.0.20240516001/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-05-16 19:36:01.000000 graphlit_client-1.0.20240516001/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-16 19:36:01.000000 graphlit_client-1.0.20240516001/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-16 19:36:01.000000 graphlit_client-1.0.20240516001/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-16 19:36:01.000000 graphlit_client-1.0.20240516001/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-16 19:36:01.618694 graphlit_client-1.0.20240516001/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-16 19:35:45.000000 graphlit_client-1.0.20240516001/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:49:19.977531 graphlit_client-1.0.20240519001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    86074 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    99668 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8595 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17559 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9942 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7098 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_share_point_consent_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5777 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8029 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    81097 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68926 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/publish_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10811 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12210 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_contents_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      975 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_contents_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7902 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      834 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_microsoft_teams_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      782 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_microsoft_teams_teams.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      718 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_one_drive_folders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_share_point_folders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_share_point_libraries.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1645 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9007 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8595 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/setup.py
```

### Comparing `graphlit_client-1.0.20240516001/LICENSE` & `graphlit_client-1.0.20240519001/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/PKG-INFO` & `graphlit_client-1.0.20240519001/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240516001
+Version: 1.0.20240519001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240516001/README.md` & `graphlit_client-1.0.20240519001/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit/graphlit.py` & `graphlit_client-1.0.20240519001/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/__init__.py` & `graphlit_client-1.0.20240519001/graphlit_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,14 +500,15 @@
     CohereModelPropertiesUpdateInput,
     CollectionFilter,
     CollectionInput,
     CollectionUpdateInput,
     ContentCriteriaInput,
     ContentFacetInput,
     ContentFilter,
+    ContentFilterLevel,
     ContentGraphInput,
     ContentInput,
     ContentPublishingConnectorInput,
     ContentPublishingConnectorUpdateInput,
     ContentUpdateInput,
     ConversationFilter,
     ConversationInput,
@@ -1323,14 +1324,15 @@
     "CollectionInput",
     "CollectionTypes",
     "CollectionUpdateInput",
     "ContentCriteriaInput",
     "ContentFacetInput",
     "ContentFacetTypes",
     "ContentFilter",
+    "ContentFilterLevel",
     "ContentGraphInput",
     "ContentInput",
     "ContentPublishingConnectorInput",
     "ContentPublishingConnectorUpdateInput",
     "ContentPublishingFormats",
     "ContentPublishingServiceTypes",
     "ContentTypes",
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240519001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240519001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/base_model.py` & `graphlit_client-1.0.20240519001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240519001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/client.py` & `graphlit_client-1.0.20240519001/graphlit_api/client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240519001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240519001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240519001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240519001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240519001/graphlit_api/create_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240519001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/delete_all_organizations.py` & `graphlit_client-1.0.20240519001/graphlit_api/delete_all_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/delete_all_specifications.py` & `graphlit_client-1.0.20240519001/graphlit_api/delete_all_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/enums.py` & `graphlit_client-1.0.20240519001/graphlit_api/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,14 +315,15 @@
     I_TUNES = "I_TUNES"
     PANDORA = "PANDORA"
     SOUND_CLOUD = "SOUND_CLOUD"
     BANDCAMP = "BANDCAMP"
     TIK_TOK = "TIK_TOK"
     YOU_TUBE = "YOU_TUBE"
     TWITTER = "TWITTER"
+    X = "X"
     MEDIUM = "MEDIUM"
     NOTION = "NOTION"
     LINEAR = "LINEAR"
     GIT_HUB = "GIT_HUB"
     GIT_HUB_PAGES = "GIT_HUB_PAGES"
     RSS = "RSS"
     EMAIL = "EMAIL"
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240519001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240519001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_content.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,15 @@
 
 
 class GetContentContentObservations(BaseModel):
     id: str
     type: ObservableTypes
     observable: "GetContentContentObservationsObservable"
     related: Optional["GetContentContentObservationsRelated"]
+    related_type: Optional[ObservableTypes] = Field(alias="relatedType")
     relation: Optional[str]
     occurrences: Optional[List[Optional["GetContentContentObservationsOccurrences"]]]
     state: EntityState
 
 
 class GetContentContentObservationsObservable(BaseModel):
     id: str
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_event.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_event.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_feed.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_organization.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_organization.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_person.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_person.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_place.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_place.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_product.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_product.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_project.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_software.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_software.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240519001/graphlit_api/get_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240519001/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240519001/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240519001/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/input_types.py` & `graphlit_client-1.0.20240519001/graphlit_api/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,20 @@
         alias="originalDateRange", default=None
     )
     formats: Optional[List[Optional[str]]] = None
     file_extensions: Optional[List[str]] = Field(alias="fileExtensions", default=None)
     file_size_range: Optional["Int64RangeFilter"] = Field(
         alias="fileSizeRange", default=None
     )
+    or_: Optional[List[Optional["ContentFilterLevel"]]] = Field(
+        alias="or", default=None
+    )
+    and_: Optional[List[Optional["ContentFilterLevel"]]] = Field(
+        alias="and", default=None
+    )
 
 
 class ConversationFilter(BaseModel):
     search: Optional[str] = None
     order_by: Optional[OrderByTypes] = Field(alias="orderBy", default=None)
     direction: Optional[OrderDirectionTypes] = None
     offset: Optional[int] = None
@@ -548,14 +554,15 @@
 
 
 class ObservationInput(BaseModel):
     content: "EntityReferenceInput"
     type: ObservableTypes
     observable: "NamedEntityReferenceInput"
     related: Optional["NamedEntityReferenceInput"] = None
+    related_type: Optional[ObservableTypes] = Field(alias="relatedType", default=None)
     relation: Optional[str] = None
     occurrences: List["ObservationOccurrenceInput"]
 
 
 class OrganizationInput(BaseModel):
     name: str
     uri: Optional[Any] = None
@@ -799,14 +806,15 @@
 
 
 class ObservationUpdateInput(BaseModel):
     id: str
     type: Optional[ObservableTypes] = None
     observable: Optional["NamedEntityReferenceInput"] = None
     related: Optional["NamedEntityReferenceInput"] = None
+    related_type: Optional[ObservableTypes] = Field(alias="relatedType", default=None)
     relation: Optional[str] = None
     occurrences: Optional[List["ObservationOccurrenceInput"]] = None
 
 
 class OrganizationUpdateInput(BaseModel):
     id: str
     name: Optional[str] = None
@@ -968,14 +976,21 @@
 
 
 class Int64RangeFilter(BaseModel):
     from_: Optional[Any] = Field(alias="from", default=None)
     to: Optional[Any] = None
 
 
+class ContentFilterLevel(BaseModel):
+    feeds: Optional[List["EntityReferenceFilter"]] = None
+    workflows: Optional[List["EntityReferenceFilter"]] = None
+    collections: Optional[List["EntityReferenceFilter"]] = None
+    observations: Optional[List["ObservationReferenceFilter"]] = None
+
+
 class AddressFilter(BaseModel):
     street_address: Optional[str] = Field(alias="streetAddress", default=None)
     city: Optional[str] = None
     region: Optional[str] = None
     country: Optional[str] = None
     postal_code: Optional[str] = Field(alias="postalCode", default=None)
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240519001/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240519001/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/operations.py` & `graphlit_client-1.0.20240519001/graphlit_api/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -846,14 +846,15 @@
         id
         name
       }
       related {
         id
         name
       }
+      relatedType
       relation
       occurrences {
         type
         confidence
         startTime
         endTime
         pageIndex
@@ -1225,14 +1226,15 @@
           id
           name
         }
         related {
           id
           name
         }
+        relatedType
         relation
         occurrences {
           type
           confidence
           startTime
           endTime
           pageIndex
@@ -1455,14 +1457,15 @@
           id
           name
         }
         related {
           id
           name
         }
+        relatedType
         relation
         occurrences {
           type
           confidence
           startTime
           endTime
           pageIndex
@@ -1787,14 +1790,15 @@
           name
         }
       }
     }
     graph {
       nodes {
         id
+        name
         type
         metadata
       }
       edges {
         from
         to
         relation
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240519001/graphlit_api/prompt_conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 class PromptConversationPromptConversationGraph(BaseModel):
     nodes: Optional[List[Optional["PromptConversationPromptConversationGraphNodes"]]]
     edges: Optional[List[Optional["PromptConversationPromptConversationGraphEdges"]]]
 
 
 class PromptConversationPromptConversationGraphNodes(BaseModel):
     id: str
+    name: str
     type: EntityTypes
     metadata: Optional[str]
 
 
 class PromptConversationPromptConversationGraphEdges(BaseModel):
     from_: str = Field(alias="from")
     to: str
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240519001/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240519001/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240519001/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/publish_text.py` & `graphlit_client-1.0.20240519001/graphlit_api/publish_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_categories.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_categories.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_contents.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,14 +249,15 @@
 
 
 class QueryContentsContentsResultsObservations(BaseModel):
     id: str
     type: ObservableTypes
     observable: "QueryContentsContentsResultsObservationsObservable"
     related: Optional["QueryContentsContentsResultsObservationsRelated"]
+    related_type: Optional[ObservableTypes] = Field(alias="relatedType")
     relation: Optional[str]
     occurrences: Optional[
         List[Optional["QueryContentsContentsResultsObservationsOccurrences"]]
     ]
     state: EntityState
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_contents_facets.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_contents_facets.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,15 @@
 
 
 class QueryContentsFacetsContentsResultsObservations(BaseModel):
     id: str
     type: ObservableTypes
     observable: "QueryContentsFacetsContentsResultsObservationsObservable"
     related: Optional["QueryContentsFacetsContentsResultsObservationsRelated"]
+    related_type: Optional[ObservableTypes] = Field(alias="relatedType")
     relation: Optional[str]
     occurrences: Optional[
         List[Optional["QueryContentsFacetsContentsResultsObservationsOccurrences"]]
     ]
     state: EntityState
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_contents_graph.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_contents_graph.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_credits.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_events.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_events.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_labels.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_labels.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_microsoft_teams_channels.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_microsoft_teams_channels.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_microsoft_teams_teams.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_microsoft_teams_teams.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_one_drive_folders.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_one_drive_folders.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_organizations.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_persons.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_persons.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_places.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_places.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_products.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_products.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_repos.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_repos.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_share_point_folders.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_share_point_folders.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_share_point_libraries.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_share_point_libraries.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_softwares.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_softwares.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_usage.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240519001/graphlit_api/query_workflows.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240519001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240519001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240519001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/update_content.py` & `graphlit_client-1.0.20240519001/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240519001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240519001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240519001/graphlit_api/update_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240519001/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240516001
+Version: 1.0.20240519001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240516001/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240519001/graphlit_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240516001/setup.py` & `graphlit_client-1.0.20240519001/setup.py`

 * *Files identical despite different names*

