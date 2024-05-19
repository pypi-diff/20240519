# Comparing `tmp/sageworks-0.6.2.tar.gz` & `tmp/sageworks-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.6.2.tar", last modified: Wed May  8 22:04:08 2024, max compression
+gzip compressed data, was "sageworks-0.6.3.tar", last modified: Sun May 19 19:53:07 2024, max compression
```

## Comparing `sageworks-0.6.2.tar` & `sageworks-0.6.3.tar`

### file list

```diff
@@ -1,552 +1,563 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.636184 sageworks-0.6.2/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.528100 sageworks-0.6.2/.github/
--rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.2/.github/dependabot.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.528592 sageworks-0.6.2/.github/workflows/
--rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.2/.github/workflows/deploy-docs.yml
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.2/.github/workflows/python-lint.yml
--rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.6.2/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.2/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.2/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.2/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     4942 2024-05-08 22:04:08.636116 sageworks-0.6.2/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     3519 2024-05-04 22:17:44.000000 sageworks-0.6.2/README.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.2/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.517327 sageworks-0.6.2/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.531045 sageworks-0.6.2/applications/aws_dashboard/
--rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-23 23:37:03.000000 sageworks-0.6.2/applications/aws_dashboard/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/Dockerfile_plugins
--rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.2/applications/aws_dashboard/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.2/applications/aws_dashboard/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.532906 sageworks-0.6.2/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/aws_dashboard/assets/bootstrap_darkly.min.css
--rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/aws_dashboard/assets/default.css
--rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/aws_dashboard/assets/trash.png
--rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.2/applications/aws_dashboard/dashboard
--rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/aws_dashboard/nginx.conf
--rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/open_source_config.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.517255 sageworks-0.6.2/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.533610 sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.534289 sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)     4212 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2458 2024-04-23 23:23:47.000000 sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.534990 sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.535742 sageworks-0.6.2/applications/aws_dashboard/pages/main/
--rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/aws_dashboard/pages/main/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/main/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/main/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.536488 sageworks-0.6.2/applications/aws_dashboard/pages/models/
--rw-r--r--   0 briford    (501) staff       (20)     3954 2024-04-23 23:23:47.000000 sageworks-0.6.2/applications/aws_dashboard/pages/models/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.2/applications/aws_dashboard/pages/models/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2152 2024-04-23 23:23:47.000000 sageworks-0.6.2/applications/aws_dashboard/pages/models/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.537225 sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/page.py
--rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/aws_dashboard/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/aws_dashboard/supervisord.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.517380 sageworks-0.6.2/applications/experiments/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.538591 sageworks-0.6.2/applications/experiments/compound_explorer/
--rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/README.md
--rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/experiments/compound_explorer/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.539051 sageworks-0.6.2/applications/experiments/compound_explorer/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/experiments/compound_explorer/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/experiments/compound_explorer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.539539 sageworks-0.6.2/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/aws_identity_check.py
--rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.539699 sageworks-0.6.2/aws_setup/event_bridge/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/event_bridge/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.540451 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/cdk.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.540696 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/lambda/
--rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
--rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.541943 sageworks-0.6.2/aws_setup/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_core/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.2/aws_setup/sageworks_core/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.542237 sageworks-0.6.2/aws_setup/sageworks_core/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/aws_setup/sageworks_core/sageworks_core/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.542670 sageworks-0.6.2/aws_setup/sageworks_core/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.542868 sageworks-0.6.2/aws_setup/sageworks_core/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.544501 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.544753 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.545006 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.545224 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.546022 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.546272 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-23 23:39:47.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.547574 sageworks-0.6.2/data/
--rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.2/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.2/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.2/data/test_data.json
--rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.2/data/wine_dataset.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.547868 sageworks-0.6.2/docs/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.548467 sageworks-0.6.2/docs/admin/
--rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.2/docs/admin/docker_push.md
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/admin/pypi_release.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.550355 sageworks-0.6.2/docs/api_classes/
--rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/api_classes/data_source.md
--rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/api_classes/endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/api_classes/feature_set.md
--rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.2/docs/api_classes/meta.md
--rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/api_classes/model.md
--rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/api_classes/monitor.md
--rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/api_classes/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.2/docs/api_classes/pipelines.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.551859 sageworks-0.6.2/docs/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/aws_setup/aws_access_management.md
--rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.2/docs/aws_setup/aws_tips_and_tricks.md
--rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/aws_setup/core_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/aws_setup/dashboard_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/aws_setup/full_pipeline.md
--rw-r--r--   0 briford    (501) staff       (20)     3270 2024-05-06 16:57:43.000000 sageworks-0.6.2/docs/aws_setup/sso_setup.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.552279 sageworks-0.6.2/docs/concepts/
--rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/concepts/model_monitoring.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.552525 sageworks-0.6.2/docs/core_classes/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.554329 sageworks-0.6.2/docs/core_classes/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/core_classes/artifacts/artifact.md
--rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/athena_source.md
--rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/core_classes/artifacts/data_source_abstract.md
--rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/endpoint_core.md
--rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/feature_set_core.md
--rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/model_core.md
--rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/monitor_core.md
--rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.556078 sageworks-0.6.2/docs/core_classes/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/data_loaders_heavy.md
--rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/data_loaders_light.md
--rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/core_classes/transforms/data_to_features.md
--rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/features_to_model.md
--rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/model_to_endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/overview.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/core_classes/transforms/pandas_transforms.md
--rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/core_classes/transforms/transform.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.556894 sageworks-0.6.2/docs/enterprise/
--rw-r--r--   0 briford    (501) staff       (20)     4075 2024-04-28 19:13:56.000000 sageworks-0.6.2/docs/enterprise/index.md
--rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.2/docs/enterprise/project_branding.md
--rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.2/docs/enterprise/themes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.557171 sageworks-0.6.2/docs/glue/
--rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/glue/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.562078 sageworks-0.6.2/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)     4380 2024-05-06 15:24:03.000000 sageworks-0.6.2/docs/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.563702 sageworks-0.6.2/docs/misc/
--rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/misc/faq.md
--rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/misc/general_info.md
--rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/misc/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/misc/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.564195 sageworks-0.6.2/docs/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.2/docs/plugins/index.md
--rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.2/docs/plugins/plugin_api_changes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.564437 sageworks-0.6.2/docs/repl/
--rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/repl/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.564851 sageworks-0.6.2/docs/research/
--rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/research/eda.md
--rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/research/htg.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.565175 sageworks-0.6.2/examples/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.565328 sageworks-0.6.2/examples/ag-grid/
--rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/ag-grid/hello_world.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.566570 sageworks-0.6.2/examples/datasource/
--rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/datasource/datasource_from_df.py
--rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/datasource/datasource_from_s3.py
--rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/datasource/datasource_query.py
--rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/datasource/datasource_stats.py
--rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/datasource/datasource_to_featureset.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.567263 sageworks-0.6.2/examples/endpoint/
--rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/endpoint/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/endpoint/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/endpoint/endpoint_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.567758 sageworks-0.6.2/examples/featureset/
--rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/featureset/featureset_eda.py
--rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/featureset/featureset_query.py
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.2/examples/featureset/featureset_to_model.py
--rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/full_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.568596 sageworks-0.6.2/examples/glue/
--rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/glue/glue_hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/glue/glue_hello_world_with_log.py
--rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/glue/glue_load_s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.569305 sageworks-0.6.2/examples/meta/
--rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/meta/meta_list_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/meta/meta_list_models.py
--rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/meta/meta_model_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.570005 sageworks-0.6.2/examples/model/
--rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/model/model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.2/examples/model/model_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.2/examples/model/onboard_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.570653 sageworks-0.6.2/examples/monitor/
--rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/monitor/monitor_setup.py
--rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/monitor/monitor_usage.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.572610 sageworks-0.6.2/examples/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.2/examples/pipelines/abalone_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.2/examples/pipelines/abalone_pipeline_v2.json
--rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.2/examples/pipelines/aqsol_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.2/examples/pipelines/pipeline_details.py
--rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.2/examples/pipelines/pipeline_execute.py
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.2/examples/pipelines/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.520572 sageworks-0.6.2/examples/plugins/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.573726 sageworks-0.6.2/examples/plugins/pages/
--rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.2/examples/plugins/pages/my_plugin_page.py
--rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/pages/plugin_page_1.py
--rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/pages/plugin_page_2.py
--rw-r--r--   0 briford    (501) staff       (20)     4528 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/pages/plugin_page_3.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.574168 sageworks-0.6.2/examples/plugins/views/
--rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/plugins/views/model_plugin_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/plugins/views/my_view_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.574997 sageworks-0.6.2/examples/plugins/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/custom_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/endpoint_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/endpoint_turbo.py
--rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/model_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/model_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.576220 sageworks-0.6.2/examples/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.2/examples/storage/data_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.2/examples/storage/data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/hello_world_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/storage/plugin_page_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.576759 sageworks-0.6.2/examples/storage/sagemaker_pipelines/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/all_steps.py
--rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.520840 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.577671 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-05-06 15:23:23.000000 sageworks-0.6.2/mkdocs.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.578763 sageworks-0.6.2/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.6.2/notebooks/ML_Pipeline_with_SageWorks.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.6.2/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
--rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.6.2/notebooks/Outliers_in_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.586843 sageworks-0.6.2/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-06 16:51:44.000000 sageworks-0.6.2/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.591081 sageworks-0.6.2/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.2/scripts/ag_table_row_selection.py
--rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/athena_ddl_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.2/scripts/copy_data_catalog_db.py
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.2/scripts/create_glue_workflow_with_trigger.py
--rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.2/scripts/delete_redis_keys.py
--rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/glue_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/model_endpoint_sanity_check.py
--rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/onboard_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/onboard_models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.591563 sageworks-0.6.2/scripts/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.2/scripts/storage/dns_data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.2/scripts/storage/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/test_feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)      533 2024-05-08 22:04:08.636497 sageworks-0.6.2/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.6.2/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.521345 sageworks-0.6.2/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.591796 sageworks-0.6.2/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.592790 sageworks-0.6.2/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.594524 sageworks-0.6.2/src/sageworks/algorithms/dataframe/
--rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/aggregation.py
--rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
--rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.521715 sageworks-0.6.2/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.594727 sageworks-0.6.2/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.596238 sageworks-0.6.2/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.596493 sageworks-0.6.2/src/sageworks/algorithms/spark/
--rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/spark/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.597971 sageworks-0.6.2/src/sageworks/algorithms/sql/
--rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/column_stats.py
--rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/correlations.py
--rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/descriptive_stats.py
--rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/outliers.py
--rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/sample_rows.py
--rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/value_counts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.600219 sageworks-0.6.2/src/sageworks/api/
--rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.2/src/sageworks/api/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/api/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/api/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/api/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.2/src/sageworks/api/meta.py
--rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/api/model.py
--rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/api/monitor.py
--rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.2/src/sageworks/api/pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.2/src/sageworks/api/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.600954 sageworks-0.6.2/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)    11203 2024-05-08 21:03:14.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.602245 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.602398 sageworks-0.6.2/src/sageworks/core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.604969 sageworks-0.6.2/src/sageworks/core/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.2/src/sageworks/core/artifacts/artifact.py
--rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/core/artifacts/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/artifacts/data_source_abstract.py
--rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/artifacts/data_source_factory.py
--rw-r--r--   0 briford    (501) staff       (20)    36630 2024-04-21 18:44:59.000000 sageworks-0.6.2/src/sageworks/core/artifacts/endpoint_core.py
--rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.2/src/sageworks/core/artifacts/feature_set_core.py
--rw-r--r--   0 briford    (501) staff       (20)    36993 2024-05-08 21:53:45.000000 sageworks-0.6.2/src/sageworks/core/artifacts/model_core.py
--rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/artifacts/monitor_core.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.605414 sageworks-0.6.2/src/sageworks/core/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.2/src/sageworks/core/pipelines/pipeline_executor.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.605990 sageworks-0.6.2/src/sageworks/core/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.606292 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.606638 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.607550 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.607799 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.607916 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.608024 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.608305 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.608882 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609104 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609204 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609416 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609667 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609830 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609995 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/storage/
--rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.610468 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.610716 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.523780 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.610818 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.610972 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.611216 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.611753 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.612139 sageworks-0.6.2/src/sageworks/core/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.613401 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
--rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.613565 sageworks-0.6.2/src/sageworks/experiments/
--rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/experiments/view_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.613993 sageworks-0.6.2/src/sageworks/repl/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/repl/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.2/src/sageworks/repl/sageworks_shell.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.614506 sageworks-0.6.2/src/sageworks/resources/
--rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.2/src/sageworks/resources/open_source_api.key
--rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/resources/signature_verify_pub.pem
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.621348 sageworks-0.6.2/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/utils/aws_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/chem_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/utils/config_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/dashboard_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/utils/datetime_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/docker_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.2/src/sageworks/utils/ecs_info.py
--rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/endpoint_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/extract_model_artifact.py
--rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/glue_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/license_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/utils/markdown_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.2/src/sageworks/utils/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/utils/plugin_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/repl_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/s3_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/sageworks_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/utils/symbols.py
--rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/test_data_generator.py
--rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.2/src/sageworks/utils/trace_calls.py
--rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.623129 sageworks-0.6.2/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.2/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.2/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/views/endpoint_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/views/model_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.626413 sageworks-0.6.2/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.2/src/sageworks/web_components/component_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/correlation_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/web_components/data_details_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/web_components/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/endpoint_metric_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.628307 sageworks-0.6.2/src/sageworks/web_components/experiments/
--rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/color_maps.py
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/compound_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/dashboard_metric_plots.py
--rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/data_table.py
--rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/outlier_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/plugin_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     8690 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/model_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     7169 2024-04-25 21:53:16.000000 sageworks-0.6.2/src/sageworks/web_components/plugin_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3530 2024-04-25 23:09:25.000000 sageworks-0.6.2/src/sageworks/web_components/plugin_unit_test.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.628708 sageworks-0.6.2/src/sageworks/web_components/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.2/src/sageworks/web_components/plugins/ag_table.py
--rw-r--r--   0 briford    (501) staff       (20)     9653 2024-04-15 13:43:00.000000 sageworks-0.6.2/src/sageworks/web_components/plugins/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2945 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/regression_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.2/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/violin_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.635730 sageworks-0.6.2/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     4942 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)    18783 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/entry_points.txt
--rw-r--r--   0 briford    (501) staff       (20)      408 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.630058 sageworks-0.6.2/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.630962 sageworks-0.6.2/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.2/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.631353 sageworks-0.6.2/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.2/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.2/tests/aws_account/aws_service_broker_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.632561 sageworks-0.6.2/tests/connectors/
--rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.2/tests/create_aqsol_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/create_basic_test_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/create_realtime_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.2/tests/create_training_adjusted_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/create_wine_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/delete_test_artifacts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.632707 sageworks-0.6.2/tests/plugin_tests/
--rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/plugin_tests/crashing_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.633008 sageworks-0.6.2/tests/specific/
--rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/specific/capital_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/specific/deletion_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.634305 sageworks-0.6.2/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     5142 2024-04-20 00:25:37.000000 sageworks-0.6.2/tests/transforms/model_metrics_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.2/tests/transforms/pandas_to_data_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.634987 sageworks-0.6.2/tests/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/web_components/confusion_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/web_components/correlation_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/web_components/plugin_interface_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.6.2/tox.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.635418 sageworks-0.6.2/ui_testing/
--rw-r--r--   0 briford    (501) staff       (20)     4591 2024-05-06 17:49:54.000000 sageworks-0.6.2/ui_testing/table_comparison.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.731150 sageworks-0.6.3/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.622433 sageworks-0.6.3/.github/
+-rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.3/.github/dependabot.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.622911 sageworks-0.6.3/.github/workflows/
+-rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.3/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.3/.github/workflows/python-lint.yml
+-rw-r--r--   0 briford    (501) staff       (20)     2037 2024-05-15 21:28:12.000000 sageworks-0.6.3/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.3/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.3/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.3/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     4933 2024-05-19 19:53:07.731079 sageworks-0.6.3/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     3510 2024-05-09 14:32:45.000000 sageworks-0.6.3/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.3/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.610376 sageworks-0.6.3/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.625182 sageworks-0.6.3/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-23 23:37:03.000000 sageworks-0.6.3/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.3/applications/aws_dashboard/Dockerfile_plugins
+-rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.3/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.3/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.626701 sageworks-0.6.3/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.3/applications/aws_dashboard/assets/bootstrap_darkly.min.css
+-rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.3/applications/aws_dashboard/assets/default.css
+-rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.3/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.3/applications/aws_dashboard/assets/trash.png
+-rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.3/applications/aws_dashboard/dashboard
+-rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.3/applications/aws_dashboard/nginx.conf
+-rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.3/applications/aws_dashboard/open_source_config.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.610306 sageworks-0.6.3/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.627550 sageworks-0.6.3/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.3/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.3/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.3/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.628426 sageworks-0.6.3/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)     4212 2024-04-16 15:58:18.000000 sageworks-0.6.3/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.3/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2458 2024-04-23 23:23:47.000000 sageworks-0.6.3/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.629111 sageworks-0.6.3/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.3/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.3/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.3/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.629403 sageworks-0.6.3/applications/aws_dashboard/pages/license/
+-rw-r--r--   0 briford    (501) staff       (20)     1531 2024-05-19 19:25:10.000000 sageworks-0.6.3/applications/aws_dashboard/pages/license/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.630040 sageworks-0.6.3/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.3/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     3307 2024-05-19 19:21:21.000000 sageworks-0.6.3/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.3/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.630771 sageworks-0.6.3/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     3954 2024-04-23 23:23:47.000000 sageworks-0.6.3/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.3/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2152 2024-04-23 23:23:47.000000 sageworks-0.6.3/applications/aws_dashboard/pages/models/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.631495 sageworks-0.6.3/applications/aws_dashboard/pages/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.3/applications/aws_dashboard/pages/pipelines/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.3/applications/aws_dashboard/pages/pipelines/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.3/applications/aws_dashboard/pages/pipelines/page.py
+-rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-06 16:51:44.000000 sageworks-0.6.3/applications/aws_dashboard/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.3/applications/aws_dashboard/supervisord.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.610429 sageworks-0.6.3/applications/experiments/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.632949 sageworks-0.6.3/applications/experiments/compound_explorer/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.3/applications/experiments/compound_explorer/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.3/applications/experiments/compound_explorer/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.3/applications/experiments/compound_explorer/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.633543 sageworks-0.6.3/applications/experiments/compound_explorer/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.3/applications/experiments/compound_explorer/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.3/applications/experiments/compound_explorer/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.3/applications/experiments/compound_explorer/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.3/applications/experiments/compound_explorer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.3/applications/experiments/compound_explorer/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.634077 sageworks-0.6.3/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.634230 sageworks-0.6.3/aws_setup/event_bridge/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/event_bridge/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.634980 sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/cdk.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.635224 sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/lambda/
+-rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
+-rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.636589 sageworks-0.6.3/aws_setup/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_core/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_core/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_core/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_core/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_core/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.3/aws_setup/sageworks_core/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.636885 sageworks-0.6.3/aws_setup/sageworks_core/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/aws_setup/sageworks_core/sageworks_core/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_core/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.637275 sageworks-0.6.3/aws_setup/sageworks_core/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_core/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.637478 sageworks-0.6.3/aws_setup/sageworks_core/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_core/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.638947 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.639204 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.639593 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.639810 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.640586 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.640845 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-23 23:39:47.000000 sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.642183 sageworks-0.6.3/data/
+-rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.3/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.3/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.3/data/test_data.json
+-rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.3/data/wine_dataset.csv
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.642459 sageworks-0.6.3/docs/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.642966 sageworks-0.6.3/docs/admin/
+-rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.3/docs/admin/docker_push.md
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/admin/pypi_release.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.644934 sageworks-0.6.3/docs/api_classes/
+-rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.3/docs/api_classes/data_source.md
+-rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/api_classes/endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/api_classes/feature_set.md
+-rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.3/docs/api_classes/meta.md
+-rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/api_classes/model.md
+-rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/api_classes/monitor.md
+-rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/api_classes/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.3/docs/api_classes/pipelines.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.646942 sageworks-0.6.3/docs/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/aws_setup/aws_access_management.md
+-rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.3/docs/aws_setup/aws_tips_and_tricks.md
+-rw-r--r--   0 briford    (501) staff       (20)     4210 2024-05-09 14:32:45.000000 sageworks-0.6.3/docs/aws_setup/core_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/aws_setup/dashboard_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     7313 2024-05-15 23:47:50.000000 sageworks-0.6.3/docs/aws_setup/domain_cert_setup.md
+-rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.3/docs/aws_setup/full_pipeline.md
+-rw-r--r--   0 briford    (501) staff       (20)     3438 2024-05-09 14:20:27.000000 sageworks-0.6.3/docs/aws_setup/sso_setup.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.647194 sageworks-0.6.3/docs/concepts/
+-rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.6.3/docs/concepts/model_monitoring.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.647395 sageworks-0.6.3/docs/core_classes/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.648882 sageworks-0.6.3/docs/core_classes/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.3/docs/core_classes/artifacts/artifact.md
+-rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/artifacts/athena_source.md
+-rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.3/docs/core_classes/artifacts/data_source_abstract.md
+-rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/artifacts/endpoint_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/artifacts/feature_set_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/artifacts/model_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/artifacts/monitor_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/artifacts/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.650477 sageworks-0.6.3/docs/core_classes/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/transforms/data_loaders_heavy.md
+-rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/transforms/data_loaders_light.md
+-rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/core_classes/transforms/data_to_features.md
+-rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/transforms/features_to_model.md
+-rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/transforms/model_to_endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/core_classes/transforms/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.3/docs/core_classes/transforms/pandas_transforms.md
+-rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.3/docs/core_classes/transforms/transform.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.651170 sageworks-0.6.3/docs/enterprise/
+-rw-r--r--   0 briford    (501) staff       (20)     4075 2024-04-28 19:13:56.000000 sageworks-0.6.3/docs/enterprise/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.3/docs/enterprise/project_branding.md
+-rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.3/docs/enterprise/themes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.651382 sageworks-0.6.3/docs/getting_started/
+-rw-r--r--   0 briford    (501) staff       (20)     1975 2024-05-09 14:38:45.000000 sageworks-0.6.3/docs/getting_started/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.651614 sageworks-0.6.3/docs/glue/
+-rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/glue/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.660293 sageworks-0.6.3/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.3/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)     3443 2024-05-09 14:20:27.000000 sageworks-0.6.3/docs/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.661943 sageworks-0.6.3/docs/misc/
+-rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/misc/faq.md
+-rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/misc/general_info.md
+-rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/misc/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.3/docs/misc/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.662435 sageworks-0.6.3/docs/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.3/docs/plugins/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.3/docs/plugins/plugin_api_changes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.662663 sageworks-0.6.3/docs/repl/
+-rw-r--r--   0 briford    (501) staff       (20)     2080 2024-05-09 14:40:59.000000 sageworks-0.6.3/docs/repl/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.663140 sageworks-0.6.3/docs/research/
+-rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/research/eda.md
+-rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.3/docs/research/htg.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.663354 sageworks-0.6.3/examples/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.663530 sageworks-0.6.3/examples/ag-grid/
+-rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.3/examples/ag-grid/hello_world.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.664634 sageworks-0.6.3/examples/datasource/
+-rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.3/examples/datasource/datasource_from_df.py
+-rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.3/examples/datasource/datasource_from_s3.py
+-rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.3/examples/datasource/datasource_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.3/examples/datasource/datasource_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.3/examples/datasource/datasource_to_featureset.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.665047 sageworks-0.6.3/examples/endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.3/examples/endpoint/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/endpoint/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.3/examples/endpoint/endpoint_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.665478 sageworks-0.6.3/examples/featureset/
+-rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.3/examples/featureset/featureset_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/featureset/featureset_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.3/examples/featureset/featureset_to_model.py
+-rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/full_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.666241 sageworks-0.6.3/examples/glue/
+-rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.3/examples/glue/glue_hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.3/examples/glue/glue_hello_world_with_log.py
+-rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.3/examples/glue/glue_load_s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.666787 sageworks-0.6.3/examples/meta/
+-rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.3/examples/meta/meta_list_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.3/examples/meta/meta_list_models.py
+-rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.3/examples/meta/meta_model_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.667368 sageworks-0.6.3/examples/model/
+-rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/model/model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.3/examples/model/model_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.3/examples/model/onboard_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.667742 sageworks-0.6.3/examples/monitor/
+-rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.3/examples/monitor/monitor_setup.py
+-rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.3/examples/monitor/monitor_usage.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.669267 sageworks-0.6.3/examples/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.3/examples/pipelines/abalone_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.3/examples/pipelines/abalone_pipeline_v2.json
+-rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.3/examples/pipelines/aqsol_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.3/examples/pipelines/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.3/examples/pipelines/pipeline_execute.py
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.3/examples/pipelines/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.614477 sageworks-0.6.3/examples/plugins/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.670175 sageworks-0.6.3/examples/plugins/pages/
+-rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.3/examples/plugins/pages/my_plugin_page.py
+-rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/plugins/pages/plugin_page_1.py
+-rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/plugins/pages/plugin_page_2.py
+-rw-r--r--   0 briford    (501) staff       (20)     4528 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/plugins/pages/plugin_page_3.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.670563 sageworks-0.6.3/examples/plugins/views/
+-rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.3/examples/plugins/views/model_plugin_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.3/examples/plugins/views/my_view_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.671300 sageworks-0.6.3/examples/plugins/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/plugins/web_components/custom_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/plugins/web_components/endpoint_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/plugins/web_components/endpoint_turbo.py
+-rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/plugins/web_components/model_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/plugins/web_components/model_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.672596 sageworks-0.6.3/examples/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.3/examples/storage/data_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.3/examples/storage/data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/hello_world_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.3/examples/storage/plugin_page_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.673199 sageworks-0.6.3/examples/storage/sagemaker_pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/sagemaker_pipelines/all_steps.py
+-rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/sagemaker_pipelines/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/sagemaker_pipelines/ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.614777 sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.673937 sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     3117 2024-05-15 16:07:08.000000 sageworks-0.6.3/mkdocs.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.674966 sageworks-0.6.3/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.6.3/notebooks/ML_Pipeline_with_SageWorks.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.6.3/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.6.3/notebooks/Outliers_in_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.679570 sageworks-0.6.3/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.3/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.3/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.3/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.3/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.3/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.3/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-06 16:51:44.000000 sageworks-0.6.3/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.682119 sageworks-0.6.3/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.3/scripts/ag_table_row_selection.py
+-rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.3/scripts/athena_ddl_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.3/scripts/copy_data_catalog_db.py
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.3/scripts/create_glue_workflow_with_trigger.py
+-rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.3/scripts/delete_redis_keys.py
+-rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.3/scripts/glue_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.3/scripts/model_endpoint_sanity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.3/scripts/onboard_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.3/scripts/onboard_models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.682455 sageworks-0.6.3/scripts/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.3/scripts/storage/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.3/scripts/storage/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.3/scripts/test_feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)      533 2024-05-19 19:53:07.731484 sageworks-0.6.3/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.6.3/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.615289 sageworks-0.6.3/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.682686 sageworks-0.6.3/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.683585 sageworks-0.6.3/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.3/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.685208 sageworks-0.6.3/src/sageworks/algorithms/dataframe/
+-rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.3/src/sageworks/algorithms/dataframe/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/dataframe/aggregation.py
+-rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/dataframe/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
+-rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/dataframe/feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/dataframe/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/dataframe/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.615651 sageworks-0.6.3/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.685392 sageworks-0.6.3/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.3/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.685575 sageworks-0.6.3/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.3/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.685774 sageworks-0.6.3/src/sageworks/algorithms/spark/
+-rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.3/src/sageworks/algorithms/spark/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.687355 sageworks-0.6.3/src/sageworks/algorithms/sql/
+-rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.3/src/sageworks/algorithms/sql/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/sql/column_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/sql/correlations.py
+-rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/sql/descriptive_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/sql/outliers.py
+-rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/sql/sample_rows.py
+-rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/algorithms/sql/value_counts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.689558 sageworks-0.6.3/src/sageworks/api/
+-rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.3/src/sageworks/api/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/api/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/api/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/api/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.3/src/sageworks/api/meta.py
+-rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/api/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/api/monitor.py
+-rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.3/src/sageworks/api/pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.3/src/sageworks/api/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.690287 sageworks-0.6.3/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)    11198 2024-05-09 14:32:45.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.691498 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.691640 sageworks-0.6.3/src/sageworks/core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.694154 sageworks-0.6.3/src/sageworks/core/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.3/src/sageworks/core/artifacts/artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/core/artifacts/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/artifacts/data_source_abstract.py
+-rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/artifacts/data_source_factory.py
+-rw-r--r--   0 briford    (501) staff       (20)    36630 2024-04-21 18:44:59.000000 sageworks-0.6.3/src/sageworks/core/artifacts/endpoint_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.3/src/sageworks/core/artifacts/feature_set_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    37022 2024-05-19 19:25:11.000000 sageworks-0.6.3/src/sageworks/core/artifacts/model_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/artifacts/monitor_core.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.694604 sageworks-0.6.3/src/sageworks/core/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.3/src/sageworks/core/pipelines/pipeline_executor.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.695299 sageworks-0.6.3/src/sageworks/core/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.695637 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.696048 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.696996 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.697204 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.697305 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.697409 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.697707 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.698239 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.698484 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.698582 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.698788 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.699064 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.699235 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.699440 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.699975 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.700222 sageworks-0.6.3/src/sageworks/core/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.617661 sageworks-0.6.3/src/sageworks/core/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.700332 sageworks-0.6.3/src/sageworks/core/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.700512 sageworks-0.6.3/src/sageworks/core/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.700780 sageworks-0.6.3/src/sageworks/core/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.701320 sageworks-0.6.3/src/sageworks/core/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.3/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.701723 sageworks-0.6.3/src/sageworks/core/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/core/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.705763 sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/core/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.705935 sageworks-0.6.3/src/sageworks/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/experiments/view_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.706311 sageworks-0.6.3/src/sageworks/repl/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/repl/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.3/src/sageworks/repl/sageworks_shell.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.706858 sageworks-0.6.3/src/sageworks/resources/
+-rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.3/src/sageworks/resources/open_source_api.key
+-rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/resources/signature_verify_pub.pem
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.715195 sageworks-0.6.3/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.3/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/utils/aws_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/chem_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/utils/config_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/dashboard_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/utils/datetime_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/docker_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.3/src/sageworks/utils/ecs_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/endpoint_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/extract_model_artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/glue_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6396 2024-05-19 19:25:10.000000 sageworks-0.6.3/src/sageworks/utils/license_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/utils/markdown_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.3/src/sageworks/utils/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/utils/plugin_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/repl_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/s3_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/sageworks_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.3/src/sageworks/utils/symbols.py
+-rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/test_data_generator.py
+-rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.3/src/sageworks/utils/trace_calls.py
+-rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.716660 sageworks-0.6.3/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.3/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.3/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/views/endpoint_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.721401 sageworks-0.6.3/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.3/src/sageworks/web_components/component_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/correlation_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/web_components/data_details_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-06 16:51:44.000000 sageworks-0.6.3/src/sageworks/web_components/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/endpoint_metric_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.723072 sageworks-0.6.3/src/sageworks/web_components/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/compound_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/dashboard_metric_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/data_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/outlier_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/plugin_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.3/src/sageworks/web_components/experiments/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     8690 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/model_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     7191 2024-05-19 17:03:46.000000 sageworks-0.6.3/src/sageworks/web_components/plugin_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3530 2024-04-25 23:09:25.000000 sageworks-0.6.3/src/sageworks/web_components/plugin_unit_test.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.723842 sageworks-0.6.3/src/sageworks/web_components/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.3/src/sageworks/web_components/plugins/ag_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     4058 2024-05-19 19:25:10.000000 sageworks-0.6.3/src/sageworks/web_components/plugins/license_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     9653 2024-04-15 13:43:00.000000 sageworks-0.6.3/src/sageworks/web_components/plugins/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2429 2024-04-26 21:22:37.000000 sageworks-0.6.3/src/sageworks/web_components/plugins/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2945 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/regression_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.3/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.3/src/sageworks/web_components/violin_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.730594 sageworks-0.6.3/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     4933 2024-05-19 19:53:07.000000 sageworks-0.6.3/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    19102 2024-05-19 19:53:07.000000 sageworks-0.6.3/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-19 19:53:07.000000 sageworks-0.6.3/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-19 19:53:07.000000 sageworks-0.6.3/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      408 2024-05-19 19:53:07.000000 sageworks-0.6.3/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-19 19:53:07.000000 sageworks-0.6.3/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.725245 sageworks-0.6.3/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.726071 sageworks-0.6.3/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.3/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.726473 sageworks-0.6.3/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.3/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.3/tests/aws_account/aws_service_broker_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.727421 sageworks-0.6.3/tests/connectors/
+-rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/connectors/s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.3/tests/create_aqsol_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/create_basic_test_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/create_realtime_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.3/tests/create_training_adjusted_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/create_wine_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.3/tests/delete_test_artifacts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.727560 sageworks-0.6.3/tests/plugin_tests/
+-rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.3/tests/plugin_tests/crashing_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.727841 sageworks-0.6.3/tests/specific/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/specific/capital_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/specific/deletion_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.729042 sageworks-0.6.3/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     5142 2024-04-20 00:25:37.000000 sageworks-0.6.3/tests/transforms/model_metrics_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.3/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.3/tests/transforms/pandas_to_data_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.729561 sageworks-0.6.3/tests/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.3/tests/web_components/confusion_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.3/tests/web_components/correlation_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.3/tests/web_components/plugin_interface_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.6.3/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.730039 sageworks-0.6.3/ui_testing/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 19:53:07.730159 sageworks-0.6.3/ui_testing/assets/
+-rw-r--r--   0 briford    (501) staff       (20)      597 2024-05-13 15:14:49.000000 sageworks-0.6.3/ui_testing/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)     5770 2024-05-19 19:25:10.000000 sageworks-0.6.3/ui_testing/table_comparison.py
+-rw-r--r--   0 briford    (501) staff       (20)     2025 2024-05-19 19:25:10.000000 sageworks-0.6.3/ui_testing/theme_switching.py
+-rw-r--r--   0 briford    (501) staff       (20)     1819 2024-05-19 19:25:10.000000 sageworks-0.6.3/ui_testing/theme_switching_2.py
```

### Comparing `sageworks-0.6.2/.github/PULL_REQUEST_TEMPLATE.md` & `sageworks-0.6.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/.github/workflows/deploy-docs.yml` & `sageworks-0.6.3/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/.github/workflows/python-lint.yml` & `sageworks-0.6.3/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/.gitignore` & `sageworks-0.6.3/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -135,7 +135,10 @@
 .DS_Store
 
 # Generated Model Harness files
 generated_*.py
 
 # CDK context files (they are account specific, so we don't want them getting checked int)
 cdk.context.json
+
+# CDK Output files
+cdk.out/
```

### Comparing `sageworks-0.6.2/CONTRIBUTING.md` & `sageworks-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/LICENSE` & `sageworks-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/Makefile` & `sageworks-0.6.3/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/PKG-INFO` & `sageworks-0.6.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.2
+Version: 0.6.3
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
@@ -67,15 +67,15 @@
 
 - ```pip install sageworks```  Installs SageWorks
 
 - ```sageworks``` Runs the SageWorks REPL/Initial Setup
 
 For the full instructions for connecting your AWS Account see:
 
-- Initial Setup/Config: [Initial Setup](https://supercowpowers.github.io/sageworks/#initial-setupconfig) 
+- Getting Started: [Initial Setup](https://supercowpowers.github.io/sageworks/getting_started/) 
 - One time AWS Onboarding: [AWS Setup](https://supercowpowers.github.io/sageworks/aws_setup/core_stack/)
 
 
 
 ### SageWorks Documentation
 <img align="right" width="340" alt="sageworks_api" style="padding-left: 10px;"  src="https://github.com/SuperCowPowers/sageworks/assets/4806709/bf0e8591-75d4-44c1-be05-4bfdee4b7186">
```

### Comparing `sageworks-0.6.2/README.md` & `sageworks-0.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 - ```pip install sageworks```  Installs SageWorks
 
 - ```sageworks``` Runs the SageWorks REPL/Initial Setup
 
 For the full instructions for connecting your AWS Account see:
 
-- Initial Setup/Config: [Initial Setup](https://supercowpowers.github.io/sageworks/#initial-setupconfig) 
+- Getting Started: [Initial Setup](https://supercowpowers.github.io/sageworks/getting_started/) 
 - One time AWS Onboarding: [AWS Setup](https://supercowpowers.github.io/sageworks/aws_setup/core_stack/)
 
 
 
 ### SageWorks Documentation
 <img align="right" width="340" alt="sageworks_api" style="padding-left: 10px;"  src="https://github.com/SuperCowPowers/sageworks/assets/4806709/bf0e8591-75d4-44c1-be05-4bfdee4b7186">
```

### Comparing `sageworks-0.6.2/applications/aws_dashboard/Dockerfile` & `sageworks-0.6.3/applications/aws_dashboard/Dockerfile`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/README.md` & `sageworks-0.6.3/applications/aws_dashboard/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/app.py` & `sageworks-0.6.3/applications/aws_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/assets/bootstrap_darkly.min.css` & `sageworks-0.6.3/applications/aws_dashboard/assets/bootstrap_darkly.min.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/assets/default.css` & `sageworks-0.6.3/applications/aws_dashboard/assets/default.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/assets/favicon.ico` & `sageworks-0.6.3/applications/aws_dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/assets/trash.png` & `sageworks-0.6.3/applications/aws_dashboard/assets/trash.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/dashboard` & `sageworks-0.6.3/applications/aws_dashboard/dashboard`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/open_source_config.json` & `sageworks-0.6.3/applications/aws_dashboard/open_source_config.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/callbacks.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/layout.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/page.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/data_sources/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/callbacks.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/layout.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/page.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/callbacks.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/layout.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/page.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/main/callbacks.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/main/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/main/layout.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/main/layout.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,15 +34,23 @@
                                 f" v {sageworks_version}",
                                 style={
                                     "color": "rgb(180, 120, 180)",
                                     "fontSize": 15,
                                 },
                             ),
                             html.Span(
-                                f" ({license_id})",
+                                html.A(
+                                    f" ({license_id})",
+                                    href="/license",
+                                    style={
+                                        "color": "rgb(140, 140, 200)",
+                                        "fontSize": 15,
+                                        "textDecoration": "none",
+                                    },
+                                ),
                                 style={
                                     "color": "rgb(140, 140, 200)",
                                     "fontSize": 15,
                                 },
                             ),
                         ]
                     ),
```

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/main/page.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/main/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/models/callbacks.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/models/layout.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/models/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/models/page.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/models/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/callbacks.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/pipelines/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/layout.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/pipelines/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/page.py` & `sageworks-0.6.3/applications/aws_dashboard/pages/pipelines/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/experiments/compound_explorer/app.py` & `sageworks-0.6.3/applications/experiments/compound_explorer/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/experiments/compound_explorer/assets/custom.css` & `sageworks-0.6.3/applications/experiments/compound_explorer/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/experiments/compound_explorer/callbacks.py` & `sageworks-0.6.3/applications/experiments/compound_explorer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/applications/experiments/compound_explorer/layout.py` & `sageworks-0.6.3/applications/experiments/compound_explorer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/aws_account_check.py` & `sageworks-0.6.3/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/aws_identity_check.py` & `sageworks-0.6.3/aws_setup/aws_identity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/build_ml_pipeline.py` & `sageworks-0.6.3/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/app.py` & `sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/cdk.json` & `sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py` & `sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py` & `sageworks-0.6.3/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_core/README.md` & `sageworks-0.6.3/aws_setup/sageworks_core/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_core/app.py` & `sageworks-0.6.3/aws_setup/sageworks_core/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_core/cdk.json` & `sageworks-0.6.3/aws_setup/sageworks_core/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py` & `sageworks-0.6.3/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.6.3/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/README.md` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_full/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/app.py` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_full/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/cdk.json` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_full/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/README.md` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/app.py` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/cdk.json` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py` & `sageworks-0.6.3/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/data/abalone.csv` & `sageworks-0.6.3/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/data/test_data.csv` & `sageworks-0.6.3/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/data/test_data.json` & `sageworks-0.6.3/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/data/wine_dataset.csv` & `sageworks-0.6.3/data/wine_dataset.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/admin/docker_push.md` & `sageworks-0.6.3/docs/admin/docker_push.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/admin/pypi_release.md` & `sageworks-0.6.3/docs/admin/pypi_release.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/api_classes/data_source.md` & `sageworks-0.6.3/docs/api_classes/data_source.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/api_classes/endpoint.md` & `sageworks-0.6.3/docs/api_classes/endpoint.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/api_classes/feature_set.md` & `sageworks-0.6.3/docs/api_classes/feature_set.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/api_classes/meta.md` & `sageworks-0.6.3/docs/api_classes/meta.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/api_classes/model.md` & `sageworks-0.6.3/docs/api_classes/model.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/api_classes/monitor.md` & `sageworks-0.6.3/docs/api_classes/monitor.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/api_classes/overview.md` & `sageworks-0.6.3/docs/api_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/api_classes/pipelines.md` & `sageworks-0.6.3/docs/api_classes/pipelines.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/aws_setup/aws_access_management.md` & `sageworks-0.6.3/docs/aws_setup/aws_access_management.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/aws_setup/aws_tips_and_tricks.md` & `sageworks-0.6.3/docs/aws_setup/aws_tips_and_tricks.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/aws_setup/core_stack.md` & `sageworks-0.6.3/docs/aws_setup/core_stack.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
   ```
 For more information on Linux installs see [Digital Ocean NodeJS](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-20-04)
 
 ## Create an S3 Bucket for SageWorks
 SageWorks pushes and pulls data from AWS, it will use this S3 Bucket for storage and processing. You should create a **NEW** S3 Bucket, we suggest a name like `<company_name>-sageworks`
 
 ## Deploying the SageWorks Core Stack
-Do the initial setup/config here: [Getting Started: Initial Setup](../index.md#initial-setupconfig). After you've done that come back to this section. For Stack Deployment additional things need to be added to your config file. The config file will be located in your home directory `~/.sageworks/sageworks_config.json`. Edit this file and add addition stuff for the deployment. Specifically there are two additional fields to be added (optional for both)
+Do the initial setup/config here: [Getting Started](../getting_started/index.md). After you've done that come back to this section. For Stack Deployment additional things need to be added to your config file. The config file will be located in your home directory `~/.sageworks/sageworks_config.json`. Edit this file and add addition stuff for the deployment. Specifically there are two additional fields to be added (optional for both)
 
 ```
 "SAGEWORKS_SSO_GROUP": DataScientist (or whatever)
 "SAGEWORKS_ADDITIONAL_BUCKETS": "bucket1, bucket2
 ```
 These are optional but are set/used by most SageWorks users.
```

### Comparing `sageworks-0.6.2/docs/aws_setup/dashboard_stack.md` & `sageworks-0.6.3/docs/aws_setup/dashboard_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/aws_setup/full_pipeline.md` & `sageworks-0.6.3/docs/aws_setup/full_pipeline.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/aws_setup/sso_setup.md` & `sageworks-0.6.3/docs/aws_setup/sso_setup.md`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,17 @@
 ❯ aws s3 ls
 2023-03-20 20:06:53 aws-athena-query-results-XXXYYY-us-west-2
 2023-03-30 13:22:28 sagemaker-studio-XXXYYY-dbgyvq8ruka
 2023-03-24 22:05:55 sagemaker-us-west-2-XXXYYY
 2023-04-30 13:43:29 scp-sageworks-artifacts
 ```
 
+## Back to Initial Setup
+If you're doing the initial setup of SageWorks you should now go back and finish that process: [Getting Started](../getting_started/index.md)
+
  
 ## AWS Resources
 - [AWS Identity Center](https://docs.aws.amazon.com/singlesignon/latest/userguide/what-is.html)
 - [Users and Groups](https://docs.aws.amazon.com/singlesignon/latest/userguide/users-groups-provisioning.html)
 - [Permission Sets](https://docs.aws.amazon.com/singlesignon/latest/userguide/permissionsetsconcept.html)
 - [SSO Command Line/Python Configure](https://docs.aws.amazon.com/cli/latest/userguide/sso-configure-profile-token.html)
```

### Comparing `sageworks-0.6.2/docs/concepts/model_monitoring.md` & `sageworks-0.6.3/docs/concepts/model_monitoring.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/core_classes/artifacts/overview.md` & `sageworks-0.6.3/docs/core_classes/artifacts/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/core_classes/overview.md` & `sageworks-0.6.3/docs/core_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/core_classes/transforms/overview.md` & `sageworks-0.6.3/docs/core_classes/transforms/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/core_classes/transforms/pandas_transforms.md` & `sageworks-0.6.3/docs/core_classes/transforms/pandas_transforms.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/core_classes/transforms/transform.md` & `sageworks-0.6.3/docs/core_classes/transforms/transform.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/enterprise/index.md` & `sageworks-0.6.3/docs/enterprise/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/enterprise/project_branding.md` & `sageworks-0.6.3/docs/enterprise/project_branding.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/enterprise/themes.md` & `sageworks-0.6.3/docs/enterprise/themes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/glue/index.md` & `sageworks-0.6.3/docs/glue/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/big_spider.png` & `sageworks-0.6.3/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/graph_representation.png` & `sageworks-0.6.3/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/powered_aws_dark_blue.png` & `sageworks-0.6.3/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/powered_aws_transparent.png` & `sageworks-0.6.3/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/powered_aws_white.png` & `sageworks-0.6.3/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.6.3/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/sageworks.png` & `sageworks-0.6.3/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/sageworks_concepts.png` & `sageworks-0.6.3/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/scp.png` & `sageworks-0.6.3/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/scp_labs.png` & `sageworks-0.6.3/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/images/small_spider.png` & `sageworks-0.6.3/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/index.md` & `sageworks-0.6.3/docs/misc/general_info.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,70 @@
-# Welcome to SageWorks
-The SageWorks framework makes AWS® both easier to use and more powerful. SageWorks handles all the details around updating and managing a complex set of AWS Services. With a simple-to-use Python API and a beautiful set of web interfaces, SageWorks makes creating AWS ML pipelines a snap. It also dramatically improves both the usability and visibility across the entire spectrum of services: Glue Jobs, Athena, Feature Store, Models, and Endpoints. SageWorks makes it easy to build production ready, AWS powered, machine learning pipelines.
+## General Info
+<p align="center">
+<img width="720" alt="DataSource_EDA" aligh="right" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/a5b063f7-a291-4dba-a766-b2e906920066">
+</p>
 
-<figure style="float: right; width: 500px;">
-<img alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/5f8b32a2-ed72-45f2-bd96-91b7bbbccff4">
-<figcaption>SageWorks Dashboard: AWS Pipelines in a Whole New Light!</figcaption>
-</figure>
-
-### Full AWS OverView
-- Health Monitoring 🟢
-- Dynamic Updates
-- High Level Summary
-
-### Drill-Down Views
-- Glue Jobs
-- DataSources
-- FeatureSets
-- Models
-- Endpoints
+#### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
 
-## Private SaaS Architecture
-**Secure your Data, Empower your ML Pipelines**
+SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
-SageWorks is architected as a Private SaaS. This hybrid architecture is the ultimate solution for businesses that prioritize data control and security. SageWorks deploys as an AWS Stack within your own cloud environment, ensuring compliance with stringent corporate and regulatory standards. It offers the flexibility to tailor solutions to your specific business needs through our comprehensive plugin support, both components and full web interfaces. By using SageWorks, you maintain absolute control over your data while benefiting from the power, security, and scalability of AWS cloud services. [SageWorks Private SaaS Architecture](https://docs.google.com/presentation/d/1f_1gmE4-UAeUDDsoNdzK_d_MxALFXIkxORZwbJBjPq4/edit?usp=sharing)
 
-## Getting Started
 
-The SageWorks package has two main components, a Web Interface that provides visibility into AWS ML PIpelines and a Python API that makes creation and usage of the AWS ML Services easier than using/learning the services directly.
+### SageWorks Documentation
+See our Python API and AWS documentation here: [SageWorks Documentation](https://supercowpowers.github.io/sageworks/)
+
+### Full SageWorks OverView
+[SageWorks Architected FrameWork](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing)
+
+
+## Why SageWorks?
 
-### Web Interfaces
-The SageWorks Dashboard has a set of web interfaces that give visibility into the AWS Glue and SageMaker Services. There are currently 5 web interfaces available:
+- The AWS SageMaker® ecosystem is **awesome** but has a large number of services with significant complexity
+- SageWorks provides **rapid prototyping** through easy to use **classes** and **transforms**
+- SageWorks provides **visibility** and **transparency** into AWS SageMaker® Pipelines
+    - What S3 data sources are getting pulled?
+    - What Features Store/Group is the Model Using?
+    - What's the ***Provenance*** of a Model in Model Registry?
+    - What SageMaker Endpoints are associated with this model?
 
 
-- **Top Level Dashboard:** Shows all AWS ML Artifacts (Glue and SageMaker)
-- **DataSources:** DataSource Column Details, Distributions and Correlations
-- **FeatureSets:** FeatureSet Details, Distributions and Correlations
-- **Model:** Model details, performance metric, and inference plots
-- **Endpoints:** Endpoint details, realtime charts of endpoint performance and latency
+### Single Pane of Glass
+Visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
 
-### Python API
-SageWorks API Documentation: [SageWorks API Classes](api_classes/overview.md) 
+Image TBD
 
-The main functionality of the Python API is to encapsulate and manage a set of AWS services underneath a Python Object interface. The Python Classes are used to create and interact with Machine Learning Pipeline Artifacts.
+<i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
+
+
+## Getting Started
+- [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
+- [SageWorks Docs/Wiki](https://github.com/SuperCowPowers/sageworks/wiki) Our general documentation for getting started with SageWorks.
+- [SageWorks AWS Onboarding](https://github.com/SuperCowPowers/sageworks/wiki/Onboarding-SageWorks-to-AWS) Deploy the SageWorks Stack to your AWS Account. 
+- [Notebook: Start to Finish AWS ML Pipeline](https://nbviewer.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
+- [Video: Coding with SageWorks](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
+- Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
-### Initial Setup/Config
-**Notes:** Use the SageWorks REPL to setup your AWS connection for both API Usage (Data Scientists/Engineers) and AWS Initial Setup (AWS Folks). Also if you don't already have an AWS Profile or SSO Setup you'll need to do that first [Developer SSO Setup](aws_setup/sso_setup.md) 
+### SageWorks Zen
+- The AWS SageMaker® set of services is vast and **complex**.
+- SageWorks Classes encapsulate, organize, and manage sets of AWS® Services.
+- **Heavy** transforms typically use **[AWS Athena](https://aws.amazon.com/athena/)** or **[Apache Spark](https://spark.apache.org/)** (AWS Glue/EMR Serverless).
+- **Light** transforms will typically use **[Pandas](https://pandas.pydata.org/)**.
+- Heavy and Light transforms both update **AWS Artifacts** (collections of AWS Services).
+- **Quick prototypes** are typically built with the **light path** and then flipped to the **heavy path** as the system matures and usage grows.
 
-```
-> pip install sageworks
-> sageworks <-- This starts the REPL
+### Classes and Concepts
+The SageWorks Classes are organized to work in concert with AWS Services. For more details on the current classes and class hierarchies see [SageWorks Classes and Concepts](sageworks_classes_concepts.md).
 
-Welcome to SageWorks!
-Looks like this is your first time using SageWorks...
-Let's get you set up...
-AWS_PROFILE: my_aws_profile
-SAGEWORKS_BUCKET: my-company-sageworks
-[optional] REDIS_HOST(localhost): my-redis.cache.amazon (or leave blank)
-[optional] REDIS_PORT(6379):
-[optional] REDIS_PASSWORD():
-[optional] SAGEWORKS_API_KEY(open_source): my_api_key (or leave blank)
-```
-**That's It:** You're now all set. This configuration only needs to be **ONCE** :)
+### Contributions
+If you'd like to contribute to the SageWorks project, you're more than welcome. All contributions will fall under the existing project [license](https://github.com/SuperCowPowers/sageworks/blob/main/LICENSE). If you are interested in contributing or have questions please feel free to contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
-### AWS Administrators (initial setup)
-Setting up SageWorks on your AWS Account: [AWS Setup](aws_setup/core_stack.md)
 
-### Data Scientists/Engineers
-- SageWorks REPL: [SageWorks REPL](repl/index.md)
-- Using SageWorks for ML Pipelines: [SageWorks API Classes](api_classes/overview.md)
-- SCP SageWorks Github: [Github Repo](https://github.com/SuperCowPowers/sageworks)
+### SageWorks Alpha Testers Wanted
+Our experienced team can provide development and consulting services to help you effectively use Amazon’s Machine Learning services within your organization.
 
+The popularity of cloud based Machine Learning services is booming. The problem many companies face is how that capability gets effectively used and harnessed to drive real business decisions and provide concrete value for their organization.
 
-## Additional Resources
+Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Alpha Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
-<img align="right" src="images/scp.png" width="180">
+® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates.
 
-- SageWorks Core Classes: [Core Classes](core_classes/overview.md)
-- Consulting Available: [SuperCowPowers LLC](https://www.supercowpowers.com)
+Readme change
```

### Comparing `sageworks-0.6.2/docs/misc/faq.md` & `sageworks-0.6.3/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/misc/general_info.md` & `sageworks-0.6.3/src/sageworks.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,93 @@
-## General Info
-<p align="center">
-<img width="720" alt="DataSource_EDA" aligh="right" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/a5b063f7-a291-4dba-a766-b2e906920066">
-</p>
+Metadata-Version: 2.1
+Name: sageworks
+Version: 0.6.3
+Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
+Home-page: https://github.com/SuperCowPowers/sageworks
+Author: SuperCowPowers LLC
+Author-email: support@supercowpowers.com
+License: MIT
+Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: boto3>=1.28.76
+Requires-Dist: botocore>=1.31.76
+Requires-Dist: redis>=5.0.1
+Requires-Dist: numpy>=1.26.1
+Requires-Dist: pandas>=2.1.2
+Requires-Dist: scikit-learn>=1.4.1
+Requires-Dist: awswrangler>=3.4.0
+Requires-Dist: sagemaker>=2.143
+Requires-Dist: plotly>=5.18.0
+Requires-Dist: dash>=2.16.1
+Requires-Dist: dash-bootstrap-components>=1.5.0
+Requires-Dist: dash-bootstrap-templates==1.1.1
+Requires-Dist: tabulate>=0.9.0
+Requires-Dist: shap>=0.43.0
+Requires-Dist: xgboost>=2.0.2
+Requires-Dist: joblib>=1.3.2
+Requires-Dist: cryptography>=42.0.5
+Requires-Dist: rdkit>=2023.9.1
+Requires-Dist: mordred>=1.2.0
+Requires-Dist: ipython>=8.17.2
+Requires-Dist: setuptools>=69.0.2
+Requires-Dist: pyreadline3; sys_platform == "win32"
+
+
+# Welcome to SageWorks
+The SageWorks framework makes AWS® both easier to use and more powerful. SageWorks handles all the details around updating and managing a complex set of AWS Services. With a simple-to-use Python API and a beautiful set of web interfaces, SageWorks makes creating AWS ML pipelines a snap. It also dramatically improves both the usability and visibility across the entire spectrum of services: Glue Job, Athena, Feature Store, Models, and Endpoints, SageWorks makes it easy to build production ready, AWS powered, machine learning pipelines.
+
+<img align="right" width="480" alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/ed2ed1bd-e2d8-49a1-b350-b2e19e2b7832">
+
+### Full AWS ML OverView
+- Health Monitoring 🟢
+- Dynamic Updates
+- High Level Summary
+
+### Drill-Down Views
+- Incoming Data
+- Glue Jobs
+- DataSources
+- FeatureSets
+- Models
+- Endpoints
+
+## Private SaaS Architecture
+*Secure your Data, Empower your ML Pipelines*
+
+SageWorks is architected as a **Private SaaS**. This hybrid architecture is the ultimate solution for businesses that prioritize data control and security. SageWorks deploys as an AWS Stack within your own cloud environment, ensuring compliance with stringent corporate and regulatory standards. It offers the flexibility to tailor solutions to your specific business needs through our comprehensive plugin support, both components and full web interfaces. By using SageWorks, you maintain absolute control over your data while benefiting from the power, security, and scalability of AWS cloud services. [SageWorks Private SaaS Architecture](https://docs.google.com/presentation/d/1f_1gmE4-UAeUDDsoNdzK_d_MxALFXIkxORZwbJBjPq4/edit?usp=sharing)
+
+
+### API Installation
 
-#### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
+- ```pip install sageworks```  Installs SageWorks
 
-SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
+- ```sageworks``` Runs the SageWorks REPL/Initial Setup
 
+For the full instructions for connecting your AWS Account see:
 
+- Getting Started: [Initial Setup](https://supercowpowers.github.io/sageworks/getting_started/) 
+- One time AWS Onboarding: [AWS Setup](https://supercowpowers.github.io/sageworks/aws_setup/core_stack/)
 
-### SageWorks Documentation
-See our Python API and AWS documentation here: [SageWorks Documentation](https://supercowpowers.github.io/sageworks/)
-
-### Full SageWorks OverView
-[SageWorks Architected FrameWork](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing)
-
-
-## Why SageWorks?
-
-- The AWS SageMaker® ecosystem is **awesome** but has a large number of services with significant complexity
-- SageWorks provides **rapid prototyping** through easy to use **classes** and **transforms**
-- SageWorks provides **visibility** and **transparency** into AWS SageMaker® Pipelines
-    - What S3 data sources are getting pulled?
-    - What Features Store/Group is the Model Using?
-    - What's the ***Provenance*** of a Model in Model Registry?
-    - What SageMaker Endpoints are associated with this model?
-
-
-### Single Pane of Glass
-Visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
 
-Image TBD
-
-<i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
+### SageWorks Documentation
+<img align="right" width="340" alt="sageworks_api" style="padding-left: 10px;"  src="https://github.com/SuperCowPowers/sageworks/assets/4806709/bf0e8591-75d4-44c1-be05-4bfdee4b7186">
 
-## Getting Started
-- [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
-- [SageWorks Docs/Wiki](https://github.com/SuperCowPowers/sageworks/wiki) Our general documentation for getting started with SageWorks.
-- [SageWorks AWS Onboarding](https://github.com/SuperCowPowers/sageworks/wiki/Onboarding-SageWorks-to-AWS) Deploy the SageWorks Stack to your AWS Account. 
-- [Notebook: Start to Finish AWS ML Pipeline](https://nbviewer.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
-- [Video: Coding with SageWorks](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
-- Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
+[SageWorks Documentation](https://supercowpowers.github.io/sageworks/): The documentation contains examples from the SageWorks source code in this repository under the `examples/` directory. For a full code listing of any example please visit our [SageWorks Examples](https://github.com/SuperCowPowers/sageworks/blob/main/examples)
 
-### SageWorks Zen
-- The AWS SageMaker® set of services is vast and **complex**.
-- SageWorks Classes encapsulate, organize, and manage sets of AWS® Services.
-- **Heavy** transforms typically use **[AWS Athena](https://aws.amazon.com/athena/)** or **[Apache Spark](https://spark.apache.org/)** (AWS Glue/EMR Serverless).
-- **Light** transforms will typically use **[Pandas](https://pandas.pydata.org/)**.
-- Heavy and Light transforms both update **AWS Artifacts** (collections of AWS Services).
-- **Quick prototypes** are typically built with the **light path** and then flipped to the **heavy path** as the system matures and usage grows.
 
-### Classes and Concepts
-The SageWorks Classes are organized to work in concert with AWS Services. For more details on the current classes and class hierarchies see [SageWorks Classes and Concepts](sageworks_classes_concepts.md).
+### SageWorks Beta Program
+Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Beta Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 ### Contributions
 If you'd like to contribute to the SageWorks project, you're more than welcome. All contributions will fall under the existing project [license](https://github.com/SuperCowPowers/sageworks/blob/main/LICENSE). If you are interested in contributing or have questions please feel free to contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
+<img align="right" src="docs/images/scp.png" width="180">
 
-### SageWorks Alpha Testers Wanted
-Our experienced team can provide development and consulting services to help you effectively use Amazon’s Machine Learning services within your organization.
-
-The popularity of cloud based Machine Learning services is booming. The problem many companies face is how that capability gets effectively used and harnessed to drive real business decisions and provide concrete value for their organization.
-
-Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Alpha Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
-
-® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates.
-
-Readme change
+® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates
```

### Comparing `sageworks-0.6.2/docs/misc/sageworks_classes_concepts.md` & `sageworks-0.6.3/docs/misc/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/misc/scp_consulting.md` & `sageworks-0.6.3/docs/misc/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/plugins/index.md` & `sageworks-0.6.3/docs/plugins/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/plugins/plugin_api_changes.md` & `sageworks-0.6.3/docs/plugins/plugin_api_changes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/repl/index.md` & `sageworks-0.6.3/docs/repl/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 `pip install sageworks`
 
 ### Usage
 Just type `sageworks` at the command line and the SageWorks shell will spin up and provide a command view of your AWS Machine Learning Pipelines.
 
 At startup the SageWorks shell, will connect to your AWS Account and create a summary of the Machine Learning artifacts currently residing on the account.
 
-<img alt="sageworks_repl" style="float: right; width: 500px; padding-left: 5px;"
+<img alt="sageworks_repl" style="float: right; width: 450px; padding-left: 5px;"
 src="https://github.com/SuperCowPowers/sageworks/assets/4806709/10a969ed-3415-4d9f-ad0d-ac23706e6202">
 
 **Available Commands:**
 
 - status
 - config
 - incoming_data
 - glue_jobs
 - data_sources
 - feature_sets
 - models
 - endpoints
-- meta_refresh
+- aws_refresh
 - and more...
 
 
 All of the [API Classes](../api_classes/overview.md) are auto-loaded, so drilling down on an individual artifact is easy. The same Python API is provided so if you want additional info on a **model**, for instance, simply create a model object and use any of the documented API methods.
 
 ```
 m = Model("abalone-regression")
```

### Comparing `sageworks-0.6.2/docs/research/eda.md` & `sageworks-0.6.3/docs/research/eda.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/docs/research/htg.md` & `sageworks-0.6.3/docs/research/htg.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/datasource/datasource_query.py` & `sageworks-0.6.3/examples/datasource/datasource_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/datasource/datasource_stats.py` & `sageworks-0.6.3/examples/datasource/datasource_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/endpoint/endpoint_inference.py` & `sageworks-0.6.3/examples/endpoint/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/featureset/featureset_eda.py` & `sageworks-0.6.3/examples/featureset/featureset_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/featureset/featureset_query.py` & `sageworks-0.6.3/examples/featureset/featureset_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/full_ml_pipeline.py` & `sageworks-0.6.3/examples/full_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/glue/glue_hello_world.py` & `sageworks-0.6.3/examples/glue/glue_hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/glue/glue_hello_world_with_log.py` & `sageworks-0.6.3/examples/glue/glue_hello_world_with_log.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/glue/glue_load_s3_bucket.py` & `sageworks-0.6.3/examples/glue/glue_load_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/meta/meta_model_metrics.py` & `sageworks-0.6.3/examples/meta/meta_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/model/model_metrics.py` & `sageworks-0.6.3/examples/model/model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/model/onboard_model.py` & `sageworks-0.6.3/examples/model/onboard_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/monitor/monitor_usage.py` & `sageworks-0.6.3/examples/monitor/monitor_usage.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/pipelines/abalone_pipeline_v1.json` & `sageworks-0.6.3/examples/pipelines/abalone_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/pipelines/abalone_pipeline_v2.json` & `sageworks-0.6.3/examples/pipelines/abalone_pipeline_v2.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/pipelines/aqsol_pipeline_v1.json` & `sageworks-0.6.3/examples/pipelines/aqsol_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/pipelines/pipeline_manager.py` & `sageworks-0.6.3/examples/pipelines/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/pages/my_plugin_page.py` & `sageworks-0.6.3/examples/plugins/pages/my_plugin_page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/pages/plugin_page_1.py` & `sageworks-0.6.3/examples/plugins/pages/plugin_page_1.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/pages/plugin_page_2.py` & `sageworks-0.6.3/examples/plugins/pages/plugin_page_2.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/pages/plugin_page_3.py` & `sageworks-0.6.3/examples/plugins/pages/plugin_page_3.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/views/model_plugin_view.py` & `sageworks-0.6.3/examples/plugins/views/model_plugin_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/views/my_view_plugin.py` & `sageworks-0.6.3/examples/plugins/views/my_view_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/web_components/custom_plugin.py` & `sageworks-0.6.3/examples/plugins/web_components/custom_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/web_components/endpoint_plugin.py` & `sageworks-0.6.3/examples/plugins/web_components/endpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/web_components/endpoint_turbo.py` & `sageworks-0.6.3/examples/plugins/web_components/endpoint_turbo.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/web_components/model_markdown.py` & `sageworks-0.6.3/examples/plugins/web_components/model_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/plugins/web_components/model_plugin.py` & `sageworks-0.6.3/examples/plugins/web_components/model_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/data_to_data.py` & `sageworks-0.6.3/examples/storage/data_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/data_to_features.py` & `sageworks-0.6.3/examples/storage/data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/endpoint_inference.py` & `sageworks-0.6.3/examples/storage/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/hello_world_pipeline.py` & `sageworks-0.6.3/examples/storage/hello_world_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/plugin_page_example.py` & `sageworks-0.6.3/examples/storage/plugin_page_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/sagemaker_pipelines/all_steps.py` & `sageworks-0.6.3/examples/storage/sagemaker_pipelines/all_steps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/sagemaker_pipelines/ml_pipeline.py` & `sageworks-0.6.3/examples/storage/sagemaker_pipelines/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py` & `sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py` & `sageworks-0.6.3/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/mkdocs.yml` & `sageworks-0.6.3/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 site_name: SageWorks
 nav:
   - Welcome: index.md
+  - Getting Started: getting_started/index.md
   - SageWorks REPL: repl/index.md
   - API Classes: 
     - OverView: api_classes/overview.md
     - Meta: api_classes/meta.md
     - DataSource: api_classes/data_source.md
     - FeatureSet: api_classes/feature_set.md
     - Model: api_classes/model.md
@@ -44,14 +45,15 @@
       - HTG: research/htg.md
   - AWS Glue Jobs: glue/index.md 
   - AWS Setup: 
     - Developer SSO Setup: aws_setup/sso_setup.md
     - Full Pipeline Testing: aws_setup/full_pipeline.md
     - AWS Admin Initial Setup: aws_setup/core_stack.md
     - Dashboard Setup: aws_setup/dashboard_stack.md
+    - Domain/SSL Cert Setup: aws_setup/domain_cert_setup.md
     - AWS Tips and Tricks: aws_setup/aws_tips_and_tricks.md
     - AWS Access Management: aws_setup/aws_access_management.md
   - Admin: 
     - PyPI Release:  admin/pypi_release.md
     - Docker Push:  admin/docker_push.md
 
 theme:
```

### Comparing `sageworks-0.6.2/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.6.3/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/notebooks/ML_Pipeline_with_SageWorks_2.ipynb` & `sageworks-0.6.3/notebooks/ML_Pipeline_with_SageWorks_2.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/notebooks/Outliers_in_SageWorks.ipynb` & `sageworks-0.6.3/notebooks/Outliers_in_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/notebooks/images/athena_query_aqsol.png` & `sageworks-0.6.3/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.6.3/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.6.3/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/notebooks/images/model_screenshot.png` & `sageworks-0.6.3/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/notebooks/images/sageworks_concepts.png` & `sageworks-0.6.3/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/notebooks/images/scp_labs.png` & `sageworks-0.6.3/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/ag_table_row_selection.py` & `sageworks-0.6.3/scripts/ag_table_row_selection.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/athena_ddl_mixed_case.py` & `sageworks-0.6.3/scripts/athena_ddl_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/copy_data_catalog_db.py` & `sageworks-0.6.3/scripts/copy_data_catalog_db.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/create_glue_workflow_with_trigger.py` & `sageworks-0.6.3/scripts/create_glue_workflow_with_trigger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/delete_redis_keys.py` & `sageworks-0.6.3/scripts/delete_redis_keys.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/glue_mixed_case.py` & `sageworks-0.6.3/scripts/glue_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/model_endpoint_sanity_check.py` & `sageworks-0.6.3/scripts/model_endpoint_sanity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/onboard_endpoints.py` & `sageworks-0.6.3/scripts/onboard_endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/onboard_models.py` & `sageworks-0.6.3/scripts/onboard_models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/storage/dns_data_to_features.py` & `sageworks-0.6.3/scripts/storage/dns_data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/storage/generate_jsonl_data.py` & `sageworks-0.6.3/scripts/storage/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/scripts/test_feature_resolution.py` & `sageworks-0.6.3/scripts/test_feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/setup.cfg` & `sageworks-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/setup.py` & `sageworks-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/__init__.py` & `sageworks-0.6.3/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/dataframe/aggregation.py` & `sageworks-0.6.3/src/sageworks/algorithms/dataframe/aggregation.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/dataframe/data_source_eda.py` & `sageworks-0.6.3/src/sageworks/algorithms/dataframe/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/dataframe/dimensionality_reduction.py` & `sageworks-0.6.3/src/sageworks/algorithms/dataframe/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/dataframe/feature_resolution.py` & `sageworks-0.6.3/src/sageworks/algorithms/dataframe/feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/dataframe/feature_spider.py` & `sageworks-0.6.3/src/sageworks/algorithms/dataframe/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/dataframe/row_tagger.py` & `sageworks-0.6.3/src/sageworks/algorithms/dataframe/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/spark/Readme.md` & `sageworks-0.6.3/src/sageworks/algorithms/spark/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/sql/Readme.md` & `sageworks-0.6.3/src/sageworks/algorithms/sql/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/sql/column_stats.py` & `sageworks-0.6.3/src/sageworks/algorithms/sql/column_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/sql/correlations.py` & `sageworks-0.6.3/src/sageworks/algorithms/sql/correlations.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/sql/descriptive_stats.py` & `sageworks-0.6.3/src/sageworks/algorithms/sql/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/sql/outliers.py` & `sageworks-0.6.3/src/sageworks/algorithms/sql/outliers.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/sql/sample_rows.py` & `sageworks-0.6.3/src/sageworks/algorithms/sql/sample_rows.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/algorithms/sql/value_counts.py` & `sageworks-0.6.3/src/sageworks/algorithms/sql/value_counts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/__init__.py` & `sageworks-0.6.3/src/sageworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/data_source.py` & `sageworks-0.6.3/src/sageworks/api/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/endpoint.py` & `sageworks-0.6.3/src/sageworks/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/feature_set.py` & `sageworks-0.6.3/src/sageworks/api/feature_set.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/meta.py` & `sageworks-0.6.3/src/sageworks/api/meta.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/model.py` & `sageworks-0.6.3/src/sageworks/api/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/monitor.py` & `sageworks-0.6.3/src/sageworks/api/monitor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/pipeline.py` & `sageworks-0.6.3/src/sageworks/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/api/pipeline_manager.py` & `sageworks-0.6.3/src/sageworks/api/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         # Grab our SageWorks Bucket
         cm = ConfigManager()
         cls.sageworks_bucket = cm.get_config("SAGEWORKS_BUCKET")
 
         # Sanity check our SageWorks Bucket
         if cls.sageworks_bucket is None:
             cls.log.critical("SAGEWORKS_BUCKET is not defined")
-            cls.log.critical("Run Initial Setup here: https://supercowpowers.github.io/sageworks/#initial-setupconfig ")
+            cls.log.critical("Run Initial Setup here: https://supercowpowers.github.io/sageworks/getting_started/")
             sys.exit(1)
 
         # Construct bucket paths
         cls.incoming_data_bucket = "s3://" + cls.sageworks_bucket + "/incoming-data/"
         cls.data_sources_bucket = "s3://" + cls.sageworks_bucket + "/data-sources/"
         cls.feature_sets_bucket = "s3://" + cls.sageworks_bucket + "/feature-sets/"
```

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.6.3/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/__init__.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/artifact.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/athena_source.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/data_source_abstract.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/data_source_factory.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/data_source_factory.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/endpoint_core.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/endpoint_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/feature_set_core.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/feature_set_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/model_core.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/model_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,16 +516,22 @@
             owner = input("Model Owner: ")
             if owner in ["None", "none", ""]:
                 owner = "unknown"
 
         # Now that we have all the details, let's onboard the Model with all the args
         return self.onboard_with_args(self.model_type, target_column, feature_columns, endpoints, owner)
 
-    def onboard_with_args(self, model_type: ModelType, target_column: str = None, feature_list: list = None,
-                          endpoints: list = None, owner: str = None) -> bool:
+    def onboard_with_args(
+        self,
+        model_type: ModelType,
+        target_column: str = None,
+        feature_list: list = None,
+        endpoints: list = None,
+        owner: str = None,
+    ) -> bool:
         """Onboard the Model with the given arguments
 
         Args:
             model_type (ModelType): Model Type
             target_column (str): Target Column
             feature_list (list): List of Feature Columns
             endpoints (list, optional): List of Endpoints. Defaults to None.
```

### Comparing `sageworks-0.6.2/src/sageworks/core/artifacts/monitor_core.py` & `sageworks-0.6.3/src/sageworks/core/artifacts/monitor_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/pipelines/pipeline_executor.py` & `sageworks-0.6.3/src/sageworks/core/pipelines/pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/Readme.md` & `sageworks-0.6.3/src/sageworks/core/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/__init__.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/clean_data.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py` & `sageworks-0.6.3/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/features_to_model.py` & `sageworks-0.6.3/src/sageworks/core/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.6.3/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.6.3/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/__init__.py` & `sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py` & `sageworks-0.6.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/core/transforms/transform.py` & `sageworks-0.6.3/src/sageworks/core/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/experiments/view_manager.py` & `sageworks-0.6.3/src/sageworks/experiments/view_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/repl/sageworks_shell.py` & `sageworks-0.6.3/src/sageworks/repl/sageworks_shell.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/aws_utils.py` & `sageworks-0.6.3/src/sageworks/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/cache.py` & `sageworks-0.6.3/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/chem_utils.py` & `sageworks-0.6.3/src/sageworks/utils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/config_manager.py` & `sageworks-0.6.3/src/sageworks/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/dashboard_metrics.py` & `sageworks-0.6.3/src/sageworks/utils/dashboard_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/datetime_utils.py` & `sageworks-0.6.3/src/sageworks/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.6.3/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/docker_utils.py` & `sageworks-0.6.3/src/sageworks/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/ecs_info.py` & `sageworks-0.6.3/src/sageworks/utils/ecs_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/endpoint_metrics.py` & `sageworks-0.6.3/src/sageworks/utils/endpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/endpoint_utils.py` & `sageworks-0.6.3/src/sageworks/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/extract_model_artifact.py` & `sageworks-0.6.3/src/sageworks/utils/extract_model_artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/glue_utils.py` & `sageworks-0.6.3/src/sageworks/utils/glue_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/license_manager.py` & `sageworks-0.6.3/src/sageworks/utils/license_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Internal: SageWorks API License Manager (used by ConfigManager, do not use directly)"""
 
 import sys
 import base64
 import json
 import logging
+import requests
 from typing import Union
 import importlib.resources as resources
 from datetime import datetime
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.backends import default_backend
@@ -32,14 +33,17 @@
         Args:
             aws_account_id(str): The AWS Account ID to verify the license against (None for Open Source)
             api_key(str): The SageWorks API Key to verify (base64 encoded)
         Returns:
             dict/None: The SageWorks API License Information or None if the license is invalid
         """
 
+        # Store the API Key for later use
+        cls.api_key = api_key
+
         # Decode the API Key
         try:
             decoded_license_key = base64.b64decode(api_key)
             _license_data, signature = cls.extract_data_and_signature(decoded_license_key)
         except Exception as e:
             cls.log.critical(f"Failed to decode API Key: {e}")
             cls.log.critical("Please contact SageWorks support")
@@ -130,21 +134,33 @@
         with resources.path("sageworks.resources", "signature_verify_pub.pem") as public_key_path:
             with open(public_key_path, "rb") as key_file:
                 public_key_data = key_file.read()
 
         public_key = serialization.load_pem_public_key(public_key_data, backend=default_backend())
         return public_key
 
+    @classmethod
+    def contact_license_server(cls) -> requests.Response:
+        """Contact the SageWorks License Server to verify the license."""
+        server_url = "https://sageworks-keyserver.com/decode-key"
+        headers = {"Content-Type": "application/json", "x-api-key": "Z3dDGm4392V3klijcBbT3ccEutwwWMp82IbYa5i0"}
+        data = {"api_key": cls.api_key}
+        return requests.post(server_url, headers=headers, json=data)
+
 
 if __name__ == "__main__":
     """Exercise the License Manager class"""
     from sageworks.utils.config_manager import ConfigManager
 
     # Grab the API Key from the SageWorks ConfigManager
     cm = ConfigManager()
     api_key = cm.get_config("SAGEWORKS_API_KEY")
     print(LicenseManager.get_license_id())
 
     my_license_info = LicenseManager.load_api_license(aws_account_id=None, api_key=api_key)
     print(my_license_info)
     LicenseManager.print_license_info()
     print(LicenseManager.get_license_id())
+
+    # Test the license server
+    response = LicenseManager.contact_license_server()
+    print(response.json())
```

### Comparing `sageworks-0.6.2/src/sageworks/utils/markdown_utils.py` & `sageworks-0.6.3/src/sageworks/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/pandas_utils.py` & `sageworks-0.6.3/src/sageworks/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/plugin_manager.py` & `sageworks-0.6.3/src/sageworks/utils/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/redis_cache.py` & `sageworks-0.6.3/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/repl_utils.py` & `sageworks-0.6.3/src/sageworks/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/s3_utils.py` & `sageworks-0.6.3/src/sageworks/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/sageworks_cache.py` & `sageworks-0.6.3/src/sageworks/utils/sageworks_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.6.3/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.6.3/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.6.3/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/symbols.py` & `sageworks-0.6.3/src/sageworks/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/test_data_generator.py` & `sageworks-0.6.3/src/sageworks/utils/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/trace_calls.py` & `sageworks-0.6.3/src/sageworks/utils/trace_calls.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/utils/type_abbrev.py` & `sageworks-0.6.3/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.6.3/src/sageworks/views/artifacts_text_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.6.3/src/sageworks/views/artifacts_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/views/data_source_web_view.py` & `sageworks-0.6.3/src/sageworks/views/data_source_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/views/endpoint_web_view.py` & `sageworks-0.6.3/src/sageworks/views/endpoint_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.6.3/src/sageworks/views/feature_set_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/views/model_web_view.py` & `sageworks-0.6.3/src/sageworks/views/model_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/views/view.py` & `sageworks-0.6.3/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/component_interface.py` & `sageworks-0.6.3/src/sageworks/web_components/component_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.6.3/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/correlation_matrix.py` & `sageworks-0.6.3/src/sageworks/web_components/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/data_details_markdown.py` & `sageworks-0.6.3/src/sageworks/web_components/data_details_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/endpoint_details.py` & `sageworks-0.6.3/src/sageworks/web_components/endpoint_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/endpoint_metric_plots.py` & `sageworks-0.6.3/src/sageworks/web_components/endpoint_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/color_maps.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/color_maps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/compound_details.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/compound_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/dashboard_metric_plots.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/dashboard_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/data_table.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/data_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/histogram.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/line_chart.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/outlier_plot.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/outlier_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/plugin_callbacks.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/plugin_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/experiments/scatter_plot.py` & `sageworks-0.6.3/src/sageworks/web_components/experiments/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/model_details.py` & `sageworks-0.6.3/src/sageworks/web_components/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/model_plot.py` & `sageworks-0.6.3/src/sageworks/web_components/model_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/plugin_interface.py` & `sageworks-0.6.3/src/sageworks/web_components/plugin_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     DATA_SOURCE = "data_source"
     FEATURE_SET = "feature_set"
     MODEL = "model"
     ENDPOINT = "endpoint"
     PIPELINE = "pipeline"
     MODEL_TABLE = "model_table"
     PIPELINE_TABLE = "pipeline_table"
+    CUSTOM = "custom"
 
 
 class PluginInterface(ComponentInterface):
     """A Web Plugin Interface
     Notes:
       - The 'create_component' method must be implemented by the child class
       - The 'update_properties' method must be implemented by the child class
```

### Comparing `sageworks-0.6.2/src/sageworks/web_components/plugin_unit_test.py` & `sageworks-0.6.3/src/sageworks/web_components/plugin_unit_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/plugins/ag_table.py` & `sageworks-0.6.3/src/sageworks/web_components/plugins/ag_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/plugins/model_details.py` & `sageworks-0.6.3/src/sageworks/web_components/plugins/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/regression_plot.py` & `sageworks-0.6.3/src/sageworks/web_components/regression_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/table.py` & `sageworks-0.6.3/src/sageworks/web_components/table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks/web_components/violin_plots.py` & `sageworks-0.6.3/src/sageworks/web_components/violin_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.6.3/src/sageworks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 applications/aws_dashboard/pages/data_sources/page.py
 applications/aws_dashboard/pages/endpoints/callbacks.py
 applications/aws_dashboard/pages/endpoints/layout.py
 applications/aws_dashboard/pages/endpoints/page.py
 applications/aws_dashboard/pages/feature_sets/callbacks.py
 applications/aws_dashboard/pages/feature_sets/layout.py
 applications/aws_dashboard/pages/feature_sets/page.py
+applications/aws_dashboard/pages/license/page.py
 applications/aws_dashboard/pages/main/callbacks.py
 applications/aws_dashboard/pages/main/layout.py
 applications/aws_dashboard/pages/main/page.py
 applications/aws_dashboard/pages/models/callbacks.py
 applications/aws_dashboard/pages/models/layout.py
 applications/aws_dashboard/pages/models/page.py
 applications/aws_dashboard/pages/pipelines/callbacks.py
@@ -108,14 +109,15 @@
 docs/api_classes/monitor.md
 docs/api_classes/overview.md
 docs/api_classes/pipelines.md
 docs/aws_setup/aws_access_management.md
 docs/aws_setup/aws_tips_and_tricks.md
 docs/aws_setup/core_stack.md
 docs/aws_setup/dashboard_stack.md
+docs/aws_setup/domain_cert_setup.md
 docs/aws_setup/full_pipeline.md
 docs/aws_setup/sso_setup.md
 docs/concepts/model_monitoring.md
 docs/core_classes/overview.md
 docs/core_classes/artifacts/artifact.md
 docs/core_classes/artifacts/athena_source.md
 docs/core_classes/artifacts/data_source_abstract.md
@@ -131,14 +133,15 @@
 docs/core_classes/transforms/model_to_endpoint.md
 docs/core_classes/transforms/overview.md
 docs/core_classes/transforms/pandas_transforms.md
 docs/core_classes/transforms/transform.md
 docs/enterprise/index.md
 docs/enterprise/project_branding.md
 docs/enterprise/themes.md
+docs/getting_started/index.md
 docs/glue/index.md
 docs/images/big_spider.png
 docs/images/graph_representation.png
 docs/images/powered_aws_dark_blue.png
 docs/images/powered_aws_transparent.png
 docs/images/powered_aws_white.png
 docs/images/powered_aws_with_tm_grey.png
@@ -388,15 +391,17 @@
 src/sageworks/web_components/experiments/data_table.py
 src/sageworks/web_components/experiments/histogram.py
 src/sageworks/web_components/experiments/line_chart.py
 src/sageworks/web_components/experiments/outlier_plot.py
 src/sageworks/web_components/experiments/plugin_callbacks.py
 src/sageworks/web_components/experiments/scatter_plot.py
 src/sageworks/web_components/plugins/ag_table.py
+src/sageworks/web_components/plugins/license_details.py
 src/sageworks/web_components/plugins/model_details.py
+src/sageworks/web_components/plugins/pipeline_details.py
 tests/create_aqsol_artifacts.py
 tests/create_basic_test_artifacts.py
 tests/create_realtime_endpoint.py
 tests/create_training_adjusted_artifacts.py
 tests/create_wine_artifacts.py
 tests/delete_test_artifacts.py
 tests/artifacts/data_source_tests.py
@@ -419,8 +424,11 @@
 tests/transforms/features_to_model_tests.py
 tests/transforms/model_metrics_tests.py
 tests/transforms/model_to_endpoint_tests.py
 tests/transforms/pandas_to_data_tests.py
 tests/web_components/confusion_matrix_test.py
 tests/web_components/correlation_matrix_test.py
 tests/web_components/plugin_interface_test.py
-ui_testing/table_comparison.py
+ui_testing/table_comparison.py
+ui_testing/theme_switching.py
+ui_testing/theme_switching_2.py
+ui_testing/assets/custom.css
```

### Comparing `sageworks-0.6.2/tests/artifacts/data_source_tests.py` & `sageworks-0.6.3/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/artifacts/endpoint_tests.py` & `sageworks-0.6.3/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/artifacts/feature_set_tests.py` & `sageworks-0.6.3/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/artifacts/model_tests.py` & `sageworks-0.6.3/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.6.3/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.6.3/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/connectors/data_catalog.py` & `sageworks-0.6.3/tests/connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/connectors/endpoints.py` & `sageworks-0.6.3/tests/connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/connectors/feature_store.py` & `sageworks-0.6.3/tests/connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/connectors/glue_jobs.py` & `sageworks-0.6.3/tests/connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/connectors/model_registry.py` & `sageworks-0.6.3/tests/connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/connectors/s3_bucket.py` & `sageworks-0.6.3/tests/connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/create_aqsol_artifacts.py` & `sageworks-0.6.3/tests/create_aqsol_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/create_basic_test_artifacts.py` & `sageworks-0.6.3/tests/create_basic_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/create_realtime_endpoint.py` & `sageworks-0.6.3/tests/create_realtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/create_training_adjusted_artifacts.py` & `sageworks-0.6.3/tests/create_training_adjusted_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/create_wine_artifacts.py` & `sageworks-0.6.3/tests/create_wine_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/delete_test_artifacts.py` & `sageworks-0.6.3/tests/delete_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/plugin_tests/crashing_plugin.py` & `sageworks-0.6.3/tests/plugin_tests/crashing_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/specific/capital_tests.py` & `sageworks-0.6.3/tests/specific/capital_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/specific/deletion_tests.py` & `sageworks-0.6.3/tests/specific/deletion_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/transforms/data_to_data_tests.py` & `sageworks-0.6.3/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/transforms/data_to_features_tests.py` & `sageworks-0.6.3/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/transforms/features_to_model_tests.py` & `sageworks-0.6.3/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/transforms/model_metrics_tests.py` & `sageworks-0.6.3/tests/transforms/model_metrics_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.6.3/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.6.3/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/web_components/confusion_matrix_test.py` & `sageworks-0.6.3/tests/web_components/confusion_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/web_components/correlation_matrix_test.py` & `sageworks-0.6.3/tests/web_components/correlation_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tests/web_components/plugin_interface_test.py` & `sageworks-0.6.3/tests/web_components/plugin_interface_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/tox.ini` & `sageworks-0.6.3/tox.ini`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.2/ui_testing/table_comparison.py` & `sageworks-0.6.3/ui_testing/table_comparison.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,29 +24,30 @@
 
     def __init__(self):
         self.component_id = None
         self.container = None
         self.properties = []
         self.signals = []
 
-    def create_component(self, component_id: str) -> AgGrid:
+    def create_component(self, component_id: str, theme: str) -> AgGrid:
         """Create a Table Component without any data.
         Args:
             component_id (str): The ID of the web component
+            theme (str): The class of the web component
         Returns:
             AgGrid: The Table Component using AG Grid
         """
         self.component_id = component_id
         self.container = AgGrid(
             id=component_id,
-            # className="ag-theme-balham-dark",
-            className="ag-theme-alpine-auto-dark",
-            columnSize="sizeToFit",
+            className=theme,
             dashGridOptions={"rowSelection": "single"},
+            defaultColDef={"flex": 1, "filter": True},
             style={"maxHeight": "200px", "overflow": "auto"},
+            dangerously_allow_code=True,  # to allow hyperlinks in dag
         )
 
         # Fill in plugin properties
         self.properties = [
             (self.component_id, "columnDefs"),
             (self.component_id, "rowData"),
             (self.component_id, "selectedRows"),
@@ -72,15 +73,30 @@
         """
         print(f"Updating Table Plugin with a table dataframe and kwargs: {kwargs}")
 
         # Convert the DataFrame to a list of dictionaries for AG Grid
         table_data = table_df.to_dict("records")
 
         # Define column definitions based on the DataFrame
-        column_defs = [{"headerName": col, "field": col, "filter": "agTextColumnFilter"} for col in table_df.columns]
+        column_defs = [
+            (
+                {"field": col, "valueFormatter": {"function": "d3.format(',')(params.value)"}}
+                if col == "Salary"
+                else (
+                    {"field": col, "valueFormatter": {"function": "d3.format('.2f')(params.value)"}}
+                    if col == "Bonus"
+                    else (
+                        {"field": col, "valueFormatter": {"function": "params.value.toUpperCase()"}}
+                        if col == "Name"
+                        else {"field": col, "cellRenderer": "markdown"} if col == "Company" else {"field": col}
+                    )
+                )
+            )
+            for col in table_df.columns
+        ]
 
         # Select the first row by default
         selected_rows = table_df.head(1).to_dict("records")
 
         # Return the column definitions and table data (must match the plugin properties)
         return [column_defs, table_data, selected_rows]
 
@@ -93,43 +109,48 @@
     health_icons = [health_icons[h] for h in health_list]
     data = {
         "Name": ["joe", "bob", "sue", "jane", "jill", "jack"],
         "Health": health_icons,
         "Age": [10, 20, 30, 40, 50, 60],
         "Company": ["IBM", "Google", "Amazon", "Facebook", "Apple", "Microsoft"],
         "Title": ["CEO", "CFO", "CTO", "CIO", "COO", "CMO"],
-        "Salary": [100, 200, 300, 400, 500, 600],
-        "Bonus": [10, 20, 30, 40, 50, 60],
+        "Salary": [1000, 2000, 3000, 4000, 5000, 6000],
+        "Bonus": [0.2445, 0.3641, 0.5647, 0.7865, 0.4565, 0.2956],
     }
     df = pd.DataFrame(data)
-
     # Testing HTML Links
     df["Company"] = df["Company"].map(lambda x: f"<a href='https://www.google.com' target='_blank'>{x}</a>")
 
-    # Create a Dash app
-    app = Dash(__name__)
+    # Create the new AG Table component
+    AG_grid_themes = ["alpine", "balham", "material", "quartz"]
+    dag_tables = []
+
+    for ag_theme in AG_grid_themes:
+        dag_tables += [html.Hr(), html.Div(f"Dash AG Grid - {ag_theme}:")]
+        for light_dark in ["", "-dark"]:
+            ag_table = AGTable()
+            theme = f"ag-theme-{ag_theme + light_dark} ag-theme-custom{light_dark}"
+            ag_table_component = ag_table.create_component(f"ag-table-{ag_theme}{light_dark}", theme)
+            # This would normally be a callback, but we're just testing
+            ag_table_component.columnDefs, ag_table_component.rowData, ag_table_component.selectedRows = (
+                ag_table.update_properties(df)
+            )
+            dag_tables += [ag_table_component, html.Br()]
 
     # Create the existing table component
     my_table = Table()
-    existing_table = my_table.create_component(
+    data_table = my_table.create_component(
         "current-table", header_color="rgb(60, 100, 60)", row_select="single", transparent=False
     )
-
     # Note: This is old style API, but will be replaced anyway
-    existing_table.columns = my_table.column_setup(df, markdown_columns=["Company"])
-    existing_table.data = df.to_dict("records")
-
-    # Create the new AG Table component
-    ag_table = AGTable()
-    ag_table_component = ag_table.create_component("ag-table")
+    data_table.columns = my_table.column_setup(df, markdown_columns=["Company"])
+    data_table.data = df.to_dict("records")
 
-    # This would normally be a callback, but we're just testing
-    ag_table_component.columnDefs, ag_table_component.rowData, ag_table_component.selectedRows = (
-        ag_table.update_properties(df)
-    )
+    # Create a Dash app
+    app = Dash(__name__)
 
     # Set up the layout
-    app.layout = html.Div([existing_table, ag_table_component])
+    app.layout = html.Div([html.Div("Current DataTable:"), data_table] + dag_tables)
 
     # Run the app
     webbrowser.open("http://localhost:8050")
     app.run(debug=True)
```

