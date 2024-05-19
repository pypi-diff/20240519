# Comparing `tmp/repoqa-0.1.0rc2.tar.gz` & `tmp/repoqa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repoqa-0.1.0rc2.tar", last modified: Wed Apr 24 19:42:48 2024, max compression
+gzip compressed data, was "repoqa-0.1.1.tar", last modified: Sun May 19 19:28:07 2024, max compression
```

## Comparing `repoqa-0.1.0rc2.tar` & `repoqa-0.1.1.tar`

### file list

```diff
@@ -1,84 +1,92 @@
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3194 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/.gitignore
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      913 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/.pre-commit-config.yaml
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    11558 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/LICENSE
--rw-r--r--   0 ganler    (1000) ganler    (1000)     4439 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/PKG-INFO
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3683 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/README.md
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/docs/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2575 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/docs/curate_dataset.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      825 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/docs/dev_note.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      244 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/pyproject.toml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/repoqa/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      208 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      414 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa/_version.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    10634 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/compute_score.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1659 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/data.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      600 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/metric.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/repoqa/provider/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      136 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/repoqa/provider/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1021 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/repoqa/provider/anthropic.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      330 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/base.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1470 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/hf.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1018 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/openai.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/repoqa/provider/request/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      317 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/request/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2037 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/repoqa/provider/request/anthropic.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1703 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/request/openai.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1376 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/provider/vllm.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    12885 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/repoqa/search_needle_function.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1918 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/repoqa/utility.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/repoqa.egg-info/
--rw-r--r--   0 ganler    (1000) ganler    (1000)     4439 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/PKG-INFO
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1815 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/SOURCES.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        1 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/dependency_links.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      134 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/entry_points.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      149 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/requires.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-24 19:42:48.000000 repoqa-0.1.0rc2/repoqa.egg-info/top_level.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)       73 2024-04-24 19:42:11.000000 repoqa-0.1.0rc2/requirements.txt
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/results/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)       13 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/results/.gitignore
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      675 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/results/README.md
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/scripts/cherrypick/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      720 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/cherrypick/README.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    10742 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/cherrypick/lists.json
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/scripts/curate/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1987 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dataset_ensemble_clone.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2480 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/dataset_ensemble_gh_api.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4086 2024-04-19 09:21:06.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/cpp.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.244574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/data/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/data/.gitignore
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1652 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/java-lib/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)  6013426 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2984 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/pom.xml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.240574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     5415 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2199 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/java.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2610 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/python.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     5579 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/rust.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4294 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/dep_analysis/typescript.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4163 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/function_analysis.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3980 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/curate/github_fetch.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1589 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/merge_annotation.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1173 2024-04-16 20:28:57.000000 repoqa-0.1.0rc2/scripts/curate/merge_dep.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4756 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/needle_annotation.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3223 2024-04-19 09:21:06.000000 repoqa-0.1.0rc2/scripts/curate/needle_selection.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      129 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/requirements.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      320 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/curate/utility.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/demos/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      751 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/demos/model_request_oai.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/dev/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)       84 2024-02-25 13:11:01.000000 repoqa-0.1.0rc2/scripts/dev/license-hdr.txt
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-04-24 19:42:48.248574 repoqa-0.1.0rc2/scripts/misc/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      877 2024-04-06 02:26:24.000000 repoqa-0.1.0rc2/scripts/misc/estimate_max_char.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2432 2024-04-24 00:46:21.000000 repoqa-0.1.0rc2/scripts/misc/repo_token_size.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      891 2024-04-24 19:42:48.252574 repoqa-0.1.0rc2/setup.cfg
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3194 2024-04-24 00:46:21.000000 repoqa-0.1.1/.gitignore
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      913 2024-04-24 00:46:21.000000 repoqa-0.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    11558 2024-04-24 00:46:21.000000 repoqa-0.1.1/LICENSE
+-rw-r--r--   0 ganler    (1000) ganler    (1000)     6273 2024-05-19 19:28:07.287425 repoqa-0.1.1/PKG-INFO
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     5375 2024-05-19 19:27:40.000000 repoqa-0.1.1/README.md
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/docs/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2575 2024-04-24 00:46:21.000000 repoqa-0.1.1/docs/curate_dataset.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      825 2024-04-24 00:46:21.000000 repoqa-0.1.1/docs/dev_note.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      244 2024-04-24 00:46:21.000000 repoqa-0.1.1/pyproject.toml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/repoqa/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      208 2024-04-24 00:46:21.000000 repoqa-0.1.1/repoqa/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      411 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa/_version.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    13467 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/compute_score.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1639 2024-04-26 09:19:08.000000 repoqa-0.1.1/repoqa/data.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      600 2024-04-24 00:46:21.000000 repoqa-0.1.1/repoqa/metric.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/repoqa/provider/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      136 2024-04-24 19:42:11.000000 repoqa-0.1.1/repoqa/provider/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1023 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/anthropic.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      332 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/base.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1435 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/google.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2487 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/hf.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1522 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/openai.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/repoqa/provider/request/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      649 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/request/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2038 2024-04-26 09:19:08.000000 repoqa-0.1.1/repoqa/provider/request/anthropic.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1857 2024-04-24 22:48:39.000000 repoqa-0.1.1/repoqa/provider/request/google.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1704 2024-04-26 09:19:08.000000 repoqa-0.1.1/repoqa/provider/request/openai.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1620 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/vllm.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    13669 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/search_needle_function.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2527 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/utility.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/repoqa.egg-info/
+-rw-r--r--   0 ganler    (1000) ganler    (1000)     6273 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/PKG-INFO
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2040 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/SOURCES.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        1 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/dependency_links.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      134 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/entry_points.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      234 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/requires.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/top_level.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      129 2024-05-19 19:27:40.000000 repoqa-0.1.1/requirements.txt
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/results/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)       13 2024-04-24 00:46:21.000000 repoqa-0.1.1/results/.gitignore
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      675 2024-04-24 00:46:21.000000 repoqa-0.1.1/results/README.md
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/cherrypick/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      720 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/cherrypick/README.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    12868 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/cherrypick/lists.json
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1986 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/curate/dataset_ensemble_clone.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2480 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/dataset_ensemble_gh_api.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4086 2024-04-19 09:21:06.000000 repoqa-0.1.1/scripts/curate/dep_analysis/cpp.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/data/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/data/.gitignore
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/go-analysis/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3118 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/curate/dep_analysis/go-analysis/dependency_analysis.go
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2843 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/curate/dep_analysis/go.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1652 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/java-lib/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)  6013426 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2984 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/pom.xml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     5415 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2199 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2610 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/python.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     5579 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/rust.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4294 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/dep_analysis/typescript.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4163 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/function_analysis.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3980 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/github_fetch.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1589 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/merge_annotation.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1173 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/merge_dep.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4756 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/needle_annotation.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3223 2024-04-19 09:21:06.000000 repoqa-0.1.1/scripts/curate/needle_selection.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3378 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/curate/obfuscate_nl.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      129 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/requirements.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      320 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/utility.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/demos/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      751 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/demos/model_request_oai.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/dev/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)       84 2024-02-25 13:11:01.000000 repoqa-0.1.1/scripts/dev/license-hdr.txt
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/eval/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      502 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/eval/recompute_all_scores.sh
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/misc/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      877 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/misc/estimate_max_char.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2432 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/misc/repo_token_size.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      980 2024-05-19 19:28:07.287425 repoqa-0.1.1/setup.cfg
```

### Comparing `repoqa-0.1.0rc2/.gitignore` & `repoqa-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/.pre-commit-config.yaml` & `repoqa-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/LICENSE` & `repoqa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/docs/curate_dataset.md` & `repoqa-0.1.1/docs/curate_dataset.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/docs/dev_note.md` & `repoqa-0.1.1/docs/dev_note.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/repoqa/compute_score.py` & `repoqa-0.1.1/repoqa/compute_score.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 from collections import defaultdict
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
+import tempdir
 from rich.console import Console
 from rich.table import Table
+from transformers import AutoConfig
 from tree_sitter_languages import get_language, get_parser
 
 from repoqa.data import get_repoqa_data
 from repoqa.metric import compute_function_similarity
-from repoqa.utility import FUNCTION_QUERY, progress
+from repoqa.utility import COMMENT_QUERY, FUNCTION_QUERY, progress
 
 LANGUAGES = list(FUNCTION_QUERY.keys())
 THRESHOLDS = [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
 
 
 class Result(Enum):
     BEST_MATCH = "best_match"
@@ -55,32 +57,48 @@
         num_samples_it = iter(num_samples)
 
     return np.array(
         [estimator(int(n), int(c), k) for n, c in zip(num_samples_it, num_correct)]
     )
 
 
+def remove_comments(source_code: str, lang: str) -> str:
+    source_bytes = bytes(source_code, "utf8")
+    parser = get_parser(lang)
+    tree = parser.parse(source_bytes)
+    root_node = tree.root_node
+
+    # Remove comments from source code
+    capture_list = []
+    for query_str in COMMENT_QUERY[lang]:
+        comment_query = get_language(lang).query(query_str)
+        capture_list += comment_query.captures(root_node)
+
+    capture_list.sort(key=lambda cap: cap[0].start_byte, reverse=True)
+
+    for node, _ in capture_list:
+        source_bytes = source_bytes[: node.start_byte] + source_bytes[node.end_byte :]
+
+    return source_bytes.decode("utf-8")
+
+
 def sanitize_output(model_output: str, lang: str) -> str:
-    search_pattern = r"```(.*?)```"
-    code_blocks = re.findall(search_pattern, model_output, re.DOTALL)
+    model_output = model_output.strip()
+    search_pattern = r"^```(?:\w+)?\s*\n(.*?)(?=^```)```"
+    code_blocks = re.findall(search_pattern, model_output, re.DOTALL | re.MULTILINE)
 
     parser = get_parser(lang)
     fn_query = get_language(lang).query(FUNCTION_QUERY[lang])
 
     # If not code blocks found, simply return model output
     if not code_blocks:
         return model_output
 
     processed_blocks = []
     for block in code_blocks:
-        # Clean up language specific markdown blocks
-        lines = block.split("\n")
-        if lines[0] == lang:
-            block = "\n".join(lines[1:])
-
         processed_blocks.append(block)
 
         # Try to use tree-sitter to parse if possible
         try:
             block_bytes = bytes(block, "utf8")
             tree = parser.parse(block_bytes)
             for capture in fn_query.captures(tree.root_node):
@@ -93,17 +111,17 @@
     # no valid functions found by tree-sitter approach return first block
     return processed_blocks[0]
 
 
 def print_result_table(model_name, pass_results):
     # Printing scores in a table
     table = Table(title=f"Scores (%) of {model_name} at different thresholds")
-    table.add_column("Language", justify="center", style="bold magenta")
+    table.add_column("Threshold", justify="center", style="bold magenta")
     for threshold in THRESHOLDS:
-        table.add_column(f"thresh={threshold}", justify="center")
+        table.add_column(f"{threshold}", justify="center")
 
     # Prepare data to determine the maximum values for each threshold
     threshold_scores = {threshold: [] for threshold in THRESHOLDS}
     for lang_results in pass_results.values():
         for thresh, value in lang_results.items():
             threshold_scores[thresh].append(value["pass@1"])
 
@@ -113,47 +131,55 @@
     }
     min_scores = {
         threshold: min(scores) for threshold, scores in threshold_scores.items()
     }
 
     # Fill the table rows
     for language, lang_results in pass_results.items():
-        row = [language]
+        row = [("⭐" if language == "all" else "") + language]
         for threshold, value in lang_results.items():
             score = value["pass@1"]
             formatted_score = f"{100 * score:.1f}"
             if max_scores[threshold] - score < 0.01:
                 formatted_score = f"[bold green]{formatted_score}[/]"
             elif score - min_scores[threshold] < 0.01:
                 formatted_score = f"[bold red]{formatted_score}[/]"
             row.append(formatted_score)
         if language == "all":
-            row = [f"[bold on white]{r}[/]" for r in row]
+            row = [f"[bold yellow]{r}[/]" for r in row]
         table.add_row(*row)
 
     Console().print(table)
 
 
 def needle_evaluator(
-    model_output: str, ground_truth: str, repo_info: Dict, lang: str
+    model_output: str,
+    ground_truth: str,
+    repo_info: Dict,
+    lang: str,
+    ignore_comments: bool,
 ) -> Tuple[Result, str, float]:
     contents = repo_info["content"]
     needles = repo_info["needles"]
 
     best_target = None
     best_similarity = 0
     sanitized_output = sanitize_output(model_output, lang)
+    if ignore_comments:
+        sanitized_output = remove_comments(sanitized_output, lang)
     for needle in needles:
         current_path = needle["path"]
         current_name = needle["name"]
         current_func = "\n".join(
             contents[current_path].split("\n")[
                 needle["start_line"] : needle["end_line"]
             ]
         )
+        if ignore_comments:
+            current_func = remove_comments(current_func, lang)
 
         current_similarity = compute_function_similarity(sanitized_output, current_func)
         if current_similarity > best_similarity:
             best_similarity = current_similarity
             best_target = current_name
 
     if best_target == ground_truth:
@@ -188,27 +214,67 @@
                 for k in [1, 10, 100]
                 if total.min() >= k
             }
             current_result[threshold] = pass_at_k
         all_results[language] = current_result
 
 
-def compute_score(model_name: str, dataset: Dict, model_output: List[Dict]) -> Dict:
+def fetch_hf_context(model_name: str) -> str:
+    # Retrieved from https://github.com/vllm-project/vllm/blob/main/vllm/config.py#L1073
+    possible_keys = [
+        # OPT
+        "max_position_embeddings",
+        # GPT-2
+        "n_positions",
+        # MPT
+        "max_seq_len",
+        # ChatGLM2
+        "seq_length",
+        # Command-R
+        "model_max_length",
+        # Others
+        "max_sequence_length",
+        "max_seq_length",
+        "seq_len",
+    ]
+    try:
+        with tempdir.TempDir() as temp_dir:
+            config = AutoConfig.from_pretrained(
+                model_name,
+                cache_dir=temp_dir,
+                force_download=True,
+                trust_remote_code=True,
+            ).to_dict()
+            longest_context = 0
+            for key in possible_keys:
+                if key in config:
+                    longest_context = max(config[key], longest_context)
+            if not (longest_context):
+                return "N/A"
+            return str(int(longest_context / 1024)) + "k"
+    except Exception as err:
+        print(f"fetching failed... Reason:\n{err}")
+        return "N/A"
+
+
+def compute_score(
+    model_name: str, dataset: Dict, model_output: List[Dict], ignore_comments: bool
+) -> Dict:
     evaluation_result = defaultdict(list)
     with progress(f"Scoring {model_name}") as pbar:
         for result in pbar.track(model_output):
             lang = result["language"]
             repo_name = result["repo"]
             model_outputs = result["output"]
             ground_truth = result["name"]
             repo_info = _get_repo(dataset[lang], repo_name)
 
             model_output = model_outputs[0]
             verdict, best_target, best_similarity = needle_evaluator(
-                model_output, ground_truth, repo_info, lang
+                model_output, ground_truth, repo_info, lang, ignore_comments
             )
 
             is_best_similar = False
             if verdict == Result.BEST_MATCH:
                 is_best_similar = True
 
             current_task = {
@@ -251,16 +317,36 @@
 
     compute_language_results(evaluation_result, pass_results)
     print_result_table(model_name, pass_results)
 
     output_json = {}
     model_json = {}
     model_json["eval_date"] = str(datetime.now())
-    # TODO(@Tom): Include trainning and evaluation size
-    model_json["train_size"] = None
+
+    # hardcode paid models
+    if "/" in model_name:
+        if model_name.startswith("bigcode/starcoder2"):
+            train_context = "16k"
+        else:
+            train_context = fetch_hf_context(model_name)
+    elif model_name.startswith("gpt-4-turbo") or model_name.startswith("gpt-4o-"):
+        train_context = "128k"
+    elif model_name.startswith("gpt-3.5-"):
+        train_context = "16k"
+    elif model_name.startswith("gemini-1.5-pro") or model_name.startswith(
+        "gemini-1.5-flash"
+    ):
+        train_context = "1000k"
+    elif model_name.startswith("gemini-1.0-pro"):
+        train_context = "32k"
+    elif model_name.startswith("claude-3-"):
+        train_context = "200k"
+    else:
+        train_context = "N/A"
+    model_json["train_size"] = train_context
     model_json["scores"] = pass_results
     model_json["results"] = evaluation_result
 
     output_json[model_name] = model_json
 
     return output_json
 
@@ -293,30 +379,32 @@
             print(f"Backup {result_path} to {new_path}")
 
     if not os.path.isfile(result_path):
         with open(result_path, "w") as f:
             json.dump(output_json, f)
 
 
-def compute_main(model_output_path: str, dataset_path: str = None):
+def compute_main(
+    model_output_path: str, ignore_comments: bool = False, dataset_path: str = None
+):
     if dataset_path is None:
         dataset = get_repoqa_data()
     else:
         with open(dataset_path, "r") as dataset_f:
             dataset = json.load(dataset_f)
 
     model_outputs = []
     with open(model_output_path, "r") as output_f:
         for line in output_f:
             model_outputs.append(json.loads(line))
 
     file_base, _ = os.path.splitext(model_output_path)
     result_path = file_base + "-SCORES.json"
     model_name = get_model_name(model_output_path)
-    output_json = compute_score(model_name, dataset, model_outputs)
+    output_json = compute_score(model_name, dataset, model_outputs, ignore_comments)
     save_json(output_json, result_path)
 
 
 def main():
     from fire import Fire
 
     Fire(compute_main)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `repoqa-0.1.0rc2/repoqa/data.py` & `repoqa-0.1.1/repoqa/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,8 +43,8 @@
             f.write(repoqa_data)
 
     return cache_path
 
 
 def get_repoqa_data():
     with open(_get_repoqa_data_ready_path(), "r") as f:
-        return [json.loads(line) for line in f]
+        return json.load(f)
```

### Comparing `repoqa-0.1.0rc2/repoqa/metric.py` & `repoqa-0.1.1/repoqa/metric.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/repoqa/provider/anthropic.py` & `repoqa-0.1.1/repoqa/provider/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class AnthropicProvider(BaseProvider):
     def __init__(self, model):
         self.model = model
         self.client = Client(api_key=os.getenv("ANTHROPIC_KEY"))
 
     def generate_reply(
-        self, question, n=1, max_tokens=1024, temperature=0, system_msg=None
+        self, question, n=1, max_tokens=1024, temperature=0.0, system_msg=None
     ) -> List[str]:
         assert temperature != 0 or n == 1, "n must be 1 when temperature is 0"
         replies = []
         for _ in range(n):
             reply = make_auto_request(
                 self.client,
                 message=question,
```

### Comparing `repoqa-0.1.0rc2/repoqa/provider/hf.py` & `repoqa-0.1.1/repoqa/provider/hf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,75 @@
 # SPDX-FileCopyrightText: (c) 2024 EvalPlus Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import List
 
 import torch
+from stop_sequencer import StopSequencer
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from repoqa.provider.base import BaseProvider
-from repoqa.provider.request import construct_message_list
+from repoqa.provider.request import construct_message_list, hacky_assistant_stop_seq
 
 
 class HfProvider(BaseProvider):
-    def __init__(self, model, trust_remote_code=False):
+    def __init__(self, model, trust_remote_code=False, attn_implementation=None):
         self.tokenizer = AutoTokenizer.from_pretrained(model)
         self.hf_model = AutoModelForCausalLM.from_pretrained(
-            model, trust_remote_code=trust_remote_code
+            model,
+            trust_remote_code=trust_remote_code,
+            attn_implementation=attn_implementation,
+            torch_dtype="auto",
         ).cuda()
+        self.stop_sequencer = StopSequencer(
+            self.hf_model,
+            model_type="causal",  # or seq2seq
+            tokenizer=self.tokenizer,
+        )
+        self.stop_seq = []
+        if self.tokenizer.chat_template:
+            self.stop_seq.append(hacky_assistant_stop_seq(self.tokenizer))
 
     @torch.inference_mode()
     def generate_reply(
-        self, question, n=1, max_tokens=1024, temperature=0, system_msg=None
+        self, question, n=1, max_tokens=1024, temperature=0.0, system_msg=None
     ) -> List[str]:
         assert temperature != 0 or n == 1, "n must be 1 when temperature is 0"
+
         prompt_tokens = self.tokenizer.apply_chat_template(
-            construct_message_list(question, system_msg), return_tensors="pt"
+            construct_message_list(question, system_msg),
+            return_tensors="pt",
+            add_generation_prompt=True,
         ).cuda()
-        output_text = self.hf_model.generate(
+
+        hf_model = self.hf_model
+        input_length = prompt_tokens.size(-1)
+        if self.stop_seq:
+            hf_model = self.stop_sequencer.register_stop_texts(
+                stop_texts=self.stop_seq,
+                input_length=input_length,
+            )
+
+        gen_args = {"do_sample": False}
+        if temperature > 0:
+            gen_args["do_sample"] = True
+            gen_args["temperature"] = temperature
+
+        output_text = hf_model.generate(
             input_ids=prompt_tokens,
             max_new_tokens=max_tokens,
             num_return_sequences=n,
-            temperature=temperature,
             pad_token_id=self.tokenizer.eos_token_id,
             use_cache=True,
+            **gen_args,
         )
 
         gen_strs = [
             self.tokenizer.decode(
-                x, skip_special_tokens=True, clean_up_tokenization_spaces=False
+                x[input_length:],
+                skip_special_tokens=True,
+                clean_up_tokenization_spaces=False,
             )
             for x in output_text
         ]
         return gen_strs
```

### Comparing `repoqa-0.1.0rc2/repoqa/provider/openai.py` & `repoqa-0.1.1/repoqa/provider/google.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 # SPDX-FileCopyrightText: (c) 2024 EvalPlus Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 from typing import List
 
-from openai import Client
+import google.generativeai as genai
 
 from repoqa.provider.base import BaseProvider
-from repoqa.provider.request.openai import make_auto_request
+from repoqa.provider.request.google import make_auto_request
 
 
-class OpenAIProvider(BaseProvider):
-    def __init__(self, model, base_url: str = None):
+class GoogleProvider(BaseProvider):
+    def __init__(self, model):
+        genai.configure(api_key=os.getenv("GOOGLE_API_KEY"))
         self.model = model
-        self.client = Client(
-            api_key=os.getenv("OPENAI_API_KEY", "none"), base_url=base_url
-        )
+        self.client = genai.GenerativeModel(model)
 
     def generate_reply(
-        self, question, n=1, max_tokens=1024, temperature=0, system_msg=None
+        self, question, n=1, max_tokens=1024, temperature=0.0, system_msg=None
     ) -> List[str]:
         assert temperature != 0 or n == 1, "n must be 1 when temperature is 0"
         replies = make_auto_request(
             self.client,
-            message=question,
-            model=self.model,
-            temperature=temperature,
+            question,
+            self.model,
             n=n,
             max_tokens=max_tokens,
+            temperature=temperature,
             system_msg=system_msg,
         )
 
-        return [reply.message.content for reply in replies.choices]
+        if len(replies.candidates) != n:
+            print(f"[WARNING] # replies = {len(replies.candidates)} != {n = }")
+
+        ret_texts = []
+        for candidate in replies.candidates:
+            parts = candidate.content.parts
+            if parts:
+                ret_texts.append(parts[0].text)
+            else:
+                print("Empty response!")
+                ret_texts.append("")
+                print(f"{candidate.safety_ratings = }")
+
+        return ret_texts + [""] * (n - len(ret_texts))
```

### Comparing `repoqa-0.1.0rc2/repoqa/provider/request/anthropic.py` & `repoqa-0.1.1/repoqa/provider/request/anthropic.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             signal.signal(signal.SIGALRM, handler)
             signal.alarm(100)
             ret = make_request(client, *args, **kwargs)
             signal.alarm(0)
         except anthropic.RateLimitError:
             print("Rate limit exceeded. Waiting...")
             signal.alarm(0)
-            time.sleep(5)
+            time.sleep(10)
         except anthropic.APIConnectionError:
             print("API connection error. Waiting...")
             signal.alarm(0)
             time.sleep(5)
         except anthropic.InternalServerError:
             print("Internal server error. Waiting...")
             signal.alarm(0)
```

### Comparing `repoqa-0.1.0rc2/repoqa/provider/request/openai.py` & `repoqa-0.1.1/repoqa/provider/request/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             signal.signal(signal.SIGALRM, handler)
             signal.alarm(100)
             ret = make_request(*args, **kwargs)
             signal.alarm(0)
         except openai.RateLimitError:
             print("Rate limit exceeded. Waiting...")
             signal.alarm(0)
-            time.sleep(5)
+            time.sleep(10)
         except openai.APIConnectionError:
             print("API connection error. Waiting...")
             signal.alarm(0)
             time.sleep(5)
         except openai.APIError as e:
             print(e)
             signal.alarm(0)
```

### Comparing `repoqa-0.1.0rc2/repoqa/provider/vllm.py` & `repoqa-0.1.1/repoqa/provider/vllm.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,40 +4,47 @@
 
 from typing import List
 
 from transformers import AutoTokenizer
 from vllm import LLM, SamplingParams
 
 from repoqa.provider.base import BaseProvider
-from repoqa.provider.request import construct_message_list
+from repoqa.provider.request import construct_message_list, hacky_assistant_stop_seq
 
 
 class VllmProvider(BaseProvider):
     def __init__(
-        self, model, tensor_parallel_size, max_model_len, trust_remote_code=False
+        self, model, tensor_parallel_size, max_model_len=None, trust_remote_code=False
     ):
         self.tokenizer = AutoTokenizer.from_pretrained(model)
         self.llm = LLM(
             model=model,
             tensor_parallel_size=tensor_parallel_size,
             max_model_len=max_model_len,
             trust_remote_code=trust_remote_code,
         )
+        self.stop_seq = []
+        if self.tokenizer.chat_template:
+            self.stop_seq.append(hacky_assistant_stop_seq(self.tokenizer))
 
     def generate_reply(
-        self, question, n=1, max_tokens=1024, temperature=0, system_msg=None
+        self, question, n=1, max_tokens=1024, temperature=0.0, system_msg=None
     ) -> List[str]:
         assert temperature != 0 or n == 1, "n must be 1 when temperature is 0"
+
         prompt = self.tokenizer.apply_chat_template(
-            construct_message_list(question, system_msg), tokenize=False
+            construct_message_list(question, system_msg),
+            tokenize=False,
+            add_generation_prompt=True,
         )
         vllm_outputs = self.llm.generate(
             [prompt],
             SamplingParams(
                 temperature=temperature,
                 max_tokens=max_tokens,
+                stop=self.stop_seq,
             ),
             use_tqdm=False,
         )
 
-        gen_strs = [x.outputs[0].text.replace("\t", "    ") for x in vllm_outputs]
+        gen_strs = [x.outputs[0].text for x in vllm_outputs]
         return gen_strs
```

### Comparing `repoqa-0.1.0rc2/repoqa/search_needle_function.py` & `repoqa-0.1.1/repoqa/search_needle_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,44 +26,49 @@
 
 INSTRUCTION = (
     "Based on the function description and code context,"
     " please retrieve and repeat the exact described function from the code context in a code block wrapped by ```:"
 )
 
 
+# Count number of tokens ignoring null byte (used for obfuscate-nl)
+def count_tokens(tokens: List[str]) -> int:
+    return len([x for x in tokens if x != "<0x00>"])
+
+
 def _backward_tokenizable_lines(lines, tokenizer, max_tokens):
     """Return the text and tokens from bottom to top"""
     text = ""
     ntokens = 0
     is_break = False
     for line in reversed(lines):
-        new_ntokens = len(tokenizer.tokenize(line + "\n"))
+        new_ntokens = count_tokens(tokenizer.tokenize(line + "\n"))
         if ntokens + new_ntokens > max_tokens:
             is_break = True
             break
         text = line + "\n" + text
         ntokens += new_ntokens
     return text, ntokens, is_break
 
 
 def _forward_tokenizable_lines(lines, tokenizer, max_tokens):
     """Return the text and tokens from top to bottom"""
     text = ""
     ntokens = 0
     is_break = False
     for line in lines:
-        new_ntokens = len(tokenizer.tokenize(line + "\n"))
+        new_ntokens = count_tokens(tokenizer.tokenize(line + "\n"))
         if ntokens + new_ntokens > max_tokens:
             is_break = True
             break
         text += line + "\n"
         ntokens += new_ntokens
     if is_break:
         text = text + "...\n"
-        ntokens += len(tokenizer.tokenize("...\n"))
+        ntokens += count_tokens(tokenizer.tokenize("...\n"))
     return text, ntokens, is_break
 
 
 def make_code_context(
     needle,
     file_content_list: List[Tuple[str, str]],
     position_ratio,
@@ -83,15 +88,15 @@
     needle_file_idx, needle_file_content = [
         (i, content)
         for i, (f, content) in enumerate(file_content_list)
         if f == needle["path"]
     ][0]
 
     needle_code = needle_file_content[needle["start_byte"] : needle["end_byte"]]
-    ntoken_needle = len(tokenizer.tokenize(needle_code))
+    ntoken_needle = count_tokens(tokenizer.tokenize(needle_code))
 
     prefix_size = int(code_context_size * position_ratio - ntoken_needle / 2)
     suffix_size = code_context_size - ntoken_needle - prefix_size
 
     # handling prefix of the needle file
     code_prefix, ntokens, is_break = _backward_tokenizable_lines(
         [COMMENT_PREFIX[language] + " Path: " + needle["path"]]
@@ -129,15 +134,21 @@
             tokenizer,
             suffix_size,
         )
         code_suffix += suffix
         suffix_size -= ntokens
         index += 1
 
+    # Remove all null characters from all three portions (obfuscate-nl)
+    code_prefix = code_prefix.replace("\0", "")
+    needle_code = needle_code.replace("\0", "")
+    code_suffix = code_suffix.replace("\0", "")
+
     code_context = code_prefix + needle_code + code_suffix
+
     needle_token_start = len(tokenizer.tokenize(code_prefix))
     needle_token_end = needle_token_start + len(tokenizer.tokenize(needle_code))
     code_context_ntokens = needle_token_end + len(tokenizer.tokenize(code_suffix))
 
     return {
         "code_context": code_context,
         "needle_token_start": needle_token_start,
@@ -159,18 +170,20 @@
     base_url: str = None,
     backend: str = None,
     tensor_parallel_size: int = 1,
     code_context_size: int = 16 * 1024,
     max_new_tokens: int = 1024,
     result_dir: str = "results",
     languages: List[str] = None,
-    caching: bool = False,  # if enabled, will cache the tasks which can be used to resume
+    caching: bool = True,  # if enabled, will cache the tasks which can be used to resume
     system_message: str = None,
     dataset_path: str = None,
+    ignore_comments: bool = False,
     trust_remote_code: bool = False,
+    attn_implementation=None,
 ):
     if backend is None:
         if base_url is not None:
             backend = "openai"
         else:
             backend = "vllm"
         print(f"Using {backend} as the backend")
@@ -317,15 +330,25 @@
     elif backend == "anthropic":
         from repoqa.provider.anthropic import AnthropicProvider
 
         engine = AnthropicProvider(model)
     elif backend == "hf":
         from repoqa.provider.hf import HfProvider
 
-        engine = HfProvider(model, trust_remote_code=trust_remote_code)
+        engine = HfProvider(
+            model,
+            trust_remote_code=trust_remote_code,
+            attn_implementation=attn_implementation,
+        )
+    elif backend == "google":
+        from repoqa.provider.google import GoogleProvider
+
+        engine = GoogleProvider(model)
+    else:
+        raise ValueError(f"Unknown backend: {backend}")
 
     if not system_message:
         print("🔥 System message is disabled")
         system_message = None
 
     with open(model_output_path, "a") as f_out:
         with progress(f"Running {model}") as pbar:
@@ -347,15 +370,15 @@
                 result = {**task, "output": replies}
                 f_out.write(json.dumps(result) + "\n")
                 f_out.flush()
                 model_outputs.append(result)
 
     file_base, _ = os.path.splitext(model_output_path)
     result_path = file_base + "-SCORES.json"
-    output_json = compute_score(model, dataset, model_outputs)
+    output_json = compute_score(model, dataset, model_outputs, ignore_comments)
     save_json(output_json, result_path)
 
 
 def main():
     from fire import Fire
 
     Fire(evaluate_model)
```

### Comparing `repoqa-0.1.0rc2/repoqa/utility.py` & `repoqa-0.1.1/repoqa/utility.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,25 +12,50 @@
 
 FUNCTION_QUERY = {
     "python": "(function_definition name: (_)) @fdef",
     "java": "(method_declaration name: (_)) @fdef",
     "typescript": "(function_declaration name: (_)) @fdef",
     "rust": "(function_item name: (_)) @fdef",
     "cpp": "(function_definition declarator: (function_declarator declarator: (identifier))) @fdef",
+    "go": "(function_declaration name: (_)) @fdef",
 }
 
 COMMENT_QUERY = {
     "python": [
         "(block (expression_statement (string) @docstring))",
         "(comment) @comment",
     ],
     "java": ["(line_comment) @comment", "(block_comment) @comment"],
     "cpp": ["(comment) @comment"],
     "rust": ["(line_comment) @comment", "(block_comment) @comment"],
     "typescript": ["(comment) @comment"],
+    "go": ["(comment) @comment"],
+}
+
+FUNCTION_NAME_QUERY = {
+    "python": """
+        ((function_definition
+          name: (identifier) @function_name))
+    """,
+    "java": """
+        (method_declaration
+          name: (identifier) @method_name)
+    """,
+    "typescript": """
+        (function_declaration
+          name: (identifier) @function_name)
+    """,
+    "rust": """
+        (function_item
+          name: (identifier) @function_name)
+    """,
+    "cpp": """
+        (function_definition
+          name: (identifier) @function_name)
+    """,
 }
 
 
 def topological_sort(graph):
     # Stack to store the topological order
     stack = []
     # Set to keep track of visited nodes
```

### Comparing `repoqa-0.1.0rc2/repoqa.egg-info/SOURCES.txt` & `repoqa-0.1.1/repoqa.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,41 +19,47 @@
 repoqa.egg-info/dependency_links.txt
 repoqa.egg-info/entry_points.txt
 repoqa.egg-info/requires.txt
 repoqa.egg-info/top_level.txt
 repoqa/provider/__init__.py
 repoqa/provider/anthropic.py
 repoqa/provider/base.py
+repoqa/provider/google.py
 repoqa/provider/hf.py
 repoqa/provider/openai.py
 repoqa/provider/vllm.py
 repoqa/provider/request/__init__.py
 repoqa/provider/request/anthropic.py
+repoqa/provider/request/google.py
 repoqa/provider/request/openai.py
 results/.gitignore
 results/README.md
 scripts/cherrypick/README.md
 scripts/cherrypick/lists.json
 scripts/curate/dataset_ensemble_clone.py
 scripts/curate/dataset_ensemble_gh_api.py
 scripts/curate/function_analysis.py
 scripts/curate/github_fetch.py
 scripts/curate/merge_annotation.py
 scripts/curate/merge_dep.py
 scripts/curate/needle_annotation.py
 scripts/curate/needle_selection.py
+scripts/curate/obfuscate_nl.py
 scripts/curate/requirements.txt
 scripts/curate/utility.py
 scripts/curate/dep_analysis/cpp.py
+scripts/curate/dep_analysis/go.py
 scripts/curate/dep_analysis/java.py
 scripts/curate/dep_analysis/python.py
 scripts/curate/dep_analysis/rust.py
 scripts/curate/dep_analysis/typescript.py
 scripts/curate/dep_analysis/data/.gitignore
+scripts/curate/dep_analysis/go-analysis/dependency_analysis.go
 scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml
 scripts/curate/dep_analysis/java-analysis/pom.xml
 scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar
 scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java
 scripts/demos/model_request_oai.py
 scripts/dev/license-hdr.txt
+scripts/eval/recompute_all_scores.sh
 scripts/misc/estimate_max_char.py
 scripts/misc/repo_token_size.py
```

### Comparing `repoqa-0.1.0rc2/results/README.md` & `repoqa-0.1.1/results/README.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/cherrypick/README.md` & `repoqa-0.1.1/scripts/cherrypick/README.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/cherrypick/lists.json` & `repoqa-0.1.1/scripts/cherrypick/lists.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'go'": "[OrderedDict([('repo', 'junegunn/fzf'), ('commit_sha', "*

 * *         "'e352b6887849cb6c3c8ae1d98ed357f94273e90a'), ('entrypoint_path', 'src'), ('topic', "*

 * *         "'command-line tool')]), OrderedDict([('repo', 'fatedier/frp'), ('commit_sha', "*

 * *         "'eaae212d2d1b17360754afd9432c21640f15c832'), ('entrypoint_path', 'pkg'), ('topic', "*

 * *         "'reverse proxy')]), OrderedDict([('repo', 'caddyserver/caddy'), ('commit_sha', "*

 * *         "'4d6370bf92de163a53aec9081c5d5ae6614597a0'), ('entrypoint_path', […]*

```diff
@@ -57,14 +57,76 @@
         {
             "commit_sha": "17ef2a7f6c8a932498799b2a5ae5aab2869975c7",
             "entrypoint_path": "src/oatpp",
             "repo": "oatpp/oatpp",
             "topic": "web-framework"
         }
     ],
+    "go": [
+        {
+            "commit_sha": "e352b6887849cb6c3c8ae1d98ed357f94273e90a",
+            "entrypoint_path": "src",
+            "repo": "junegunn/fzf",
+            "topic": "command-line tool"
+        },
+        {
+            "commit_sha": "eaae212d2d1b17360754afd9432c21640f15c832",
+            "entrypoint_path": "pkg",
+            "repo": "fatedier/frp",
+            "topic": "reverse proxy"
+        },
+        {
+            "commit_sha": "4d6370bf92de163a53aec9081c5d5ae6614597a0",
+            "entrypoint_path": "modules",
+            "repo": "caddyserver/caddy",
+            "topic": "web server"
+        },
+        {
+            "commit_sha": "2127c0a1ce50a66d61d78496033b15ef5cb5e250",
+            "entrypoint_path": "internal",
+            "repo": "nsqio/nsq",
+            "topic": "messaging platform"
+        },
+        {
+            "commit_sha": "3dfcec0a36dbf5ebc529ce0478076279cb975b71",
+            "entrypoint_path": "pkg",
+            "repo": "projectdiscovery/nuclei",
+            "topic": "vulnerability scanner"
+        },
+        {
+            "commit_sha": "80af149b023f4d9be68a643412183d389d73368d",
+            "entrypoint_path": "pkg",
+            "repo": "jesseduffield/lazydocker",
+            "topic": "docker management"
+        },
+        {
+            "commit_sha": "b337ae36e50092488c1899069f860007447fa17c",
+            "entrypoint_path": "core",
+            "repo": "zeromicro/go-zero",
+            "topic": "cloud-native microservices"
+        },
+        {
+            "commit_sha": "d81116382fcb9dddb79b02ed4b0da99e7aecb2ab",
+            "entrypoint_path": "src",
+            "repo": "schollz/croc",
+            "topic": "data transfer"
+        },
+        {
+            "commit_sha": "59f517bb7138acd4fffcced4560197e83a592fc2",
+            "entrypoint_path": "extractors",
+            "repo": "iawia002/lux",
+            "topic": "video download"
+        },
+        {
+            "commit_sha": "5f6bfc951f5df6f8d21e3e2ccf9693146216ef4d",
+            "entrypoint_path": "cmd",
+            "repo": "lima-vm/lima",
+            "topic": "Linux virtual machines"
+        }
+    ],
     "java": [
         {
             "commit_sha": "ee61e3f020351f0498dd3ff8f8386b96454a4dfe",
             "entrypoint_path": "gson/src/main/java",
             "repo": "google/gson",
             "topic": "developer-tool"
         },
```

### Comparing `repoqa-0.1.0rc2/scripts/curate/dataset_ensemble_clone.py` & `repoqa-0.1.1/scripts/curate/dataset_ensemble_clone.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,13 @@
                     gh_repo, entrypoint, lang_suffix
                 )
 
                 repo["content"] = {}
                 for path, abspath in files_to_include:
                     with open(abspath, "r") as f:
                         repo["content"][path] = f.read()
-
     with open(target_path, "w") as f_out:
         json.dump(lists, f_out)
 
 
 if __name__ == "__main__":
     Fire(main)
```

### Comparing `repoqa-0.1.0rc2/scripts/curate/dataset_ensemble_gh_api.py` & `repoqa-0.1.1/scripts/curate/dataset_ensemble_gh_api.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/cpp.py` & `repoqa-0.1.1/scripts/curate/dep_analysis/cpp.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml` & `repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar` & `repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/pom.xml` & `repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/pom.xml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java` & `repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/java.py` & `repoqa-0.1.1/scripts/curate/dep_analysis/java.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/python.py` & `repoqa-0.1.1/scripts/curate/dep_analysis/python.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/rust.py` & `repoqa-0.1.1/scripts/curate/dep_analysis/rust.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/dep_analysis/typescript.py` & `repoqa-0.1.1/scripts/curate/dep_analysis/typescript.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/function_analysis.py` & `repoqa-0.1.1/scripts/curate/function_analysis.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/github_fetch.py` & `repoqa-0.1.1/scripts/curate/github_fetch.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/merge_annotation.py` & `repoqa-0.1.1/scripts/curate/merge_annotation.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/merge_dep.py` & `repoqa-0.1.1/scripts/curate/merge_dep.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/needle_annotation.py` & `repoqa-0.1.1/scripts/curate/needle_annotation.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/curate/needle_selection.py` & `repoqa-0.1.1/scripts/curate/needle_selection.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/demos/model_request_oai.py` & `repoqa-0.1.1/scripts/demos/model_request_oai.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/misc/estimate_max_char.py` & `repoqa-0.1.1/scripts/misc/estimate_max_char.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/scripts/misc/repo_token_size.py` & `repoqa-0.1.1/scripts/misc/repo_token_size.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.0rc2/setup.cfg` & `repoqa-0.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 	License :: OSI Approved :: Apache Software License
 
 [options]
 packages = find:
 python_requires = >=3.8
 dependency_links = 
 install_requires = 
+	tempdir>=0.7.1
 	appdirs>=1.4.4
 	fire>=0.6.0
-	openai>=1.23.2
 	nltk>=3.8.1
 	rich>=13.5.2
-	tree_sitter_languages>=1.10.2
 	numpy>=1.25.2
+	tree_sitter_languages>=1.10.2
+	transformers>=4.40.0
+	openai>=1.23.2
 	anthropic>=0.25.6
+	google-generativeai>=0.5.2
+	stop-sequencer>=1.2.3
 
 [options.entry_points]
 console_scripts = 
 	repoqa.search_needle_function = repoqa.search_needle_function:main
 	repoqa.compute_score = repoqa.compute_score:main
 
 [options.extras_require]
```

