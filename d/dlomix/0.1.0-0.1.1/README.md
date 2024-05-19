# Comparing `tmp/dlomix-0.1.0.tar.gz` & `tmp/dlomix-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlomix-0.1.0.tar", last modified: Fri May  3 11:20:27 2024, max compression
+gzip compressed data, was "dlomix-0.1.1.tar", last modified: Sun May 19 10:39:01 2024, max compression
```

## Comparing `dlomix-0.1.0.tar` & `dlomix-0.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.639659 dlomix-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 11:20:21.000000 dlomix-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-03 11:20:27.639659 dlomix-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-03 11:20:21.000000 dlomix-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:20:21.000000 dlomix-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:20:27.639659 dlomix-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-03 11:20:21.000000 dlomix-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.627658 dlomix-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.631659 dlomix-0.1.0/src/dlomix/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.631659 dlomix-0.1.0/src/dlomix/data/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    25154 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/fragment_ion_intensity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/data/processing/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/feature_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/
--rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/mz_diff.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/red_smiles.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24289 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_ac_count.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    23161 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_gained_atoms.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    23161 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_loss_atoms.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/processing/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/data/retention_time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/eval/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/eval/rt_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/layers/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/losses/intensity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/models/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/models/deepLC.py
--rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/models/prosit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.635659 dlomix-0.1.0/src/dlomix/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/pipelines/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.639659 dlomix-0.1.0/src/dlomix/reports/
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/IntensityReport.py
--rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/RetentionTimeReport.py
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/RetentionTimeReportModelComparisonWandb.py
--rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/RetentionTimeReportRunComparisonWandb.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-03 11:20:21.000000 dlomix-0.1.0/src/dlomix/reports/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.639659 dlomix-0.1.0/src/dlomix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 11:20:27.000000 dlomix-0.1.0/src/dlomix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:20:27.639659 dlomix-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-03 11:20:21.000000 dlomix-0.1.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-03 11:20:21.000000 dlomix-0.1.0/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-03 11:20:21.000000 dlomix-0.1.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.648917 dlomix-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 10:38:55.000000 dlomix-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-19 10:39:01.648917 dlomix-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-19 10:38:55.000000 dlomix-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-19 10:38:56.000000 dlomix-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 10:39:01.648917 dlomix-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-19 10:38:56.000000 dlomix-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.636917 dlomix-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.636917 dlomix-0.1.1/src/dlomix/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.640917 dlomix-0.1.1/src/dlomix/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26061 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/fragment_ion_intensity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.640917 dlomix-0.1.1/src/dlomix/data/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/feature_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.644917 dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/mz_diff.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/red_smiles.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24289 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/saved_ac_count.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    23161 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/saved_gained_atoms.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    23161 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/saved_loss_atoms.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/processing/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/data/retention_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.644917 dlomix-0.1.1/src/dlomix/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/eval/rt_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.644917 dlomix-0.1.1/src/dlomix/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/layers/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.644917 dlomix-0.1.1/src/dlomix/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/losses/intensity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.644917 dlomix-0.1.1/src/dlomix/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/models/deepLC.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/models/prosit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.644917 dlomix-0.1.1/src/dlomix/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/pipelines/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.644917 dlomix-0.1.1/src/dlomix/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/reports/IntensityReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/reports/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/reports/RetentionTimeReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/reports/RetentionTimeReportModelComparisonWandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/reports/RetentionTimeReportRunComparisonWandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-19 10:38:56.000000 dlomix-0.1.1/src/dlomix/reports/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.648917 dlomix-0.1.1/src/dlomix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-19 10:39:01.000000 dlomix-0.1.1/src/dlomix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-19 10:39:01.000000 dlomix-0.1.1/src/dlomix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 10:39:01.000000 dlomix-0.1.1/src/dlomix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-19 10:39:01.000000 dlomix-0.1.1/src/dlomix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 10:39:01.000000 dlomix-0.1.1/src/dlomix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:39:01.648917 dlomix-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-19 10:38:56.000000 dlomix-0.1.1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-19 10:38:56.000000 dlomix-0.1.1/tests/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-19 10:38:56.000000 dlomix-0.1.1/tests/test_models.py
```

### Comparing `dlomix-0.1.0/LICENSE` & `dlomix-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/PKG-INFO` & `dlomix-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlomix
-Version: 0.1.0
+Version: 0.1.1
 Summary: Deep Learning for Proteomics
 Home-page: https://github.com/wilhelm-lab/dlomix
 Author: Omar Shouman
 Author-email: o.shouman@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -70,16 +70,14 @@
 -  `eval`: classes for evaluating models and reporting results
 -  `layers`: custom layers used for building models, based on `tf.keras.layers.Layer`
 -  `losses`: custom losses to be used for training with `model.fit()`
 - `models`: common model architectures for the relevant use-cases based on `tf.keras.Model` to allow for using the Keras training API
 -  `pipelines`: an exemplary high-level pipeline implementation
 -  `reports`: classes for generating reports related to the different tasks
 -  `constants.py`: constants and configuration values
--  `utils.py`: utility functions
-
 
 
 **Use-cases**
 
 - Retention Time Prediction:
     - a regression problem where the retention time of a peptide sequence is to be predicted.
```

### Comparing `dlomix-0.1.0/README.md` & `dlomix-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 -  `eval`: classes for evaluating models and reporting results
 -  `layers`: custom layers used for building models, based on `tf.keras.layers.Layer`
 -  `losses`: custom losses to be used for training with `model.fit()`
 - `models`: common model architectures for the relevant use-cases based on `tf.keras.Model` to allow for using the Keras training API
 -  `pipelines`: an exemplary high-level pipeline implementation
 -  `reports`: classes for generating reports related to the different tasks
 -  `constants.py`: constants and configuration values
--  `utils.py`: utility functions
-
 
 
 **Use-cases**
 
 - Retention Time Prediction:
     - a regression problem where the retention time of a peptide sequence is to be predicted.
```

### Comparing `dlomix-0.1.0/setup.py` & `dlomix-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/constants.py` & `dlomix-0.1.1/src/dlomix/constants.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/charge_state.py` & `dlomix-0.1.1/src/dlomix/data/charge_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         features_to_extract (Optional[List[Union[Callable, str]]]): The list of features to extract from the dataset. Default is None.
         pad (bool): Whether to pad the sequences to the maximum length. Default is True.
         padding_value (int): The value to use for padding. Default is 0.
         alphabet (Dict): The mapping of characters to integers for encoding the sequences. Default is ALPHABET_UNMOD.
         encoding_scheme (Union[str, EncodingScheme]): The encoding scheme to use for encoding the sequences. Default is EncodingScheme.UNMOD.
         processed (bool): Whether the data has been preprocessed. Default is False.
         enable_tf_dataset_cache (bool): Flag to indicate whether to enable TensorFlow Dataset caching (call `.cahce()` on the generate TF Datasets).
-        disable_cache (bool): Whether to disable Hugging Face datasets caching. Default is True.
+        disable_cache (bool): Whether to disable Hugging Face datasets caching. Default is False.
     """
 
     def __init__(
         self,
         data_source: Optional[Union[str, List]] = None,
         val_data_source: Optional[Union[str, List]] = None,
         test_data_source: Optional[Union[str, List]] = None,
@@ -49,15 +49,18 @@
         features_to_extract: Optional[List[Union[Callable, str]]] = None,
         pad: bool = True,
         padding_value: int = 0,
         alphabet: Dict = ALPHABET_UNMOD,
         encoding_scheme: Union[str, EncodingScheme] = EncodingScheme.UNMOD,
         processed: bool = False,
         enable_tf_dataset_cache: bool = False,
-        disable_cache: bool = True,
+        disable_cache: bool = False,
+        auto_cleanup_cache: bool = True,
+        num_proc: Optional[int] = None,
+        batch_processing_size: int = 1000,
     ):
         super().__init__(
             data_source,
             val_data_source,
             test_data_source,
             data_format,
             sequence_column,
@@ -72,8 +75,11 @@
             pad,
             padding_value,
             alphabet,
             encoding_scheme,
             processed,
             enable_tf_dataset_cache,
             disable_cache,
+            auto_cleanup_cache,
+            num_proc,
+            batch_processing_size,
         )
```

### Comparing `dlomix-0.1.0/src/dlomix/data/dataset.py` & `dlomix-0.1.1/src/dlomix/data/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 import importlib
 import logging
 import os
 import warnings
 from typing import Callable, Dict, List, Optional, Union
 
-import numpy as np
-from datasets import Dataset, DatasetDict, load_dataset, load_from_disk
+from datasets import Dataset, DatasetDict, Sequence, Value, load_dataset, load_from_disk
 
 from ..constants import ALPHABET_UNMOD
 from .dataset_config import DatasetConfig
 from .dataset_utils import EncodingScheme, get_num_processors
 from .processing.feature_extractors import (
     AVAILABLE_FEATURE_EXTRACTORS,
     FEATURE_EXTRACTORS_PARAMETERS,
@@ -72,17 +71,21 @@
     encoding_scheme : Union[str, EncodingScheme]
         Encoding scheme to use for encoding the sequences. Possible values are "unmod" and "naive-mods" for unmodified sequences and sequences with PTMs respectively.
     processed : bool
         Flag to indicate whether the dataset has been processed or not.
     enable_tf_dataset_cache : bool
         Flag to indicate whether to enable TensorFlow Dataset caching (call `.cahce()` on the generate TF Datasets).
     disable_cache : bool
-        Flag to indicate whether to disable Hugging Face Datasets caching.
+        Flag to indicate whether to disable Hugging Face Datasets caching. Default is False.
     auto_cleanup_cache : bool
-        Flag to indicate whether to automatically clean up the temporary Hugging Face Datasets cache files.
+        Flag to indicate whether to automatically clean up the temporary Hugging Face Datasets cache files. Default is True.
+    num_proc : Optional[int]
+        Number of processes to use for processing the dataset. Default is None, no multi-processing.
+    batch_processing_size : Optional[int]
+        Batch size for processing the dataset, passed to the HuggingFace `Dataset.map()` function calls. Default is 1000.
 
     Attributes
     ----------
     DEFAULT_SPLIT_NAMES : List[str]
         Default split names for the dataset.
     CONFIG_JSON_NAME : str
         Name of the configuration JSON file.
@@ -117,16 +120,18 @@
         features_to_extract: Optional[List[Union[Callable, str]]] = None,
         pad: bool = True,
         padding_value: int = 0,
         alphabet: Dict = ALPHABET_UNMOD,
         encoding_scheme: Union[str, EncodingScheme] = EncodingScheme.UNMOD,
         processed: bool = False,
         enable_tf_dataset_cache: bool = False,
-        disable_cache: bool = True,
+        disable_cache: bool = False,
         auto_cleanup_cache: bool = True,
+        num_proc: Optional[int] = None,
+        batch_processing_size: Optional[int] = 1000,
     ):
         super(PeptideDataset, self).__init__()
         self.data_source = data_source
         self.val_data_source = val_data_source
         self.test_data_source = test_data_source
 
         self.data_format = data_format
@@ -162,16 +167,17 @@
         self._refresh_config()
 
         if not self.processed:
             self.hf_dataset: Optional[Union[Dataset, DatasetDict]] = None
             self._empty_dataset_mode = False
             self._is_predefined_split = False
             self._test_set_only = False
-            self._default_num_proc = get_num_processors()
-            self._default_batch_processing_size = 1000
+            self._num_proc = num_proc
+            self._set_num_proc()
+            self._batch_processing_size = batch_processing_size
 
             self._data_files_available_splits = {}
             self._load_dataset()
             self._decide_on_splitting()
 
             self._relevant_columns = []
             self._extracted_features_columns = []
@@ -181,19 +187,28 @@
                 self._remove_unnecessary_columns()
                 self._split_dataset()
                 self._parse_sequences()
 
                 self._configure_processing_pipeline()
                 self._apply_processing_pipeline()
                 if self.model_features is not None:
-                    self._cast_model_feature_types_expand_zero_dims()
+                    self._cast_model_feature_types_to_float()
                 self._cleanup_temp_dataset_cache_files()
                 self.processed = True
                 self._refresh_config()
 
+    def _set_num_proc(self):
+        if self._num_proc:
+            n_processors = get_num_processors()
+            if self._num_proc > n_processors:
+                warnings.warn(
+                    f"Number of processors provided is greater than the available processors. Using the maximum number of processors available: {n_processors}."
+                )
+                self._num_proc = n_processors
+
     def _set_hf_cache_management(self):
         if self.disable_cache:
             from datasets import disable_caching
 
             disable_caching()
 
     def _refresh_config(self):
@@ -421,52 +436,55 @@
         for processor in self._processors:
             logger.info(f"Applying step: {processor.__class__.__name__}...")
             logger.debug(f"Applying step with arguments:\n\n{processor}...")
             self.hf_dataset = self.hf_dataset.map(
                 processor,
                 desc=f"Mapping {processor.__class__.__name__}",
                 batched=processor.batched,
-                batch_size=self._default_batch_processing_size,
-                num_proc=self._default_num_proc,
+                batch_size=self._batch_processing_size,
+                num_proc=self._num_proc,
             )
             logger.info(f"Done with step: {processor.__class__.__name__}.\n")
 
             if isinstance(processor, SequencePaddingProcessor):
                 for split in self.hf_dataset.keys():
                     if split != "test":
                         logger.info(
                             f"Removing truncated sequences in the {split} split ..."
                         )
 
                         self.hf_dataset[split] = self.hf_dataset[split].filter(
                             lambda batch: batch[processor.KEEP_COLUMN_NAME],
                             batched=True,
-                            num_proc=self._default_num_proc,
-                            batch_size=self._default_batch_processing_size,
+                            num_proc=self._num_proc,
+                            batch_size=self._batch_processing_size,
                         )
                 self.hf_dataset = self.hf_dataset.remove_columns(
                     processor.KEEP_COLUMN_NAME
                 )
 
-    def _cast_model_feature_types_expand_zero_dims(self):
-        def __cast_types_expand_zero_dims(example, column):
-            np_casted = np.array(example[column], dtype=np.float16)
-
-            # model features (metadata in prosit) are expected to be have at least 1 dimension + batch_size
-            if np_casted.ndim == 0:
-                np_casted = np.expand_dims(np_casted, axis=-1)
-            example[column] = np_casted
-            return example
-
-        for c in self.model_features:
-            self.hf_dataset = self.hf_dataset.map(
-                lambda x: __cast_types_expand_zero_dims(x, c),
-                batched=False,
-                num_proc=self._default_num_proc,
-                desc=f"Casting model feature {c} to float ...",
+    def _cast_model_feature_types_to_float(self):
+        for split in self.hf_dataset.keys():
+            new_features = self.hf_dataset[split].features.copy()
+
+            for feature_name, feature_type in self.hf_dataset[split].features.items():
+                # ensure model features are casted to float for concatenation later
+                if feature_name not in self.model_features:
+                    continue
+                if feature_type.dtype.startswith("float"):
+                    continue
+                if isinstance(feature_type, Sequence):
+                    new_features[feature_name] = Sequence(Value("float32"))
+                if isinstance(feature_type, Value):
+                    new_features[feature_name] = Value("float32")
+
+            self.hf_dataset[split] = self.hf_dataset[split].cast(
+                new_features,
+                num_proc=self._num_proc,
+                batch_size=self._batch_processing_size,
             )
 
     def _cleanup_temp_dataset_cache_files(self):
         if self.auto_cleanup_cache:
             cleaned_up = self.hf_dataset.cleanup_cache_files()
             logger.info(f"Cleaned up cache files: {cleaned_up}.")
 
@@ -606,24 +624,21 @@
         tf_dataset = self._get_split_tf_dataset(PeptideDataset.DEFAULT_SPLIT_NAMES[2])
 
         if self.enable_tf_dataset_cache:
             tf_dataset = tf_dataset.cache()
 
         return tf_dataset
 
-    def _check_split_exists(self, split_name: str):
+    def _get_split_tf_dataset(self, split_name: str):
         existing_splits = list(self.hf_dataset.keys())
         if split_name not in existing_splits:
             raise ValueError(
                 f"Split '{split_name}' does not exist in the dataset. Available splits are: {existing_splits}"
             )
 
-    def _get_split_tf_dataset(self, split_name: str):
-        self._check_split_exists(split_name)
-
         return self.hf_dataset[split_name].to_tf_dataset(
             columns=self._get_input_tensor_column_names(),
             label_cols=self.label_column,
             shuffle=False,
             batch_size=self.batch_size,
         )
```

### Comparing `dlomix-0.1.0/src/dlomix/data/dataset_config.py` & `dlomix-0.1.1/src/dlomix/data/dataset_config.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/dataset_utils.py` & `dlomix-0.1.1/src/dlomix/data/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/fragment_ion_intensity.py` & `dlomix-0.1.1/src/dlomix/data/fragment_ion_intensity.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         features_to_extract (Optional[List[Union[Callable, str]]]): The list of features to extract from the dataset.
         pad (bool): Whether to pad the sequences to the maximum length.
         padding_value (int): The value to use for padding.
         alphabet (Dict): The mapping of characters to integers for encoding the sequences.
         encoding_scheme (Union[str, EncodingScheme]): The encoding scheme to use for encoding the sequences.
         processed (bool): Whether the data has been preprocessed before or not.
         enable_tf_dataset_cache (bool): Flag to indicate whether to enable TensorFlow Dataset caching (call `.cahce()` on the generate TF Datasets).
-        disable_cache (bool): Whether to disable Hugging Face datasets caching. Default is True.
+        disable_cache (bool): Whether to disable Hugging Face datasets caching. Default is False.
 
     """
 
     def __init__(
         self,
         data_source: Optional[Union[str, List]] = None,
         val_data_source: Optional[Union[str, List]] = None,
@@ -50,15 +50,18 @@
         features_to_extract: Optional[List[Union[Callable, str]]] = None,
         pad: bool = True,
         padding_value: int = 0,
         alphabet: Dict = ALPHABET_UNMOD,
         encoding_scheme: Union[str, EncodingScheme] = EncodingScheme.UNMOD,
         processed: bool = False,
         enable_tf_dataset_cache: bool = False,
-        disable_cache: bool = True,
+        disable_cache: bool = False,
+        auto_cleanup_cache: bool = True,
+        num_proc: Optional[int] = None,
+        batch_processing_size: int = 1000,
     ):
         super().__init__(
             data_source,
             val_data_source,
             test_data_source,
             data_format,
             sequence_column,
@@ -73,8 +76,11 @@
             pad,
             padding_value,
             alphabet,
             encoding_scheme,
             processed,
             enable_tf_dataset_cache,
             disable_cache,
+            auto_cleanup_cache,
+            num_proc,
+            batch_processing_size,
         )
```

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/__init__.py` & `dlomix-0.1.1/src/dlomix/data/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/feature_extractors.py` & `dlomix-0.1.1/src/dlomix/data/processing/feature_extractors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from collections import defaultdict
+from operator import itemgetter
+
 import numpy as np
 
 from .feature_tables import (
     PTM_ATOM_COUNT_LOOKUP,
     PTM_GAIN_LOOKUP,
     PTM_LOSS_LOOKUP,
     PTM_MOD_DELTA_MASS_LOOKUP,
@@ -73,48 +76,47 @@
         description: str,
         max_length: int = 30,
         batched: bool = False,
     ):
         super().__init__(sequence_column_name, batched)
         self.feature_column_name = feature_column_name
         self.feature_default_value = feature_default_value
+        self._feature_shape = np.array(self.feature_default_value).shape
         self.description = description
         self.max_length = max_length
 
-    def pad_feature_to_seq_length(self, single_feature):
+    def pad_feature_to_seq_length(self, single_feature, unpadded_seq_len):
         """
         Pad the feature to the maximum sequence length.
 
         Parameters
         ----------
         single_feature : list
             List of feature values.
+        unpadded_seq_len : int
+            Length of the unpadded original sequence.
 
         Returns
         -------
         list
             Padded feature list.
         """
 
-        feature_length = len(single_feature)
-
-        if feature_length > self.max_length:
+        if unpadded_seq_len > self.max_length:
             raise ValueError(
-                f"Feature length ({len(single_feature)}) is longer than sequence length provided ({self.max_length})."
+                f"Feature length ({unpadded_seq_len}) is longer than sequence length provided ({self.max_length})."
             )
 
-        padding_length = self.max_length - feature_length
-        single_feature += [self.feature_default_value] * padding_length
+        single_feature[unpadded_seq_len:] = self.feature_default_value
 
-        single_feature = self._cast_expand_dims(single_feature)
+        # expand dims if needed
+        single_feature = self._expand_dims(single_feature)
         return single_feature
 
-    def _cast_expand_dims(self, single_feature):
-        single_feature = np.array(single_feature).astype(np.float32)
-
+    def _expand_dims(self, single_feature):
         if single_feature.ndim == 1:
             single_feature = np.expand_dims(single_feature, axis=-1)
         return single_feature
 
 
 class LookupFeatureExtractor(FeatureExtractor):
     """
@@ -153,15 +155,18 @@
             feature_column_name,
             feature_default_value,
             description,
             max_length,
             batched,
         )
 
-        self.lookup_table = lookup_table
+        d = defaultdict(lambda: self.feature_default_value)
+        d.update(lookup_table)
+
+        self.lookup_table = d
         self.description = description
 
     def batch_process(self, input_data, **kwargs):
         feature_column = []
 
         for n_term, sequence, c_term in zip(
             input_data[SequenceParsingProcessor.PARSED_COL_NAMES["n_term"]],
@@ -179,12 +184,13 @@
             + input_data[self.sequence_column_name]
             + [input_data[SequenceParsingProcessor.PARSED_COL_NAMES["c_term"]]]
         )
         feature = self._extract_feature(seq_with_terms)
         return {self.feature_column_name: feature}
 
     def _extract_feature(self, sequence):
-        feature = [
-            self.lookup_table.get(aa, self.feature_default_value) for aa in sequence
-        ]
-        feature = self.pad_feature_to_seq_length(feature)
+        feature = np.empty((self.max_length, *self._feature_shape), dtype=np.float32)
+        feature[: len(sequence)] = itemgetter(*sequence)(self.lookup_table)
+
+        feature = self.pad_feature_to_seq_length(feature, len(sequence))
+
         return feature
```

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/feature_tables.py` & `dlomix-0.1.1/src/dlomix/data/processing/feature_tables.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/mz_diff.pkl` & `dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/mz_diff.pkl`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/red_smiles.pkl` & `dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/red_smiles.pkl`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_ac_count.pkl` & `dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/saved_ac_count.pkl`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_gained_atoms.pkl` & `dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/saved_gained_atoms.pkl`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/pickled_feature_dicts/saved_loss_atoms.pkl` & `dlomix-0.1.1/src/dlomix/data/processing/pickled_feature_dicts/saved_loss_atoms.pkl`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/processing/processors.py` & `dlomix-0.1.1/src/dlomix/data/processing/processors.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/data/retention_time.py` & `dlomix-0.1.1/src/dlomix/data/retention_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         features_to_extract (Optional[List[Union[Callable, str]]]): The features to extract from the dataset. Defaults to None.
         pad (bool): Whether to pad sequences to the maximum length. Defaults to True.
         padding_value (int): The value to use for padding sequences. Defaults to 0.
         alphabet (Dict): The alphabet used for encoding sequences. Defaults to ALPHABET_UNMOD.
         encoding_scheme (Union[str, EncodingScheme]): The encoding scheme to use for sequences. Defaults to EncodingScheme.UNMOD.
         processed (bool): Whether the dataset has been preprocessed. Defaults to False.
         enable_tf_dataset_cache (bool): Flag to indicate whether to enable TensorFlow Dataset caching (call `.cahce()` on the generate TF Datasets).
-        disable_cache (bool): Whether to disable Hugging Face datasets caching. Default is True.
+        disable_cache (bool): Whether to disable Hugging Face datasets caching. Default is False.
     """
 
     def __init__(
         self,
         data_source: Optional[Union[str, List]] = None,
         val_data_source: Optional[Union[str, List]] = None,
         test_data_source: Optional[Union[str, List]] = None,
@@ -49,15 +49,18 @@
         features_to_extract: Optional[List[Union[Callable, str]]] = None,
         pad: bool = True,
         padding_value: int = 0,
         alphabet: Dict = ALPHABET_UNMOD,
         encoding_scheme: Union[str, EncodingScheme] = EncodingScheme.UNMOD,
         processed: bool = False,
         enable_tf_dataset_cache: bool = False,
-        disable_cache: bool = True,
+        disable_cache: bool = False,
+        auto_cleanup_cache: bool = True,
+        num_proc: Optional[int] = None,
+        batch_processing_size: int = 1000,
     ):
         super().__init__(
             data_source,
             val_data_source,
             test_data_source,
             data_format,
             sequence_column,
@@ -72,8 +75,11 @@
             pad,
             padding_value,
             alphabet,
             encoding_scheme,
             processed,
             enable_tf_dataset_cache,
             disable_cache,
+            auto_cleanup_cache,
+            num_proc,
+            batch_processing_size,
         )
```

### Comparing `dlomix-0.1.0/src/dlomix/eval/rt_eval.py` & `dlomix-0.1.1/src/dlomix/eval/rt_eval.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/layers/attention.py` & `dlomix-0.1.1/src/dlomix/layers/attention.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/losses/intensity.py` & `dlomix-0.1.1/src/dlomix/losses/intensity.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/models/base.py` & `dlomix-0.1.1/src/dlomix/models/base.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/models/deepLC.py` & `dlomix-0.1.1/src/dlomix/models/deepLC.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/models/prosit.py` & `dlomix-0.1.1/src/dlomix/models/prosit.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,9 +353,11 @@
         elif isinstance(keys_mapping, list):
             keys = keys_mapping
 
         for key_in_inputs in keys:
             # get the input under the specified key if exists
             single_input = inputs.get(key_in_inputs, None)
             if single_input is not None:
+                if single_input.ndim == 1:
+                    single_input = tf.expand_dims(single_input, axis=-1)
                 collected_values.append(single_input)
         return collected_values
```

### Comparing `dlomix-0.1.0/src/dlomix/pipelines/pipeline.py` & `dlomix-0.1.1/src/dlomix/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/reports/IntensityReport.py` & `dlomix-0.1.1/src/dlomix/reports/IntensityReport.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/reports/Report.py` & `dlomix-0.1.1/src/dlomix/reports/Report.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/reports/RetentionTimeReport.py` & `dlomix-0.1.1/src/dlomix/reports/RetentionTimeReport.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/reports/RetentionTimeReportModelComparisonWandb.py` & `dlomix-0.1.1/src/dlomix/reports/RetentionTimeReportModelComparisonWandb.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/reports/RetentionTimeReportRunComparisonWandb.py` & `dlomix-0.1.1/src/dlomix/reports/RetentionTimeReportRunComparisonWandb.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix/reports/postprocessing.py` & `dlomix-0.1.1/src/dlomix/reports/postprocessing.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/src/dlomix.egg-info/PKG-INFO` & `dlomix-0.1.1/src/dlomix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlomix
-Version: 0.1.0
+Version: 0.1.1
 Summary: Deep Learning for Proteomics
 Home-page: https://github.com/wilhelm-lab/dlomix
 Author: Omar Shouman
 Author-email: o.shouman@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -70,16 +70,14 @@
 -  `eval`: classes for evaluating models and reporting results
 -  `layers`: custom layers used for building models, based on `tf.keras.layers.Layer`
 -  `losses`: custom losses to be used for training with `model.fit()`
 - `models`: common model architectures for the relevant use-cases based on `tf.keras.Model` to allow for using the Keras training API
 -  `pipelines`: an exemplary high-level pipeline implementation
 -  `reports`: classes for generating reports related to the different tasks
 -  `constants.py`: constants and configuration values
--  `utils.py`: utility functions
-
 
 
 **Use-cases**
 
 - Retention Time Prediction:
     - a regression problem where the retention time of a peptide sequence is to be predicted.
```

### Comparing `dlomix-0.1.0/src/dlomix.egg-info/SOURCES.txt` & `dlomix-0.1.1/src/dlomix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/tests/test_datasets.py` & `dlomix-0.1.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/tests/test_losses.py` & `dlomix-0.1.1/tests/test_losses.py`

 * *Files identical despite different names*

### Comparing `dlomix-0.1.0/tests/test_models.py` & `dlomix-0.1.1/tests/test_models.py`

 * *Files identical despite different names*

