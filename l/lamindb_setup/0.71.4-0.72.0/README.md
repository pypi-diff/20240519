# Comparing `tmp/lamindb_setup-0.71.4.tar.gz` & `tmp/lamindb_setup-0.72.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.71.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.72.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.71.4.tar` & `lamindb_setup-0.72.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
--rw-r--r--   0        0        0     8499 2024-05-07 15:02:32.273843 lamindb_setup-0.71.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 12:04:01.937708 lamindb_setup-0.71.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 12:04:01.937784 lamindb_setup-0.71.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-02-29 12:04:01.937868 lamindb_setup-0.71.4/.gitignore
--rw-r--r--   0        0        0     1474 2024-04-29 09:50:29.256493 lamindb_setup-0.71.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 12:04:01.938089 lamindb_setup-0.71.4/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 12:04:01.938164 lamindb_setup-0.71.4/README.md
--rw-r--r--   0        0        0   101357 2024-05-14 11:22:43.186340 lamindb_setup-0.71.4/docs/changelog.md
--rw-r--r--   0        0        0     2574 2024-04-29 09:50:29.257640 lamindb_setup-0.71.4/docs/hub-cloud/01-init-local-instance.ipynb
--rw-r--r--   0        0        0     3948 2024-04-29 09:50:29.257800 lamindb_setup-0.71.4/docs/hub-cloud/02-connect-local-instance.ipynb
--rw-r--r--   0        0        0    10851 2024-05-13 09:56:45.668066 lamindb_setup-0.71.4/docs/hub-cloud/03-add-managed-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-03-07 19:17:51.102702 lamindb_setup-0.71.4/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3191 2024-05-03 13:46:52.497497 lamindb_setup-0.71.4/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3886 2024-05-03 13:46:52.498391 lamindb_setup-0.71.4/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     5454 2024-05-02 14:13:25.437615 lamindb_setup-0.71.4/docs/hub-cloud/07-keep-artifacts-local.ipynb
--rw-r--r--   0        0        0     3160 2024-03-07 19:17:51.103066 lamindb_setup-0.71.4/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      177 2024-04-29 09:50:29.259621 lamindb_setup-0.71.4/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-03-07 19:17:51.103480 lamindb_setup-0.71.4/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-03-25 10:01:42.202871 lamindb_setup-0.71.4/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-03-19 12:58:36.468528 lamindb_setup-0.71.4/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2712 2024-04-29 09:50:29.259864 lamindb_setup-0.71.4/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-03-11 10:42:56.000471 lamindb_setup-0.71.4/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-03-07 19:17:51.104281 lamindb_setup-0.71.4/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-03-07 19:17:51.104386 lamindb_setup-0.71.4/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6182 2024-04-29 09:50:29.260752 lamindb_setup-0.71.4/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      177 2024-04-29 09:50:29.260962 lamindb_setup-0.71.4/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 12:04:01.938771 lamindb_setup-0.71.4/docs/index.md
--rw-r--r--   0        0        0      513 2024-05-02 14:13:25.438254 lamindb_setup-0.71.4/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 12:04:01.940681 lamindb_setup-0.71.4/docs/reference.md
--rw-r--r--   0        0        0     1542 2024-05-14 11:22:19.685276 lamindb_setup-0.71.4/lamindb_setup/__init__.py
--rw-r--r--   0        0        0      846 2024-04-29 09:50:29.261873 lamindb_setup-0.71.4/lamindb_setup/_cache.py
--rw-r--r--   0        0        0      129 2024-04-29 09:50:29.262000 lamindb_setup-0.71.4/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2613 2024-04-29 09:50:29.262479 lamindb_setup-0.71.4/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1186 2024-04-29 09:50:29.263120 lamindb_setup-0.71.4/lamindb_setup/_close.py
--rw-r--r--   0        0        0    12728 2024-05-09 13:59:53.552357 lamindb_setup-0.71.4/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     5498 2024-05-09 13:59:53.553371 lamindb_setup-0.71.4/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1534 2024-04-29 09:50:29.264420 lamindb_setup-0.71.4/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2120 2024-04-29 09:50:29.265153 lamindb_setup-0.71.4/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1874 2024-04-29 09:50:29.265389 lamindb_setup-0.71.4/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11897 2024-05-13 09:56:45.669008 lamindb_setup-0.71.4/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8815 2024-04-29 09:50:29.266219 lamindb_setup-0.71.4/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      940 2024-05-02 14:13:25.440107 lamindb_setup-0.71.4/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      679 2024-04-29 09:50:29.266496 lamindb_setup-0.71.4/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1419 2024-05-13 09:56:45.669863 lamindb_setup-0.71.4/lamindb_setup/_set_managed_storage.py
--rw-r--r--   0        0        0     3670 2024-04-29 09:50:29.266915 lamindb_setup-0.71.4/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1568 2024-04-29 09:50:29.267349 lamindb_setup-0.71.4/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      416 2024-05-02 14:13:25.440536 lamindb_setup-0.71.4/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     1799 2024-04-29 09:50:29.268812 lamindb_setup-0.71.4/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2520 2024-04-29 09:50:29.269069 lamindb_setup-0.71.4/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      276 2024-04-29 09:50:29.269197 lamindb_setup-0.71.4/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5504 2024-04-29 09:50:29.269650 lamindb_setup-0.71.4/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    16043 2024-05-09 13:59:53.554745 lamindb_setup-0.71.4/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4859 2024-05-03 10:21:42.522659 lamindb_setup-0.71.4/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1875 2024-04-29 09:50:29.270865 lamindb_setup-0.71.4/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3141 2024-05-02 14:13:25.441639 lamindb_setup-0.71.4/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    16191 2024-05-09 13:59:53.555705 lamindb_setup-0.71.4/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3922 2024-05-03 10:21:42.523183 lamindb_setup-0.71.4/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2704 2024-05-03 10:21:42.523417 lamindb_setup-0.71.4/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    12751 2024-05-13 09:56:45.670685 lamindb_setup-0.71.4/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     2084 2024-05-03 10:21:42.524061 lamindb_setup-0.71.4/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1344 2024-05-07 15:02:32.276034 lamindb_setup-0.71.4/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     3002 2024-04-29 09:50:29.273885 lamindb_setup-0.71.4/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6893 2024-04-29 09:50:29.274411 lamindb_setup-0.71.4/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3542 2024-05-13 09:56:43.703710 lamindb_setup-0.71.4/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      305 2024-04-29 09:50:29.274891 lamindb_setup-0.71.4/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2269 2024-05-13 09:56:45.671582 lamindb_setup-0.71.4/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      532 2024-04-29 09:50:29.276245 lamindb_setup-0.71.4/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    28342 2024-05-06 16:40:35.041470 lamindb_setup-0.71.4/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     3325 2024-05-02 14:13:25.443812 lamindb_setup-0.71.4/noxfile.py
--rw-r--r--   0        0        0     4138 2024-04-29 09:50:29.278441 lamindb_setup-0.71.4/pyproject.toml
--rw-r--r--   0        0        0     5387 2024-05-07 15:02:32.277415 lamindb_setup-0.71.4/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      270 2024-05-03 10:21:42.524497 lamindb_setup-0.71.4/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     5716 2024-05-03 10:21:42.524786 lamindb_setup-0.71.4/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      538 2024-04-29 09:50:29.279431 lamindb_setup-0.71.4/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      504 2024-04-29 09:50:29.279656 lamindb_setup-0.71.4/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      482 2024-05-03 10:21:42.525026 lamindb_setup-0.71.4/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      595 2024-05-07 15:02:32.277929 lamindb_setup-0.71.4/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11234 2024-05-07 15:02:32.278778 lamindb_setup-0.71.4/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      772 2024-05-09 13:59:53.556852 lamindb_setup-0.71.4/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      401 2024-04-29 09:50:29.281008 lamindb_setup-0.71.4/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      193 2024-04-29 09:50:29.281261 lamindb_setup-0.71.4/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1469 2024-04-29 09:50:29.281514 lamindb_setup-0.71.4/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0     1109 2024-04-29 09:50:29.281652 lamindb_setup-0.71.4/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1642 2024-04-29 09:50:29.281814 lamindb_setup-0.71.4/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     2023 2024-04-29 09:50:29.281965 lamindb_setup-0.71.4/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      891 2024-05-05 15:00:22.453756 lamindb_setup-0.71.4/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      878 2024-04-29 09:50:29.283900 lamindb_setup-0.71.4/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1058 2024-04-29 09:50:29.283991 lamindb_setup-0.71.4/tests/storage/test_to_url.py
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.71.4/PKG-INFO
+-rw-r--r--   0        0        0     8499 2024-05-10 21:24:49.730141 lamindb_setup-0.72.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-05-10 21:24:49.730245 lamindb_setup-0.72.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-05-10 21:24:49.730323 lamindb_setup-0.72.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-05-10 21:24:49.730400 lamindb_setup-0.72.0/.gitignore
+-rw-r--r--   0        0        0     1474 2024-05-10 21:24:49.730816 lamindb_setup-0.72.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-05-10 21:24:49.730899 lamindb_setup-0.72.0/LICENSE
+-rw-r--r--   0        0        0      265 2024-05-10 21:24:49.730963 lamindb_setup-0.72.0/README.md
+-rw-r--r--   0        0        0   101693 2024-05-19 16:54:54.607099 lamindb_setup-0.72.0/docs/changelog.md
+-rw-r--r--   0        0        0     2574 2024-05-10 21:24:49.732231 lamindb_setup-0.72.0/docs/hub-cloud/01-init-local-instance.ipynb
+-rw-r--r--   0        0        0     3948 2024-05-10 21:24:49.732413 lamindb_setup-0.72.0/docs/hub-cloud/02-connect-local-instance.ipynb
+-rw-r--r--   0        0        0    10851 2024-05-10 21:27:09.131102 lamindb_setup-0.72.0/docs/hub-cloud/03-add-managed-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-05-10 21:24:49.732848 lamindb_setup-0.72.0/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3202 2024-05-19 16:54:54.607860 lamindb_setup-0.72.0/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3886 2024-05-10 21:24:49.733461 lamindb_setup-0.72.0/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     5454 2024-05-10 21:24:49.733811 lamindb_setup-0.72.0/docs/hub-cloud/07-keep-artifacts-local.ipynb
+-rw-r--r--   0        0        0     3160 2024-05-10 21:24:49.734110 lamindb_setup-0.72.0/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      177 2024-05-10 21:24:49.734470 lamindb_setup-0.72.0/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-05-10 21:24:49.735076 lamindb_setup-0.72.0/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-05-10 21:24:49.735685 lamindb_setup-0.72.0/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-05-10 21:24:49.736223 lamindb_setup-0.72.0/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2712 2024-05-10 21:24:49.736468 lamindb_setup-0.72.0/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-05-10 21:24:49.736795 lamindb_setup-0.72.0/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-05-10 21:24:49.737035 lamindb_setup-0.72.0/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-05-10 21:24:49.737170 lamindb_setup-0.72.0/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6182 2024-05-10 21:24:49.737508 lamindb_setup-0.72.0/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      177 2024-05-10 21:24:49.737594 lamindb_setup-0.72.0/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-05-10 21:24:49.737664 lamindb_setup-0.72.0/docs/index.md
+-rw-r--r--   0        0        0      513 2024-05-10 21:24:49.737976 lamindb_setup-0.72.0/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-05-10 21:24:49.738046 lamindb_setup-0.72.0/docs/reference.md
+-rw-r--r--   0        0        0     1542 2024-05-19 16:55:21.066045 lamindb_setup-0.72.0/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0      846 2024-05-10 21:24:49.738940 lamindb_setup-0.72.0/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0      129 2024-05-10 21:24:49.739174 lamindb_setup-0.72.0/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2613 2024-05-10 21:24:49.739337 lamindb_setup-0.72.0/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1186 2024-05-10 21:24:49.739588 lamindb_setup-0.72.0/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    12728 2024-05-10 21:27:09.131888 lamindb_setup-0.72.0/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     5524 2024-05-19 16:54:54.608343 lamindb_setup-0.72.0/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1534 2024-05-10 21:24:49.740572 lamindb_setup-0.72.0/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2120 2024-05-10 21:24:49.740766 lamindb_setup-0.72.0/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1874 2024-05-10 21:24:49.741154 lamindb_setup-0.72.0/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11897 2024-05-10 21:27:09.133186 lamindb_setup-0.72.0/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8815 2024-05-10 21:24:49.741821 lamindb_setup-0.72.0/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      940 2024-05-10 21:24:49.742316 lamindb_setup-0.72.0/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      679 2024-05-10 21:24:49.742498 lamindb_setup-0.72.0/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1419 2024-05-10 21:27:09.133733 lamindb_setup-0.72.0/lamindb_setup/_set_managed_storage.py
+-rw-r--r--   0        0        0     3670 2024-05-10 21:24:49.743106 lamindb_setup-0.72.0/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1568 2024-05-10 21:24:49.743380 lamindb_setup-0.72.0/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      416 2024-05-10 21:24:49.743642 lamindb_setup-0.72.0/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     4749 2024-05-19 16:54:54.608601 lamindb_setup-0.72.0/lamindb_setup/core/_aws_credentials.py
+-rw-r--r--   0        0        0     1799 2024-05-10 21:24:49.743767 lamindb_setup-0.72.0/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2520 2024-05-10 21:24:49.743894 lamindb_setup-0.72.0/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      276 2024-05-10 21:24:49.744017 lamindb_setup-0.72.0/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5504 2024-05-10 21:24:49.744168 lamindb_setup-0.72.0/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    16447 2024-05-19 16:54:54.608919 lamindb_setup-0.72.0/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4859 2024-05-10 21:24:49.745092 lamindb_setup-0.72.0/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1875 2024-05-10 21:24:49.745226 lamindb_setup-0.72.0/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3141 2024-05-10 21:24:49.745514 lamindb_setup-0.72.0/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    16612 2024-05-16 15:52:55.373201 lamindb_setup-0.72.0/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3922 2024-05-10 21:24:49.746016 lamindb_setup-0.72.0/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2704 2024-05-10 21:24:49.746338 lamindb_setup-0.72.0/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    13236 2024-05-19 16:54:54.609402 lamindb_setup-0.72.0/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     2084 2024-05-10 21:24:49.747202 lamindb_setup-0.72.0/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1344 2024-05-10 21:24:49.747359 lamindb_setup-0.72.0/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     3002 2024-05-10 21:24:49.747517 lamindb_setup-0.72.0/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6893 2024-05-10 21:24:49.747774 lamindb_setup-0.72.0/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3542 2024-05-16 15:52:55.373912 lamindb_setup-0.72.0/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      305 2024-05-10 21:24:49.748488 lamindb_setup-0.72.0/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2269 2024-05-16 15:52:55.374538 lamindb_setup-0.72.0/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      532 2024-05-10 21:24:49.749051 lamindb_setup-0.72.0/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    26339 2024-05-19 16:54:54.609931 lamindb_setup-0.72.0/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     3325 2024-05-10 21:24:49.749714 lamindb_setup-0.72.0/noxfile.py
+-rw-r--r--   0        0        0     4138 2024-05-10 21:24:49.750224 lamindb_setup-0.72.0/pyproject.toml
+-rw-r--r--   0        0        0     5387 2024-05-10 21:24:49.750488 lamindb_setup-0.72.0/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      270 2024-05-10 21:24:49.751063 lamindb_setup-0.72.0/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     5716 2024-05-10 21:24:49.751513 lamindb_setup-0.72.0/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      538 2024-05-10 21:24:49.751867 lamindb_setup-0.72.0/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      504 2024-05-10 21:24:49.752008 lamindb_setup-0.72.0/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      482 2024-05-10 21:24:49.752363 lamindb_setup-0.72.0/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      595 2024-05-10 21:24:49.752562 lamindb_setup-0.72.0/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11234 2024-05-10 21:24:49.752730 lamindb_setup-0.72.0/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      772 2024-05-10 21:27:09.135946 lamindb_setup-0.72.0/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      401 2024-05-10 21:24:49.753243 lamindb_setup-0.72.0/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      193 2024-05-10 21:24:49.753482 lamindb_setup-0.72.0/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1469 2024-05-10 21:24:49.753625 lamindb_setup-0.72.0/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0     1109 2024-05-10 21:24:49.754187 lamindb_setup-0.72.0/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1642 2024-05-10 21:24:49.754795 lamindb_setup-0.72.0/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     2023 2024-05-10 21:24:49.755035 lamindb_setup-0.72.0/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      891 2024-05-10 21:24:49.755350 lamindb_setup-0.72.0/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      878 2024-05-10 21:24:49.755587 lamindb_setup-0.72.0/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1058 2024-05-10 21:24:49.755741 lamindb_setup-0.72.0/tests/storage/test_to_url.py
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.72.0/PKG-INFO
```

### Comparing `lamindb_setup-0.71.4/.github/workflows/build.yml` & `lamindb_setup-0.72.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/.github/workflows/latest-changes.yml` & `lamindb_setup-0.72.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/.gitignore` & `lamindb_setup-0.72.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/.pre-commit-config.yaml` & `lamindb_setup-0.72.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/LICENSE` & `lamindb_setup-0.72.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/changelog.md` & `lamindb_setup-0.72.0/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Check empty after storage record root init in delete | [763](https://github.com/laminlabs/lamindb-setup/pull/763) | [Koncopd](https://github.com/Koncopd) | 2024-05-18 |
+✨ Call `access_aws` for all paths and cache | [762](https://github.com/laminlabs/lamindb-setup/pull/762) | [Koncopd](https://github.com/Koncopd) | 2024-05-18 |
 ⚡️ Speed-up file hash | [761](https://github.com/laminlabs/lamindb-setup/pull/761) | [Koncopd](https://github.com/Koncopd) | 2024-05-11 | 0.71.4
 ♻️ Account for public storage locations | [758](https://github.com/laminlabs/lamindb-setup/pull/758) | [falexwolf](https://github.com/falexwolf) | 2024-05-10 |
 ♻️ Make init_instance_hub idempotent | [757](https://github.com/laminlabs/lamindb-setup/pull/757) | [falexwolf](https://github.com/falexwolf) | 2024-05-09 |
 ♻️ Refactor delete & connect | [756](https://github.com/laminlabs/lamindb-setup/pull/756) | [falexwolf](https://github.com/falexwolf) | 2024-05-09 |
 🔥 Remove laminapp-admin logic | [755](https://github.com/laminlabs/lamindb-setup/pull/755) | [falexwolf](https://github.com/falexwolf) | 2024-05-08 |
 ♻️ Better treatment of current_user_id | [754](https://github.com/laminlabs/lamindb-setup/pull/754) | [falexwolf](https://github.com/falexwolf) | 2024-05-06 | 0.71.2
 💚 Fix tests | [753](https://github.com/laminlabs/lamindb-setup/pull/753) | [fredericenard](https://github.com/fredericenard) | 2024-05-06 |
```

### Comparing `lamindb_setup-0.71.4/docs/hub-cloud/01-init-local-instance.ipynb` & `lamindb_setup-0.72.0/docs/hub-cloud/01-init-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-cloud/02-connect-local-instance.ipynb` & `lamindb_setup-0.72.0/docs/hub-cloud/02-connect-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-cloud/03-add-managed-storage.ipynb` & `lamindb_setup-0.72.0/docs/hub-cloud/03-add-managed-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.72.0/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.72.0/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986111111111111%*

 * *Differences: {"'cells'": "{6: {'source': ['from lamindb_setup.core._aws_credentials import HOSTED_BUCKETS']}}"}*

```diff
@@ -77,15 +77,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lamindb_setup.core.upath import HOSTED_BUCKETS"
+                "from lamindb_setup.core._aws_credentials import HOSTED_BUCKETS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `lamindb_setup-0.71.4/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.72.0/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-cloud/07-keep-artifacts-local.ipynb` & `lamindb_setup-0.72.0/docs/hub-cloud/07-keep-artifacts-local.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.72.0/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.72.0/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.72.0/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.72.0/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.72.0/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.72.0/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.72.0/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.72.0/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.72.0/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/docs/notebooks.md` & `lamindb_setup-0.72.0/docs/notebooks.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/__init__.py` & `lamindb_setup-0.72.0/lamindb_setup/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.71.4"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.72.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._check_setup import _check_instance_setup
 from ._close import close
```

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_cache.py` & `lamindb_setup-0.72.0/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_check_setup.py` & `lamindb_setup-0.72.0/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_close.py` & `lamindb_setup-0.72.0/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.72.0/lamindb_setup/_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_delete.py` & `lamindb_setup-0.72.0/lamindb_setup/_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import shutil
 from typing import TYPE_CHECKING
 from uuid import UUID
 
 from lamin_utils import logger
 
 from ._connect_instance import _connect_instance, get_owner_name_from_identifier
+from .core._aws_credentials import HOSTED_BUCKETS
 from .core._hub_core import delete_instance as delete_instance_on_hub
 from .core._hub_core import get_storage_records_for_instance
 from .core._settings import settings
 from .core._settings_storage import StorageSettings
-from .core.upath import HOSTED_BUCKETS, check_storage_is_empty
+from .core.upath import check_storage_is_empty
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from .core._settings_instance import InstanceSettings
 
 
@@ -105,19 +106,19 @@
         )
     # now everything that's on the hub
     if settings.user.handle != "anonymous":
         storage_records = get_storage_records_for_instance(isettings._id)
         for storage_record in storage_records:
             if storage_record["root"] == isettings.storage.root_as_str:
                 continue
+            ssettings = StorageSettings(storage_record["root"])  # type: ignore
             check_storage_is_empty(
-                storage_record["root"],  # type: ignore
+                ssettings.root,  # type: ignore
                 raise_error=require_empty,
             )
-            ssettings = StorageSettings(storage_record["root"])  # type: ignore
             if ssettings._mark_storage_root.exists():
                 ssettings._mark_storage_root.unlink(
                     missing_ok=True  # this is totally weird, but needed on Py3.11
                 )
     logger.info(f"deleting instance {isettings.slug}")
     # below we can skip check_storage_is_empty() because we already called
     # it above
```

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_django.py` & `lamindb_setup-0.72.0/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_exportdb.py` & `lamindb_setup-0.72.0/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_importdb.py` & `lamindb_setup-0.72.0/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_init_instance.py` & `lamindb_setup-0.72.0/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_migrate.py` & `lamindb_setup-0.72.0/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_register_instance.py` & `lamindb_setup-0.72.0/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_schema.py` & `lamindb_setup-0.72.0/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_set_managed_storage.py` & `lamindb_setup-0.72.0/lamindb_setup/_set_managed_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_setup_user.py` & `lamindb_setup-0.72.0/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.72.0/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_hub_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,43 +349,51 @@
             port=instance["db_port"],
             database=instance["db_database"],
         )
         instance["db"] = db_dsn
     return instance, storage
 
 
-def access_aws(storage_root: str, access_token: str | None = None) -> dict[str, str]:
+def access_aws(storage_root: str, access_token: str | None = None) -> dict[str, dict]:
     from ._settings import settings
 
     if settings.user.handle != "anonymous" or access_token is not None:
-        credentials = call_with_fallback_auth(
+        storage_root_info = call_with_fallback_auth(
             _access_aws, storage_root=storage_root, access_token=access_token
         )
-        return credentials
+        return storage_root_info
     else:
         raise RuntimeError("Can only get access to AWS if authenticated.")
 
 
-def _access_aws(*, storage_root: str, client: Client) -> dict[str, str]:
+def _access_aws(*, storage_root: str, client: Client) -> dict[str, dict]:
     import lamindb_setup
 
+    storage_root_info: dict[str, dict] = {"credentials": {}, "accessibility": {}}
     response = client.functions.invoke(
         "access-aws",
         invoke_options={"body": {"storage_root": storage_root}},
     )
     if response is not None and response != b"{}":
-        loaded_credentials = json.loads(response)["Credentials"]
-        credentials = {}
+        data = json.loads(response)
+
+        loaded_credentials = data["Credentials"]
+        loaded_accessibility = data["StorageAccessibility"]
+
+        credentials = storage_root_info["credentials"]
         credentials["key"] = loaded_credentials["AccessKeyId"]
         credentials["secret"] = loaded_credentials["SecretAccessKey"]
         credentials["token"] = loaded_credentials["SessionToken"]
-        return credentials
+
+        accessibility = storage_root_info["accessibility"]
+        accessibility["storage_root"] = loaded_accessibility["storageRoot"]
+        accessibility["is_managed"] = loaded_accessibility["isManaged"]
     elif lamindb_setup._TESTING:
         raise RuntimeError(f"access-aws errored: {response}")
-    return {}
+    return storage_root_info
 
 
 def get_lamin_site_base_url():
     if "LAMIN_ENV" in os.environ:
         if os.environ["LAMIN_ENV"] == "local":
             return "http://localhost:3000"
         elif os.environ["LAMIN_ENV"] == "staging":
```

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_settings.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_settings_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -363,25 +363,33 @@
                 return False
         # returns True for cloud SQLite
         # and remote postgres
         return True
 
     @property
     def is_on_hub(self) -> bool:
-        """Is this instance on the hub.
+        """Is this instance on the hub?
 
-        Only works if user has access to the instance.
+        Can only reliably establish if user has access to the instance. Will
+        return `False` in case the instance isn't found.
         """
         if self._is_on_hub is None:
             from ._hub_client import call_with_fallback_auth
             from ._hub_crud import select_instance_by_id
+            from ._settings import settings
 
-            response = call_with_fallback_auth(
-                select_instance_by_id, instance_id=self._id.hex
-            )
+            if settings.user.handle != "anonymous":
+                response = call_with_fallback_auth(
+                    select_instance_by_id, instance_id=self._id.hex
+                )
+            else:
+                response = call_with_fallback(
+                    select_instance_by_id, instance_id=self._id.hex
+                )
+                logger.warning("calling anonymously, will miss private instances")
             if response is None:
                 self._is_on_hub = False
             else:
                 self._is_on_hub = True
         return self._is_on_hub
 
     def _get_settings_file(self) -> Path:
```

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_settings_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import string
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal, Optional, Union
 
 from appdirs import AppDirs
 from lamin_utils import logger
 
+from ._aws_credentials import HOSTED_REGIONS, get_aws_credentials_manager
 from ._aws_storage import find_closest_aws_region
 from ._settings_save import save_system_storage_settings
 from ._settings_store import system_storage_settings_file
 from .upath import (
-    HOSTED_REGIONS,
     LocalPathClasses,
     UPath,
     convert_pathlike,
     create_path,
 )
 
 if TYPE_CHECKING:
@@ -147,14 +147,15 @@
     def __init__(
         self,
         root: UPathStr,
         region: str | None = None,
         uid: str | None = None,
         uuid: UUID | None = None,
         instance_id: UUID | None = None,
+        # note that passing access_token prevents credentials caching
         access_token: str | None = None,
     ):
         self._uid = uid
         self._uuid_ = uuid
         self._root_init = convert_pathlike(root)
         if isinstance(self._root_init, LocalPathClasses):  # local paths
             try:
@@ -231,14 +232,20 @@
 
     @property
     def root(self) -> UPath:
         """Root storage location."""
         if self._root is None:
             # below makes network requests to get credentials
             self._root = create_path(self._root_init, access_token=self.access_token)
+        elif getattr(self._root, "protocol", "") == "s3":
+            # this is needed to be sure that the root always has nonexpired credentials
+            # this just checks for time of the cached credentials in most cases
+            return get_aws_credentials_manager().enrich_path(
+                self._root, access_token=self.access_token
+            )
         return self._root
 
     def _set_fs_kwargs(self, **kwargs):
         """Set additional fsspec arguments for cloud root.
 
         Example:
```

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.72.0/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.72.0/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/django.py` & `lamindb_setup-0.72.0/lamindb_setup/core/django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/hashing.py` & `lamindb_setup-0.72.0/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/types.py` & `lamindb_setup-0.72.0/lamindb_setup/core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/lamindb_setup/core/upath.py` & `lamindb_setup-0.72.0/lamindb_setup/core/upath.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from collections import defaultdict
 from datetime import datetime, timezone
 from functools import partial
 from itertools import islice
 from pathlib import Path, PurePosixPath
 from typing import TYPE_CHECKING, Any, Literal
 
-import botocore.session
 import fsspec
 from lamin_utils import logger
 from upath import UPath
 from upath.implementations.cloud import CloudPath, S3Path  # keep CloudPath!
 from upath.implementations.local import LocalPath, PosixUPath, WindowsUPath
 
+from ._aws_credentials import HOSTED_BUCKETS, get_aws_credentials_manager
 from .hashing import b16_to_b64, hash_md5s_from_dir
 
 if TYPE_CHECKING:
     from .types import UPathStr
 
 LocalPathClasses = (PosixUPath, WindowsUPath, LocalPath)
 
@@ -154,15 +154,16 @@
         )
 
 
 def print_hook(size: int, value: int, objectname: str, action: str):
     progress_in_percent = (value / size) * 100
     out = f"... {action} {objectname}:" f" {min(progress_in_percent, 100):4.1f}%"
     if "NBPRJ_TEST_NBPATH" not in os.environ:
-        print(out, end="\r")
+        end = "\n" if progress_in_percent >= 100 else "\r"
+        print(out, end=end)
 
 
 class ProgressCallback(fsspec.callbacks.Callback):
     def __init__(
         self,
         objectname: str,
         action: Literal["uploading", "downloading", "synchronizing"],
@@ -666,85 +667,20 @@
         raise ValueError("pathlike should be of type UPathStr")
     # remove trailing slash
     if path._parts and path._parts[-1] == "":
         path._parts = path._parts[:-1]
     return path
 
 
-HOSTED_REGIONS = [
-    "eu-central-1",
-    "eu-west-2",
-    "us-east-1",
-    "us-east-2",
-    "us-west-1",
-    "us-west-2",
-]
-lamin_env = os.getenv("LAMIN_ENV")
-if lamin_env is None or lamin_env == "prod":
-    hosted_buckets_list = [f"s3://lamin-{region}" for region in HOSTED_REGIONS]
-    hosted_buckets_list.append("s3://scverse-spatial-eu-central-1")
-    HOSTED_BUCKETS = tuple(hosted_buckets_list)
-else:
-    HOSTED_BUCKETS = ("s3://lamin-hosted-test",)  # type: ignore
-credentials_cache: dict[str, dict[str, str]] = {}
-AWS_CREDENTIALS_PRESENT = None
-
-
 def create_path(path: UPath, access_token: str | None = None) -> UPath:
     path = convert_pathlike(path)
     # test whether we have an AWS S3 path
     if not isinstance(path, S3Path):
         return path
-    # test whether AWS credentials are present
-    global AWS_CREDENTIALS_PRESENT
-
-    if AWS_CREDENTIALS_PRESENT is not None:
-        anon = AWS_CREDENTIALS_PRESENT
-    else:
-        if path.fs.key is not None and path.fs.secret is not None:
-            anon = False
-        else:
-            # we could do path.fs.connect()
-            # and check path.fs.session._credentials, but it'd be slower
-            session = botocore.session.get_session()
-            credentials = session.get_credentials()
-            if credentials is None or credentials.access_key is None:
-                anon = True
-            else:
-                anon = False
-            # cache credentials and reuse further
-            AWS_CREDENTIALS_PRESENT = anon
-
-    # test whether we are on hosted storage or not
-    path_str = path.as_posix()
-    is_hosted_storage = path_str.startswith(HOSTED_BUCKETS)
-
-    if not is_hosted_storage:
-        # make anon request if no credentials present
-        return UPath(path, cache_regions=True, anon=anon)
-
-    root_folder = "/".join(path_str.replace("s3://", "").split("/")[:2])
-
-    if access_token is None and root_folder in credentials_cache:
-        credentials = credentials_cache[root_folder]
-    else:
-        from ._hub_core import access_aws
-
-        credentials = access_aws(
-            storage_root=f"s3://{root_folder}", access_token=access_token
-        )
-        if access_token is None:
-            credentials_cache[root_folder] = credentials
-
-    return UPath(
-        path,
-        key=credentials["key"],
-        secret=credentials["secret"],
-        token=credentials["token"],
-    )
+    return get_aws_credentials_manager().enrich_path(path, access_token)
 
 
 def get_stat_file_cloud(stat: dict) -> tuple[int, str, str]:
     size = stat["size"]
     # small files
     if "-" not in stat["ETag"]:
         # only store hash for non-multipart uploads
```

### Comparing `lamindb_setup-0.71.4/noxfile.py` & `lamindb_setup-0.72.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/pyproject.toml` & `lamindb_setup-0.72.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.72.0/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.72.0/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/hub-cloud/test_login.py` & `lamindb_setup-0.72.0/tests/hub-cloud/test_login.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/hub-local/conftest.py` & `lamindb_setup-0.72.0/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/hub-local/test_all.py` & `lamindb_setup-0.72.0/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/hub-prod/conftest.py` & `lamindb_setup-0.72.0/tests/hub-prod/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.72.0/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/hub-prod/test_upath.py` & `lamindb_setup-0.72.0/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/storage/test_hashing.py` & `lamindb_setup-0.72.0/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/storage/test_storage_access.py` & `lamindb_setup-0.72.0/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/storage/test_storage_basis.py` & `lamindb_setup-0.72.0/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/storage/test_storage_stats.py` & `lamindb_setup-0.72.0/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/tests/storage/test_to_url.py` & `lamindb_setup-0.72.0/tests/storage/test_to_url.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.4/PKG-INFO` & `lamindb_setup-0.72.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.71.4
+Version: 0.72.0
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

