# Comparing `tmp/ffun-1.5.1.tar.gz` & `tmp/ffun-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffun-1.5.1.tar", max compression
+gzip compressed data, was "ffun-1.5.2.tar", max compression
```

## Comparing `ffun-1.5.1.tar` & `ffun-1.5.2.tar`

### file list

```diff
@@ -1,230 +1,231 @@
--rw-r--r--   0        0        0      344 2024-05-14 20:03:50.415841 ffun-1.5.1/README.md
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/api/__init__.py
--rw-r--r--   0        0        0    10249 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/api/entities.py
--rw-r--r--   0        0        0    13578 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/api/http_handlers.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/application/__init__.py
--rw-r--r--   0        0        0     4314 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/application/application.py
--rw-r--r--   0        0        0      115 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/application/errors.py
--rw-r--r--   0        0        0       68 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/application/resources.py
--rw-r--r--   0        0        0     1635 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/application/settings.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/application/tests/__init__.py
--rw-r--r--   0        0        0      422 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/application/tests/test_settings.py
--rw-r--r--   0        0        0     3724 2024-05-14 20:03:50.415841 ffun-1.5.1/ffun/application/user_settings.py
--rw-r--r--   0        0        0      281 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/application/utils.py
--rw-r--r--   0        0        0     1252 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/application/workers.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/auth/__init__.py
--rw-r--r--   0        0        0      984 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/auth/dependencies.py
--rw-r--r--   0        0        0      828 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/auth/settings.py
--rw-r--r--   0        0        0     2800 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/auth/supertokens.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/__init__.py
--rw-r--r--   0        0        0      174 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/application.py
--rw-r--r--   0        0        0      439 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/cli.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/commands/__init__.py
--rw-r--r--   0        0        0      732 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/commands/configs.py
--rw-r--r--   0        0        0     1050 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/commands/entries.py
--rw-r--r--   0        0        0     1393 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/commands/failed_entries.py
--rw-r--r--   0        0        0      538 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/commands/meta.py
--rw-r--r--   0        0        0     1001 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/commands/supertokens.py
--rw-r--r--   0        0        0      884 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/commands/workers.py
--rw-r--r--   0        0        0      209 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/cli/commands/yoyo.py
--rw-r--r--   0        0        0     1333 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/conftest.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/__init__.py
--rw-r--r--   0        0        0      631 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/api.py
--rw-r--r--   0        0        0     3139 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/background_tasks.py
--rw-r--r--   0        0        0      493 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/entities.py
--rw-r--r--   0        0        0      552 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/errors.py
--rw-r--r--   0        0        0     2773 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/json.py
--rw-r--r--   0        0        0     5440 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/logging.py
--rw-r--r--   0        0        0     1516 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/middlewares.py
--rw-r--r--   0        0        0      882 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/migrations.py
--rw-r--r--   0        0        0     4019 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/postgresql.py
--rw-r--r--   0        0        0      695 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/register.py
--rw-r--r--   0        0        0     1442 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/sentry.py
--rw-r--r--   0        0        0      347 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/settings.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/tests/__init__.py
--rw-r--r--   0        0        0     4551 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/tests/helpers.py
--rw-r--r--   0        0        0       82 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/tests/make.py
--rw-r--r--   0        0        0      486 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/text.py
--rw-r--r--   0        0        0     1088 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/core/utils.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/domain/tests/__init__.py
--rw-r--r--   0        0        0     6590 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/domain/tests/test_urls.py
--rw-r--r--   0        0        0     3811 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/domain/urls.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/__init__.py
--rw-r--r--   0        0        0      826 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/domain.py
--rw-r--r--   0        0        0     1905 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/entities.py
--rw-r--r--   0        0        0      131 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/errors.py
--rw-r--r--   0        0        0     1027 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
--rw-r--r--   0        0        0      641 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
--rw-r--r--   0        0        0      561 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
--rw-r--r--   0        0        0      531 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
--rw-r--r--   0        0        0      725 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
--rw-r--r--   0        0        0     4062 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/tests/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/tests/fixtures.py
--rw-r--r--   0        0        0     1178 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/tests/make.py
--rw-r--r--   0        0        0      445 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/tests/test_domain.py
--rw-r--r--   0        0        0     7782 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_collections/__init__.py
--rw-r--r--   0        0        0      495 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_collections/collections/artificial_intelligence.py
--rw-r--r--   0        0        0     1357 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_collections/collections/gamedev.py
--rw-r--r--   0        0        0      777 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_collections/domain.py
--rw-r--r--   0        0        0      128 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_collections/entities.py
--rw-r--r--   0        0        0      573 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_collections/predefines.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_collections/tests/__init__.py
--rw-r--r--   0        0        0      684 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_collections/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_discoverer/__init__.py
--rw-r--r--   0        0        0     3974 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_discoverer/domain.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_links/__init__.py
--rw-r--r--   0        0        0      553 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_links/domain.py
--rw-r--r--   0        0        0      163 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_links/entities.py
--rw-r--r--   0        0        0      810 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
--rw-r--r--   0        0        0     2326 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_links/operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_links/tests/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/feeds_links/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/__init__.py
--rw-r--r--   0        0        0     4734 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/background_processors.py
--rw-r--r--   0        0        0     3512 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/domain.py
--rw-r--r--   0        0        0      205 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/entities.py
--rw-r--r--   0        0        0      217 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/errors.py
--rw-r--r--   0        0        0     2101 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
--rw-r--r--   0        0        0     3035 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
--rw-r--r--   0        0        0     5112 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/__init__.py
--rw-r--r--   0        0        0     1255 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/base.py
--rw-r--r--   0        0        0     1548 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/domain.py
--rw-r--r--   0        0        0      468 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/native_tags.py
--rw-r--r--   0        0        0     3295 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/openai_chat_3_5.py
--rw-r--r--   0        0        0     4421 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/openai_chat_3_5_functions.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/tests/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/tests/test_upper_case_title.py
--rw-r--r--   0        0        0      434 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/processors/upper_case_title.py
--rw-r--r--   0        0        0     1089 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/settings.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/tests/__init__.py
--rw-r--r--   0        0        0      845 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/tests/fixtures.py
--rw-r--r--   0        0        0      487 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/tests/helpers.py
--rw-r--r--   0        0        0      553 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/tests/make.py
--rw-r--r--   0        0        0     2737 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/tests/test_background_processors.py
--rw-r--r--   0        0        0    13605 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/tests/test_domain.py
--rw-r--r--   0        0        0    14031 2024-05-14 20:03:50.419841 ffun-1.5.1/ffun/librarian/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/__init__.py
--rw-r--r--   0        0        0     1591 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/domain.py
--rw-r--r--   0        0        0     1168 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/entities.py
--rw-r--r--   0        0        0      149 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/errors.py
--rw-r--r--   0        0        0     1498 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
--rw-r--r--   0        0        0     1288 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
--rw-r--r--   0        0        0      710 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
--rw-r--r--   0        0        0     1125 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
--rw-r--r--   0        0        0     1003 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
--rw-r--r--   0        0        0     1194 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
--rw-r--r--   0        0        0      784 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
--rw-r--r--   0        0        0     5590 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/operations.py
--rw-r--r--   0        0        0      294 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/settings.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/tests/__init__.py
--rw-r--r--   0        0        0      799 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/tests/fixtures.py
--rw-r--r--   0        0        0     1663 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/tests/make.py
--rw-r--r--   0        0        0     1414 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/tests/test_domain.py
--rw-r--r--   0        0        0    15557 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/library/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/loader/__init__.py
--rw-r--r--   0        0        0      882 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/loader/background_loader.py
--rw-r--r--   0        0        0    11676 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/loader/domain.py
--rw-r--r--   0        0        0      181 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/loader/errors.py
--rw-r--r--   0        0        0      477 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/loader/settings.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/loader/tests/__init__.py
--rw-r--r--   0        0        0     7271 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/loader/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/markers/__init__.py
--rw-r--r--   0        0        0      504 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/markers/domain.py
--rw-r--r--   0        0        0       57 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/markers/entities.py
--rw-r--r--   0        0        0      855 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
--rw-r--r--   0        0        0     2447 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/markers/operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/markers/tests/__init__.py
--rw-r--r--   0        0        0     4835 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/markers/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/meta/__init__.py
--rw-r--r--   0        0        0     2582 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/meta/domain.py
--rw-r--r--   0        0        0      345 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/meta/tests/__init__.py
--rw-r--r--   0        0        0    12775 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/meta/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/__init__.py
--rw-r--r--   0        0        0     3840 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/domain.py
--rw-r--r--   0        0        0     1683 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/entities.py
--rw-r--r--   0        0        0     1092 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
--rw-r--r--   0        0        0      520 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
--rw-r--r--   0        0        0      799 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
--rw-r--r--   0        0        0     1008 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
--rw-r--r--   0        0        0     6307 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/tests/__init__.py
--rw-r--r--   0        0        0      834 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/tests/fixtures.py
--rw-r--r--   0        0        0      408 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/tests/helpers.py
--rw-r--r--   0        0        0     9964 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/ontology/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/__init__.py
--rw-r--r--   0        0        0     5962 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/client.py
--rw-r--r--   0        0        0      612 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/entities.py
--rw-r--r--   0        0        0      150 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/errors.py
--rw-r--r--   0        0        0     7597 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/keys_rotator.py
--rw-r--r--   0        0        0     1919 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/keys_statuses.py
--rw-r--r--   0        0        0      372 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/settings.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/tests/__init__.py
--rw-r--r--   0        0        0      130 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/tests/conftest.py
--rw-r--r--   0        0        0     2518 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/tests/fixtures.py
--rw-r--r--   0        0        0    19734 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/tests/test_keys_rotator.py
--rw-r--r--   0        0        0     2833 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/openai/tests/test_keys_statuses.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/__init__.py
--rw-r--r--   0        0        0      228 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/domain.py
--rw-r--r--   0        0        0      560 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/entities.py
--rw-r--r--   0        0        0     2355 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/feed.py
--rw-r--r--   0        0        0     1325 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/feedly.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/tests/__init__.py
--rw-r--r--   0        0        0     1219 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
--rw-r--r--   0        0        0      639 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
--rw-r--r--   0        0        0     4745 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
--rw-r--r--   0        0        0     1072 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
--rw-r--r--   0        0        0      966 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/tests/make.py
--rw-r--r--   0        0        0     1205 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/parsers/tests/test_feed.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/__init__.py
--rw-r--r--   0        0        0      769 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/domain.py
--rw-r--r--   0        0        0      280 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/entities.py
--rw-r--r--   0        0        0      120 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/errors.py
--rw-r--r--   0        0        0      865 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
--rw-r--r--   0        0        0     3984 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/tests/__init__.py
--rw-r--r--   0        0        0     1945 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/tests/test_domain.py
--rw-r--r--   0        0        0     9480 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/resources/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/scores/__init__.py
--rw-r--r--   0        0        0      884 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/scores/domain.py
--rw-r--r--   0        0        0      250 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/scores/entities.py
--rw-r--r--   0        0        0      104 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/scores/errors.py
--rw-r--r--   0        0        0      851 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
--rw-r--r--   0        0        0      603 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
--rw-r--r--   0        0        0     2603 2024-05-14 20:03:50.423841 ffun-1.5.1/ffun/scores/operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/scores/tests/__init__.py
--rw-r--r--   0        0        0     1239 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/scores/tests/test_domain.py
--rw-r--r--   0        0        0     6810 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/scores/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/tags/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/tags/converters.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/tags/tests/__init__.py
--rw-r--r--   0        0        0     1352 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/tags/tests/test_converters.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/__init__.py
--rw-r--r--   0        0        0     1842 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/domain.py
--rw-r--r--   0        0        0       54 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/entities.py
--rw-r--r--   0        0        0      137 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/errors.py
--rw-r--r--   0        0        0      732 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
--rw-r--r--   0        0        0      534 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
--rw-r--r--   0        0        0     1748 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/operations.py
--rw-r--r--   0        0        0      581 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/settings.py
--rw-r--r--   0        0        0      508 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/tests/asserts.py
--rw-r--r--   0        0        0     6956 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/tests/test_domain.py
--rw-r--r--   0        0        0     5492 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/tests/test_operations.py
--rw-r--r--   0        0        0     2297 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/types.py
--rw-r--r--   0        0        0      489 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/user_settings/values.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/__init__.py
--rw-r--r--   0        0        0      586 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/domain.py
--rw-r--r--   0        0        0      161 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/entities.py
--rw-r--r--   0        0        0      111 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/errors.py
--rw-r--r--   0        0        0      718 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
--rw-r--r--   0        0        0     1232 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/operations.py
--rw-r--r--   0        0        0        0 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/tests/fixtures.py
--rw-r--r--   0        0        0      348 2024-05-14 20:03:50.427841 ffun-1.5.1/ffun/users/tests/make.py
--rw-r--r--   0        0        0     4263 2024-05-14 20:03:58.983873 ffun-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      344 2024-05-19 16:42:13.929798 ffun-1.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/api/__init__.py
+-rw-r--r--   0        0        0    10249 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/api/entities.py
+-rw-r--r--   0        0        0    13637 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/api/http_handlers.py
+-rw-r--r--   0        0        0      245 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/api/settings.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/application/__init__.py
+-rw-r--r--   0        0        0     4314 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/application.py
+-rw-r--r--   0        0        0      115 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/errors.py
+-rw-r--r--   0        0        0       68 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/resources.py
+-rw-r--r--   0        0        0     1635 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/settings.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/tests/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/tests/test_settings.py
+-rw-r--r--   0        0        0     3724 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/user_settings.py
+-rw-r--r--   0        0        0      281 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/utils.py
+-rw-r--r--   0        0        0     1252 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/workers.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/auth/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/auth/dependencies.py
+-rw-r--r--   0        0        0      828 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/auth/settings.py
+-rw-r--r--   0        0        0     2800 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/auth/supertokens.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/application.py
+-rw-r--r--   0        0        0      439 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/configs.py
+-rw-r--r--   0        0        0     1050 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/entries.py
+-rw-r--r--   0        0        0     1393 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/failed_entries.py
+-rw-r--r--   0        0        0      538 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/meta.py
+-rw-r--r--   0        0        0     1001 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/supertokens.py
+-rw-r--r--   0        0        0      884 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/workers.py
+-rw-r--r--   0        0        0      209 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/yoyo.py
+-rw-r--r--   0        0        0     1333 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/api.py
+-rw-r--r--   0        0        0     3139 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/background_tasks.py
+-rw-r--r--   0        0        0      493 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/entities.py
+-rw-r--r--   0        0        0      552 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/errors.py
+-rw-r--r--   0        0        0     2773 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/json.py
+-rw-r--r--   0        0        0     5440 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/logging.py
+-rw-r--r--   0        0        0     1516 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/middlewares.py
+-rw-r--r--   0        0        0      882 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/migrations.py
+-rw-r--r--   0        0        0     4019 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/postgresql.py
+-rw-r--r--   0        0        0      695 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/register.py
+-rw-r--r--   0        0        0     1442 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/sentry.py
+-rw-r--r--   0        0        0      347 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/settings.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/tests/__init__.py
+-rw-r--r--   0        0        0     4551 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/tests/helpers.py
+-rw-r--r--   0        0        0       82 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/tests/make.py
+-rw-r--r--   0        0        0      486 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/text.py
+-rw-r--r--   0        0        0     1088 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/utils.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/domain/tests/__init__.py
+-rw-r--r--   0        0        0     6590 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/domain/tests/test_urls.py
+-rw-r--r--   0        0        0     3811 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/domain/urls.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/domain.py
+-rw-r--r--   0        0        0     1905 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/entities.py
+-rw-r--r--   0        0        0      131 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/errors.py
+-rw-r--r--   0        0        0     1027 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
+-rw-r--r--   0        0        0      641 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
+-rw-r--r--   0        0        0      561 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
+-rw-r--r--   0        0        0      531 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
+-rw-r--r--   0        0        0      725 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
+-rw-r--r--   0        0        0     4062 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/fixtures.py
+-rw-r--r--   0        0        0     1178 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/make.py
+-rw-r--r--   0        0        0      445 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/test_domain.py
+-rw-r--r--   0        0        0     7782 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/collections/artificial_intelligence.py
+-rw-r--r--   0        0        0     1357 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/collections/gamedev.py
+-rw-r--r--   0        0        0      777 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/domain.py
+-rw-r--r--   0        0        0      128 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/entities.py
+-rw-r--r--   0        0        0      573 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/predefines.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/tests/__init__.py
+-rw-r--r--   0        0        0      684 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_discoverer/__init__.py
+-rw-r--r--   0        0        0     3974 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_discoverer/domain.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/__init__.py
+-rw-r--r--   0        0        0      553 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/domain.py
+-rw-r--r--   0        0        0      163 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/entities.py
+-rw-r--r--   0        0        0      810 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
+-rw-r--r--   0        0        0     2326 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/tests/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/__init__.py
+-rw-r--r--   0        0        0     4734 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/background_processors.py
+-rw-r--r--   0        0        0     3512 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/domain.py
+-rw-r--r--   0        0        0      205 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/entities.py
+-rw-r--r--   0        0        0      217 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/errors.py
+-rw-r--r--   0        0        0     2101 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
+-rw-r--r--   0        0        0     3035 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
+-rw-r--r--   0        0        0     5112 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/__init__.py
+-rw-r--r--   0        0        0     1255 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/base.py
+-rw-r--r--   0        0        0     1548 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/domain.py
+-rw-r--r--   0        0        0      468 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/native_tags.py
+-rw-r--r--   0        0        0     3295 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/openai_chat_3_5.py
+-rw-r--r--   0        0        0     4421 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/openai_chat_3_5_functions.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/tests/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/tests/test_upper_case_title.py
+-rw-r--r--   0        0        0      434 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/upper_case_title.py
+-rw-r--r--   0        0        0     1089 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/settings.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/tests/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/tests/fixtures.py
+-rw-r--r--   0        0        0      487 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/helpers.py
+-rw-r--r--   0        0        0      553 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/make.py
+-rw-r--r--   0        0        0     2737 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/test_background_processors.py
+-rw-r--r--   0        0        0    13605 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/test_domain.py
+-rw-r--r--   0        0        0    14031 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/__init__.py
+-rw-r--r--   0        0        0     1476 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/domain.py
+-rw-r--r--   0        0        0     1168 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/entities.py
+-rw-r--r--   0        0        0      149 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/errors.py
+-rw-r--r--   0        0        0     1498 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
+-rw-r--r--   0        0        0     1288 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
+-rw-r--r--   0        0        0      710 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
+-rw-r--r--   0        0        0     1125 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
+-rw-r--r--   0        0        0     1003 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
+-rw-r--r--   0        0        0     1194 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
+-rw-r--r--   0        0        0      784 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
+-rw-r--r--   0        0        0     5926 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/fixtures.py
+-rw-r--r--   0        0        0     1663 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/make.py
+-rw-r--r--   0        0        0     1414 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/test_domain.py
+-rw-r--r--   0        0        0    15331 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/background_loader.py
+-rw-r--r--   0        0        0    11775 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/domain.py
+-rw-r--r--   0        0        0      181 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/errors.py
+-rw-r--r--   0        0        0      477 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/settings.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/tests/__init__.py
+-rw-r--r--   0        0        0     8583 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/domain.py
+-rw-r--r--   0        0        0       57 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/entities.py
+-rw-r--r--   0        0        0      855 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
+-rw-r--r--   0        0        0     2447 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/tests/__init__.py
+-rw-r--r--   0        0        0     4835 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/__init__.py
+-rw-r--r--   0        0        0     3557 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/domain.py
+-rw-r--r--   0        0        0      345 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
+-rw-r--r--   0        0        0      246 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/settings.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/tests/__init__.py
+-rw-r--r--   0        0        0    15939 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/__init__.py
+-rw-r--r--   0        0        0     3840 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/domain.py
+-rw-r--r--   0        0        0     1683 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/entities.py
+-rw-r--r--   0        0        0     1092 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
+-rw-r--r--   0        0        0      520 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
+-rw-r--r--   0        0        0      799 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
+-rw-r--r--   0        0        0     1008 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
+-rw-r--r--   0        0        0     6307 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/tests/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/tests/fixtures.py
+-rw-r--r--   0        0        0      408 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/tests/helpers.py
+-rw-r--r--   0        0        0     9964 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/__init__.py
+-rw-r--r--   0        0        0     5962 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/client.py
+-rw-r--r--   0        0        0      612 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/entities.py
+-rw-r--r--   0        0        0      150 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/errors.py
+-rw-r--r--   0        0        0     7597 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/keys_rotator.py
+-rw-r--r--   0        0        0     1919 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/keys_statuses.py
+-rw-r--r--   0        0        0      372 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/settings.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/conftest.py
+-rw-r--r--   0        0        0     2518 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/fixtures.py
+-rw-r--r--   0        0        0    19734 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/test_keys_rotator.py
+-rw-r--r--   0        0        0     2833 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/test_keys_statuses.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/domain.py
+-rw-r--r--   0        0        0      560 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/entities.py
+-rw-r--r--   0        0        0     2355 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/feed.py
+-rw-r--r--   0        0        0     1325 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/feedly.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/__init__.py
+-rw-r--r--   0        0        0     1219 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
+-rw-r--r--   0        0        0      639 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
+-rw-r--r--   0        0        0     4745 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
+-rw-r--r--   0        0        0     1072 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
+-rw-r--r--   0        0        0      966 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/make.py
+-rw-r--r--   0        0        0     1205 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/test_feed.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/domain.py
+-rw-r--r--   0        0        0      280 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/entities.py
+-rw-r--r--   0        0        0      120 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/errors.py
+-rw-r--r--   0        0        0      865 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
+-rw-r--r--   0        0        0     3984 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/tests/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/tests/test_domain.py
+-rw-r--r--   0        0        0     9480 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/scores/__init__.py
+-rw-r--r--   0        0        0      884 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/scores/domain.py
+-rw-r--r--   0        0        0      250 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/scores/entities.py
+-rw-r--r--   0        0        0      104 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/errors.py
+-rw-r--r--   0        0        0      851 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
+-rw-r--r--   0        0        0      603 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
+-rw-r--r--   0        0        0     2603 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/tests/__init__.py
+-rw-r--r--   0        0        0     1239 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/tests/test_domain.py
+-rw-r--r--   0        0        0     6810 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/tags/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/tags/converters.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/tags/tests/__init__.py
+-rw-r--r--   0        0        0     1352 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/tags/tests/test_converters.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/__init__.py
+-rw-r--r--   0        0        0     1842 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/domain.py
+-rw-r--r--   0        0        0       54 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/entities.py
+-rw-r--r--   0        0        0      137 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/errors.py
+-rw-r--r--   0        0        0      732 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
+-rw-r--r--   0        0        0      534 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
+-rw-r--r--   0        0        0     1748 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/operations.py
+-rw-r--r--   0        0        0      581 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/settings.py
+-rw-r--r--   0        0        0      508 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/tests/asserts.py
+-rw-r--r--   0        0        0     6956 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/tests/test_domain.py
+-rw-r--r--   0        0        0     5492 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/tests/test_operations.py
+-rw-r--r--   0        0        0     2297 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/types.py
+-rw-r--r--   0        0        0      489 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/values.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/domain.py
+-rw-r--r--   0        0        0      161 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/entities.py
+-rw-r--r--   0        0        0      111 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/errors.py
+-rw-r--r--   0        0        0      718 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
+-rw-r--r--   0        0        0     1232 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/operations.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/tests/fixtures.py
+-rw-r--r--   0        0        0      348 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/tests/make.py
+-rw-r--r--   0        0        0     4263 2024-05-19 16:42:23.089859 ffun-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.5.2/PKG-INFO
```

### Comparing `ffun-1.5.1/ffun/api/entities.py` & `ffun-1.5.2/ffun/api/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/api/http_handlers.py` & `ffun-1.5.2/ffun/api/http_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import fastapi
 from fastapi.openapi.docs import get_swagger_ui_html
 from fastapi.openapi.utils import get_openapi
 from fastapi.responses import HTMLResponse, JSONResponse
 
 from ffun.api import entities
+from ffun.api.settings import settings
 from ffun.auth.dependencies import User
 from ffun.core import logging
 from ffun.feeds import domain as f_domain
 from ffun.feeds import entities as f_entities
 from ffun.feeds_collections import domain as fc_domain
 from ffun.feeds_discoverer import domain as fd_domain
 from ffun.feeds_links import domain as fl_domain
@@ -93,16 +94,17 @@
 
 @router.post("/api/get-last-entries")
 async def api_get_last_entries(request: entities.GetLastEntriesRequest, user: User) -> entities.GetLastEntriesResponse:
     linked_feeds = await fl_domain.get_linked_feeds(user.id)
 
     linked_feeds_ids = [link.feed_id for link in linked_feeds]
 
-    # TODO: limit
-    entries = await l_domain.get_entries_by_filter(feeds_ids=linked_feeds_ids, period=request.period, limit=10000)
+    entries = await l_domain.get_entries_by_filter(
+        feeds_ids=linked_feeds_ids, period=request.period, limit=settings.max_returned_entries
+    )
 
     external_entries = await _external_entries(entries, with_body=False, user_id=user.id)
 
     return entities.GetLastEntriesResponse(entries=external_entries)
 
 
 @router.post("/api/get-entries-by-ids")
```

### Comparing `ffun-1.5.1/ffun/application/application.py` & `ffun-1.5.2/ffun/application/application.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/application/settings.py` & `ffun-1.5.2/ffun/application/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/application/user_settings.py` & `ffun-1.5.2/ffun/application/user_settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/application/workers.py` & `ffun-1.5.2/ffun/application/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/auth/dependencies.py` & `ffun-1.5.2/ffun/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/auth/settings.py` & `ffun-1.5.2/ffun/auth/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/auth/supertokens.py` & `ffun-1.5.2/ffun/auth/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/cli/commands/configs.py` & `ffun-1.5.2/ffun/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/cli/commands/entries.py` & `ffun-1.5.2/ffun/cli/commands/entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/cli/commands/failed_entries.py` & `ffun-1.5.2/ffun/cli/commands/failed_entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/cli/commands/meta.py` & `ffun-1.5.2/ffun/cli/commands/meta.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/cli/commands/supertokens.py` & `ffun-1.5.2/ffun/cli/commands/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/cli/commands/workers.py` & `ffun-1.5.2/ffun/cli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/conftest.py` & `ffun-1.5.2/ffun/conftest.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/api.py` & `ffun-1.5.2/ffun/core/api.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/background_tasks.py` & `ffun-1.5.2/ffun/core/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/errors.py` & `ffun-1.5.2/ffun/core/errors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/json.py` & `ffun-1.5.2/ffun/core/json.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/logging.py` & `ffun-1.5.2/ffun/core/logging.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/middlewares.py` & `ffun-1.5.2/ffun/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/migrations.py` & `ffun-1.5.2/ffun/core/migrations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/postgresql.py` & `ffun-1.5.2/ffun/core/postgresql.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/register.py` & `ffun-1.5.2/ffun/core/register.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/sentry.py` & `ffun-1.5.2/ffun/core/sentry.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/tests/helpers.py` & `ffun-1.5.2/ffun/core/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/core/utils.py` & `ffun-1.5.2/ffun/core/utils.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/domain/tests/test_urls.py` & `ffun-1.5.2/ffun/domain/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/domain/urls.py` & `ffun-1.5.2/ffun/domain/urls.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/domain.py` & `ffun-1.5.2/ffun/feeds/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/entities.py` & `ffun-1.5.2/ffun/feeds/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py` & `ffun-1.5.2/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py` & `ffun-1.5.2/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py` & `ffun-1.5.2/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py` & `ffun-1.5.2/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py` & `ffun-1.5.2/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/operations.py` & `ffun-1.5.2/ffun/feeds/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/tests/fixtures.py` & `ffun-1.5.2/ffun/feeds/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/tests/make.py` & `ffun-1.5.2/ffun/feeds/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds/tests/test_operations.py` & `ffun-1.5.2/ffun/feeds/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_collections/collections/gamedev.py` & `ffun-1.5.2/ffun/feeds_collections/collections/gamedev.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_collections/domain.py` & `ffun-1.5.2/ffun/feeds_collections/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_collections/predefines.py` & `ffun-1.5.2/ffun/feeds_collections/predefines.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_collections/tests/fixtures.py` & `ffun-1.5.2/ffun/feeds_collections/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_discoverer/domain.py` & `ffun-1.5.2/ffun/feeds_discoverer/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_links/domain.py` & `ffun-1.5.2/ffun/feeds_links/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py` & `ffun-1.5.2/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_links/operations.py` & `ffun-1.5.2/ffun/feeds_links/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/feeds_links/tests/test_operations.py` & `ffun-1.5.2/ffun/feeds_links/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/background_processors.py` & `ffun-1.5.2/ffun/librarian/background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/domain.py` & `ffun-1.5.2/ffun/librarian/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py` & `ffun-1.5.2/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py` & `ffun-1.5.2/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/operations.py` & `ffun-1.5.2/ffun/librarian/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/processors/base.py` & `ffun-1.5.2/ffun/librarian/processors/base.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/processors/domain.py` & `ffun-1.5.2/ffun/librarian/processors/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/processors/openai_chat_3_5.py` & `ffun-1.5.2/ffun/librarian/processors/openai_chat_3_5.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/processors/openai_chat_3_5_functions.py` & `ffun-1.5.2/ffun/librarian/processors/openai_chat_3_5_functions.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/processors/tests/test_upper_case_title.py` & `ffun-1.5.2/ffun/librarian/processors/tests/test_upper_case_title.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/settings.py` & `ffun-1.5.2/ffun/librarian/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/tests/fixtures.py` & `ffun-1.5.2/ffun/librarian/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/tests/make.py` & `ffun-1.5.2/ffun/librarian/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/tests/test_background_processors.py` & `ffun-1.5.2/ffun/librarian/tests/test_background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/tests/test_domain.py` & `ffun-1.5.2/ffun/librarian/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/librarian/tests/test_operations.py` & `ffun-1.5.2/ffun/librarian/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/domain.py` & `ffun-1.5.2/ffun/library/domain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import uuid
 
-from ffun.core.postgresql import ExecuteType, run_in_transaction
 from ffun.domain import urls as d_urls
 from ffun.feeds import domain as f_domain
 from ffun.library import operations
 from ffun.library.entities import Entry, EntryChange
 
 catalog_entries = operations.catalog_entries
 get_entries_by_ids = operations.get_entries_by_ids
 get_entries_by_filter = operations.get_entries_by_filter
 check_stored_entries_by_external_ids = operations.check_stored_entries_by_external_ids
 all_entries_iterator = operations.all_entries_iterator
 get_entries_after_pointer = operations.get_entries_after_pointer
 tech_move_entry = operations.tech_move_entry
+tech_get_feed_entries_tail = operations.tech_get_feed_entries_tail
+tech_remove_entries_by_ids = operations.tech_remove_entries_by_ids
 
 
 async def get_entry(entry_id: uuid.UUID) -> Entry:
     entries = await get_entries_by_ids([entry_id])
     found_entry = entries.get(entry_id)
     assert found_entry is not None
     return found_entry
@@ -33,12 +34,7 @@
         changes.append(
             EntryChange(id=entry.id, field="external_url", old_value=entry.external_url, new_value=new_external_url)
         )
         if apply:
             await operations.update_external_url(entry.id, new_external_url)
 
     return changes
-
-
-@run_in_transaction
-async def tech_remove_entries_by_feed_id(execute: ExecuteType, feed_id: uuid.UUID) -> None:
-    await operations.tech_remove_entries_by_feed_id(execute, feed_id)
```

### Comparing `ffun-1.5.1/ffun/library/entities.py` & `ffun-1.5.2/ffun/library/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/migrations/20230331_01_UsHwp-entries-table.py` & `ffun-1.5.2/ffun/library/migrations/20230331_01_UsHwp-entries-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py` & `ffun-1.5.2/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/migrations/20230514_01_Bwb35-processed-state.py` & `ffun-1.5.2/ffun/library/migrations/20230514_01_Bwb35-processed-state.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py` & `ffun-1.5.2/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py` & `ffun-1.5.2/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py` & `ffun-1.5.2/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py` & `ffun-1.5.2/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/operations.py` & `ffun-1.5.2/ffun/library/operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import uuid
 from typing import Any, AsyncGenerator, Iterable
 
 import psycopg
 
 from ffun.core import logging
-from ffun.core.postgresql import ExecuteType, execute
+from ffun.core.postgresql import execute
 from ffun.library import errors
 from ffun.library.entities import Entry
 
 logger = logging.get_module_logger()
 
 
 sql_insert_entry = """
@@ -142,36 +142,46 @@
     SET external_url = %(url)s
     WHERE id = %(entity_id)s
     """
 
     await execute(sql, {"entity_id": entity_id, "url": url})
 
 
-async def tech_remove_entries_by_ids(execute: ExecuteType, entries_ids: Iterable[uuid.UUID]) -> None:
+async def tech_remove_entries_by_ids(entries_ids: Iterable[uuid.UUID]) -> None:
     sql = """
     DELETE FROM l_entries
     WHERE id = ANY(%(entries_ids)s)
     """
 
     await execute(sql, {"entries_ids": list(entries_ids)})
 
 
-async def tech_remove_entries_by_feed_id(execute: ExecuteType, feed_id: uuid.UUID) -> None:
-    sql = """
-    DELETE FROM l_entries
-    WHERE feed_id = %(feed_id)s
-    """
-
-    await execute(sql, {"feed_id": feed_id})
-
-
 async def tech_move_entry(entry_id: uuid.UUID, feed_id: uuid.UUID) -> None:
     sql = """
     UPDATE l_entries
     SET feed_id = %(feed_id)s
     WHERE id = %(entry_id)s
     """
 
     try:
         await execute(sql, {"entry_id": entry_id, "feed_id": feed_id})
     except psycopg.errors.UniqueViolation as e:
         raise errors.CanNotMoveEntryAlreadyInFeed(entry_id=entry_id, feed_id=feed_id) from e
+
+
+async def tech_get_feed_entries_tail(feed_id: uuid.UUID, offset: int) -> set[uuid.UUID]:
+    """
+    Get the last entries for the feed.
+    """
+    # Order by published_at because we want to keep the newest entries
+    # and it is better to take decission based on time from an entry's source rather than on time when we collected it
+    sql = """
+    SELECT id
+    FROM l_entries
+    WHERE feed_id = %(feed_id)s
+    ORDER BY published_at DESC
+    OFFSET %(offset)s
+    """
+
+    result = await execute(sql, {"feed_id": feed_id, "offset": offset})
+
+    return {row["id"] for row in result}
```

### Comparing `ffun-1.5.1/ffun/library/tests/fixtures.py` & `ffun-1.5.2/ffun/library/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/tests/make.py` & `ffun-1.5.2/ffun/library/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/tests/test_domain.py` & `ffun-1.5.2/ffun/library/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/library/tests/test_operations.py` & `ffun-1.5.2/ffun/library/tests/test_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from ffun.library.operations import (
     all_entries_iterator,
     catalog_entries,
     check_stored_entries_by_external_ids,
     get_entries_after_pointer,
     get_entries_by_filter,
     get_entries_by_ids,
+    tech_get_feed_entries_tail,
     tech_move_entry,
-    tech_remove_entries_by_feed_id,
     tech_remove_entries_by_ids,
     update_external_url,
 )
 from ffun.library.tests import make
 
 
 class TestCatalogEntries:
@@ -331,62 +331,64 @@
         entries = await make.n_entries(loaded_feed_id, n=3)
         another_entries = await make.n_entries(another_loaded_feed_id, n=3)
 
         entries_list = list(entries.values())
         another_entries_list = list(another_entries.values())
 
         async with TableSizeDelta("l_entries", delta=-2):
-            await tech_remove_entries_by_ids(execute, [entries_list[0].id, another_entries_list[0].id])
+            await tech_remove_entries_by_ids([entries_list[0].id, another_entries_list[0].id])
 
         loaded_entries = await get_entries_by_ids([entry.id for entry in entries_list + another_entries_list])
 
         assert loaded_entries[entries_list[0].id] is None
         assert loaded_entries[another_entries_list[0].id] is None
 
     @pytest.mark.asyncio
     async def test_no_entries(self) -> None:
         async with TableSizeNotChanged("l_entries"):
-            await tech_remove_entries_by_ids(execute, [])
-            await tech_remove_entries_by_ids(execute, [uuid.uuid4()])
+            await tech_remove_entries_by_ids([])
+            await tech_remove_entries_by_ids([uuid.uuid4()])
 
     @pytest.mark.asyncio
     async def test_already_removed(self, loaded_feed_id: uuid.UUID) -> None:
         entries = await make.n_entries(loaded_feed_id, n=3)
 
         entries_list = list(entries.values())
 
-        await tech_remove_entries_by_ids(execute, [entry.id for entry in entries_list])
+        await tech_remove_entries_by_ids([entry.id for entry in entries_list])
 
         async with TableSizeNotChanged("l_entries"):
-            await tech_remove_entries_by_ids(execute, [entry.id for entry in entries_list])
+            await tech_remove_entries_by_ids([entry.id for entry in entries_list])
 
 
-class TestTechRemoveEntriesByFeedId:
+class TestTechGetFeedEntriesTail:
     @pytest.mark.asyncio
-    async def test_removed(self, loaded_feed_id: uuid.UUID, another_loaded_feed_id: uuid.UUID) -> None:
-        entries = await make.n_entries(loaded_feed_id, n=3)
-        another_entries = await make.n_entries(another_loaded_feed_id, n=3)
+    async def test_nothing_to_return(self, loaded_feed_id: uuid.UUID) -> None:
+        await make.n_entries(loaded_feed_id, n=5)
 
-        async with TableSizeDelta("l_entries", delta=-3):
-            await tech_remove_entries_by_feed_id(execute, loaded_feed_id)
+        ids = await tech_get_feed_entries_tail(loaded_feed_id, offset=10)
 
-        loaded_entries = await get_entries_by_ids([entry.id for entry in entries.values()])
+        assert ids == set()
 
-        assert loaded_entries == {entry.id: None for entry in entries.values()}
+    @pytest.mark.asyncio
+    async def test_zero_head(self, loaded_feed_id: uuid.UUID) -> None:
+        entries = await make.n_entries(loaded_feed_id, n=5)
 
-        another_loaded_entries = await get_entries_by_ids([entry.id for entry in another_entries.values()])
+        ids = await tech_get_feed_entries_tail(loaded_feed_id, offset=0)
 
-        assert another_loaded_entries == another_entries
+        assert ids == set(entry.id for entry in entries.values())
 
     @pytest.mark.asyncio
-    async def test_no_entries(self) -> None:
-        async with TableSizeNotChanged("l_entries"):
-            await tech_remove_entries_by_feed_id(execute, uuid.uuid4())
+    async def test_not_excceed_limit(self, loaded_feed_id: uuid.UUID) -> None:
+        await make.n_entries(loaded_feed_id, n=5)
+
+        ids = await tech_get_feed_entries_tail(loaded_feed_id, offset=10)
+
+        assert ids == set()
 
     @pytest.mark.asyncio
-    async def test_already_removed(self, loaded_feed_id: uuid.UUID) -> None:
-        await make.n_entries(loaded_feed_id, n=3)
+    async def test_offset(self, loaded_feed_id: uuid.UUID) -> None:
+        entries = await make.n_entries_list(loaded_feed_id, n=15)
 
-        await tech_remove_entries_by_feed_id(execute, loaded_feed_id)
+        ids = await tech_get_feed_entries_tail(loaded_feed_id, offset=10)
 
-        async with TableSizeNotChanged("l_entries"):
-            await tech_remove_entries_by_feed_id(execute, loaded_feed_id)
+        assert ids == set(entry.id for entry in entries[10:])
```

### Comparing `ffun-1.5.1/ffun/loader/background_loader.py` & `ffun-1.5.2/ffun/loader/background_loader.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/loader/domain.py` & `ffun-1.5.2/ffun/loader/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ffun.feeds.entities import Feed, FeedError, FeedState
 from ffun.feeds_collections import domain as fc_domain
 from ffun.feeds_links import domain as fl_domain
 from ffun.library import domain as l_domain
 from ffun.library import entities as l_entities
 from ffun.loader import errors
 from ffun.loader.settings import Proxy, settings
+from ffun.meta import domain as meta_domain
 from ffun.parsers import entities as p_entities
 from ffun.parsers.domain import parse_feed
 
 logger = logging.get_module_logger()
 
 
 _user_agent: str = "unknown"
@@ -307,10 +308,12 @@
     if feed_info is None:
         return
 
     await sync_feed_info(feed, feed_info)
 
     await store_entries(feed.id, feed_info.entries)
 
+    await meta_domain.limit_entries_for_feed(feed.id)
+
     await f_domain.mark_feed_as_loaded(feed.id)
 
     logger.info("entries_loaded")
```

### Comparing `ffun-1.5.1/ffun/loader/tests/test_domain.py` & `ffun-1.5.2/ffun/loader/tests/test_domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import uuid
 
 import pytest
 from pytest_mock import MockerFixture
+from structlog.testing import capture_logs
 
+from ffun.core.tests.helpers import assert_logs
 from ffun.feeds import domain as f_domain
 from ffun.feeds import entities as f_entities
 from ffun.feeds_links import domain as fl_domain
 from ffun.library import domain as l_domain
 from ffun.library import entities as l_entities
 from ffun.loader.domain import detect_orphaned, process_feed, store_entries, sync_feed_info
 from ffun.parsers import entities as p_entities
@@ -190,21 +192,55 @@
             url=saved_feed.url, title=saved_feed.title, description=saved_feed.description, entries=entry_infos
         )
 
         extract_feed_info = mocker.patch("ffun.loader.domain.extract_feed_info", return_value=feed_info)
 
         await fl_domain.add_link(internal_user_id, saved_feed.id)
 
-        await process_feed(feed=saved_feed)
+        with capture_logs() as logs:
+            await process_feed(feed=saved_feed)
+
+        assert_logs(logs, feed_has_no_entries_tail=1, feed_entries_tail_removed=0)
 
         extract_feed_info.assert_called_once_with(saved_feed)
 
         loaded_entries = await l_domain.get_entries_by_filter([saved_feed.id], limit=n + 1)
 
         assert len(loaded_entries) == n
 
         entry_infos.sort(key=lambda e: e.title)
         loaded_entries.sort(key=lambda e: e.title)
 
         for entry_info, entry in zip(entry_infos, loaded_entries):
             assert entry.feed_id == saved_feed.id
             assert_entriy_equal_to_info(entry_info, entry)
+
+    @pytest.mark.asyncio
+    async def test_remove_too_long_entries_tail(
+        self, internal_user_id: uuid.UUID, saved_feed: f_entities.Feed, mocker: MockerFixture
+    ) -> None:
+        n = 5
+        m = 3
+
+        entry_infos = [p_make.fake_entry_info() for _ in range(n)]
+        entry_infos.sort(key=lambda e: e.title)
+
+        assert saved_feed.title
+        assert saved_feed.description
+
+        feed_info = p_entities.FeedInfo(
+            url=saved_feed.url, title=saved_feed.title, description=saved_feed.description, entries=entry_infos
+        )
+
+        mocker.patch("ffun.loader.domain.extract_feed_info", return_value=feed_info)
+        mocker.patch("ffun.meta.settings.settings.max_entries_per_feed", m)
+
+        await fl_domain.add_link(internal_user_id, saved_feed.id)
+
+        with capture_logs() as logs:
+            await process_feed(feed=saved_feed)
+
+        assert_logs(logs, feed_has_no_entries_tail=0, feed_entries_tail_removed=1)
+
+        loaded_entries = await l_domain.get_entries_by_filter([saved_feed.id], limit=n + 1)
+
+        assert len(loaded_entries) == m
```

### Comparing `ffun-1.5.1/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py` & `ffun-1.5.2/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/markers/operations.py` & `ffun-1.5.2/ffun/markers/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/markers/tests/test_operations.py` & `ffun-1.5.2/ffun/markers/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/meta/tests/test_domain.py` & `ffun-1.5.2/ffun/meta/tests/test_domain.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ffun.feeds import domain as f_domain
 from ffun.feeds import errors as f_errors
 from ffun.feeds_links import domain as fl_domain
 from ffun.library import domain as l_domain
 from ffun.library.tests import make as l_make
 from ffun.markers import domain as m_domains
 from ffun.markers.entities import Marker
-from ffun.meta.domain import merge_feeds, remove_feed
+from ffun.meta.domain import limit_entries_for_feed, merge_feeds, remove_entries, remove_feed
 from ffun.ontology import domain as o_domain
 from ffun.ontology.entities import ProcessorTag
 from ffun.users.tests import make as u_make
 
 
 class TestRemoveFeed:
     @pytest.mark.asyncio
@@ -305,7 +305,94 @@
         markers_a = await m_domains.get_markers(user_a, [entry.id for entry in another_entries])
         markers_b = await m_domains.get_markers(user_b, [entry.id for entry in another_entries])
         markers_c = await m_domains.get_markers(user_c, [entry.id for entry in another_entries])
 
         assert markers_a == {another_entries[1].id: {Marker.read}}
         assert markers_b == {another_entries[0].id: {Marker.read}, another_entries[2].id: {Marker.read}}
         assert markers_c == {another_entries[1].id: {Marker.read}}
+
+
+class TestRemoveEntries:
+    @pytest.mark.asyncio
+    async def test_no_entries(self) -> None:
+        await remove_entries([])
+
+    @pytest.mark.asyncio
+    async def test_success(
+        self,
+        loaded_feed_id: uuid.UUID,
+        another_loaded_feed_id: uuid.UUID,
+        fake_processor_id: int,
+        another_fake_processor_id: int,
+        three_processor_tags: tuple[ProcessorTag, ProcessorTag, ProcessorTag],
+    ) -> None:
+        entries = await l_make.n_entries_list(loaded_feed_id, 3)
+        another_entries = await l_make.n_entries_list(another_loaded_feed_id, 3)
+
+        tag_a, tag_b, tag_c = three_processor_tags
+
+        # fill feed 1
+        await o_domain.apply_tags_to_entry(entry_id=entries[0].id, processor_id=fake_processor_id, tags=[tag_a])
+
+        await o_domain.apply_tags_to_entry(entry_id=entries[1].id, processor_id=fake_processor_id, tags=[tag_a])
+
+        await o_domain.apply_tags_to_entry(
+            entry_id=entries[1].id, processor_id=another_fake_processor_id, tags=[tag_b]
+        )
+
+        # fill feed 2
+        await o_domain.apply_tags_to_entry(
+            entry_id=another_entries[1].id, processor_id=fake_processor_id, tags=[tag_a]
+        )
+
+        await o_domain.apply_tags_to_entry(
+            entry_id=another_entries[1].id, processor_id=another_fake_processor_id, tags=[tag_b]
+        )
+
+        await o_domain.apply_tags_to_entry(
+            entry_id=another_entries[2].id, processor_id=another_fake_processor_id, tags=[tag_c]
+        )
+
+        await remove_entries([entries[0].id, another_entries[1].id, entries[2].id])
+
+        loaded_entries = await l_domain.get_entries_by_ids(
+            [entry.id for entry in entries] + [entry.id for entry in another_entries]
+        )
+
+        assert loaded_entries == {
+            entries[0].id: None,
+            entries[1].id: entries[1],
+            entries[2].id: None,
+            another_entries[0].id: another_entries[0],
+            another_entries[1].id: None,
+            another_entries[2].id: another_entries[2],
+        }
+
+
+class TestLimitEntriesForFeed:
+    @pytest.mark.asyncio
+    async def test_no_feed(self) -> None:
+        await limit_entries_for_feed(uuid.uuid4(), limit=10)
+
+    @pytest.mark.asyncio
+    async def test_no_entries(self, loaded_feed_id: uuid.UUID) -> None:
+        await limit_entries_for_feed(loaded_feed_id, limit=10)
+
+    @pytest.mark.asyncio
+    async def test_not_exceed_limit(self, loaded_feed_id: uuid.UUID) -> None:
+        entries = await l_make.n_entries_list(loaded_feed_id, 3)
+
+        await limit_entries_for_feed(loaded_feed_id, limit=10)
+
+        loaded_entries = await l_domain.get_entries_by_filter(feeds_ids=[loaded_feed_id], limit=100)
+
+        assert loaded_entries == entries
+
+    @pytest.mark.asyncio
+    async def test_exceed_limit(self, loaded_feed_id: uuid.UUID) -> None:
+        entries = await l_make.n_entries_list(loaded_feed_id, 10)
+
+        await limit_entries_for_feed(loaded_feed_id, limit=5)
+
+        loaded_entries = await l_domain.get_entries_by_filter(feeds_ids=[loaded_feed_id], limit=100)
+
+        assert loaded_entries == entries[:5]
```

### Comparing `ffun-1.5.1/ffun/ontology/domain.py` & `ffun-1.5.2/ffun/ontology/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/ontology/entities.py` & `ffun-1.5.2/ffun/ontology/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py` & `ffun-1.5.2/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py` & `ffun-1.5.2/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py` & `ffun-1.5.2/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py` & `ffun-1.5.2/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/ontology/operations.py` & `ffun-1.5.2/ffun/ontology/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/ontology/tests/fixtures.py` & `ffun-1.5.2/ffun/ontology/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/ontology/tests/test_operations.py` & `ffun-1.5.2/ffun/ontology/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/openai/client.py` & `ffun-1.5.2/ffun/openai/client.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/openai/entities.py` & `ffun-1.5.2/ffun/openai/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/openai/keys_rotator.py` & `ffun-1.5.2/ffun/openai/keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/openai/keys_statuses.py` & `ffun-1.5.2/ffun/openai/keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/openai/tests/fixtures.py` & `ffun-1.5.2/ffun/openai/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/openai/tests/test_keys_rotator.py` & `ffun-1.5.2/ffun/openai/tests/test_keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/openai/tests/test_keys_statuses.py` & `ffun-1.5.2/ffun/openai/tests/test_keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/entities.py` & `ffun-1.5.2/ffun/parsers/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/feed.py` & `ffun-1.5.2/ffun/parsers/feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/feedly.py` & `ffun-1.5.2/ffun/parsers/feedly.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml` & `ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json` & `ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml` & `ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json` & `ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/tests/make.py` & `ffun-1.5.2/ffun/parsers/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/parsers/tests/test_feed.py` & `ffun-1.5.2/ffun/parsers/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/resources/domain.py` & `ffun-1.5.2/ffun/resources/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/resources/migrations/20230702_01_LEEES-resources-table.py` & `ffun-1.5.2/ffun/resources/migrations/20230702_01_LEEES-resources-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/resources/operations.py` & `ffun-1.5.2/ffun/resources/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/resources/tests/test_domain.py` & `ffun-1.5.2/ffun/resources/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/resources/tests/test_operations.py` & `ffun-1.5.2/ffun/resources/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/scores/domain.py` & `ffun-1.5.2/ffun/scores/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py` & `ffun-1.5.2/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py` & `ffun-1.5.2/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/scores/operations.py` & `ffun-1.5.2/ffun/scores/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/scores/tests/test_domain.py` & `ffun-1.5.2/ffun/scores/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/scores/tests/test_operations.py` & `ffun-1.5.2/ffun/scores/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/tags/converters.py` & `ffun-1.5.2/ffun/tags/converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/tags/tests/test_converters.py` & `ffun-1.5.2/ffun/tags/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/user_settings/domain.py` & `ffun-1.5.2/ffun/user_settings/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py` & `ffun-1.5.2/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py` & `ffun-1.5.2/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/user_settings/operations.py` & `ffun-1.5.2/ffun/user_settings/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/user_settings/settings.py` & `ffun-1.5.2/ffun/user_settings/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/user_settings/tests/test_domain.py` & `ffun-1.5.2/ffun/user_settings/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/user_settings/tests/test_operations.py` & `ffun-1.5.2/ffun/user_settings/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/user_settings/types.py` & `ffun-1.5.2/ffun/user_settings/types.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/users/domain.py` & `ffun-1.5.2/ffun/users/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/users/migrations/20230527_01_soIr3-users-mapping.py` & `ffun-1.5.2/ffun/users/migrations/20230527_01_soIr3-users-mapping.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/users/operations.py` & `ffun-1.5.2/ffun/users/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/ffun/users/tests/fixtures.py` & `ffun-1.5.2/ffun/users/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.1/pyproject.toml` & `ffun-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffun"
-version = "1.5.1"
+version = "1.5.2"
 description = "Backend for the Feeds Fun — web-based news reader"
 repository = "https://github.com/Tiendil/feeds.fun"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = " BSD-3-Clause"
 readme = "README.md"
 homepage = "https://feeds.fun"
 keywords = ["news", "news-reader", "news-aggregator",
```

### Comparing `ffun-1.5.1/PKG-INFO` & `ffun-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffun
-Version: 1.5.1
+Version: 1.5.2
 Summary: Backend for the Feeds Fun — web-based news reader
 Home-page: https://feeds.fun
 License:  BSD-3-Clause
 Keywords: news,news-reader,news-aggregator,rss,rss-reader,rss-aggregator,feed,feed-reader,feed-aggregator,atom,self-hosted
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.11,<4.0
```

