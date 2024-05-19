# Comparing `tmp/scikit_surprise-1.1.4.tar.gz` & `tmp/scikit-surprise-1.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_surprise-1.1.4.tar", last modified: Sun May 19 14:13:51 2024, max compression
+gzip compressed data, was "dist/scikit-surprise-1.1rc0.tar", last modified: Fri Sep 13 14:54:19 2019, max compression
```

## Comparing `scikit_surprise-1.1.4.tar` & `scikit-surprise-1.1rc0.tar`

### file list

```diff
@@ -1,116 +1,293 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.556909 scikit_surprise-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15622 2024-05-19 14:13:51.556909 scikit_surprise-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.536909 scikit_surprise-1.1.4/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.540909 scikit_surprise-1.1.4/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/FAQ.rst
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/accuracy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/algobase.rst
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/basic_algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/building_custom_algo.rst
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/co_clustering.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/dataset.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/dump.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18910 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/knn_inspired.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/matrix_factorization.rst
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/notation_standards.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/prediction_algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/prediction_algorithms_package.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/predictions_module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/similarities.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/slope_one.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/doc/source/trainset.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.544909 scikit_surprise-1.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/baselines_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.544909 scikit_surprise-1.1.4/examples/building_custom_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/building_custom_algorithms/mean_rating_user_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/building_custom_algorithms/most_basic_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/building_custom_algorithms/most_basic_algorithm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/building_custom_algorithms/with_baselines_or_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/evaluate_on_trainset.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/generate_grid_search_cv_results_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/grid_search_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/k_nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/load_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/load_custom_dataset_predefined_folds.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/load_from_dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.544909 scikit_surprise-1.1.4/examples/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    87502 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/notebooks/Compare.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    90547 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/notebooks/KNNBasic_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/precision_recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/predict_ratings.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/run_all_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/serialize_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/similarity_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/split_data_for_unbiased_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/top_n_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/examples/use_cross_validation_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.552909 scikit_surprise-1.1.4/scikit_surprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15622 2024-05-19 14:13:51.000000 scikit_surprise-1.1.4/scikit_surprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-19 14:13:51.000000 scikit_surprise-1.1.4/scikit_surprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 14:13:51.000000 scikit_surprise-1.1.4/scikit_surprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 14:13:51.000000 scikit_surprise-1.1.4/scikit_surprise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 14:13:51.000000 scikit_surprise-1.1.4/scikit_surprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 14:13:51.000000 scikit_surprise-1.1.4/scikit_surprise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 14:13:51.556909 scikit_surprise-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.548909 scikit_surprise-1.1.4/surprise/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6508 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/builtin_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/dump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.548909 scikit_surprise-1.1.4/surprise/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23931 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/model_selection/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    16905 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/model_selection/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/model_selection/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.552909 scikit_surprise-1.1.4/surprise/prediction_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/algo_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/baseline_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/co_clustering.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/knns.py
--rw-r--r--   0 runner    (1001) docker     (127)    32164 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/matrix_factorization.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/optimize_baselines.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/random_pred.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/prediction_algorithms/slope_one.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/similarities.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/trainset.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/surprise/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:13:51.552909 scikit_surprise-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_NMF.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_SVD.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_bsl_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_co_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17105 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_sim_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_similarities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-19 14:13:39.000000 scikit_surprise-1.1.4/tests/test_zero_ratings.py
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/
+-rw-r--r--   0 nico      (1000) nico      (1000)     1495 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/LICENSE.md
+-rw-r--r--   0 nico      (1000) nico      (1000)      152 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/MANIFEST.in
+-rw-r--r--   0 nico      (1000) nico      (1000)    14161 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/PKG-INFO
+-rw-r--r--   0 nico      (1000) nico      (1000)    11762 2019-09-13 14:51:18.000000 scikit-surprise-1.1rc0/README.md
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/
+-rw-r--r--   0 nico      (1000) nico      (1000)     7499 2019-02-16 12:52:22.000000 scikit-surprise-1.1rc0/doc/Makefile
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/doctrees/
+-rw-r--r--   0 nico      (1000) nico      (1000)    58297 2019-09-12 20:19:25.000000 scikit-surprise-1.1rc0/doc/build/doctrees/FAQ.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    33928 2019-09-12 20:19:25.000000 scikit-surprise-1.1rc0/doc/build/doctrees/accuracy.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    52077 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/algobase.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    15547 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/basic_algorithms.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    34252 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/building_custom_algo.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    16109 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/co_clustering.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    44786 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/dataset.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    16543 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/dump.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)   190546 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 nico      (1000) nico      (1000)   115541 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/getting_started.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)     9631 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/index.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    55685 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/knn_inspired.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)   109306 2019-09-12 20:19:26.000000 scikit-surprise-1.1rc0/doc/build/doctrees/matrix_factorization.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)   206450 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/model_selection.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    25680 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/notation_standards.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    40179 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/prediction_algorithms.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    22259 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/prediction_algorithms_package.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    14153 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/predictions_module.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    13882 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/reader.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    30854 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/similarities.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)     8436 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/slope_one.doctree
+-rw-r--r--   0 nico      (1000) nico      (1000)    65207 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/doctrees/trainset.doctree
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/
+-rw-r--r--   0 nico      (1000) nico      (1000)      230 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/.buildinfo
+-rw-r--r--   0 nico      (1000) nico      (1000)    56899 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/FAQ.html
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/
+-rw-r--r--   0 nico      (1000) nico      (1000)     7423 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/index.html
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/
+-rw-r--r--   0 nico      (1000) nico      (1000)    22893 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/accuracy.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    35889 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/dataset.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    11127 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/dump.html
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/model_selection/
+-rw-r--r--   0 nico      (1000) nico      (1000)    71120 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/model_selection/search.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    57340 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/model_selection/split.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    35672 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/model_selection/validation.html
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/prediction_algorithms/
+-rw-r--r--   0 nico      (1000) nico      (1000)    39824 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/prediction_algorithms/algo_base.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    11130 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/prediction_algorithms/baseline_only.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    58251 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/prediction_algorithms/knns.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    11847 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/prediction_algorithms/predictions.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    11040 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/prediction_algorithms/random_pred.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    17396 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/reader.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    31958 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_modules/surprise/trainset.html
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/
+-rw-r--r--   0 nico      (1000) nico      (1000)     8318 2019-09-12 19:19:29.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/FAQ.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      144 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/accuracy.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      151 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/algobase.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      371 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/basic_algorithms.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)     5405 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/building_custom_algo.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      159 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/co_clustering.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      167 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/dataset.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)       91 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/dump.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)    18957 2019-09-12 19:29:52.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/getting_started.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)     1428 2019-09-12 20:19:05.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/index.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)     1348 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/knn_inspired.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      403 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/matrix_factorization.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      922 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/model_selection.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)     1981 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/notation_standards.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)     6018 2019-09-12 19:19:00.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/prediction_algorithms.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      410 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/prediction_algorithms_package.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      204 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/predictions_module.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      126 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/reader.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      175 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/similarities.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)      138 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/slope_one.rst.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)       93 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/build/html/_sources/trainset.rst.txt
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_static/
+-rw-r--r--   0 nico      (1000) nico      (1000)      673 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/ajax-loader.gif
+-rw-r--r--   0 nico      (1000) nico      (1000)    10912 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_static/basic.css
+-rw-r--r--   0 nico      (1000) nico      (1000)      756 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/comment-bright.png
+-rw-r--r--   0 nico      (1000) nico      (1000)      829 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/comment-close.png
+-rw-r--r--   0 nico      (1000) nico      (1000)      641 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/comment.png
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_static/css/
+-rw-r--r--   0 nico      (1000) nico      (1000)     3358 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/css/badge_only.css
+-rw-r--r--   0 nico      (1000) nico      (1000)   116310 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/css/theme.css
+-rw-r--r--   0 nico      (1000) nico      (1000)     9313 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/doctools.js
+-rw-r--r--   0 nico      (1000) nico      (1000)      305 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_static/documentation_options.js
+-rw-r--r--   0 nico      (1000) nico      (1000)      222 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/down-pressed.png
+-rw-r--r--   0 nico      (1000) nico      (1000)      202 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/down.png
+-rw-r--r--   0 nico      (1000) nico      (1000)      286 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/file.png
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/
+-rw-r--r--   0 nico      (1000) nico      (1000)   256056 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-bold.eot
+-rw-r--r--   0 nico      (1000) nico      (1000)   600856 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-bold.ttf
+-rw-r--r--   0 nico      (1000) nico      (1000)   309728 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-bold.woff
+-rw-r--r--   0 nico      (1000) nico      (1000)   184912 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-bold.woff2
+-rw-r--r--   0 nico      (1000) nico      (1000)   266158 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-bolditalic.eot
+-rw-r--r--   0 nico      (1000) nico      (1000)   622572 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-bolditalic.ttf
+-rw-r--r--   0 nico      (1000) nico      (1000)   323344 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-bolditalic.woff
+-rw-r--r--   0 nico      (1000) nico      (1000)   193308 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-bolditalic.woff2
+-rw-r--r--   0 nico      (1000) nico      (1000)   268604 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-italic.eot
+-rw-r--r--   0 nico      (1000) nico      (1000)   639388 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-italic.ttf
+-rw-r--r--   0 nico      (1000) nico      (1000)   328412 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-italic.woff
+-rw-r--r--   0 nico      (1000) nico      (1000)   195704 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-italic.woff2
+-rw-r--r--   0 nico      (1000) nico      (1000)   253461 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-regular.eot
+-rw-r--r--   0 nico      (1000) nico      (1000)   607720 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-regular.ttf
+-rw-r--r--   0 nico      (1000) nico      (1000)   309192 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-regular.woff
+-rw-r--r--   0 nico      (1000) nico      (1000)   182708 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/Lato/lato-regular.woff2
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/
+-rw-r--r--   0 nico      (1000) nico      (1000)    79520 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
+-rw-r--r--   0 nico      (1000) nico      (1000)   170616 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
+-rw-r--r--   0 nico      (1000) nico      (1000)    87624 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
+-rw-r--r--   0 nico      (1000) nico      (1000)    67312 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
+-rw-r--r--   0 nico      (1000) nico      (1000)    78331 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
+-rw-r--r--   0 nico      (1000) nico      (1000)   169064 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
+-rw-r--r--   0 nico      (1000) nico      (1000)    86288 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
+-rw-r--r--   0 nico      (1000) nico      (1000)    66444 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
+-rw-r--r--   0 nico      (1000) nico      (1000)   165742 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 nico      (1000) nico      (1000)   444379 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 nico      (1000) nico      (1000)   165548 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 nico      (1000) nico      (1000)    98024 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 nico      (1000) nico      (1000)    77160 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 nico      (1000) nico      (1000)      299 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/graphviz.css
+-rw-r--r--   0 nico      (1000) nico      (1000)   268039 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/jquery-3.2.1.js
+-rw-r--r--   0 nico      (1000) nico      (1000)    86659 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/jquery.js
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/build/html/_static/js/
+-rw-r--r--   0 nico      (1000) nico      (1000)    15414 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/js/modernizr.min.js
+-rw-r--r--   0 nico      (1000) nico      (1000)     4400 2018-09-21 20:38:50.000000 scikit-surprise-1.1rc0/doc/build/html/_static/js/theme.js
+-rw-r--r--   0 nico      (1000) nico      (1000)    10847 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_static/language_data.js
+-rw-r--r--   0 nico      (1000) nico      (1000)       90 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/minus.png
+-rw-r--r--   0 nico      (1000) nico      (1000)       90 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/plus.png
+-rw-r--r--   0 nico      (1000) nico      (1000)     4395 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/_static/pygments.css
+-rw-r--r--   0 nico      (1000) nico      (1000)    15059 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 nico      (1000) nico      (1000)    35168 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 nico      (1000) nico      (1000)    12140 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/underscore.js
+-rw-r--r--   0 nico      (1000) nico      (1000)      214 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/up-pressed.png
+-rw-r--r--   0 nico      (1000) nico      (1000)      203 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/up.png
+-rw-r--r--   0 nico      (1000) nico      (1000)    25355 2019-02-16 13:42:55.000000 scikit-surprise-1.1rc0/doc/build/html/_static/websupport.js
+-rw-r--r--   0 nico      (1000) nico      (1000)    17780 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/accuracy.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    24888 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/algobase.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    11796 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/basic_algorithms.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    31831 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/building_custom_algo.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    11779 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/co_clustering.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    20365 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/dataset.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    11289 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/dump.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    26731 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/genindex.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    77657 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/getting_started.html
+-rw-r--r--   0 nico      (1000) nico      (1000)     7743 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/index.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    23013 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/knn_inspired.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    43929 2019-09-12 20:19:27.000000 scikit-surprise-1.1rc0/doc/build/html/matrix_factorization.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    76028 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/model_selection.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    16069 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/notation_standards.html
+-rw-r--r--   0 nico      (1000) nico      (1000)     3045 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/objects.inv
+-rw-r--r--   0 nico      (1000) nico      (1000)    24401 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/prediction_algorithms.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    13955 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/prediction_algorithms_package.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    11175 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/predictions_module.html
+-rw-r--r--   0 nico      (1000) nico      (1000)     8116 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/py-modindex.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    10248 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/reader.html
+-rw-r--r--   0 nico      (1000) nico      (1000)     6166 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/search.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    23573 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/searchindex.js
+-rw-r--r--   0 nico      (1000) nico      (1000)    16359 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/similarities.html
+-rw-r--r--   0 nico      (1000) nico      (1000)     9506 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/slope_one.html
+-rw-r--r--   0 nico      (1000) nico      (1000)    27439 2019-09-12 20:19:28.000000 scikit-surprise-1.1rc0/doc/build/html/trainset.html
+-rw-r--r--   0 nico      (1000) nico      (1000)     7258 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/make.bat
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/doc/source/
+-rw-r--r--   0 nico      (1000) nico      (1000)     8525 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/doc/source/FAQ.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      144 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/accuracy.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      151 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/algobase.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      371 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/basic_algorithms.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)     5405 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/building_custom_algo.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      159 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/co_clustering.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)     9652 2019-07-06 17:05:31.000000 scikit-surprise-1.1rc0/doc/source/conf.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      167 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/dataset.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)       91 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/dump.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)    18957 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/doc/source/getting_started.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)     1428 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/doc/source/index.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)     1348 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/knn_inspired.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      403 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/matrix_factorization.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      922 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/model_selection.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)     1981 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/notation_standards.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)     6018 2019-09-12 19:19:00.000000 scikit-surprise-1.1rc0/doc/source/prediction_algorithms.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      410 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/prediction_algorithms_package.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      204 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/predictions_module.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      126 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/reader.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)     2549 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/refs.bib
+-rw-r--r--   0 nico      (1000) nico      (1000)      175 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/similarities.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      138 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/slope_one.rst
+-rw-r--r--   0 nico      (1000) nico      (1000)      472 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/spelling_wordlist.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)       93 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/doc/source/trainset.rst
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/examples/
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/examples/__pycache__/
+-rw-r--r--   0 nico      (1000) nico      (1000)     1001 2019-09-12 20:12:11.000000 scikit-surprise-1.1rc0/examples/__pycache__/baselines_conf.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      669 2019-09-12 20:13:30.000000 scikit-surprise-1.1rc0/examples/__pycache__/basic_usage.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1044 2019-09-12 20:16:52.000000 scikit-surprise-1.1rc0/examples/__pycache__/evaluate_on_trainset.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1440 2019-09-12 20:12:43.000000 scikit-surprise-1.1rc0/examples/__pycache__/generate_grid_search_cv_results_example.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      975 2019-09-12 20:13:56.000000 scikit-surprise-1.1rc0/examples/__pycache__/grid_search_usage.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1896 2019-09-12 20:15:05.000000 scikit-surprise-1.1rc0/examples/__pycache__/k_nearest_neighbors.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      866 2019-09-12 20:17:14.000000 scikit-surprise-1.1rc0/examples/__pycache__/load_custom_dataset.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1307 2019-09-12 20:11:47.000000 scikit-surprise-1.1rc0/examples/__pycache__/load_custom_dataset_predefined_folds.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      833 2019-09-12 20:12:11.000000 scikit-surprise-1.1rc0/examples/__pycache__/load_from_dataframe.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     2213 2019-09-12 20:16:04.000000 scikit-surprise-1.1rc0/examples/__pycache__/precision_recall_at_k.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      686 2019-09-12 20:17:18.000000 scikit-surprise-1.1rc0/examples/__pycache__/predict_ratings.cpython-36.pyc
+-rw-------   0 nico      (1000) nico      (1000)     1399 2019-09-12 20:07:14.000000 scikit-surprise-1.1rc0/examples/__pycache__/run_all_examples.cpython-36-PYTEST.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      998 2019-09-12 20:14:44.000000 scikit-surprise-1.1rc0/examples/__pycache__/serialize_algorithm.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      717 2019-09-12 20:15:08.000000 scikit-surprise-1.1rc0/examples/__pycache__/similarity_conf.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1373 2019-09-12 20:16:29.000000 scikit-surprise-1.1rc0/examples/__pycache__/split_data_for_unbiased_estimation.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1997 2019-09-12 20:17:19.000000 scikit-surprise-1.1rc0/examples/__pycache__/top_n_recommendations.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      682 2019-09-12 20:13:25.000000 scikit-surprise-1.1rc0/examples/__pycache__/train_test_split.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      721 2019-09-12 20:14:52.000000 scikit-surprise-1.1rc0/examples/__pycache__/use_cross_validation_iterators.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1251 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/baselines_conf.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1216 2018-05-27 14:10:11.000000 scikit-surprise-1.1rc0/examples/baselines_conf.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      649 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/basic_usage.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      804 2018-05-27 14:17:15.000000 scikit-surprise-1.1rc0/examples/basic_usage.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     4417 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/benchmark.py
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/__pycache__/
+-rw-r--r--   0 nico      (1000) nico      (1000)     1552 2019-09-12 20:07:14.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/__pycache__/mean_rating_user_item.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1556 2019-09-12 20:44:40.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/__pycache__/mean_rating_user_item.cpython-37.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1060 2019-09-12 20:07:40.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/__pycache__/most_basic_algorithm.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1442 2019-09-12 20:07:24.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/__pycache__/most_basic_algorithm2.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     2101 2019-09-12 20:07:42.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/__pycache__/with_baselines_or_sim.cpython-36.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1009 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/mean_rating_user_item.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      645 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/most_basic_algorithm.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1051 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/most_basic_algorithm2.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1738 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/building_custom_algorithms/with_baselines_or_sim.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1102 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/evaluate_on_trainset.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1107 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/generate_grid_search_cv_results_example.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1577 2018-05-27 14:12:46.000000 scikit-surprise-1.1rc0/examples/generate_grid_search_cv_results_example.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      933 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/grid_search_usage.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1192 2018-05-27 14:17:36.000000 scikit-surprise-1.1rc0/examples/grid_search_usage.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     2085 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/k_nearest_neighbors.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     2375 2018-05-27 14:18:39.000000 scikit-surprise-1.1rc0/examples/k_nearest_neighbors.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      992 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/examples/load_custom_dataset.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1287 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/examples/load_custom_dataset_predefined_folds.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      968 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/examples/load_from_dataframe.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      943 2018-05-27 14:18:48.000000 scikit-surprise-1.1rc0/examples/load_from_dataframe.pyc
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/examples/notebooks/
+-rw-r--r--   0 nico      (1000) nico      (1000)   103129 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/examples/notebooks/Compare.ipynb
+-rw-r--r--   0 nico      (1000) nico      (1000)   102545 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/examples/notebooks/KNNBasic_analysis.ipynb
+-rw-r--r--   0 nico      (1000) nico      (1000)     2123 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/precision_recall_at_k.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      818 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/predict_ratings.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1156 2019-09-12 20:07:08.000000 scikit-surprise-1.1rc0/examples/run_all_examples.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1232 2018-05-27 14:17:11.000000 scikit-surprise-1.1rc0/examples/run_all_examples.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1019 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/serialize_algorithm.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1197 2018-05-27 14:18:16.000000 scikit-surprise-1.1rc0/examples/serialize_algorithm.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      864 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/similarity_conf.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      878 2018-05-27 14:21:28.000000 scikit-surprise-1.1rc0/examples/similarity_conf.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)     1567 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/split_data_for_unbiased_estimation.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1914 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/top_n_recommendations.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      788 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/train_test_split.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      829 2018-05-27 14:17:11.000000 scikit-surprise-1.1rc0/examples/train_test_split.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)      684 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/examples/use_cross_validation_iterators.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      890 2018-05-27 14:18:26.000000 scikit-surprise-1.1rc0/examples/use_cross_validation_iterators.pyc
+-rw-r--r--   0 nico      (1000) nico      (1000)       52 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/requirements.txt
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/scikit_surprise.egg-info/
+-rw-r--r--   0 nico      (1000) nico      (1000)    14161 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/scikit_surprise.egg-info/PKG-INFO
+-rw-r--r--   0 nico      (1000) nico      (1000)    11018 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/scikit_surprise.egg-info/SOURCES.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)        1 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/scikit_surprise.egg-info/dependency_links.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)       53 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/scikit_surprise.egg-info/entry_points.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)       52 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/scikit_surprise.egg-info/requires.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)        9 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/scikit_surprise.egg-info/top_level.txt
+-rw-r--r--   0 nico      (1000) nico      (1000)       79 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/setup.cfg
+-rw-r--r--   0 nico      (1000) nico      (1000)     4560 2019-09-13 14:51:25.000000 scikit-surprise-1.1rc0/setup.py
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/surprise/
+-rw-r--r--   0 nico      (1000) nico      (1000)     1262 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/__init__.py
+-rwxr-xr-x   0 nico      (1000) nico      (1000)     7786 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/__main__.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     5047 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/accuracy.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     2548 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/builtin_datasets.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     9634 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/dataset.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1965 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/dump.py
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/surprise/model_selection/
+-rw-r--r--   0 nico      (1000) nico      (1000)      472 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/model_selection/__init__.py
+-rw-r--r--   0 nico      (1000) nico      (1000)    24013 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/model_selection/search.py
+-rw-r--r--   0 nico      (1000) nico      (1000)    17129 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/model_selection/split.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     8815 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/model_selection/validation.py
+drwxr-xr-x   0 nico      (1000) nico      (1000)        0 2019-09-13 14:54:19.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/
+-rw-r--r--   0 nico      (1000) nico      (1000)     1230 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/__init__.py
+-rw-r--r--   0 nico      (1000) nico      (1000)    10894 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/algo_base.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1348 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/baseline_only.py
+-rw-r--r--   0 nico      (1000) nico      (1000)   650250 2019-09-13 14:53:22.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/co_clustering.c
+-rw-r--r--   0 nico      (1000) nico      (1000)     9976 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/co_clustering.pyx
+-rw-r--r--   0 nico      (1000) nico      (1000)    14193 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/knns.py
+-rw-r--r--   0 nico      (1000) nico      (1000)   970022 2019-09-13 14:53:22.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/matrix_factorization.c
+-rw-r--r--   0 nico      (1000) nico      (1000)    30526 2019-07-06 17:05:31.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/matrix_factorization.pyx
+-rw-r--r--   0 nico      (1000) nico      (1000)   399180 2019-09-13 14:53:23.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/optimize_baselines.c
+-rw-r--r--   0 nico      (1000) nico      (1000)     2664 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/optimize_baselines.pyx
+-rw-r--r--   0 nico      (1000) nico      (1000)     1624 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/predictions.py
+-rw-r--r--   0 nico      (1000) nico      (1000)     1319 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/random_pred.py
+-rw-r--r--   0 nico      (1000) nico      (1000)   520893 2019-09-13 14:53:23.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/slope_one.c
+-rw-r--r--   0 nico      (1000) nico      (1000)     2981 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/prediction_algorithms/slope_one.pyx
+-rw-r--r--   0 nico      (1000) nico      (1000)     3851 2019-09-12 20:37:53.000000 scikit-surprise-1.1rc0/surprise/reader.py
+-rw-r--r--   0 nico      (1000) nico      (1000)   673190 2019-09-13 14:53:23.000000 scikit-surprise-1.1rc0/surprise/similarities.c
+-rw-r--r--   0 nico      (1000) nico      (1000)    11932 2019-09-12 19:19:00.000000 scikit-surprise-1.1rc0/surprise/similarities.pyx
+-rw-r--r--   0 nico      (1000) nico      (1000)     8783 2019-09-12 19:19:29.000000 scikit-surprise-1.1rc0/surprise/trainset.py
+-rw-r--r--   0 nico      (1000) nico      (1000)      919 2019-01-04 13:05:49.000000 scikit-surprise-1.1rc0/surprise/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `scikit_surprise-1.1.4/LICENSE.md` & `scikit-surprise-1.1rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scikit_surprise-1.1.4/PKG-INFO` & `scikit-surprise-1.1rc0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,78 @@
-Metadata-Version: 2.1
-Name: scikit-surprise
-Version: 1.1.4
-Summary: An easy-to-use library for recommender systems.
-Author-email: Nicolas Hug <contact@nicolas-hug.com>
-License: Copyright (c) 2016, Nicolas Hug
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-          this list of conditions and the following disclaimer in the documentation
-          and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its contributors
-           may be used to endorse or promote products derived from this software
-           without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: homepage, https://surpriselib.com
-Project-URL: repository, https://github.com/NicolasHug/Surprise
-Keywords: recommender,recommendation system
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: joblib>=1.2.0
-Requires-Dist: numpy>=1.19.5
-Requires-Dist: scipy>=1.6.0
-
 [![GitHub version](https://badge.fury.io/gh/nicolashug%2FSurprise.svg)](https://badge.fury.io/gh/nicolashug%2FSurprise)
-[![Documentation Status](https://readthedocs.org/projects/surprise/badge/?version=stable)](https://surprise.readthedocs.io/en/stable/?badge=stable)
-[![python versions](https://img.shields.io/badge/python-3.8+-blue.svg)](https://surpriselib.com)
+[![Documentation Status](https://readthedocs.org/projects/surprise/badge/?version=stable)](http://surprise.readthedocs.io/en/stable/?badge=stable)
+[![Build Status](https://travis-ci.org/NicolasHug/Surprise.svg?branch=master)](https://travis-ci.org/NicolasHug/Surprise)
+[![python versions](https://img.shields.io/badge/python-2.7%2C%203.5%2C%203.6-blue.svg)](http://surpriselib.com)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![DOI](https://joss.theoj.org/papers/10.21105/joss.02174/status.svg)](https://doi.org/10.21105/joss.02174)
 
-[![logo](./logo_black.svg)](https://surpriselib.com)
+[![logo](logo_black.svg)](http://surpriselib.com)
 
 Overview
 --------
 
-[Surprise](https://surpriselib.com) is a Python
-[scikit](https://projects.scipy.org/scikits.html) for building and analyzing
+[Surprise](http://surpriselib.com) is a Python
+[scikit](https://www.scipy.org/scikits.html) building and analyzing
 recommender systems that deal with explicit rating data.
 
-[Surprise](https://surpriselib.com) **was designed with the
+[Surprise](http://surpriselib.com) **was designed with the
 following purposes in mind**:
 
 - Give users perfect control over their experiments. To this end, a strong
   emphasis is laid on
-  [documentation](https://surprise.readthedocs.io/en/stable/index.html), which we
+  [documentation](http://surprise.readthedocs.io/en/stable/index.html), which we
   have tried to make as clear and precise as possible by pointing out every
   detail of the algorithms.
 - Alleviate the pain of [Dataset
-  handling](https://surprise.readthedocs.io/en/stable/getting_started.html#load-a-custom-dataset).
+  handling](http://surprise.readthedocs.io/en/stable/getting_started.html#load-a-custom-dataset).
   Users can use both *built-in* datasets
-  ([Movielens](https://grouplens.org/datasets/movielens/),
-  [Jester](https://eigentaste.berkeley.edu/dataset/)), and their own *custom*
+  ([Movielens](http://grouplens.org/datasets/movielens/),
+  [Jester](http://eigentaste.berkeley.edu/dataset/)), and their own *custom*
   datasets.
 - Provide various ready-to-use [prediction
-  algorithms](https://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html)
+  algorithms](http://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html)
   such as [baseline
-  algorithms](https://surprise.readthedocs.io/en/stable/basic_algorithms.html),
+  algorithms](http://surprise.readthedocs.io/en/stable/basic_algorithms.html),
   [neighborhood
-  methods](https://surprise.readthedocs.io/en/stable/knn_inspired.html), matrix
+  methods](http://surprise.readthedocs.io/en/stable/knn_inspired.html), matrix
   factorization-based (
-  [SVD](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD),
-  [PMF](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#unbiased-note),
-  [SVD++](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp),
-  [NMF](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)),
+  [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD),
+  [PMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#unbiased-note),
+  [SVD++](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp),
+  [NMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)),
   and [many
-  others](https://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html).
+  others](http://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html).
   Also, various [similarity
-  measures](https://surprise.readthedocs.io/en/stable/similarities.html)
+  measures](http://surprise.readthedocs.io/en/stable/similarities.html)
   (cosine, MSD, pearson...) are built-in.
 - Make it easy to implement [new algorithm
-  ideas](https://surprise.readthedocs.io/en/stable/building_custom_algo.html).
-- Provide tools to [evaluate](https://surprise.readthedocs.io/en/stable/model_selection.html),
-  [analyse](https://nbviewer.jupyter.org/github/NicolasHug/Surprise/tree/master/examples/notebooks/KNNBasic_analysis.ipynb/)
+  ideas](http://surprise.readthedocs.io/en/stable/building_custom_algo.html).
+- Provide tools to [evaluate](http://surprise.readthedocs.io/en/stable/model_selection.html),
+  [analyse](http://nbviewer.jupyter.org/github/NicolasHug/Surprise/tree/master/examples/notebooks/KNNBasic_analysis.ipynb/)
   and
-  [compare](https://nbviewer.jupyter.org/github/NicolasHug/Surprise/blob/master/examples/notebooks/Compare.ipynb)
-  the algorithms' performance. Cross-validation procedures can be run very
+  [compare](http://nbviewer.jupyter.org/github/NicolasHug/Surprise/blob/master/examples/notebooks/Compare.ipynb)
+  the algorithms performance. Cross-validation procedures can be run very
   easily using powerful CV iterators (inspired by
-  [scikit-learn](https://scikit-learn.org/) excellent tools), as well as
+  [scikit-learn](http://scikit-learn.org/) excellent tools), as well as
   [exhaustive search over a set of
-  parameters](https://surprise.readthedocs.io/en/stable/getting_started.html#tune-algorithm-parameters-with-gridsearchcv).
+  parameters](http://surprise.readthedocs.io/en/stable/getting_started.html#tune-algorithm-parameters-with-gridsearchcv).
 
 
-The name *SurPRISE* (roughly :) ) stands for *Simple Python RecommendatIon
-System Engine*.
+The name *SurPRISE* (roughly :) ) stands for Simple Python RecommendatIon
+System Engine.
 
 Please note that surprise does not support implicit ratings or content-based
 information.
 
 
 Getting started, example
 ------------------------
 
 Here is a simple example showing how you can (down)load a dataset, split it for
 5-fold cross-validation, and compute the MAE and RMSE of the
-[SVD](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)
+[SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)
 algorithm.
 
 
 ```python
 from surprise import SVD
 from surprise import Dataset
 from surprise.model_selection import cross_validate
@@ -142,137 +88,122 @@
 ```
 
 **Output**:
 
 ```
 Evaluating RMSE, MAE of algorithm SVD on 5 split(s).
 
-                  Fold 1  Fold 2  Fold 3  Fold 4  Fold 5  Mean    Std     
-RMSE (testset)    0.9367  0.9355  0.9378  0.9377  0.9300  0.9355  0.0029  
-MAE (testset)     0.7387  0.7371  0.7393  0.7397  0.7325  0.7375  0.0026  
-Fit time          0.62    0.63    0.63    0.65    0.63    0.63    0.01    
-Test time         0.11    0.11    0.14    0.14    0.14    0.13    0.02    
+            Fold 1  Fold 2  Fold 3  Fold 4  Fold 5  Mean    Std
+RMSE        0.9311  0.9370  0.9320  0.9317  0.9391  0.9342  0.0032
+MAE         0.7350  0.7375  0.7341  0.7342  0.7375  0.7357  0.0015
+Fit time    6.53    7.11    7.23    7.15    3.99    6.40    1.23
+Test time   0.26    0.26    0.25    0.15    0.13    0.21    0.06
 ```
 
-[Surprise](https://surpriselib.com) can do **much** more (e.g,
-[GridSearchCV](https://surprise.readthedocs.io/en/stable/getting_started.html#tune-algorithm-parameters-with-gridsearchcv))!
+[Surprise](http://surpriselib.com) can do **much** more (e.g,
+[GridSearchCV](http://surprise.readthedocs.io/en/stable/getting_started.html#tune-algorithm-parameters-with-gridsearchcv))!
 You'll find [more usage
-examples](https://surprise.readthedocs.io/en/stable/getting_started.html) in the
-[documentation ](https://surprise.readthedocs.io/en/stable/index.html).
+examples](http://surprise.readthedocs.io/en/stable/getting_started.html) in the
+[documentation ](http://surprise.readthedocs.io/en/stable/index.html).
 
 
 Benchmarks
 ----------
 
 Here are the average RMSE, MAE and total execution time of various algorithms
 (with their default parameters) on a 5-fold cross-validation procedure. The
-datasets are the [Movielens](https://grouplens.org/datasets/movielens/) 100k and
+datasets are the [Movielens](http://grouplens.org/datasets/movielens/) 100k and
 1M datasets. The folds are the same for all the algorithms. All experiments are
-run on a laptop with an intel i5 11th Gen 2.60GHz. The code
+run on a notebook with Intel Core i5 7th gen (2.5 GHz) and 8Go RAM.  The code
 for generating these tables can be found in the [benchmark
 example](https://github.com/NicolasHug/Surprise/tree/master/examples/benchmark.py).
 
 | [Movielens 100k](http://grouplens.org/datasets/movielens/100k)                                                                         |   RMSE |   MAE | Time    |
 |:---------------------------------------------------------------------------------------------------------------------------------------|-------:|------:|:--------|
-| [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)      |  0.934 | 0.737 | 0:00:06 |
-| [SVD++ (cache_ratings=False)](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.919 | 0.721 | 0:01:39 |
-| [SVD++ (cache_ratings=True)](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.919 | 0.721 | 0:01:22 |
-| [NMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)      |  0.963 | 0.758 | 0:00:06 |
-| [Slope One](http://surprise.readthedocs.io/en/stable/slope_one.html#surprise.prediction_algorithms.slope_one.SlopeOne)                 |  0.946 | 0.743 | 0:00:09 |
-| [k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBasic)                        |  0.98  | 0.774 | 0:00:08 |
-| [Centered k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNWithMeans)           |  0.951 | 0.749 | 0:00:09 |
-| [k-NN Baseline](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBaseline)            |  0.931 | 0.733 | 0:00:13 |
-| [Co-Clustering](http://surprise.readthedocs.io/en/stable/co_clustering.html#surprise.prediction_algorithms.co_clustering.CoClustering) |  0.963 | 0.753 | 0:00:06 |
-| [Baseline](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.baseline_only.BaselineOnly)   |  0.944 | 0.748 | 0:00:02 |
-| [Random](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.random_pred.NormalPredictor)    |  1.518 | 1.219 | 0:00:01 |
-
-
-| [Movielens 1M](https://grouplens.org/datasets/movielens/1m)                                                                             |   RMSE |   MAE | Time    |
-|:----------------------------------------------------------------------------------------------------------------------------------------|-------:|------:|:--------|
-| [SVD](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)      |  0.873 | 0.686 | 0:01:07 |
-| [SVD++ (cache_ratings=False)](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.862 | 0.672 | 0:41:06 |
-| [SVD++ (cache_ratings=True)](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.862 | 0.672 | 0:34:55 |
-| [NMF](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)      |  0.916 | 0.723 | 0:01:39 |
+| [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)      |  0.934 | 0.737 | 0:00:11 |
+| [SVD++](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.92  | 0.722 | 0:09:03 |
+| [NMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)      |  0.963 | 0.758 | 0:00:15 |
+| [Slope One](http://surprise.readthedocs.io/en/stable/slope_one.html#surprise.prediction_algorithms.slope_one.SlopeOne)                 |  0.946 | 0.743 | 0:00:08 |
+| [k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBasic)                        |  0.98  | 0.774 | 0:00:10 |
+| [Centered k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNWithMeans)           |  0.951 | 0.749 | 0:00:10 |
+| [k-NN Baseline](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBaseline)            |  0.931 | 0.733 | 0:00:12 |
+| [Co-Clustering](http://surprise.readthedocs.io/en/stable/co_clustering.html#surprise.prediction_algorithms.co_clustering.CoClustering) |  0.963 | 0.753 | 0:00:03 |
+| [Baseline](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.baseline_only.BaselineOnly)   |  0.944 | 0.748 | 0:00:01 |
+| [Random](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.random_pred.NormalPredictor)    |  1.514 | 1.215 | 0:00:01 |
+
+
+| [Movielens 1M](http://grouplens.org/datasets/movielens/1m)                                                                             |   RMSE |   MAE | Time    |
+|:---------------------------------------------------------------------------------------------------------------------------------------|-------:|------:|:--------|
+| [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)      |  0.873 | 0.686 | 0:02:13 |
+| [SVD++](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.862 | 0.673 | 2:54:19 |
+| [NMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)      |  0.916 | 0.724 | 0:02:31 |
 | [Slope One](http://surprise.readthedocs.io/en/stable/slope_one.html#surprise.prediction_algorithms.slope_one.SlopeOne)                 |  0.907 | 0.715 | 0:02:31 |
 | [k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBasic)                        |  0.923 | 0.727 | 0:05:27 |
 | [Centered k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNWithMeans)           |  0.929 | 0.738 | 0:05:43 |
 | [k-NN Baseline](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBaseline)            |  0.895 | 0.706 | 0:05:55 |
 | [Co-Clustering](http://surprise.readthedocs.io/en/stable/co_clustering.html#surprise.prediction_algorithms.co_clustering.CoClustering) |  0.915 | 0.717 | 0:00:31 |
 | [Baseline](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.baseline_only.BaselineOnly)   |  0.909 | 0.719 | 0:00:19 |
 | [Random](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.random_pred.NormalPredictor)    |  1.504 | 1.206 | 0:00:19 |
 
+
 Installation
 ------------
 
-With pip (you'll need [numpy](https://www.numpy.org/), and a C compiler. Windows
+With pip (you'll need [numpy](http://www.numpy.org/), and a C compiler. Windows
 users might prefer using conda):
 
     $ pip install numpy
     $ pip install scikit-surprise
 
 With conda:
 
     $ conda install -c conda-forge scikit-surprise
 
 For the latest version, you can also clone the repo and build the source
-(you'll first need [Cython](https://cython.org/) and
-[numpy](https://www.numpy.org/)):
+(you'll first need [Cython](http://cython.org/) and
+[numpy](http://www.numpy.org/)):
 
     $ pip install numpy cython
     $ git clone https://github.com/NicolasHug/surprise.git
     $ cd surprise
     $ python setup.py install
 
-License and reference
----------------------
+License
+-------
 
 This project is licensed under the [BSD
 3-Clause](https://opensource.org/licenses/BSD-3-Clause) license, so it can be
-used for pretty much everything, including commercial applications.
+used for pretty much everything, including commercial applications. Please let
+us know how [Surprise](http://surpriselib.com) is useful to you!
 
-I'd love to know how Surprise is useful to you. Please don't hesitate to open
-an issue and describe how you use it!
+Here is a Bibtex entry if you ever need to cite Surprise in a research paper
+(please keep us posted, we would love to know if Surprise was helpful to you):
 
-Please make sure to cite the
-[paper](https://joss.theoj.org/papers/10.21105/joss.02174) if you use
-Surprise for your research:
-
-    @article{Hug2020,
-      doi = {10.21105/joss.02174},
-      url = {https://doi.org/10.21105/joss.02174},
-      year = {2020},
-      publisher = {The Open Journal},
-      volume = {5},
-      number = {52},
-      pages = {2174},
-      author = {Nicolas Hug},
-      title = {Surprise: A Python library for recommender systems},
-      journal = {Journal of Open Source Software}
+    @Misc{Surprise,
+    author =   {Hug, Nicolas},
+    title =    { {S}urprise, a {P}ython library for recommender systems},
+    howpublished = {\url{http://surpriselib.com}},
+    year = {2017}
     }
 
 Contributors
 ------------
 
-The following persons have contributed to [Surprise](https://surpriselib.com):
+The following persons have contributed to [Surprise](http://surpriselib.com):
 
-ashtou, Abhishek Bhatia, bobbyinfj, caoyi, Chieh-Han Chen,  Raphael-Dayan, Олег
-Демиденко, Charles-Emmanuel Dias, dmamylin, Lauriane Ducasse, Marc Feger,
-franckjay, Lukas Galke, Tim Gates, Pierre-François Gimenez, Zachary Glassman,
-Jeff Hale, Nicolas Hug, Janniks, jyesawtellrickson, Doruk Kilitcioglu, Ravi Raju
-Krishna, lapidshay, Hengji Liu, Ravi Makhija, Maher Malaeb, Manoj K, James
-McNeilis, Naturale0, nju-luke, Pierre-Louis Pécheux, Jay Qi, Lucas Rebscher,
-Craig Rodrigues, Skywhat, Hercules Smith, David Stevens, Vesna Tanko,
-TrWestdoor, Victor Wang, Mike Lee Williams, Jay Wong, Chenchen Xu, YaoZh1918.
+caoyi, Олег Демиденко, Charles-Emmanuel Dias, dmamylin, Lauriane Ducasse,
+Marc Feger, franckjay, Lukas Galke, Pierre-François Gimenez, Zachary
+Glassman, Nicolas Hug, Janniks, Doruk Kilitcioglu, Ravi Raju Krishna, Hengji
+Liu, Maher Malaeb, Manoj K, Naturale0, nju-luke, Jay Qi, Skywhat, David
+Stevens, Victor Wang, Mike Lee Williams, Jay Wong, Chenchen Xu, YaoZh1918.
 
 Thanks a lot :) !
 
 Development Status
 ------------------
 
-Starting from version 1.1.0 (September 2019), I will only maintain the package,
-provide bugfixes, and perhaps sometimes perf improvements. I have less time to
-dedicate to it now, so I'm unabe to consider new features.
-
-For bugs, issues or questions about [Surprise](https://surpriselib.com), please
-avoid sending me emails; I will most likely not be able to answer). Please use
-the GitHub [project page](https://github.com/NicolasHug/Surprise) instead, so
-that others can also benefit from it.
+Starting from version 1.1.0 (September 19), we will only maintain the
+package and provide bugfixes. No new features will be considered.
+
+For bugs, issues or questions about [Surprise](http://surpriselib.com),
+please use the GitHub [project page](https://github.com/NicolasHug/Surprise).
+Please don't send emails (we will not answer).
```

### Comparing `scikit_surprise-1.1.4/README.md` & `scikit-surprise-1.1rc0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,224 +1,229 @@
-[![GitHub version](https://badge.fury.io/gh/nicolashug%2FSurprise.svg)](https://badge.fury.io/gh/nicolashug%2FSurprise)
-[![Documentation Status](https://readthedocs.org/projects/surprise/badge/?version=stable)](https://surprise.readthedocs.io/en/stable/?badge=stable)
-[![python versions](https://img.shields.io/badge/python-3.8+-blue.svg)](https://surpriselib.com)
-[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![DOI](https://joss.theoj.org/papers/10.21105/joss.02174/status.svg)](https://doi.org/10.21105/joss.02174)
-
-[![logo](./logo_black.svg)](https://surpriselib.com)
-
-Overview
---------
-
-[Surprise](https://surpriselib.com) is a Python
-[scikit](https://projects.scipy.org/scikits.html) for building and analyzing
-recommender systems that deal with explicit rating data.
-
-[Surprise](https://surpriselib.com) **was designed with the
-following purposes in mind**:
-
-- Give users perfect control over their experiments. To this end, a strong
-  emphasis is laid on
-  [documentation](https://surprise.readthedocs.io/en/stable/index.html), which we
-  have tried to make as clear and precise as possible by pointing out every
-  detail of the algorithms.
-- Alleviate the pain of [Dataset
-  handling](https://surprise.readthedocs.io/en/stable/getting_started.html#load-a-custom-dataset).
-  Users can use both *built-in* datasets
-  ([Movielens](https://grouplens.org/datasets/movielens/),
-  [Jester](https://eigentaste.berkeley.edu/dataset/)), and their own *custom*
-  datasets.
-- Provide various ready-to-use [prediction
-  algorithms](https://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html)
-  such as [baseline
-  algorithms](https://surprise.readthedocs.io/en/stable/basic_algorithms.html),
-  [neighborhood
-  methods](https://surprise.readthedocs.io/en/stable/knn_inspired.html), matrix
-  factorization-based (
-  [SVD](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD),
-  [PMF](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#unbiased-note),
-  [SVD++](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp),
-  [NMF](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)),
-  and [many
-  others](https://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html).
-  Also, various [similarity
-  measures](https://surprise.readthedocs.io/en/stable/similarities.html)
-  (cosine, MSD, pearson...) are built-in.
-- Make it easy to implement [new algorithm
-  ideas](https://surprise.readthedocs.io/en/stable/building_custom_algo.html).
-- Provide tools to [evaluate](https://surprise.readthedocs.io/en/stable/model_selection.html),
-  [analyse](https://nbviewer.jupyter.org/github/NicolasHug/Surprise/tree/master/examples/notebooks/KNNBasic_analysis.ipynb/)
-  and
-  [compare](https://nbviewer.jupyter.org/github/NicolasHug/Surprise/blob/master/examples/notebooks/Compare.ipynb)
-  the algorithms' performance. Cross-validation procedures can be run very
-  easily using powerful CV iterators (inspired by
-  [scikit-learn](https://scikit-learn.org/) excellent tools), as well as
-  [exhaustive search over a set of
-  parameters](https://surprise.readthedocs.io/en/stable/getting_started.html#tune-algorithm-parameters-with-gridsearchcv).
-
-
-The name *SurPRISE* (roughly :) ) stands for *Simple Python RecommendatIon
-System Engine*.
-
-Please note that surprise does not support implicit ratings or content-based
-information.
-
-
-Getting started, example
-------------------------
-
-Here is a simple example showing how you can (down)load a dataset, split it for
-5-fold cross-validation, and compute the MAE and RMSE of the
-[SVD](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)
-algorithm.
-
-
-```python
-from surprise import SVD
-from surprise import Dataset
-from surprise.model_selection import cross_validate
-
-# Load the movielens-100k dataset (download it if needed).
-data = Dataset.load_builtin('ml-100k')
-
-# Use the famous SVD algorithm.
-algo = SVD()
-
-# Run 5-fold cross-validation and print results.
-cross_validate(algo, data, measures=['RMSE', 'MAE'], cv=5, verbose=True)
-```
-
-**Output**:
-
-```
-Evaluating RMSE, MAE of algorithm SVD on 5 split(s).
-
-                  Fold 1  Fold 2  Fold 3  Fold 4  Fold 5  Mean    Std     
-RMSE (testset)    0.9367  0.9355  0.9378  0.9377  0.9300  0.9355  0.0029  
-MAE (testset)     0.7387  0.7371  0.7393  0.7397  0.7325  0.7375  0.0026  
-Fit time          0.62    0.63    0.63    0.65    0.63    0.63    0.01    
-Test time         0.11    0.11    0.14    0.14    0.14    0.13    0.02    
-```
-
-[Surprise](https://surpriselib.com) can do **much** more (e.g,
-[GridSearchCV](https://surprise.readthedocs.io/en/stable/getting_started.html#tune-algorithm-parameters-with-gridsearchcv))!
-You'll find [more usage
-examples](https://surprise.readthedocs.io/en/stable/getting_started.html) in the
-[documentation ](https://surprise.readthedocs.io/en/stable/index.html).
-
-
-Benchmarks
-----------
-
-Here are the average RMSE, MAE and total execution time of various algorithms
-(with their default parameters) on a 5-fold cross-validation procedure. The
-datasets are the [Movielens](https://grouplens.org/datasets/movielens/) 100k and
-1M datasets. The folds are the same for all the algorithms. All experiments are
-run on a laptop with an intel i5 11th Gen 2.60GHz. The code
-for generating these tables can be found in the [benchmark
-example](https://github.com/NicolasHug/Surprise/tree/master/examples/benchmark.py).
-
-| [Movielens 100k](http://grouplens.org/datasets/movielens/100k)                                                                         |   RMSE |   MAE | Time    |
-|:---------------------------------------------------------------------------------------------------------------------------------------|-------:|------:|:--------|
-| [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)      |  0.934 | 0.737 | 0:00:06 |
-| [SVD++ (cache_ratings=False)](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.919 | 0.721 | 0:01:39 |
-| [SVD++ (cache_ratings=True)](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.919 | 0.721 | 0:01:22 |
-| [NMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)      |  0.963 | 0.758 | 0:00:06 |
-| [Slope One](http://surprise.readthedocs.io/en/stable/slope_one.html#surprise.prediction_algorithms.slope_one.SlopeOne)                 |  0.946 | 0.743 | 0:00:09 |
-| [k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBasic)                        |  0.98  | 0.774 | 0:00:08 |
-| [Centered k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNWithMeans)           |  0.951 | 0.749 | 0:00:09 |
-| [k-NN Baseline](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBaseline)            |  0.931 | 0.733 | 0:00:13 |
-| [Co-Clustering](http://surprise.readthedocs.io/en/stable/co_clustering.html#surprise.prediction_algorithms.co_clustering.CoClustering) |  0.963 | 0.753 | 0:00:06 |
-| [Baseline](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.baseline_only.BaselineOnly)   |  0.944 | 0.748 | 0:00:02 |
-| [Random](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.random_pred.NormalPredictor)    |  1.518 | 1.219 | 0:00:01 |
-
-
-| [Movielens 1M](https://grouplens.org/datasets/movielens/1m)                                                                             |   RMSE |   MAE | Time    |
-|:----------------------------------------------------------------------------------------------------------------------------------------|-------:|------:|:--------|
-| [SVD](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)      |  0.873 | 0.686 | 0:01:07 |
-| [SVD++ (cache_ratings=False)](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.862 | 0.672 | 0:41:06 |
-| [SVD++ (cache_ratings=True)](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.862 | 0.672 | 0:34:55 |
-| [NMF](https://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)      |  0.916 | 0.723 | 0:01:39 |
-| [Slope One](http://surprise.readthedocs.io/en/stable/slope_one.html#surprise.prediction_algorithms.slope_one.SlopeOne)                 |  0.907 | 0.715 | 0:02:31 |
-| [k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBasic)                        |  0.923 | 0.727 | 0:05:27 |
-| [Centered k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNWithMeans)           |  0.929 | 0.738 | 0:05:43 |
-| [k-NN Baseline](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBaseline)            |  0.895 | 0.706 | 0:05:55 |
-| [Co-Clustering](http://surprise.readthedocs.io/en/stable/co_clustering.html#surprise.prediction_algorithms.co_clustering.CoClustering) |  0.915 | 0.717 | 0:00:31 |
-| [Baseline](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.baseline_only.BaselineOnly)   |  0.909 | 0.719 | 0:00:19 |
-| [Random](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.random_pred.NormalPredictor)    |  1.504 | 1.206 | 0:00:19 |
-
-Installation
-------------
-
-With pip (you'll need [numpy](https://www.numpy.org/), and a C compiler. Windows
-users might prefer using conda):
-
-    $ pip install numpy
-    $ pip install scikit-surprise
-
-With conda:
-
-    $ conda install -c conda-forge scikit-surprise
-
-For the latest version, you can also clone the repo and build the source
-(you'll first need [Cython](https://cython.org/) and
-[numpy](https://www.numpy.org/)):
-
-    $ pip install numpy cython
-    $ git clone https://github.com/NicolasHug/surprise.git
-    $ cd surprise
-    $ python setup.py install
-
-License and reference
----------------------
-
-This project is licensed under the [BSD
-3-Clause](https://opensource.org/licenses/BSD-3-Clause) license, so it can be
-used for pretty much everything, including commercial applications.
-
-I'd love to know how Surprise is useful to you. Please don't hesitate to open
-an issue and describe how you use it!
-
-Please make sure to cite the
-[paper](https://joss.theoj.org/papers/10.21105/joss.02174) if you use
-Surprise for your research:
-
-    @article{Hug2020,
-      doi = {10.21105/joss.02174},
-      url = {https://doi.org/10.21105/joss.02174},
-      year = {2020},
-      publisher = {The Open Journal},
-      volume = {5},
-      number = {52},
-      pages = {2174},
-      author = {Nicolas Hug},
-      title = {Surprise: A Python library for recommender systems},
-      journal = {Journal of Open Source Software}
-    }
-
-Contributors
-------------
-
-The following persons have contributed to [Surprise](https://surpriselib.com):
-
-ashtou, Abhishek Bhatia, bobbyinfj, caoyi, Chieh-Han Chen,  Raphael-Dayan, Олег
-Демиденко, Charles-Emmanuel Dias, dmamylin, Lauriane Ducasse, Marc Feger,
-franckjay, Lukas Galke, Tim Gates, Pierre-François Gimenez, Zachary Glassman,
-Jeff Hale, Nicolas Hug, Janniks, jyesawtellrickson, Doruk Kilitcioglu, Ravi Raju
-Krishna, lapidshay, Hengji Liu, Ravi Makhija, Maher Malaeb, Manoj K, James
-McNeilis, Naturale0, nju-luke, Pierre-Louis Pécheux, Jay Qi, Lucas Rebscher,
-Craig Rodrigues, Skywhat, Hercules Smith, David Stevens, Vesna Tanko,
-TrWestdoor, Victor Wang, Mike Lee Williams, Jay Wong, Chenchen Xu, YaoZh1918.
-
-Thanks a lot :) !
-
-Development Status
-------------------
-
-Starting from version 1.1.0 (September 2019), I will only maintain the package,
-provide bugfixes, and perhaps sometimes perf improvements. I have less time to
-dedicate to it now, so I'm unabe to consider new features.
-
-For bugs, issues or questions about [Surprise](https://surpriselib.com), please
-avoid sending me emails; I will most likely not be able to answer). Please use
-the GitHub [project page](https://github.com/NicolasHug/Surprise) instead, so
-that others can also benefit from it.
+Metadata-Version: 2.1
+Name: scikit-surprise
+Version: 1.1rc0
+Summary: An easy-to-use library for recommender systems.
+Home-page: http://surpriselib.com
+Author: Nicolas Hug
+Author-email: contact@nicolas-hug.com
+License: GPLv3+
+Description: [![GitHub version](https://badge.fury.io/gh/nicolashug%2FSurprise.svg)](https://badge.fury.io/gh/nicolashug%2FSurprise)
+        [![Documentation Status](https://readthedocs.org/projects/surprise/badge/?version=stable)](http://surprise.readthedocs.io/en/stable/?badge=stable)
+        [![Build Status](https://travis-ci.org/NicolasHug/Surprise.svg?branch=master)](https://travis-ci.org/NicolasHug/Surprise)
+        [![python versions](https://img.shields.io/badge/python-2.7%2C%203.5%2C%203.6-blue.svg)](http://surpriselib.com)
+        [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+        
+        [![logo](logo_black.svg)](http://surpriselib.com)
+        
+        Overview
+        --------
+        
+        [Surprise](http://surpriselib.com) is a Python
+        [scikit](https://www.scipy.org/scikits.html) building and analyzing
+        recommender systems that deal with explicit rating data.
+        
+        [Surprise](http://surpriselib.com) **was designed with the
+        following purposes in mind**:
+        
+        - Give users perfect control over their experiments. To this end, a strong
+          emphasis is laid on
+          [documentation](http://surprise.readthedocs.io/en/stable/index.html), which we
+          have tried to make as clear and precise as possible by pointing out every
+          detail of the algorithms.
+        - Alleviate the pain of [Dataset
+          handling](http://surprise.readthedocs.io/en/stable/getting_started.html#load-a-custom-dataset).
+          Users can use both *built-in* datasets
+          ([Movielens](http://grouplens.org/datasets/movielens/),
+          [Jester](http://eigentaste.berkeley.edu/dataset/)), and their own *custom*
+          datasets.
+        - Provide various ready-to-use [prediction
+          algorithms](http://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html)
+          such as [baseline
+          algorithms](http://surprise.readthedocs.io/en/stable/basic_algorithms.html),
+          [neighborhood
+          methods](http://surprise.readthedocs.io/en/stable/knn_inspired.html), matrix
+          factorization-based (
+          [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD),
+          [PMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#unbiased-note),
+          [SVD++](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp),
+          [NMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)),
+          and [many
+          others](http://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html).
+          Also, various [similarity
+          measures](http://surprise.readthedocs.io/en/stable/similarities.html)
+          (cosine, MSD, pearson...) are built-in.
+        - Make it easy to implement [new algorithm
+          ideas](http://surprise.readthedocs.io/en/stable/building_custom_algo.html).
+        - Provide tools to [evaluate](http://surprise.readthedocs.io/en/stable/model_selection.html),
+          [analyse](http://nbviewer.jupyter.org/github/NicolasHug/Surprise/tree/master/examples/notebooks/KNNBasic_analysis.ipynb/)
+          and
+          [compare](http://nbviewer.jupyter.org/github/NicolasHug/Surprise/blob/master/examples/notebooks/Compare.ipynb)
+          the algorithms performance. Cross-validation procedures can be run very
+          easily using powerful CV iterators (inspired by
+          [scikit-learn](http://scikit-learn.org/) excellent tools), as well as
+          [exhaustive search over a set of
+          parameters](http://surprise.readthedocs.io/en/stable/getting_started.html#tune-algorithm-parameters-with-gridsearchcv).
+        
+        
+        The name *SurPRISE* (roughly :) ) stands for Simple Python RecommendatIon
+        System Engine.
+        
+        Please note that surprise does not support implicit ratings or content-based
+        information.
+        
+        
+        Getting started, example
+        ------------------------
+        
+        Here is a simple example showing how you can (down)load a dataset, split it for
+        5-fold cross-validation, and compute the MAE and RMSE of the
+        [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)
+        algorithm.
+        
+        
+        ```python
+        from surprise import SVD
+        from surprise import Dataset
+        from surprise.model_selection import cross_validate
+        
+        # Load the movielens-100k dataset (download it if needed).
+        data = Dataset.load_builtin('ml-100k')
+        
+        # Use the famous SVD algorithm.
+        algo = SVD()
+        
+        # Run 5-fold cross-validation and print results.
+        cross_validate(algo, data, measures=['RMSE', 'MAE'], cv=5, verbose=True)
+        ```
+        
+        **Output**:
+        
+        ```
+        Evaluating RMSE, MAE of algorithm SVD on 5 split(s).
+        
+                    Fold 1  Fold 2  Fold 3  Fold 4  Fold 5  Mean    Std
+        RMSE        0.9311  0.9370  0.9320  0.9317  0.9391  0.9342  0.0032
+        MAE         0.7350  0.7375  0.7341  0.7342  0.7375  0.7357  0.0015
+        Fit time    6.53    7.11    7.23    7.15    3.99    6.40    1.23
+        Test time   0.26    0.26    0.25    0.15    0.13    0.21    0.06
+        ```
+        
+        [Surprise](http://surpriselib.com) can do **much** more (e.g,
+        [GridSearchCV](http://surprise.readthedocs.io/en/stable/getting_started.html#tune-algorithm-parameters-with-gridsearchcv))!
+        You'll find [more usage
+        examples](http://surprise.readthedocs.io/en/stable/getting_started.html) in the
+        [documentation ](http://surprise.readthedocs.io/en/stable/index.html).
+        
+        
+        Benchmarks
+        ----------
+        
+        Here are the average RMSE, MAE and total execution time of various algorithms
+        (with their default parameters) on a 5-fold cross-validation procedure. The
+        datasets are the [Movielens](http://grouplens.org/datasets/movielens/) 100k and
+        1M datasets. The folds are the same for all the algorithms. All experiments are
+        run on a notebook with Intel Core i5 7th gen (2.5 GHz) and 8Go RAM.  The code
+        for generating these tables can be found in the [benchmark
+        example](https://github.com/NicolasHug/Surprise/tree/master/examples/benchmark.py).
+        
+        | [Movielens 100k](http://grouplens.org/datasets/movielens/100k)                                                                         |   RMSE |   MAE | Time    |
+        |:---------------------------------------------------------------------------------------------------------------------------------------|-------:|------:|:--------|
+        | [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)      |  0.934 | 0.737 | 0:00:11 |
+        | [SVD++](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.92  | 0.722 | 0:09:03 |
+        | [NMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)      |  0.963 | 0.758 | 0:00:15 |
+        | [Slope One](http://surprise.readthedocs.io/en/stable/slope_one.html#surprise.prediction_algorithms.slope_one.SlopeOne)                 |  0.946 | 0.743 | 0:00:08 |
+        | [k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBasic)                        |  0.98  | 0.774 | 0:00:10 |
+        | [Centered k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNWithMeans)           |  0.951 | 0.749 | 0:00:10 |
+        | [k-NN Baseline](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBaseline)            |  0.931 | 0.733 | 0:00:12 |
+        | [Co-Clustering](http://surprise.readthedocs.io/en/stable/co_clustering.html#surprise.prediction_algorithms.co_clustering.CoClustering) |  0.963 | 0.753 | 0:00:03 |
+        | [Baseline](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.baseline_only.BaselineOnly)   |  0.944 | 0.748 | 0:00:01 |
+        | [Random](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.random_pred.NormalPredictor)    |  1.514 | 1.215 | 0:00:01 |
+        
+        
+        | [Movielens 1M](http://grouplens.org/datasets/movielens/1m)                                                                             |   RMSE |   MAE | Time    |
+        |:---------------------------------------------------------------------------------------------------------------------------------------|-------:|------:|:--------|
+        | [SVD](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVD)      |  0.873 | 0.686 | 0:02:13 |
+        | [SVD++](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.SVDpp)  |  0.862 | 0.673 | 2:54:19 |
+        | [NMF](http://surprise.readthedocs.io/en/stable/matrix_factorization.html#surprise.prediction_algorithms.matrix_factorization.NMF)      |  0.916 | 0.724 | 0:02:31 |
+        | [Slope One](http://surprise.readthedocs.io/en/stable/slope_one.html#surprise.prediction_algorithms.slope_one.SlopeOne)                 |  0.907 | 0.715 | 0:02:31 |
+        | [k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBasic)                        |  0.923 | 0.727 | 0:05:27 |
+        | [Centered k-NN](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNWithMeans)           |  0.929 | 0.738 | 0:05:43 |
+        | [k-NN Baseline](http://surprise.readthedocs.io/en/stable/knn_inspired.html#surprise.prediction_algorithms.knns.KNNBaseline)            |  0.895 | 0.706 | 0:05:55 |
+        | [Co-Clustering](http://surprise.readthedocs.io/en/stable/co_clustering.html#surprise.prediction_algorithms.co_clustering.CoClustering) |  0.915 | 0.717 | 0:00:31 |
+        | [Baseline](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.baseline_only.BaselineOnly)   |  0.909 | 0.719 | 0:00:19 |
+        | [Random](http://surprise.readthedocs.io/en/stable/basic_algorithms.html#surprise.prediction_algorithms.random_pred.NormalPredictor)    |  1.504 | 1.206 | 0:00:19 |
+        
+        
+        Installation
+        ------------
+        
+        With pip (you'll need [numpy](http://www.numpy.org/), and a C compiler. Windows
+        users might prefer using conda):
+        
+            $ pip install numpy
+            $ pip install scikit-surprise
+        
+        With conda:
+        
+            $ conda install -c conda-forge scikit-surprise
+        
+        For the latest version, you can also clone the repo and build the source
+        (you'll first need [Cython](http://cython.org/) and
+        [numpy](http://www.numpy.org/)):
+        
+            $ pip install numpy cython
+            $ git clone https://github.com/NicolasHug/surprise.git
+            $ cd surprise
+            $ python setup.py install
+        
+        License
+        -------
+        
+        This project is licensed under the [BSD
+        3-Clause](https://opensource.org/licenses/BSD-3-Clause) license, so it can be
+        used for pretty much everything, including commercial applications. Please let
+        us know how [Surprise](http://surpriselib.com) is useful to you!
+        
+        Here is a Bibtex entry if you ever need to cite Surprise in a research paper
+        (please keep us posted, we would love to know if Surprise was helpful to you):
+        
+            @Misc{Surprise,
+            author =   {Hug, Nicolas},
+            title =    { {S}urprise, a {P}ython library for recommender systems},
+            howpublished = {\url{http://surpriselib.com}},
+            year = {2017}
+            }
+        
+        Contributors
+        ------------
+        
+        The following persons have contributed to [Surprise](http://surpriselib.com):
+        
+        caoyi, Олег Демиденко, Charles-Emmanuel Dias, dmamylin, Lauriane Ducasse,
+        Marc Feger, franckjay, Lukas Galke, Pierre-François Gimenez, Zachary
+        Glassman, Nicolas Hug, Janniks, Doruk Kilitcioglu, Ravi Raju Krishna, Hengji
+        Liu, Maher Malaeb, Manoj K, Naturale0, nju-luke, Jay Qi, Skywhat, David
+        Stevens, Victor Wang, Mike Lee Williams, Jay Wong, Chenchen Xu, YaoZh1918.
+        
+        Thanks a lot :) !
+        
+        Development Status
+        ------------------
+        
+        Starting from version 1.1.0 (September 19), we will only maintain the
+        package and provide bugfixes. No new features will be considered.
+        
+        For bugs, issues or questions about [Surprise](http://surpriselib.com),
+        please use the GitHub [project page](https://github.com/NicolasHug/Surprise).
+        Please don't send emails (we will not answer).
+        
+Keywords: recommender recommendation system
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2.7
+Description-Content-Type: text/markdown
```

### Comparing `scikit_surprise-1.1.4/doc/Makefile` & `scikit-surprise-1.1rc0/doc/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 SPHINXOPTS    =
 SPHINXBUILD   = sphinx-build
 PAPER         =
 BUILDDIR      = build
 
 # User-friendly check for sphinx-build
 ifeq ($(shell which $(SPHINXBUILD) >/dev/null 2>&1; echo $$?), 1)
-$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don't have Sphinx installed, grab it from https://sphinx-doc.org/)
+$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don't have Sphinx installed, grab it from http://sphinx-doc.org/)
 endif
 
 # Internal variables.
 PAPEROPT_a4     = -D latex_paper_size=a4
 PAPEROPT_letter = -D latex_paper_size=letter
 ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) source
 # the i18n builder cannot share the environment and doctrees with the others
```

### Comparing `scikit_surprise-1.1.4/doc/make.bat` & `scikit-surprise-1.1rc0/doc/make.bat`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
 	echo.may add the Sphinx directory to PATH.
 	echo.
 	echo.If you don't have Sphinx installed, grab it from
-	echo.https://sphinx-doc.org/
+	echo.http://sphinx-doc.org/
 	exit /b 1
 )
 
 :sphinx_ok
 
 
 if "%1" == "html" (
```

### Comparing `scikit_surprise-1.1.4/doc/source/FAQ.rst` & `scikit-surprise-1.1rc0/doc/source/FAQ.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 an SVD algorithm on the whole dataset, and then predict all the ratings for the
 pairs (user, item) that are not in the training set. We then retrieve the
 top-10 prediction for each user.
 
 .. literalinclude:: ../../examples/top_n_recommendations.py
     :caption: From file ``examples/top_n_recommendations.py``
     :name: top_n_recommendations.py
-    :lines: 8-
+    :lines: 10-
 
 .. _precision_recall_at_k:
 
 How to compute precision@k and recall@k
 -----------------------------------------------------------------------
 
 Here is an example where we compute Precision@k and Recall@k for each user:
@@ -31,22 +31,18 @@
 :math:`\text{Recall@k} = \frac{ | \{ \text{Recommended items that are relevant} \} | }{ | \{ \text{Relevant items} \} | }`
 
 An item is considered relevant if its true rating :math:`r_{ui}` is greater
 than a given threshold.  An item is considered recommended if its estimated
 rating :math:`\hat{r}_{ui}` is greater than the threshold, and if it is among
 the k highest estimated ratings.
 
-Note that in the edge cases where division by zero occurs, 
-Precision@k and Recall@k values are undefined. 
-As a convention, we set their values to 0 in such cases. 
-
 .. literalinclude:: ../../examples/precision_recall_at_k.py
     :caption: From file ``examples/precision_recall_at_k.py``
     :name: precision_recall_at_k.py
-    :lines: 5-
+    :lines: 7-
 
 .. _get_k_nearest_neighbors:
 
 How to get the k nearest neighbors of a user (or item)
 --------------------------------------------------------------
 
 You can use the :meth:`get_neighbors()
@@ -76,15 +72,15 @@
 their raw/inner ids (see :ref:`this note <raw_inner_note>`), but it all boils
 down to the use of :meth:`get_neighbors()
 <surprise.prediction_algorithms.algo_base.AlgoBase.get_neighbors>`:
 
 .. literalinclude:: ../../examples/k_nearest_neighbors.py
     :caption: From file ``examples/k_nearest_neighbors.py``
     :name: k_nearest_neighbors.py
-    :lines: 9-
+    :lines: 10-
 
 Naturally, the same can be done for users with minor modifications.
 
 .. _serialize_an_algorithm:
 
 How to serialize an algorithm
 -----------------------------
@@ -93,26 +89,26 @@
 <surprise.dump.dump>` and :func:`load() <surprise.dump.load>` functions. Here
 is a small example where the SVD algorithm is trained on a dataset and
 serialized. It is then reloaded and can be used again for making predictions:
 
 .. literalinclude:: ../../examples/serialize_algorithm.py
     :caption: From file ``examples/serialize_algorithm.py``
     :name: serialize_algorithm.py
-    :lines: 7-
+    :lines: 9-
 
 .. _further_analysis:
 
 Algorithms can be serialized along with their predictions, so that can be
 further analyzed or compared with other algorithms, using pandas dataframes.
 Some examples are given in the two following notebooks:
 
     * `Dumping and analysis of the KNNBasic algorithm
-      <https://nbviewer.jupyter.org/github/NicolasHug/Surprise/tree/master/examples/notebooks/KNNBasic_analysis.ipynb/>`_.
+      <http://nbviewer.jupyter.org/github/NicolasHug/Surprise/tree/master/examples/notebooks/KNNBasic_analysis.ipynb/>`_.
     * `Comparison of two algorithms
-      <https://nbviewer.jupyter.org/github/NicolasHug/Surprise/tree/master/examples/notebooks/Compare.ipynb/>`_.
+      <http://nbviewer.jupyter.org/github/NicolasHug/Surprise/tree/master/examples/notebooks/Compare.ipynb/>`_.
 
 How to build my own prediction algorithm
 ----------------------------------------
 
 There's a whole guide :ref:`here<building_custom_algo>`.
 
 .. _raw_inner_note:
@@ -165,15 +161,15 @@
 <surprise.Trainset>` object to build a testset that can be then used
 with the :meth:`test()
 <surprise.prediction_algorithms.algo_base.AlgoBase.test>` method:
 
 .. literalinclude:: ../../examples/evaluate_on_trainset.py
     :caption: From file ``examples/evaluate_on_trainset.py``
     :name: evaluate_on_trainset.py
-    :lines: 7-21
+    :lines: 9-25
 
 Check out the example file for more usage examples.
 
 .. _unbiased_estimate_after_tuning:
 
 How to save some data for unbiased accuracy estimation
 ------------------------------------------------------
@@ -183,15 +179,15 @@
 you may want to split your data into two sets A and B. A is used for parameter
 tuning using grid search, and B is used for unbiased estimation. This can be
 done as follows:
 
 .. literalinclude:: ../../examples/split_data_for_unbiased_estimation.py
     :caption: From file ``examples/split_data_for_unbiased_estimation.py``
     :name: split_data_for_unbiased_estimation.py
-    :lines: 8-
+    :lines: 10-
 
 How to have reproducible experiments
 ------------------------------------
 
 Some algorithms randomly initialize their parameters (sometimes with
 ``numpy``), and the cross-validation folds are also randomly generated. If you
 need to reproduce your experiments multiple times, you just have to set the
```

### Comparing `scikit_surprise-1.1.4/doc/source/building_custom_algo.rst` & `scikit-surprise-1.1rc0/doc/build/html/_sources/building_custom_algo.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,26 @@
 <surprise.prediction_algorithms.algo_base.AlgoBase.predict>` method. It takes
 in an **inner** user id, an **inner** item id (see :ref:`this note
 <raw_inner_note>`), and returns the estimated rating :math:`\hat{r}_{ui}`:
 
 .. literalinclude:: ../../examples/building_custom_algorithms/most_basic_algorithm.py
     :caption: From file ``examples/building_custom_algorithms/most_basic_algorithm.py``
     :name: most_basic_algorithm.py
-    :lines: 7-
+    :lines: 9-
 
 This algorithm is the dumbest we could have thought of: it just predicts a
 rating of 3, regardless of users and items.
 
 If you want to store additional information about the prediction, you can also
 return a dictionary with given details: ::
 
     def estimate(self, u, i):
 
-        details = {
-            'info1' : 'That was',
-            'info2' : 'easy stuff :)'
-        }
+        details = {'info1' : 'That was',
+                   'info2' : 'easy stuff :)'}
         return 3, details
 
 This dictionary will be stored in the :class:`prediction
 <surprise.prediction_algorithms.predictions.Prediction>` as the ``details``
 field and can be used for :ref:`later analysis <further_analysis>`.
 
 
@@ -50,15 +48,15 @@
 the ratings of the trainset. As this is a constant value that does not depend
 on current user or item, we would rather compute it once and for all. This can
 be done by defining the ``fit`` method:
 
 .. literalinclude:: ../../examples/building_custom_algorithms/most_basic_algorithm2.py
     :caption: From file ``examples/building_custom_algorithms/most_basic_algorithm2.py``
     :name: most_basic_algorithm2.py
-    :lines: 13-32
+    :lines: 16-37
 
 
 The ``fit`` method is called e.g. by the :func:`cross_validate
 <surprise.model_selection.validation.cross_validate>` function at each fold of
 a cross-validation process, (but you can also :ref:`call it yourself
 <use_cross_validation_iterators>`).  Before doing anything, you should call the
 base class :meth:`fit()
@@ -80,15 +78,15 @@
 To illustrate its usage, let's make an algorithm that predicts an average
 between the mean of all ratings, the mean rating of the user and the mean
 rating for the item:
 
 .. literalinclude:: ../../examples/building_custom_algorithms/mean_rating_user_item.py
     :caption: From file ``examples/building_custom_algorithms/mean_rating_user_item.py``
     :name: mean_rating_user_item.py
-    :lines: 19-31
+    :lines: 23-35
 
 Note that it would have been a better idea to compute all the user means in the
 ``fit`` method, thus avoiding the same computations multiple times.
 
 
 When the prediction is impossible
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -123,13 +121,13 @@
 :meth:`compute_similarities()
 <surprise.prediction_algorithms.algo_base.AlgoBase.compute_similarities>` can
 be called in the ``fit`` method (or anywhere else).
 
 .. literalinclude:: ../../examples/building_custom_algorithms/with_baselines_or_sim.py
     :caption: From file ``examples/building_custom_algorithms/.with_baselines_or_sim.py``
     :name: with_baselines_or_sim.py
-    :lines: 11-43
+    :lines: 15-47
 
 
 Feel free to explore the prediction_algorithms package `source
 <https://github.com/NicolasHug/Surprise/tree/master/surprise/prediction_algorithms>`_
 to get an idea of what can be done.
```

### Comparing `scikit_surprise-1.1.4/doc/source/conf.py` & `scikit-surprise-1.1rc0/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,14 @@
     'sphinxcontrib.bibtex',
     'sphinxcontrib.spelling',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['.templates']
 
-bibtex_bibfiles = ['refs.bib']
-
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
@@ -74,15 +72,15 @@
 release = '1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = "en"
+language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
```

### Comparing `scikit_surprise-1.1.4/doc/source/getting_started.rst` & `scikit-surprise-1.1rc0/doc/build/html/_sources/getting_started.rst.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 :ref:`algorithms<prediction_algorithms>` and :ref:`datasets <dataset>` for you
 to play with. In its simplest form, it only takes a few lines of code to
 run a cross-validation procedure:
 
 .. literalinclude:: ../../examples/basic_usage.py
     :caption: From file ``examples/basic_usage.py``
     :name: basic_usage.py
-    :lines: 7-
+    :lines: 9-
 
 The result should be as follows (actual values may vary due to randomization):
 
 .. parsed-literal::
 
     Evaluating RMSE, MAE of algorithm SVD on 5 split(s).
 
@@ -33,15 +33,15 @@
     MAE         0.7350  0.7375  0.7341  0.7342  0.7375  0.7357  0.0015
     Fit time    6.53    7.11    7.23    7.15    3.99    6.40    1.23
     Test time   0.26    0.26    0.25    0.15    0.13    0.21    0.06
 
 
 The :meth:`load_builtin() <surprise.dataset.Dataset.load_builtin>` method will
 offer to download the `movielens-100k dataset
-<https://grouplens.org/datasets/movielens/>`_ if it has not already been
+<http://grouplens.org/datasets/movielens/>`_ if it has not already been
 downloaded, and it will save it in the ``.surprise_data`` folder in your home
 directory (you can also choose to save it :ref:`somewhere else <data_folder>`).
 
 We are here using the well-known
 :class:`SVD<surprise.prediction_algorithms.matrix_factorization.SVD>`
 algorithm, but many other algorithms are available. See
 :ref:`prediction_algorithms` for more details.
@@ -65,15 +65,15 @@
 train the algorithm on the trainset, and the :meth:`test()
 <surprise.prediction_algorithms.algo_base.AlgoBase.test>` method which will
 return the predictions made from the testset:
 
 .. literalinclude:: ../../examples/train_test_split.py
     :caption: From file ``examples/train_test_split.py``
     :name: train_test_split.py
-    :lines: 6-
+    :lines: 8-
 
 Result:
 
 .. parsed-literal::
 
     RMSE: 0.9411
 
@@ -98,25 +98,25 @@
 :meth:`build_full_trainset()
 <surprise.dataset.DatasetAutoFolds.build_full_trainset>` method which will
 build a :class:`trainset <surprise.Trainset>` object:
 
 .. literalinclude:: ../../examples/predict_ratings.py
     :caption: From file ``examples/predict_ratings.py``
     :name: predict_ratings.py
-    :lines: 7-17
+    :lines: 9-20
 
 We can now predict ratings by directly calling the :meth:`predict()
 <surprise.prediction_algorithms.algo_base.AlgoBase.predict>` method.  Let's say
 you're interested in user 196 and item 302 (make sure they're in the
 trainset!), and you know that the true rating :math:`r_{ui} = 4`:
 
 .. literalinclude:: ../../examples/predict_ratings.py
     :caption: From file ``examples/predict_ratings.py``
     :name: predict_ratings2.py
-    :lines: 20-24
+    :lines: 23-27
 
 The result should be:
 
 .. parsed-literal::
 
     user: 196        item: 302        r_ui = 4.00   est = 4.06   {'actual_k': 40, 'was_impossible': False}
 
@@ -148,15 +148,15 @@
 
 - To load a dataset from a file (e.g. a csv file), you will need the
   :meth:`load_from_file() <surprise.dataset.Dataset.load_from_file>` method:
 
   .. literalinclude:: ../../examples/load_custom_dataset.py
       :caption: From file ``examples/load_custom_dataset.py``
       :name: load_custom_dataset.py
-      :lines: 8-24
+      :lines: 12-28
 
   For more details about readers and how to use them, see the :class:`Reader
   class <surprise.reader.Reader>` documentation.
 
   .. note::
       As you already know from the previous section, the Movielens-100k dataset
       is built-in so a much quicker way to load the dataset is to do ``data =
@@ -171,15 +171,15 @@
   three columns, corresponding to the user (raw) ids, the item (raw) ids, and
   the ratings in this order. Each row thus corresponds to a given rating. This
   is not restrictive as you can reorder the columns of your dataframe easily.
 
   .. literalinclude:: ../../examples/load_from_dataframe.py
       :caption: From file ``examples/load_from_dataframe.py``
       :name: load_dom_dataframe.py
-      :lines: 6-27
+      :lines: 8-29
 
   The dataframe initially looks like this:
 
   .. parsed-literal::
 
             itemID  rating    userID
       0       1       3         9
@@ -192,25 +192,25 @@
 .. _use_cross_validation_iterators:
 
 Use cross-validation iterators
 ------------------------------
 
 For cross-validation, we can use the :func:`cross_validate()
 <surprise.model_selection.validation.cross_validate>` function that does all
-the hard work for us. But for a better control, we can also instantiate a
+the hard work for us. But for a better control, we can also instanciate a
 cross-validation iterator, and make predictions over each split using the
 ``split()`` method of the iterator, and the
 :meth:`test()<surprise.prediction_algorithms.algo_base.AlgoBase.test>` method
 of the algorithm. Here is an example where we use a classical K-fold
 cross-validation procedure with 3 splits:
 
 .. literalinclude:: ../../examples/use_cross_validation_iterators.py
     :caption: From file ``examples/use_cross_validation_iterators.py``
     :name: use_cross_validation_iterators.py
-    :lines: 6-
+    :lines: 8-
 
 Result could be, e.g.:
 
 .. parsed-literal::
     RMSE: 0.9374
     RMSE: 0.9476
     RMSE: 0.9478
@@ -229,15 +229,15 @@
 and test files (u1.base, u1.test ... u5.base, u5.test). Surprise can handle
 this case by using a :class:`surprise.model_selection.split.PredefinedKFold`
 object:
 
 .. literalinclude:: ../../examples/load_custom_dataset_predefined_folds.py
     :caption: From file ``examples/load_custom_dataset_predefined_folds.py``
     :name: load_custom_dataset_predefined_folds.py
-    :lines: 9-
+    :lines: 13-
 
 Of course, nothing prevents you from only loading a single file for training
 and a single file for testing. However, the ``folds_files`` parameter still
 needs to be a ``list``.
 
 .. _tuning_algorithm_parameters:
 
@@ -249,25 +249,25 @@
 metric over a cross-validation procedure for a given set of parameters.  If you
 want to know which parameter combination yields the best results, the
 :class:`GridSearchCV <surprise.model_selection.search.GridSearchCV>` class
 comes to the rescue.  Given a ``dict`` of parameters, this class exhaustively
 tries all the combinations of parameters and reports the best parameters for any
 accuracy measure (averaged over the different splits). It is heavily inspired
 from scikit-learn's `GridSearchCV
-<https://scikit-learn.org/stable/modules/generated/sklearn.model
+<http://scikit-learn.org/stable/modules/generated/sklearn.model
 _selection.GridSearchCV.html>`_.
 
 Here is an example where we try different values for parameters ``n_epochs``,
 ``lr_all`` and ``reg_all`` of the :class:`SVD
 <surprise.prediction_algorithms.matrix_factorization.SVD>` algorithm.
 
 .. literalinclude:: ../../examples/grid_search_usage.py
     :caption: From file ``examples/grid_search_usage.py``
     :name: grid_search_usage.py
-    :lines: 7-22
+    :lines: 9-26
 
 Result:
 
 .. parsed-literal::
 
     0.961300130118
     {'n_epochs': 10, 'lr_all': 0.005, 'reg_all': 0.4}
@@ -279,60 +279,52 @@
 Once ``fit()`` has been called, the ``best_estimator`` attribute gives us an
 algorithm instance with the optimal set of parameters, which can be used how we
 please:
 
 .. literalinclude:: ../../examples/grid_search_usage.py
     :caption: From file ``examples/grid_search_usage.py``
     :name: grid_search_usage2.py
-    :lines: 24-26
+    :lines: 28-30
 
 .. _grid_search_note:
 .. note::
 
     Dictionary parameters such as ``bsl_options`` and ``sim_options`` require
     particular treatment. See usage example below:
 
     .. parsed-literal::
 
-        param_grid = {
-            'k': [10, 20],
-            'sim_options': {
-                'name': ['msd', 'cosine'],
-                'min_support': [1, 5],
-                'user_based': [False],
-            },
-        }
+        param_grid = {'k': [10, 20],
+                      'sim_options': {'name': ['msd', 'cosine'],
+                                      'min_support': [1, 5],
+                                      'user_based': [False]}
+                      }
 
     Naturally, both can be combined, for example for the
     :class:`KNNBaseline <surprise.prediction_algorithms.knns.KNNBaseline>`
     algorithm:
 
     .. parsed-literal::
-        param_grid = {
-            'bsl_options': {
-                'method': ['als', 'sgd'],
-                'reg': [1, 2],
-            },
-            'k': [2, 3],
-            'sim_options': {
-                'name': ['msd', 'cosine'],
-                'min_support': [1, 5],
-                'user_based': [False],
-            },
-        }
+        param_grid = {'bsl_options': {'method': ['als', 'sgd'],
+                                      'reg': [1, 2]},
+                      'k': [2, 3],
+                      'sim_options': {'name': ['msd', 'cosine'],
+                                      'min_support': [1, 5],
+                                      'user_based': [False]}
+                      }
 
 .. _cv_results_example:
 
 For further analysis, the ``cv_results`` attribute has all the needed
 information and can be imported in a pandas dataframe:
 
 .. literalinclude:: ../../examples/grid_search_usage.py
     :caption: From file ``examples/grid_search_usage.py``
     :name: grid_search_usage3.py
-    :lines: 30
+    :lines: 33
 
 In our example, the ``cv_results`` attribute looks like this (floats are
 formatted):
 
 .. parsed-literal::
 
     'split0_test_rmse': [1.0, 1.0, 0.97, 0.98, 0.98, 0.99, 0.96, 0.97]
```

### Comparing `scikit_surprise-1.1.4/doc/source/index.rst` & `scikit-surprise-1.1rc0/doc/build/html/_sources/index.rst.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,23 +4,28 @@
    contain the root `toctree` directive.
 
 .. _index:
 
 Welcome to Surprise' documentation!
 ===================================
 
-`Surprise <https://surpriselib.com>`_  is an easy-to-use Python `scikit
-<https://projects.scipy.org/scikits.html>`_ for recommender systems.
+`Surprise <http://surpriselib.com>`_  is an easy-to-use Python `scikit
+<https://www.scipy.org/scikits.html>`_ for recommender systems.
 
-If you're new to `Surprise <https://surpriselib.com>`_, we invite you to take a
+If you're new to `Surprise <http://surpriselib.com>`_, we invite you to take a
 look at the :ref:`getting_started` guide, where you'll find a series of
 tutorials illustrating all you can do with  `Surprise
-<https://surpriselib.com>`_. You can also check out the :ref:`FAQ` for many
+<http://surpriselib.com>`_. You can also check out the :ref:`FAQ` for many
 use-case example. For installation guidelines, please refer to the `project
-page <https://surpriselib.com>`_.
+page <http://surpriselib.com>`_.
+
+Any kind of feedback/criticism would be greatly appreciated (software design,
+documentation, improvement ideas, spelling mistakes, etc...). Please feel free
+to contribute and send pull requests (see `GitHub page
+<https://github.com/NicolasHug/Surprise>`_)!
 
 
 .. toctree::
    :caption: User Guide
    :hidden:
 
    getting_started
```

### Comparing `scikit_surprise-1.1.4/doc/source/knn_inspired.rst` & `scikit-surprise-1.1rc0/doc/build/html/_sources/knn_inspired.rst.txt`

 * *Files identical despite different names*

### Comparing `scikit_surprise-1.1.4/doc/source/model_selection.rst` & `scikit-surprise-1.1rc0/doc/build/html/_sources/model_selection.rst.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 The model_selection package
 ---------------------------
 
 Surprise provides various tools to run cross-validation procedures and search
 the best parameters for a prediction algorithm. The tools presented here are
 all heavily inspired from the excellent `scikit learn
-<https://scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection>`_
+<http://scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection>`_
 library.
 
 
 .. _cross_validation_iterators_api:
 
 Cross validation iterators
 ==========================
```

### Comparing `scikit_surprise-1.1.4/doc/source/notation_standards.rst` & `scikit-surprise-1.1rc0/doc/build/html/_sources/notation_standards.rst.txt`

 * *Files identical despite different names*

### Comparing `scikit_surprise-1.1.4/doc/source/prediction_algorithms.rst` & `scikit-surprise-1.1rc0/doc/build/html/_sources/prediction_algorithms.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,46 +67,48 @@
   :math:`\lambda_2` in :cite:`Koren:2010`.  Default is ``10``.
 - ``'reg_u'``: The regularization parameter for users. Corresponding to
   :math:`\lambda_3` in :cite:`Koren:2010`.  Default is ``15``.
 - ``'n_epochs'``: The number of iteration of the ALS procedure. Default is
   ``10``.  Note that in :cite:`Koren:2010`, what is described is a **single**
   iteration ALS process.
 
-.. literalinclude:: ../../examples/baselines_conf.py
-    :caption: From file ``examples/baselines_conf.py``
-    :name: baselines_als
-    :lines: 15-16
-
 And for SGD:
 
 - ``'reg'``: The regularization parameter of the cost function that is
   optimized, corresponding to :math:`\lambda_1` in
   :cite:`Koren:2010`. Default is ``0.02``.
 - ``'learning_rate'``: The learning rate of SGD, corresponding to
   :math:`\gamma` in :cite:`Koren:2010`.  Default is ``0.005``.
 - ``'n_epochs'``: The number of iteration of the SGD procedure. Default is 20. 
 
-.. literalinclude:: ../../examples/baselines_conf.py
-    :caption: From file ``examples/baselines_conf.py``
-    :name: baselines_sgd
-    :lines: 22-26
-
 .. note::
   For both procedures (ALS and SGD), user and item biases (:math:`b_u` and
   :math:`b_i`) are initialized to zero.
 
-Some similarity measures may use baselines, such as the
+Usage examples:
+
+.. literalinclude:: ../../examples/baselines_conf.py
+    :caption: From file ``examples/baselines_conf.py``
+    :name: baselines_als
+    :lines: 19-25
+
+.. literalinclude:: ../../examples/baselines_conf.py
+    :caption: From file ``examples/baselines_conf.py``
+    :name: baselines_sgd
+    :lines: 30-34
+
+Note that some similarity measures may use baselines, such as the
 :func:`pearson_baseline <surprise.similarities.pearson_baseline>` similarity.
 Configuration works just the same, whether the baselines are used in the actual
 prediction :math:`\hat{r}_{ui}` or not:
 
 .. literalinclude:: ../../examples/baselines_conf.py
     :caption: From file ``examples/baselines_conf.py``
     :name: baselines_als_pearson_sim
-    :lines: 32-37
+    :lines: 40-44
 
 
 This leads us to similarity measure configuration, which we will review right
 now.
 
 .. _similarity_measures_configuration:
 
@@ -133,16 +135,16 @@
   Default is 100.
 
 Usage examples:
 
 .. literalinclude:: ../../examples/similarity_conf.py
     :caption: From file ``examples/similarity_conf.py``
     :name: sim_conf_cos
-    :lines: 15-19
+    :lines: 18-21
 
 .. literalinclude:: ../../examples/similarity_conf.py
     :caption: From file ``examples/similarity_conf.py``
     :name: sim_conf_pearson_baseline
-    :lines: 24-25
+    :lines: 26-29
 
 .. seealso::
     The :mod:`similarities <surprise.similarities>` module.
```

### Comparing `scikit_surprise-1.1.4/doc/source/refs.bib` & `scikit-surprise-1.1rc0/doc/source/refs.bib`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 @article{Koren:2010,
  author = {Koren, Yehuda},
  title = {Factor in the Neighbors: Scalable and Accurate Collaborative Filtering},
  journal = {},
  year = {2010},
- url = {https://courses.ischool.berkeley.edu/i290-dm/s11/SECURE/a1-koren.pdf},
+ url = {http://courses.ischool.berkeley.edu/i290-dm/s11/SECURE/a1-koren.pdf},
 }
 
 @book{Ricci:2010,
  author = {Ricci, Francesco and Rokach, Lior and Shapira, Bracha and Kantor, Paul B.},
  title = {Recommender Systems Handbook},
  year = {2010},
  edition = {1st},
@@ -15,47 +15,47 @@
 }
 
 @article{salakhutdinov2008a,
   author = {Salakhutdinov, Ruslan and Mnih, Andriy},
   journal = {},
   title = {Probabilistic Matrix Factorization},
   year = 2008,
-  url = {https://papers.nips.cc/paper/3208-probabilistic-matrix-factorization.pdf},
+  url = {http://papers.nips.cc/paper/3208-probabilistic-matrix-factorization.pdf},
 }
 
 @article{Koren:2009,
  author = {Koren, Yehuda and Bell, Robert and Volinsky, Chris},
  title = {Matrix Factorization Techniques for Recommender Systems},
  journal = {},
  year = {2009},
 }
 
 @article{lemire2007a,
 	author    = {Daniel Lemire and Anna Maclachlan},
   title     = {Slope One Predictors for Online Rating-Based Collaborative Filtering},
   journal   = {},
   year      = {2007},
-  url       = {https://arxiv.org/abs/cs/0702144},
+  url       = {http://arxiv.org/abs/cs/0702144},
 }
 
 @article{Koren:2008:FMN,
  author = {Koren, Yehuda},
  title = {Factorization Meets the Neighborhood: A Multifaceted Collaborative Filtering Model},
  journal = {},
  year = {2008},
- url = {https://people.engr.tamu.edu/huangrh/Spring16/papers_course/matrix_factorization.pdf},
+ url = {http://www.cs.rochester.edu/twiki/pub/Main/HarpSeminar/Factorization_Meets_the_Neighborhood-_a_Multifaceted_Collaborative_Filtering_Model.pdf},
 }
 
 @article{George:2005,
   author = {George, Thomas and Merugu, Srujana},
   title = {A Scalable Collaborative Filtering Framework Based on
     Co-Clustering},
   journal = {},
   year = {2005},
-  url = {https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.113.6458&rep=rep1&type=pdf},
+  url = {http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.113.6458&rep=rep1&type=pdf},
 }
 
 @article{NMF:2014,
   author = {Luo, Xin and Zhou, Mengchu and Xia, Yunni and Zhu, Qinsheng},
   title = {An Efficient Non-Negative Matrix Factorization-Based Approach to
     Collaborative Filtering for Recommender Systems},
   journal = {},
@@ -63,17 +63,17 @@
 }
 
 @article{Zhang96,
   author = {Sheng Zhang and Weihong Wang and James Ford and Fillia Makedon},
   title = {Learning from incomplete ratings using non-negative matrix factorization},
   journal = {},
   year = {1996},
-  url = {https://www.siam.org/meetings/sdm06/proceedings/059zhangs2.pdf}
+  url = {http://www.siam.org/meetings/sdm06/proceedings/059zhangs2.pdf}
 }
 
 @article{NMF_algo,
 title = {Algorithms for Non-negative Matrix Factorization},
 author = {Daniel D. Lee and Seung, H. Sebastian},
 journal = {},
 year = {2001},
-url = {https://papers.nips.cc/paper/1861-algorithms-for-non-negative-matrix-factorization.pdf}
+url = {http://papers.nips.cc/paper/1861-algorithms-for-non-negative-matrix-factorization.pdf}
 }
```

### Comparing `scikit_surprise-1.1.4/examples/baselines_conf.py` & `scikit-surprise-1.1rc0/examples/baselines_conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 """
 This module gives an example of how to configure baseline estimates
 computation.
 """
 
-from surprise import BaselineOnly, Dataset, KNNBasic
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+
+from surprise import BaselineOnly
+from surprise import KNNBasic
+from surprise import Dataset
 from surprise.model_selection import cross_validate
 
 
 # Load the movielens-100k dataset.
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 
 # Example using ALS
-print("Using ALS")
-bsl_options = {"method": "als", "n_epochs": 5, "reg_u": 12, "reg_i": 5}
+print('Using ALS')
+bsl_options = {'method': 'als',
+               'n_epochs': 5,
+               'reg_u': 12,
+               'reg_i': 5
+               }
 algo = BaselineOnly(bsl_options=bsl_options)
 
 cross_validate(algo, data, verbose=True)
 
 # Example using SGD
-print("Using SGD")
-bsl_options = {
-    "method": "sgd",
-    "learning_rate": 0.00005,
-}
+print('Using SGD')
+bsl_options = {'method': 'sgd',
+               'learning_rate': .00005,
+               }
 algo = BaselineOnly(bsl_options=bsl_options)
 
 cross_validate(algo, data, verbose=True)
 
 # Some similarity measures may use baselines. It works just the same.
-print("Using ALS with pearson_baseline similarity")
-bsl_options = {
-    "method": "als",
-    "n_epochs": 20,
-}
-sim_options = {"name": "pearson_baseline"}
+print('Using ALS with pearson_baseline similarity')
+bsl_options = {'method': 'als',
+               'n_epochs': 20,
+               }
+sim_options = {'name': 'pearson_baseline'}
 algo = KNNBasic(bsl_options=bsl_options, sim_options=sim_options)
 
 cross_validate(algo, data, verbose=True)
```

### Comparing `scikit_surprise-1.1.4/examples/basic_usage.py` & `scikit-surprise-1.1rc0/examples/train_test_split.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 """
-This module describes the most basic usage of Surprise: you define a prediction
-algorithm, (down)load a dataset and run a cross-validation procedure.
+This module describes how to use the train_test_split() function.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
-from surprise import Dataset, SVD
-from surprise.model_selection import cross_validate
-
+from surprise import SVD
+from surprise import Dataset
+from surprise import accuracy
+from surprise.model_selection import train_test_split
 
 # Load the movielens-100k dataset (download it if needed),
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
+
+# sample random trainset and testset
+# test set is made of 25% of the ratings.
+trainset, testset = train_test_split(data, test_size=.25)
 
 # We'll use the famous SVD algorithm.
 algo = SVD()
 
-# Run 5-fold cross-validation and print results
-cross_validate(algo, data, measures=["RMSE", "MAE"], cv=5, verbose=True)
+# Train the algorithm on the trainset, and predict ratings for the testset
+algo.fit(trainset)
+predictions = algo.test(testset)
+
+# Then compute RMSE
+accuracy.rmse(predictions)
```

### Comparing `scikit_surprise-1.1.4/examples/building_custom_algorithms/most_basic_algorithm2.py` & `scikit-surprise-1.1rc0/examples/building_custom_algorithms/most_basic_algorithm2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 """
 This module descibes how to build your own prediction algorithm. Please refer
 to User Guide for more insight.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 import numpy as np
 
-from surprise import AlgoBase, Dataset
+from surprise import AlgoBase
+from surprise import Dataset
 from surprise.model_selection import cross_validate
 
 
 class MyOwnAlgorithm(AlgoBase):
+
     def __init__(self):
 
         # Always call base method before doing anything.
         AlgoBase.__init__(self)
 
     def fit(self, trainset):
 
         # Here again: call base method before doing anything.
         AlgoBase.fit(self, trainset)
 
         # Compute the average rating. We might as well use the
         # trainset.global_mean attribute ;)
-        self.the_mean = np.mean([r for (_, _, r) in self.trainset.all_ratings()])
+        self.the_mean = np.mean([r for (_, _, r) in
+                                 self.trainset.all_ratings()])
 
         return self
 
     def estimate(self, u, i):
 
         return self.the_mean
 
 
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 algo = MyOwnAlgorithm()
 
 cross_validate(algo, data, verbose=True)
```

### Comparing `scikit_surprise-1.1.4/examples/building_custom_algorithms/with_baselines_or_sim.py` & `scikit-surprise-1.1rc0/examples/building_custom_algorithms/with_baselines_or_sim.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 """
 This module descibes how to build your own prediction algorithm. Please refer
 to User Guide for more insight.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
-from surprise import AlgoBase, Dataset, PredictionImpossible
+from surprise import AlgoBase
+from surprise import Dataset
 from surprise.model_selection import cross_validate
+from surprise import PredictionImpossible
 
 
 class MyOwnAlgorithm(AlgoBase):
+
     def __init__(self, sim_options={}, bsl_options={}):
 
-        AlgoBase.__init__(self, sim_options=sim_options, bsl_options=bsl_options)
+        AlgoBase.__init__(self, sim_options=sim_options,
+                          bsl_options=bsl_options)
 
     def fit(self, trainset):
 
         AlgoBase.fit(self, trainset)
 
         # Compute baselines and similarities
         self.bu, self.bi = self.compute_baselines()
         self.sim = self.compute_similarities()
 
         return self
 
     def estimate(self, u, i):
 
         if not (self.trainset.knows_user(u) and self.trainset.knows_item(i)):
-            raise PredictionImpossible("User and/or item is unknown.")
+            raise PredictionImpossible('User and/or item is unkown.')
 
         # Compute similarities between u and v, where v describes all other
         # users that have also rated item i.
         neighbors = [(v, self.sim[u, v]) for (v, r) in self.trainset.ir[i]]
         # Sort these neighbors by similarity
         neighbors = sorted(neighbors, key=lambda x: x[1], reverse=True)
 
-        print("The 3 nearest neighbors of user", str(u), "are:")
+        print('The 3 nearest neighbors of user', str(u), 'are:')
         for v, sim_uv in neighbors[:3]:
-            print(f"user {v} with sim {sim_uv:1.2f}")
+            print('user {0:} with sim {1:1.2f}'.format(v, sim_uv))
 
         # ... Aaaaand return the baseline estimate anyway ;)
         bsl = self.trainset.global_mean + self.bu[u] + self.bi[i]
         return bsl
 
 
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 algo = MyOwnAlgorithm()
 
 cross_validate(algo, data, verbose=True)
```

### Comparing `scikit_surprise-1.1.4/examples/generate_grid_search_cv_results_example.py` & `scikit-surprise-1.1rc0/examples/generate_grid_search_cv_results_example.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 """
 This module is used for generating the doc tables about the
 GridSearchCV.cv_results attribute.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
-from surprise import Dataset, SVD
-from surprise.model_selection import GridSearchCV
 from tabulate import tabulate
+from six import iteritems
+
+from surprise import SVD
+from surprise import Dataset
+from surprise.model_selection import GridSearchCV
 
 # Use movielens-100K
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 
-param_grid = {"n_epochs": [5, 10], "lr_all": [0.002, 0.005], "reg_all": [0.4, 0.6]}
-gs = GridSearchCV(SVD, param_grid, measures=["rmse", "mae"], cv=3)
+param_grid = {'n_epochs': [5, 10], 'lr_all': [0.002, 0.005],
+              'reg_all': [0.4, 0.6]}
+gs = GridSearchCV(SVD, param_grid, measures=['rmse', 'mae'], cv=3)
 
 gs.fit(data)
 
-table = [[] for _ in range(len(gs.cv_results["params"]))]
-for i in range(len(gs.cv_results["params"])):
+table = [[] for _ in range(len(gs.cv_results['params']))]
+for i in range(len(gs.cv_results['params'])):
     for key in gs.cv_results.keys():
         table[i].append(gs.cv_results[key][i])
 
 header = gs.cv_results.keys()
 print(tabulate(table, header, tablefmt="rst"))
 
 print()
 
-for key, val in gs.cv_results.items():
-    print("{:<20}".format("'" + key + "':"), end="")
+for key, val in iteritems(gs.cv_results):
+    print('{:<20}'.format("'" + key + "':"), end='')
     if isinstance(val[0], float):
-        print([float(f"{f:.2f}") for f in val])
+        print([float('{:.2f}'.format(f)) for f in val])
     else:
         print(val)
```

### Comparing `scikit_surprise-1.1.4/examples/k_nearest_neighbors.py` & `scikit-surprise-1.1rc0/examples/k_nearest_neighbors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 """
 This module illustrates how to retrieve the k-nearest neighbors of an item. The
 same can be done for users with minor changes. There's a lot of boilerplate
 because of the id conversions, but it all boils down to the use of
 algo.get_neighbors().
 """
 
-# needed because of weird encoding of u.item file
-import io  # noqa
-
-from surprise import Dataset, get_dataset_dir, KNNBaseline
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+import io  # needed because of weird encoding of u.item file
+
+from surprise import KNNBaseline
+from surprise import Dataset
+from surprise import get_dataset_dir
 
 
 def read_item_names():
     """Read the u.item file from MovieLens 100-k dataset and return two
     mappings to convert raw ids into movie names and movie names into raw ids.
     """
 
-    file_name = get_dataset_dir() + "/ml-100k/ml-100k/u.item"
+    file_name = get_dataset_dir() + '/ml-100k/ml-100k/u.item'
     rid_to_name = {}
     name_to_rid = {}
-    with open(file_name, encoding="ISO-8859-1") as f:
+    with io.open(file_name, 'r', encoding='ISO-8859-1') as f:
         for line in f:
-            line = line.split("|")
+            line = line.split('|')
             rid_to_name[line[0]] = line[1]
             name_to_rid[line[1]] = line[0]
 
     return rid_to_name, name_to_rid
 
 
-# First, train the algorithm to compute the similarities between items
-data = Dataset.load_builtin("ml-100k")
+# First, train the algortihm to compute the similarities between items
+data = Dataset.load_builtin('ml-100k')
 trainset = data.build_full_trainset()
-sim_options = {"name": "pearson_baseline", "user_based": False}
+sim_options = {'name': 'pearson_baseline', 'user_based': False}
 algo = KNNBaseline(sim_options=sim_options)
 algo.fit(trainset)
 
 # Read the mappings raw id <-> movie name
 rid_to_name, name_to_rid = read_item_names()
 
 # Retrieve inner id of the movie Toy Story
-toy_story_raw_id = name_to_rid["Toy Story (1995)"]
+toy_story_raw_id = name_to_rid['Toy Story (1995)']
 toy_story_inner_id = algo.trainset.to_inner_iid(toy_story_raw_id)
 
 # Retrieve inner ids of the nearest neighbors of Toy Story.
 toy_story_neighbors = algo.get_neighbors(toy_story_inner_id, k=10)
 
 # Convert inner ids of the neighbors into names.
-toy_story_neighbors = (
-    algo.trainset.to_raw_iid(inner_id) for inner_id in toy_story_neighbors
-)
-toy_story_neighbors = (rid_to_name[rid] for rid in toy_story_neighbors)
+toy_story_neighbors = (algo.trainset.to_raw_iid(inner_id)
+                       for inner_id in toy_story_neighbors)
+toy_story_neighbors = (rid_to_name[rid]
+                       for rid in toy_story_neighbors)
 
 print()
-print("The 10 nearest neighbors of Toy Story are:")
+print('The 10 nearest neighbors of Toy Story are:')
 for movie in toy_story_neighbors:
     print(movie)
```

### Comparing `scikit_surprise-1.1.4/examples/load_custom_dataset_predefined_folds.py` & `scikit-surprise-1.1rc0/examples/load_custom_dataset_predefined_folds.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 This module descibes how to load a custom dataset when folds (for
 cross-validation) are predefined by train and test files.
 
 As a custom dataset we will actually use the movielens-100k dataset, but act as
 if it were not built-in.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 import os
 
-from surprise import accuracy, Dataset, Reader, SVD
+from surprise import SVD
+from surprise import Dataset
+from surprise import Reader
+from surprise import accuracy
 from surprise.model_selection import PredefinedKFold
 
 # path to dataset folder
-files_dir = os.path.expanduser("~/.surprise_data/ml-100k/ml-100k/")
+files_dir = os.path.expanduser('~/.surprise_data/ml-100k/ml-100k/')
 
 # This time, we'll use the built-in reader.
-reader = Reader("ml-100k")
+reader = Reader('ml-100k')
 
 # folds_files is a list of tuples containing file paths:
 # [(u1.base, u1.test), (u2.base, u2.test), ... (u5.base, u5.test)]
-train_file = files_dir + "u%d.base"
-test_file = files_dir + "u%d.test"
+train_file = files_dir + 'u%d.base'
+test_file = files_dir + 'u%d.test'
 folds_files = [(train_file % i, test_file % i) for i in (1, 2, 3, 4, 5)]
 
 data = Dataset.load_from_folds(folds_files, reader=reader)
 pkf = PredefinedKFold()
 
 algo = SVD()
```

### Comparing `scikit_surprise-1.1.4/examples/load_from_dataframe.py` & `scikit-surprise-1.1rc0/examples/load_from_dataframe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 This module descibes how to load a dataset from a pandas dataframe.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 import pandas as pd
 
-from surprise import Dataset, NormalPredictor, Reader
+from surprise import NormalPredictor
+from surprise import Dataset
+from surprise import Reader
 from surprise.model_selection import cross_validate
 
 
 # Creation of the dataframe. Column names are irrelevant.
-ratings_dict = {
-    "itemID": [1, 1, 1, 2, 2],
-    "userID": [9, 32, 2, 45, "user_foo"],
-    "rating": [3, 2, 4, 3, 1],
-}
+ratings_dict = {'itemID': [1, 1, 1, 2, 2],
+                'userID': [9, 32, 2, 45, 'user_foo'],
+                'rating': [3, 2, 4, 3, 1]}
 df = pd.DataFrame(ratings_dict)
 
-# A reader is still needed but only the rating_scale param is required.
+# A reader is still needed but only the rating_scale param is requiered.
 reader = Reader(rating_scale=(1, 5))
 
 # The columns must correspond to user id, item id and ratings (in that order).
-data = Dataset.load_from_df(df[["userID", "itemID", "rating"]], reader)
+data = Dataset.load_from_df(df[['userID', 'itemID', 'rating']], reader)
 
 # We can now use this dataset as we please, e.g. calling cross_validate
 cross_validate(NormalPredictor(), data, cv=2)
```

### Comparing `scikit_surprise-1.1.4/examples/notebooks/Compare.ipynb` & `scikit-surprise-1.1rc0/examples/notebooks/KNNBasic_analysis.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9549184421801253%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Analysis of the KNNBasic algorithm\\n'), (2, 'In this "*

 * *            'notebook, we will run a basic neighborhood algorithm on the movielens dataset, dump '*

 * *            "the results, and use pandas to make some data analysis.')], delete: [2, 0]}}, 1: "*

 * *            "{'execution_count': 1, 'source': {delete: [11, 7]}}, 2: {'execution_count': 8, "*

 * *            "'outputs': {0: {'text': {insert: [(2, 'RMSE: 0.9889\\n')]}}}, 'source': {insert: [(4, "*

 * *            '"#Datase […]*

```diff
@@ -1,623 +1,638 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#\u00a0Comparison of two algorithms\n",
+                "# Analysis of the KNNBasic algorithm\n",
                 "\n",
-                "We will see in this notebook how we can compare the prediction accuracy of two algorithms."
+                "In this notebook, we will run a basic neighborhood algorithm on the movielens dataset, dump the results, and use pandas to make some data analysis."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from __future__ import (absolute_import, division, print_function,             \n",
                 "                        unicode_literals)                                      \n",
                 "import pickle\n",
                 "import os\n",
                 "\n",
                 "import pandas as pd\n",
                 "\n",
-                "from surprise import SVD\n",
                 "from surprise import KNNBasic\n",
                 "from surprise import Dataset                                                     \n",
                 "from surprise import Reader                                                      \n",
-                "from surprise.model_selection import PredefinedKFold\n",
                 "from surprise import dump\n",
                 "from surprise.accuracy import rmse"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Computing the msd similarity matrix...\n",
-                        "Done computing similarity matrix.\n"
+                        "Done computing similarity matrix.\n",
+                        "RMSE: 0.9889\n"
                     ]
                 }
             ],
             "source": [
                 "#\u00a0We will train and test on the u1.base and u1.test files of the movielens-100k dataset.\n",
                 "# if you haven't already, you need to download the movielens-100k dataset\n",
                 "#\u00a0You can do it manually, or by running:\n",
                 "\n",
-                "# Dataset.load_builtin('ml-100k')\n",
+                "#Dataset.load_builtin('ml-100k')\n",
                 "\n",
                 "# Now, let's load the dataset\n",
                 "train_file = os.path.expanduser('~') + '/.surprise_data/ml-100k/ml-100k/u1.base'\n",
                 "test_file = os.path.expanduser('~') + '/.surprise_data/ml-100k/ml-100k/u1.test'\n",
                 "data = Dataset.load_from_folds([(train_file, test_file)], Reader('ml-100k'))\n",
                 "\n",
-                "pkf = PredefinedKFold()\n",
-                "\n",
                 "                \n",
-                "#\u00a0We'll use the well-known SVD algorithm and a basic nearest neighbors approach.\n",
-                "algo_svd = SVD()                                                       \n",
-                "algo_knn = KNNBasic()\n",
+                "#\u00a0We'll use a basic nearest neighbor approach, where similarities are computed\n",
+                "# between users.\n",
+                "algo = KNNBasic()                                                       \n",
                 "\n",
-                "for trainset, testset in pkf.split(data): \n",
-                "    algo_svd.fit(trainset)                             \n",
-                "    predictions_svd = algo_svd.test(testset)\n",
-                "    \n",
-                "    algo_knn.fit(trainset)\n",
-                "    predictions_knn = algo_knn.test(testset)\n",
-                "    \n",
-                "    rmse(predictions_svd)\n",
-                "    rmse(predictions_knn)                                                                           \n",
-                "    \n",
-                "    dump.dump('./dump_SVD', predictions_svd, algo_svd)\n",
-                "    dump.dump('./dump_KNN', predictions_knn, algo_knn)"
+                "for trainset, testset in data.folds(): \n",
+                "    algo.fit(trainset)                             \n",
+                "    predictions = algo.test(testset)\n",
+                "    rmse(predictions)\n",
+                "                                                                               \n",
+                "    dump.dump('./dump_file', predictions, algo)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# The dumps have been saved and we can now use them whenever we want.\n",
-                "\n",
-                "predictions_svd, algo_svd = dump.load('./dump_SVD')\n",
-                "predictions_knn, algo_knn = dump.load('./dump_KNN')\n",
-                "\n",
-                "df_svd = pd.DataFrame(predictions_svd, columns=['uid', 'iid', 'rui', 'est', 'details'])    \n",
-                "df_knn = pd.DataFrame(predictions_knn, columns=['uid', 'iid', 'rui', 'est', 'details'])    \n",
-                "\n",
-                "df_svd['err'] = abs(df_svd.est - df_svd.rui)\n",
-                "df_knn['err'] = abs(df_knn.est - df_knn.rui)"
+                "# The dump has been saved and we can now use it whenever we want.\n",
+                "# Let's load it and see what we can do\n",
+                "predictions, algo = dump.load('./dump_file')"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 12,
             "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "algo: KNNBasic, k = 40, min_k = 1\n"
+                    ]
+                }
+            ],
             "source": [
-                "We now have two dataframes with the all the predictions for each algorithm. The cool thing is that, as both algorithm have been tested on the same testset, the indexes of the two dataframes are the same!"
+                "trainset = algo.trainset\n",
+                "print('algo: {0}, k = {1}, min_k = {2}'.format(algo.__class__.__name__, algo.k, algo.min_k))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 13,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>uid</th>\n",
-                            "      <th>iid</th>\n",
-                            "      <th>rui</th>\n",
-                            "      <th>est</th>\n",
-                            "      <th>details</th>\n",
-                            "      <th>err</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>184</td>\n",
-                            "      <td>67</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3.070263</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>0.070263</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>766</td>\n",
-                            "      <td>487</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3.797903</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>0.797903</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>263</td>\n",
-                            "      <td>117</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3.594508</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>0.594508</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>545</td>\n",
-                            "      <td>168</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>3.961151</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>0.038849</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>525</td>\n",
-                            "      <td>255</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>3.306502</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>2.306502</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "   uid  iid  rui       est                    details       err\n",
-                            "0  184   67  3.0  3.070263  {'was_impossible': False}  0.070263\n",
-                            "1  766  487  3.0  3.797903  {'was_impossible': False}  0.797903\n",
-                            "2  263  117  3.0  3.594508  {'was_impossible': False}  0.594508\n",
-                            "3  545  168  4.0  3.961151  {'was_impossible': False}  0.038849\n",
-                            "4  525  255  1.0  3.306502  {'was_impossible': False}  2.306502"
-                        ]
-                    },
-                    "execution_count": 11,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "df_svd.head()"
+                "# Let's build a pandas dataframe with all the predictions\n",
+                "\n",
+                "def get_Iu(uid):\n",
+                "    \"\"\"Return the number of items rated by given user\n",
+                "    \n",
+                "    Args:\n",
+                "        uid: The raw id of the user.\n",
+                "    Returns:\n",
+                "        The number of items rated by the user.\n",
+                "    \"\"\"\n",
+                "    \n",
+                "    try:\n",
+                "        return len(trainset.ur[trainset.to_inner_uid(uid)])\n",
+                "    except ValueError:  # user was not part of the trainset\n",
+                "        return 0\n",
+                "    \n",
+                "def get_Ui(iid):\n",
+                "    \"\"\"Return the number of users that have rated given item\n",
+                "    \n",
+                "    Args:\n",
+                "        iid: The raw id of the item.\n",
+                "    Returns:\n",
+                "        The number of users that have rated the item.\n",
+                "    \"\"\"\n",
+                "    \n",
+                "    try:\n",
+                "        return len(trainset.ir[trainset.to_inner_iid(iid)])\n",
+                "    except ValueError:  # item was not part of the trainset\n",
+                "        return 0\n",
+                "\n",
+                "df = pd.DataFrame(predictions, columns=['uid', 'iid', 'rui', 'est', 'details'])    \n",
+                "df['Iu'] = df.uid.apply(get_Iu)\n",
+                "df['Ui'] = df.iid.apply(get_Ui)\n",
+                "df['err'] = abs(df.est - df.rui)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>uid</th>\n",
                             "      <th>iid</th>\n",
                             "      <th>rui</th>\n",
                             "      <th>est</th>\n",
                             "      <th>details</th>\n",
+                            "      <th>Iu</th>\n",
+                            "      <th>Ui</th>\n",
                             "      <th>err</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>184</td>\n",
-                            "      <td>67</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3.043189</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>0.043189</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>6</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>3.468613</td>\n",
+                            "      <td>{'actual_k': 20, 'was_impossible': False}</td>\n",
+                            "      <td>135</td>\n",
+                            "      <td>20</td>\n",
+                            "      <td>1.531387</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>766</td>\n",
-                            "      <td>487</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>10</td>\n",
                             "      <td>3.0</td>\n",
-                            "      <td>4.139804</td>\n",
+                            "      <td>3.866290</td>\n",
                             "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>1.139804</td>\n",
+                            "      <td>135</td>\n",
+                            "      <td>73</td>\n",
+                            "      <td>0.866290</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>263</td>\n",
-                            "      <td>117</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3.525691</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>12</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>4.538194</td>\n",
                             "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>0.525691</td>\n",
+                            "      <td>135</td>\n",
+                            "      <td>211</td>\n",
+                            "      <td>0.461806</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>545</td>\n",
-                            "      <td>168</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>4.393259</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>14</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>4.235741</td>\n",
                             "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>0.393259</td>\n",
+                            "      <td>135</td>\n",
+                            "      <td>140</td>\n",
+                            "      <td>0.764259</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>525</td>\n",
-                            "      <td>255</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>3.638801</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>17</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>3.228002</td>\n",
                             "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>2.638801</td>\n",
+                            "      <td>135</td>\n",
+                            "      <td>72</td>\n",
+                            "      <td>0.228002</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "   uid  iid  rui       est                                    details  \\\n",
-                            "0  184   67  3.0  3.043189  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "1  766  487  3.0  4.139804  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "2  263  117  3.0  3.525691  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "3  545  168  4.0  4.393259  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "4  525  255  1.0  3.638801  {'actual_k': 40, 'was_impossible': False}   \n",
+                            "  uid iid  rui       est                                    details   Iu   Ui  \\\n",
+                            "0   1   6  5.0  3.468613  {'actual_k': 20, 'was_impossible': False}  135   20   \n",
+                            "1   1  10  3.0  3.866290  {'actual_k': 40, 'was_impossible': False}  135   73   \n",
+                            "2   1  12  5.0  4.538194  {'actual_k': 40, 'was_impossible': False}  135  211   \n",
+                            "3   1  14  5.0  4.235741  {'actual_k': 40, 'was_impossible': False}  135  140   \n",
+                            "4   1  17  3.0  3.228002  {'actual_k': 40, 'was_impossible': False}  135   72   \n",
                             "\n",
                             "        err  \n",
-                            "0  0.043189  \n",
-                            "1  1.139804  \n",
-                            "2  0.525691  \n",
-                            "3  0.393259  \n",
-                            "4  2.638801  "
+                            "0  1.531387  \n",
+                            "1  0.866290  \n",
+                            "2  0.461806  \n",
+                            "3  0.764259  \n",
+                            "4  0.228002  "
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df_knn.head()"
+                "df.head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 15,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "best_predictions = df.sort_values(by='err')[:10]\n",
+                "worst_predictions = df.sort_values(by='err')[-10:]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>uid</th>\n",
                             "      <th>iid</th>\n",
                             "      <th>rui</th>\n",
                             "      <th>est</th>\n",
                             "      <th>details</th>\n",
+                            "      <th>Iu</th>\n",
+                            "      <th>Ui</th>\n",
                             "      <th>err</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>533</th>\n",
-                            "      <td>405</td>\n",
-                            "      <td>452</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>2.370203</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>2.629797</td>\n",
+                            "      <th>272</th>\n",
+                            "      <td>5</td>\n",
+                            "      <td>439</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>{'actual_k': 3, 'was_impossible': False}</td>\n",
+                            "      <td>91</td>\n",
+                            "      <td>3</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1557</th>\n",
-                            "      <td>295</td>\n",
-                            "      <td>183</td>\n",
+                            "      <th>886</th>\n",
+                            "      <td>13</td>\n",
+                            "      <td>314</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.275709</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>3.275709</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>{'actual_k': 2, 'was_impossible': False}</td>\n",
+                            "      <td>373</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4431</th>\n",
-                            "      <td>481</td>\n",
-                            "      <td>318</td>\n",
+                            "      <th>156</th>\n",
+                            "      <td>2</td>\n",
+                            "      <td>314</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.855612</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>3.855612</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>{'actual_k': 2, 'was_impossible': False}</td>\n",
+                            "      <td>40</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>0.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>926</th>\n",
+                            "      <td>13</td>\n",
+                            "      <td>437</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>{'actual_k': 3, 'was_impossible': False}</td>\n",
+                            "      <td>373</td>\n",
+                            "      <td>3</td>\n",
+                            "      <td>0.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>9276</th>\n",
+                            "      <td>206</td>\n",
+                            "      <td>314</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
+                            "      <td>33</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>6579</th>\n",
+                            "      <th>19118</th>\n",
                             "      <td>405</td>\n",
-                            "      <td>1218</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>3.329299</td>\n",
-                            "      <td>{'actual_k': 21, 'was_impossible': False}</td>\n",
-                            "      <td>1.670701</td>\n",
+                            "      <td>437</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>{'actual_k': 3, 'was_impossible': False}</td>\n",
+                            "      <td>582</td>\n",
+                            "      <td>3</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>10032</th>\n",
-                            "      <td>239</td>\n",
-                            "      <td>514</td>\n",
+                            "      <th>8032</th>\n",
+                            "      <td>181</td>\n",
+                            "      <td>1334</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.250013</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>3.250013</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
+                            "      <td>218</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>14311</th>\n",
-                            "      <td>425</td>\n",
-                            "      <td>313</td>\n",
+                            "      <th>8041</th>\n",
+                            "      <td>181</td>\n",
+                            "      <td>1354</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.093898</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>3.093898</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
+                            "      <td>218</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>15979</th>\n",
-                            "      <td>405</td>\n",
-                            "      <td>1053</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>3.497124</td>\n",
-                            "      <td>{'actual_k': 17, 'was_impossible': False}</td>\n",
-                            "      <td>1.502876</td>\n",
+                            "      <th>9202</th>\n",
+                            "      <td>201</td>\n",
+                            "      <td>1424</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
+                            "      <td>215</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>19292</th>\n",
+                            "      <th>3018</th>\n",
+                            "      <td>60</td>\n",
+                            "      <td>1123</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
+                            "      <td>119</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>131</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>3.779858</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>2.779858</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "       uid   iid  rui       est                                    details  \\\n",
-                            "533    405   452  5.0  2.370203  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "1557   295   183  1.0  4.275709  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "4431   481   318  1.0  4.855612  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "6579   405  1218  5.0  3.329299  {'actual_k': 21, 'was_impossible': False}   \n",
-                            "10032  239   514  1.0  4.250013  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "14311  425   313  1.0  4.093898  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "15979  405  1053  5.0  3.497124  {'actual_k': 17, 'was_impossible': False}   \n",
-                            "19292    1   131  1.0  3.779858  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "\n",
-                            "            err  \n",
-                            "533    2.629797  \n",
-                            "1557   3.275709  \n",
-                            "4431   3.855612  \n",
-                            "6579   1.670701  \n",
-                            "10032  3.250013  \n",
-                            "14311  3.093898  \n",
-                            "15979  1.502876  \n",
-                            "19292  2.779858  "
+                            "       uid   iid  rui  est                                   details   Iu  Ui  \\\n",
+                            "272      5   439  1.0  1.0  {'actual_k': 3, 'was_impossible': False}   91   3   \n",
+                            "886     13   314  1.0  1.0  {'actual_k': 2, 'was_impossible': False}  373   2   \n",
+                            "156      2   314  1.0  1.0  {'actual_k': 2, 'was_impossible': False}   40   2   \n",
+                            "926     13   437  1.0  1.0  {'actual_k': 3, 'was_impossible': False}  373   3   \n",
+                            "9276   206   314  1.0  1.0  {'actual_k': 1, 'was_impossible': False}   33   2   \n",
+                            "19118  405   437  1.0  1.0  {'actual_k': 3, 'was_impossible': False}  582   3   \n",
+                            "8032   181  1334  1.0  1.0  {'actual_k': 1, 'was_impossible': False}  218   1   \n",
+                            "8041   181  1354  1.0  1.0  {'actual_k': 1, 'was_impossible': False}  218   1   \n",
+                            "9202   201  1424  3.0  3.0  {'actual_k': 1, 'was_impossible': False}  215   1   \n",
+                            "3018    60  1123  4.0  4.0  {'actual_k': 1, 'was_impossible': False}  119   1   \n",
+                            "\n",
+                            "       err  \n",
+                            "272    0.0  \n",
+                            "886    0.0  \n",
+                            "156    0.0  \n",
+                            "926    0.0  \n",
+                            "9276   0.0  \n",
+                            "19118  0.0  \n",
+                            "8032   0.0  \n",
+                            "8041   0.0  \n",
+                            "9202   0.0  \n",
+                            "3018   0.0  "
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# Let's check how good are the KNN predictions when the SVD has a huge error:\n",
-                "df_knn[df_svd.err >= 3.5]"
+                "# Let's take a look at the best predictions of the algorithm\n",
+                "best_predictions"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "It's interesting to note that these perfect predictions are actually lucky shots: $|U_i|$ is always very small, meaning that very few users have rated the target item. This implies that the set of neighbors is very small (see the ``actual_k`` field)... And, it just happens that all the ratings from the neighbors are the same (and mostly, are equal to that of the target user).\n",
+                "\n",
+                "This may be a bit surprising but these lucky shots are actually very important to the accuracy of the algorithm... Try running the same algorithm with a value of ``min_k`` equal to $10$. This means that if there are less than $10$ neighbors, the prediction is set to the mean of all ratings. You'll see your accuracy decrease!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>uid</th>\n",
                             "      <th>iid</th>\n",
                             "      <th>rui</th>\n",
                             "      <th>est</th>\n",
                             "      <th>details</th>\n",
+                            "      <th>Iu</th>\n",
+                            "      <th>Ui</th>\n",
                             "      <th>err</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>14619</th>\n",
-                            "      <td>771</td>\n",
-                            "      <td>98</td>\n",
+                            "      <th>9406</th>\n",
+                            "      <td>208</td>\n",
+                            "      <td>302</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.153106</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>3.153106</td>\n",
+                            "      <td>4.308447</td>\n",
+                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
+                            "      <td>11</td>\n",
+                            "      <td>245</td>\n",
+                            "      <td>3.308447</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1557</th>\n",
-                            "      <td>295</td>\n",
-                            "      <td>183</td>\n",
+                            "      <th>19089</th>\n",
+                            "      <td>405</td>\n",
+                            "      <td>169</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.632378</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>3.632378</td>\n",
+                            "      <td>4.364728</td>\n",
+                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
+                            "      <td>582</td>\n",
+                            "      <td>97</td>\n",
+                            "      <td>3.364728</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>11759</th>\n",
-                            "      <td>405</td>\n",
-                            "      <td>1405</td>\n",
+                            "      <th>19785</th>\n",
+                            "      <td>436</td>\n",
+                            "      <td>132</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>1.915805</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>0.915805</td>\n",
+                            "      <td>4.365369</td>\n",
+                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
+                            "      <td>126</td>\n",
+                            "      <td>200</td>\n",
+                            "      <td>3.365369</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4493</th>\n",
-                            "      <td>181</td>\n",
-                            "      <td>1242</td>\n",
+                            "      <th>157</th>\n",
+                            "      <td>2</td>\n",
+                            "      <td>315</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>2.277950</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>1.277950</td>\n",
+                            "      <td>4.381308</td>\n",
+                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
+                            "      <td>40</td>\n",
+                            "      <td>136</td>\n",
+                            "      <td>3.381308</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>10970</th>\n",
-                            "      <td>279</td>\n",
-                            "      <td>1242</td>\n",
+                            "      <th>8503</th>\n",
+                            "      <td>193</td>\n",
+                            "      <td>56</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>3.515677</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>2.515677</td>\n",
+                            "      <td>4.386478</td>\n",
+                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
+                            "      <td>61</td>\n",
+                            "      <td>312</td>\n",
+                            "      <td>3.386478</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>5531</th>\n",
+                            "      <td>113</td>\n",
+                            "      <td>976</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>1.610771</td>\n",
+                            "      <td>{'actual_k': 7, 'was_impossible': False}</td>\n",
+                            "      <td>31</td>\n",
+                            "      <td>7</td>\n",
+                            "      <td>3.389229</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2657</th>\n",
-                            "      <td>239</td>\n",
-                            "      <td>318</td>\n",
+                            "      <th>7917</th>\n",
+                            "      <td>181</td>\n",
+                            "      <td>408</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.144616</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>3.144616</td>\n",
+                            "      <td>4.421499</td>\n",
+                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
+                            "      <td>218</td>\n",
+                            "      <td>93</td>\n",
+                            "      <td>3.421499</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4431</th>\n",
-                            "      <td>481</td>\n",
-                            "      <td>318</td>\n",
+                            "      <th>7390</th>\n",
+                            "      <td>167</td>\n",
+                            "      <td>169</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.580412</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>3.580412</td>\n",
+                            "      <td>4.664991</td>\n",
+                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
+                            "      <td>38</td>\n",
+                            "      <td>97</td>\n",
+                            "      <td>3.664991</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>12838</th>\n",
+                            "      <th>7412</th>\n",
                             "      <td>167</td>\n",
                             "      <td>1306</td>\n",
                             "      <td>5.0</td>\n",
-                            "      <td>3.136852</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>1.863148</td>\n",
+                            "      <td>1.000000</td>\n",
+                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
+                            "      <td>38</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>4.000000</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>16681</th>\n",
-                            "      <td>288</td>\n",
-                            "      <td>1358</td>\n",
+                            "      <th>5553</th>\n",
+                            "      <td>114</td>\n",
+                            "      <td>1104</td>\n",
                             "      <td>5.0</td>\n",
-                            "      <td>3.253280</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>1.746720</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>12869</th>\n",
-                            "      <td>363</td>\n",
-                            "      <td>1512</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>3.425335</td>\n",
-                            "      <td>{'was_impossible': False}</td>\n",
-                            "      <td>2.425335</td>\n",
+                            "      <td>1.000000</td>\n",
+                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
+                            "      <td>27</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>4.000000</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "       uid   iid  rui       est                    details       err\n",
-                            "14619  771    98  1.0  4.153106  {'was_impossible': False}  3.153106\n",
-                            "1557   295   183  1.0  4.632378  {'was_impossible': False}  3.632378\n",
-                            "11759  405  1405  1.0  1.915805  {'was_impossible': False}  0.915805\n",
-                            "4493   181  1242  1.0  2.277950  {'was_impossible': False}  1.277950\n",
-                            "10970  279  1242  1.0  3.515677  {'was_impossible': False}  2.515677\n",
-                            "2657   239   318  1.0  4.144616  {'was_impossible': False}  3.144616\n",
-                            "4431   481   318  1.0  4.580412  {'was_impossible': False}  3.580412\n",
-                            "12838  167  1306  5.0  3.136852  {'was_impossible': False}  1.863148\n",
-                            "16681  288  1358  5.0  3.253280  {'was_impossible': False}  1.746720\n",
-                            "12869  363  1512  1.0  3.425335  {'was_impossible': False}  2.425335"
+                            "       uid   iid  rui       est                                    details  \\\n",
+                            "9406   208   302  1.0  4.308447  {'actual_k': 40, 'was_impossible': False}   \n",
+                            "19089  405   169  1.0  4.364728  {'actual_k': 40, 'was_impossible': False}   \n",
+                            "19785  436   132  1.0  4.365369  {'actual_k': 40, 'was_impossible': False}   \n",
+                            "157      2   315  1.0  4.381308  {'actual_k': 40, 'was_impossible': False}   \n",
+                            "8503   193    56  1.0  4.386478  {'actual_k': 40, 'was_impossible': False}   \n",
+                            "5531   113   976  5.0  1.610771   {'actual_k': 7, 'was_impossible': False}   \n",
+                            "7917   181   408  1.0  4.421499  {'actual_k': 40, 'was_impossible': False}   \n",
+                            "7390   167   169  1.0  4.664991  {'actual_k': 40, 'was_impossible': False}   \n",
+                            "7412   167  1306  5.0  1.000000   {'actual_k': 1, 'was_impossible': False}   \n",
+                            "5553   114  1104  5.0  1.000000   {'actual_k': 1, 'was_impossible': False}   \n",
+                            "\n",
+                            "        Iu   Ui       err  \n",
+                            "9406    11  245  3.308447  \n",
+                            "19089  582   97  3.364728  \n",
+                            "19785  126  200  3.365369  \n",
+                            "157     40  136  3.381308  \n",
+                            "8503    61  312  3.386478  \n",
+                            "5531    31    7  3.389229  \n",
+                            "7917   218   93  3.421499  \n",
+                            "7390    38   97  3.664991  \n",
+                            "7412    38    1  4.000000  \n",
+                            "5553    27    1  4.000000  "
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# Well... Not much better.\n",
-                "# Now, let's look at the predictions of SVD on the 10 worst predictions for KNN\n",
-                "df_svd.iloc[df_knn.sort_values(by='err')[-10:].index]"
+                "# Now, let's look at the prediction with the biggest error\n",
+                "worst_predictions"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Let's focus first on the last two predictions. Well, we can't do much about them. We should have predicted $5$, but the only available neighbor had a rating of $1$, so we were screwed. The only way to avoid this kind of errors would be to increase the ``min_k`` parameter, but it would actually worsen the accuracy (see note above).\n",
+                "\n",
+                "How about the other ones? It seems that for each prediction, the users are some kind of outsiders: they rated their item with a rating of $1$ when the most of the ratings for the item where high (or inversely, rated a *bad* item with a rating of $5$). See the plot below as an illustration for the first rating.\n",
+                "\n",
+                "These are situations where baseline estimates would be quite helpful, in order to deal with highly biased users (and items)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/javascript": [
                             "/* Put everything inside the global mpl namespace */\n",
                             "window.mpl = {};\n",
@@ -625,15 +640,15 @@
                             "\n",
                             "mpl.get_websocket_type = function() {\n",
                             "    if (typeof(WebSocket) !== 'undefined') {\n",
                             "        return WebSocket;\n",
                             "    } else if (typeof(MozWebSocket) !== 'undefined') {\n",
                             "        return MozWebSocket;\n",
                             "    } else {\n",
-                            "        alert('Your browser does not have WebSocket support. ' +\n",
+                            "        alert('Your browser does not have WebSocket support.' +\n",
                             "              'Please try Chrome, Safari or Firefox \u2265 6. ' +\n",
                             "              'Firefox 4 and 5 are also supported but you ' +\n",
                             "              'have to enable WebSockets in about:config.');\n",
                             "    };\n",
                             "}\n",
                             "\n",
                             "mpl.figure = function(figure_id, websocket, ondownload, parent_element) {\n",
@@ -694,15 +709,15 @@
                             "                // there is no ghosting.\n",
                             "                fig.context.clearRect(0, 0, fig.canvas.width, fig.canvas.height);\n",
                             "            }\n",
                             "            fig.context.drawImage(fig.imageObj, 0, 0);\n",
                             "        };\n",
                             "\n",
                             "    this.imageObj.onunload = function() {\n",
-                            "        fig.ws.close();\n",
+                            "        this.ws.close();\n",
                             "    }\n",
                             "\n",
                             "    this.ws.onmessage = this._make_on_message_function(this);\n",
                             "\n",
                             "    this.ondownload = ondownload;\n",
                             "}\n",
                             "\n",
@@ -842,15 +857,15 @@
                             "\n",
                             "    window.setTimeout(set_focus, 100);\n",
                             "}\n",
                             "\n",
                             "mpl.figure.prototype._init_toolbar = function() {\n",
                             "    var fig = this;\n",
                             "\n",
-                            "    var nav_element = $('<div/>');\n",
+                            "    var nav_element = $('<div/>')\n",
                             "    nav_element.attr('style', 'width: 100%');\n",
                             "    this.root.append(nav_element);\n",
                             "\n",
                             "    // Define a callback function for later on.\n",
                             "    function toolbar_event(event) {\n",
                             "        return fig.toolbar_button_onclick(event['data']);\n",
                             "    }\n",
@@ -899,15 +914,15 @@
                             "    nav_element.append(fmt_picker_span);\n",
                             "    this.format_dropdown = fmt_picker[0];\n",
                             "\n",
                             "    for (var ind in mpl.extensions) {\n",
                             "        var fmt = mpl.extensions[ind];\n",
                             "        var option = $(\n",
                             "            '<option/>', {selected: fmt === mpl.default_extension}).html(fmt);\n",
-                            "        fmt_picker.append(option);\n",
+                            "        fmt_picker.append(option)\n",
                             "    }\n",
                             "\n",
                             "    // Add hover states to the ui-buttons\n",
                             "    $( \".ui-button\" ).hover(\n",
                             "        function() { $(this).addClass(\"ui-state-hover\");},\n",
                             "        function() { $(this).removeClass(\"ui-state-hover\");}\n",
                             "    );\n",
@@ -963,15 +978,15 @@
                             "    y1 = Math.floor(y1) + 0.5;\n",
                             "    var min_x = Math.min(x0, x1);\n",
                             "    var min_y = Math.min(y0, y1);\n",
                             "    var width = Math.abs(x1 - x0);\n",
                             "    var height = Math.abs(y1 - y0);\n",
                             "\n",
                             "    fig.rubberband_context.clearRect(\n",
-                            "        0, 0, fig.canvas.width / mpl.ratio, fig.canvas.height / mpl.ratio);\n",
+                            "        0, 0, fig.canvas.width, fig.canvas.height);\n",
                             "\n",
                             "    fig.rubberband_context.strokeRect(min_x, min_y, width, height);\n",
                             "}\n",
                             "\n",
                             "mpl.figure.prototype.handle_figure_label = function(fig, msg) {\n",
                             "    // Updates the figure title.\n",
                             "    fig.header.textContent = msg['label'];\n",
@@ -1064,17 +1079,17 @@
                             "            } catch (e) {\n",
                             "                console.log(\"Exception inside the 'handler_\" + msg_type + \"' callback:\", e, e.stack, msg);\n",
                             "            }\n",
                             "        }\n",
                             "    };\n",
                             "}\n",
                             "\n",
-                            "// from https://stackoverflow.com/questions/1114465/getting-mouse-location-in-canvas\n",
+                            "// from http://stackoverflow.com/questions/1114465/getting-mouse-location-in-canvas\n",
                             "mpl.findpos = function(e) {\n",
-                            "    //this section is from https://www.quirksmode.org/js/events_properties.html\n",
+                            "    //this section is from http://www.quirksmode.org/js/events_properties.html\n",
                             "    var targ;\n",
                             "    if (!e)\n",
                             "        e = window.event;\n",
                             "    if (e.target)\n",
                             "        targ = e.target;\n",
                             "    else if (e.srcElement)\n",
                             "        targ = e.srcElement;\n",
@@ -1089,15 +1104,15 @@
                             "\n",
                             "    return {\"x\": x, \"y\": y};\n",
                             "};\n",
                             "\n",
                             "/*\n",
                             " * return a copy of an object with only non-object keys\n",
                             " * we need this to avoid circular references\n",
-                            " * https://stackoverflow.com/a/24161582/3208463\n",
+                            " * http://stackoverflow.com/a/24161582/3208463\n",
                             " */\n",
                             "function simpleKeys (original) {\n",
                             "  return Object.keys(original).reduce(function (obj, key) {\n",
                             "    if (typeof original[key] !== 'object')\n",
                             "        obj[key] = original[key]\n",
                             "    return obj;\n",
                             "  }, {});\n",
@@ -1169,17 +1184,17 @@
                             "        this.send_message(\"toolbar_button\", {name: name});\n",
                             "    }\n",
                             "};\n",
                             "\n",
                             "mpl.figure.prototype.toolbar_button_onmouseover = function(tooltip) {\n",
                             "    this.message.textContent = tooltip;\n",
                             "};\n",
-                            "mpl.toolbar_items = [[\"Home\", \"Reset original view\", \"fa fa-home icon-home\", \"home\"], [\"Back\", \"Back to previous view\", \"fa fa-arrow-left icon-arrow-left\", \"back\"], [\"Forward\", \"Forward to next view\", \"fa fa-arrow-right icon-arrow-right\", \"forward\"], [\"\", \"\", \"\", \"\"], [\"Pan\", \"Pan axes with left mouse, zoom with right\", \"fa fa-arrows icon-move\", \"pan\"], [\"Zoom\", \"Zoom to rectangle\", \"fa fa-square-o icon-check-empty\", \"zoom\"], [\"\", \"\", \"\", \"\"], [\"Download\", \"Download plot\", \"fa fa-floppy-o icon-save\", \"download\"]];\n",
+                            "mpl.toolbar_items = [[\"Home\", \"Reset original view\", \"fa fa-home icon-home\", \"home\"], [\"Back\", \"Back to  previous view\", \"fa fa-arrow-left icon-arrow-left\", \"back\"], [\"Forward\", \"Forward to next view\", \"fa fa-arrow-right icon-arrow-right\", \"forward\"], [\"\", \"\", \"\", \"\"], [\"Pan\", \"Pan axes with left mouse, zoom with right\", \"fa fa-arrows icon-move\", \"pan\"], [\"Zoom\", \"Zoom to rectangle\", \"fa fa-square-o icon-check-empty\", \"zoom\"], [\"\", \"\", \"\", \"\"], [\"Download\", \"Download plot\", \"fa fa-floppy-o icon-save\", \"download\"]];\n",
                             "\n",
-                            "mpl.extensions = [\"eps\", \"jpeg\", \"pdf\", \"png\", \"ps\", \"raw\", \"svg\", \"tif\"];\n",
+                            "mpl.extensions = [\"eps\", \"pdf\", \"png\", \"ps\", \"raw\", \"svg\"];\n",
                             "\n",
                             "mpl.default_extension = \"png\";var comm_websocket_adapter = function(comm) {\n",
                             "    // Create a \"websocket\"-like object which calls the given IPython comm\n",
                             "    // object with the appropriate methods. Currently this is a non binary\n",
                             "    // socket, so there is still some room for performance tuning.\n",
                             "    var ws = {};\n",
                             "\n",
@@ -1189,15 +1204,15 @@
                             "    ws.send = function(m) {\n",
                             "        //console.log('sending', m);\n",
                             "        comm.send(m);\n",
                             "    };\n",
                             "    // Register the callback with on_msg.\n",
                             "    comm.on_msg(function(msg) {\n",
                             "        //console.log('receiving', msg['content']['data'], msg);\n",
-                            "        // Pass the mpl event to the overridden (by mpl) onmessage function.\n",
+                            "        // Pass the mpl event to the overriden (by mpl) onmessage function.\n",
                             "        ws.onmessage(msg['content']['data'])\n",
                             "    });\n",
                             "    return ws;\n",
                             "}\n",
                             "\n",
                             "mpl.mpl_figure_comm = function(comm, msg) {\n",
                             "    // This is the function which gets called when the mpl process\n",
@@ -1268,15 +1283,15 @@
                             "    // that it is saved nicely (might be nice to debounce this).\n",
                             "    setTimeout(function () { fig.push_to_output() }, 1000);\n",
                             "}\n",
                             "\n",
                             "mpl.figure.prototype._init_toolbar = function() {\n",
                             "    var fig = this;\n",
                             "\n",
-                            "    var nav_element = $('<div/>');\n",
+                            "    var nav_element = $('<div/>')\n",
                             "    nav_element.attr('style', 'width: 100%');\n",
                             "    this.root.append(nav_element);\n",
                             "\n",
                             "    // Define a callback function for later on.\n",
                             "    function toolbar_event(event) {\n",
                             "        return fig.toolbar_button_onclick(event['data']);\n",
                             "    }\n",
@@ -1392,96 +1407,55 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<img src=\"data:image/png;base64,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\" width=\"640\">"
+                            "<img src=\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAsAAAAIQCAYAAACPEdjAAAAgAElEQVR4XuydC9hcVXm2ExKCWkAFQ+vvKUpVRP1rLbaeDW214hFISACjpsXWaqv11HqgSoxV67H+nlq0VFQgEAKKlWKt1WgVtR57UEFrm2q1iIoIiJAT//PEb8M4zpdvZq13rb33zL2va1/fHPZ+95r7WTP7njVr5lu8iAUCEIAABCAAAQhAAAIzRGDxDD1WHioEIAABCEAAAhCAAAQWIcB0AghAAAIQgAAEIACBmSKAAM9U3DxYCEAAAhCAAAQgAAEEmD4AAQhAAAIQgAAEIDBTBBDgmYqbBwsBCEAAAhCAAAQggADTByAAAQhAAAIQgAAEZooAAjxTcfNgIQABCEAAAhCAAAQQYPoABCAAAQhAAAIQgMBMEUCAZypuHiwEIAABCEAAAhCAAAJMH4AABCAAAQhAAAIQmCkCCPBMxc2DhQAEIAABCEAAAhBAgOkDEIAABCAAAQhAAAIzRQABnqm4ebAQgAAEIAABCEAAAggwfQACEIAABCAAAQhAYKYIIMAzFTcPFgIQgAAEIAABCEAAAaYPQAACEIAABCAAAQjMFAEEeKbi5sFCAAIQgAAEIAABCCDA9AEIQAACEIAABCAAgZkigADPVNw8WAhAAAIQgAAEIAABBJg+AAEIQAACEIAABCAwUwQQ4JmKmwcLAQhAAAIQgAAEIIAA0wcgAAEIQAACEIAABGaKAAI8U3HzYCEAAQhAAAIQgAAEEGD6AAQgAAEIQAACEIDATBFAgGcqbh4sBCAAAQhAAAIQgAACTB+AAAQgAAEIQAACEJgpAgjwTMXNg4UABCAAAQhAAAIQQIDpAxCAAAQgAAEIQAACM0UAAZ6puHmwEIAABCAAAQhAAAIIMH0AAhCAAAQgAAEIQGCmCCDAMxU3DxYCEIAABCAAAQhAAAGmD0AAAhCAAAQgAAEIzBQBBHim4ubBQgACEIAABCAAAQggwPQBCEAAAhCAAAQgAIGZIoAAz1TcPFgIQAACEIAABCAAAQSYPgABCEAAAhCAAAQgMFMEEOCZipsHCwEIQAACEIAABCCAANMHIghsU5E7zRV6rP6+f56i/67b76n1SK1bIw5coMZK1fyI1o9q9eVpXp6iB/c0rYdpvcXcA721/l45zQ868LG5Dz+sw/15hdr2X1r/W6svs9QhkPIaMgtZHS78v6f1V+b642309wat39D6Ia2v1bptLxHdXfe9WOuvaz1Y62Va/07rRq3/O2K/O+q2R2l9pNb7av0Frddr/ZrW92p9g9ar6nQJjtJFAghwF1PpX5v8otUI8L/p8n207h7xMBDg7mT7GDXlb7Vep/UftF4x17Sn6++13Wlmp1uyVa1DgLsb0Uo1rY03synHXaG2zvdmpXl9vbO28eW+Ln7D/XatltWvarXAHqC1kdMf6bKF9WMjHqCfZxdpvbnWz2u1xP6SVr95/67WB8/VHNz147ryIK07tX5B639qPUjrr2k9UKvfGHowxtxZZpAAAjyDoRd4yNtU0wJscfJI4pO0vnvEcRDgAvATS75zLiePyPikxDI5ga3apcsCvK/ad6jWHVq/PvnD6/0eK/UI+iLAe8uqeX3tuwCvUB77ab10qGf5sb9K67O1+rHeRatHhpvl53ThP7R6BPcZWt88cJ9HjZ+r1VJ8xNB+5+j6J7X6XPT9gX2W6/Jmre4flm0/h1lmkAACPIOhF3jIftGyAP+51hdo9TtqvzPfPnQsBLgA/MSSH9Z+Hv3o8nSUxIdWbbetcydPGFZDPtGBLDh9EeC9PbDm9bXvAry3x2gJ9nSEm2n1VAePEDfLH+rCm+ay9PSHwWWJrlio/Ubv0Vo9JWKc5fba6JtzG3qqRHN5nH3ZZkoIIMBTEmTLD6N5gb6f2vEWrb+q9Y+0vnGoXfMJ8FZtt7eRtNN1/5O1/rZWX26Wwds/oxs9F+yhWv0x2Re1er6YT4Be/JH/H2v19Az3ex/TIwf+KG1wWTm3j+cA+wXVNdZovZ3Wy7V67tgGrYMjCoP730FXnqfV8878wurRN08L8SirR10HRza8n9vRPHZPG3m+Vn9E54/qjp073k+38Gev+eTxVK1P1HoPrb6+TesFWl8z1NbTdd0sRy0v1Y0bFjiY7z9F63zbrtd979Dqx+rLg8vxuuIRZ2fgjz5/qNUfh3oU5vVah0cp/ThO0voErffS6lx9ovLUjVdq9Uefg8vgsZ2t2+k56c7OJ8aj5zZ+hP66f7q/es7z1Vqd7cVaPbrk0aRxlq3aqMnONXw8f+TqESuflN3/TxtRyG8WT9Tqdvyi1kO0+uPff9HqfnLW0D6/r+t/qdV975h5GmY+7mf+WNl90B/7rtA638fqTT/0c2Gt1mdpvbdW3/7Pc4/FHyGPWpyf83+IVo/oXaLVz/u/mdvf+0xybhlsi/N2H3E/dh9p5qR7/qj7z2/OPS7PH3X/8fPenD8w1NCtuj7fyN7w/P6Gwe9oH38c7+N+R+vfa3251m0jKfykP/k1xR/F+3n+Wa1/NvfYJxXvFdpvOKv1us3PpfmWYSE2M7/2WBJvq/XHWj83x+d9I4r4cbkvuo6z/5OBx+L2+7G5Tfto9fPFfCyaFtXztHqww/0+YrHIuq4/QVyh1dMTmsXzg39Dq6dQjHo+mfnJWv3ccd8Zd/Hrh/vRA7V6pJhlxghM8iI1Y2h4uBMQ2KZt/UJqofDcqn/UaqHwi+U1A3VKCbBPvpZjz/H6kta7avWJzCclv3D6hO0vPHxCqwXBgu72+rLFYVBmV+q6X/z9gugXft/v0VKPZvuE6hdMS7NP/j5JDi4eCXyP1ltq9Ud2frz7a73/3F9/FOfpIYPL1rm6b9Vfi86X5/bzcdzmC4e2H77qERPPjVup1VNQ3Hb/dfv8kaFPJD4hmo0Xn0Q8X86C/vNafZI3By8WLK97WzbozhQBbvZzJhbNb2u9ldYVWn3iPkHr2QMHdj/yY3dbLTo+kfvLec7V+/iLM85j28A+63XZwuD9LEzO4Z+0+pjO2Hybbfxm49NazccZWRr/r9YXafUnGeMsW+fa4I9vn6PV0uvM/cbHJ1UvFpLXDRX7U11/mVYLvwXDbfOIlPuJRcCjXc8c2Mec/EbB9/0frd8b0Ti/0WmO5b9eVszV92P05cGlkU63w/Jg2XU/MIPm05uVujwsBu5L5ut+Z/H1G033M/e3v5hrg48zybmlaYvffHgOup+n/6P1blr9/HX+f63VcvwVrX48liV/VO6Pvb34DY/fRDWL5Wyl1t/S6ufpoCC73U3GfpPlfuc3mxZGS6y39/PeHH6g1W9UfPvgYll07l7cn90mS6T7nfOzMA6L9lCJn7q6QteGBdh938/X1Vr9psrSOfh66pybvuA3B37TuUyrXwP9GP1Rv/uUb3POLxlqwDZd9+ug+475uQ/4sft13O35llbL/V9p9dzcrVr9xsqDDO6TH9RqvrmLX2fdNr+u+E3gL2tt+oRr+/nhAQG35V9HHOzxus2vW87IbR9n8eur+7ufU8NvJMbZn22mgMAkL1JT8HB5CIUIbFPdRoD9ImSp8kljg1aPFDVLKQF2/eEToE9OPkn5ozSfoD0CbBny4pO3X7x90vYLr08OzbJSFyyRXryvT/g+EXjxyJAF1yflc7V6ZLhZPOLiE4/FzSfqd2ltXsQtVx6BsYhb1E8f2G+rLjcjVR7FfdvAfeNcfLU28kiNT3geHWva6tFSC/cqrZ/S+oChYs1xLe2+PO6yQRtOKsAeJbRI7NLqb4APfrzp4/oNi0+sFoBmsZR4ZHKLVo/qeH8vPmG9QquzHRaM9bqtGTFzvhaH4REqvxHwCc8jtRaXwcUS6vz8JmScZas2arJz5h4BbZZ1umD+FjX3jcEvFvok7evuL4OLOfjNo/uLxcWC3iybdMGSM+qTFTPxyLiPYwnz88zLCq3DUtXUa/qmv/zo56rfYHixjFh4flerR94ePtAGj875jZ2P409bNmht6lj4/bz3mwkvk5xbmhoWXbfFI9DDizlbMrcN3eFPS5y1+7uF2OLcLCt1wc/lvYmoRdifuvhTCH/SMLh/89G736hYht1HvVjQPPLsdluc/YlEs/i56Oekl1wBbmpu0wW/vs4nan7T4vb4Tbpfk/yGuFn8qzu+7j7l17Lmtc33N3Ut/ubejPj79dFvGMzcfclvEvya17y2+A2ev1RmKbUMN6+rA4fd60WP6vvNkhdf9uuia3pgwTLrNznN4uej+4UXS3dzefAAzsOf2liULbbjLE3u3s+vSSwzSGCSF6kZxMNDHpPANm03KMAepbMIe7TCo8DNR9WlBNijVM2IW9Nkv7A2v2zgj8s9sje4+KPk87X6hDA4r2zl3G3edtRPuvkja8umnzsrtFo8vDTC7ZOfT6jDi0eqfJIafsHdqtt8ovEvMfgkNMnik75H2i0d3tc1BhefDCxAvt+jSR5Za5bmuDUE2CNRbqdHd3yyW2jxKJrl0MLj0WGfoAcXS5pHHi17Pvn7o38v67VagD3i69HDbSMO5KkGFgX3j9xlqwo4O4/MWbaHF4u02+9tRn2zfdTxLZ5+E+Qv91immsUjbZYSi4efX4OLR+c8KmuJbUZEff8KrQsJ8PCXiryfPxnw6Jh/Mspv+szTiz+98Cij38D4cQ3/0kvzHPC2k5xbGgH2SLTf3Ey6eJqCn98WVn8a1CwrdWFvAmyBs/D6jZlfp9xHh5f36wZPhXqc1kZ0/TG8pwOYxfoR+/i1z1JVS4D9ZS+Lr0fPPVVmeHHf9Bt2v975DXGzbNMFv26Pen309A6/2ffivuc3GYPL/9MVf0rhN8N+MzTJMjj/ttnPz+f1Wv0aMbj4E49GvC3izZuQwW38xtF90s9rv9leaPFAgZ9L7qN+7XdOLDNIYJIXqRnEw0Mek8A2bTcowN6tGcHzC6XnF3opJcDzvQj740H/XuQoAWnmTPpja4/uNMtKXfBJ0x+3zydJzc/reJTvzLkdLWGu6dG94Y9LvYmfa80cN3+c6Z8f87J1rn3+PV6PvE2yWGo9+uLpBJ7nOmrxfFJPL/DH7haFZmmOW0OAfUyL2Aqt/pjac/X8JmK+xaP5FkDLjKVm1OL7fMIfHDVfr+sWYI+cegR11OJsV2r16KxHoXzibQRsL00aeddW3eq+NTyq32xs4fAbreHpHb7fo2wWC/cXv0FoTtweXfWbGX9i4NGwZrH0e9qHcx6Uft/fCNCwzK7QfQsJ8Hyjin7z6P7v9jRTZBrxG/Vxutvhj6jN08sk55aGv6V6b/3CMm4Z9Zsoy6s/2vdiAfIbYM8F9gh5s6zUhb0JsGXQnzD4zYM/IRq1NCO6g5LoUXALs0fHPUo+vPj1zn2rhgC7X/jTEbPxG5fhefFuW/MG1NNoLJTNsk0X/Lq9t9dHv/nxG22/SRhcmtHxU3WjpxalLu5fnpJmifZotacSDX53JFqA/abZb0Y9mjz8mpj6GNivpwQmeZHq6UOk2RUINC+kg/LnkVJ/lOUXTn+r16N5pQR4+OPn5iE37fLJqpkD29y3QhdGycFK3e6Tpk/k/mht1HKGbvTHpZ5n2MwD9Mhi888kFkLuEZBmVGOrLvsE5FG8wY8uF6rh+z1FwG80PLJrGR61NF8Q8ciQhbFZmuPWEmBPN7Fs+AtfXnyi9tQMf2xunoMfbTZyOw6DwZPYeu1gAfZPHJnNqMWS5VE9f1zuxcf1R+4WGU9baWRvnGNv1UbOzh8Pe5748HK6bniy1mFB9nQUt9H9YL7FtZ3N4OLR0Rdq9ZsIv0nw0swPtghZJppPPXzfCq0LCbCnT4z6ze5tut1yNCjIHjWztM/3ZSS3pZmqMsm5pRFgP3+GR/ubx+83A55iYvGdbzldd5h1s6zUhb0J8OB0hb2U3XOX5yB7dN6L37z6DYtf40b9vFwzelpDgBu5Xaj9vt+jpx5FbZZtuuCM9/b66E+4PD1heFmvG/xcm28UfJz2DG7jN1se/fUbPH+K4U86vEROgfBAhzPxa5Dn5Tdz5SdtK9tPCYFJXqSm5CHzMAoQaF5Ih0c/LV0eHbBYWARSBdj7+xcOhkXi9Lm6843ANe0aNcq1QvtGCnBzUvRoXDO6Ox/qwS+vbNVGlqhJRdS1GwH2iLQFc9RSW4D90bBHCkedGC04HmlbqdUjdh7J9GuQR+o96tmc9DwS7pFdf6TfzGedj+XgF/fWa6NxTsqWAIucP/70XGBPKViq1fNyPSo4+IWp+Y7r27dq3Vt2p+v+YQE2A78Z82idOfk54hFFz1W2iJqD3xSMkidP6/AnFv6ikuXZQmNO5jVqGsYK3b6QAM93DtimfecT4PnecA7KyiTnlkaA59vHj9UfcXsk0iOxng/t9vlNp5l5jrhHIof73ErdtjcB9htY1zNTvxnb2+LnmCXYS5cE2N9v8MiuBxr8RnKhZf3ABmY4nHFz9wpdmK/veBvXGee5tlB7Bu/3lwc9suzR4FMG7mg+jZjvS3CennKB1uEpQIO1/dzZqtVvEvf2ydIk7WXbnhOY5EWq5w+V5hck0LyQDguwX2x8cvfHvX7x8mjlqH+F7Pll/jhx1JxbN9sy4C9b1BTgcaZAWMqbk46/wOERIU+DGP5y097Q+0U5VYCbKRAeTZ5vNDF6CoTnWnoqxXwjKC/Vff5i4TgjQ+4f/qjYIj84j9tzQS3uw/NgF+rC67VByknZo08+4frj871NJxk+/kLZna4dhgX4kbrNI/3znaw9Su8T9Hyjh/7inkeQmzmp5ubpHqOeOyt0e6QAewTWz8FhQWm4+A1NM4dzknPLQgLsN9F+ozDfXOvmi6CTCrA/xfHz159MHLdQ5xq436O+/gTBc0n9pcXhpeYUCL9x89QqvznwNIjBX4lY6CFt0wZdEmC/bvj1w2/oPCWsWfzpjD9lme+Th+ZN/uAo/eBj9xSZrVo9ncLTr/ymselzCzHi/ikmMMmL1BRj4KFlEmheSEfNf20+tvUXSHzSGCXAlpb1Wv2RpKVncPFImSXaX+SqKcBuw6gfVvfHhR4x8kfOK7R6XqYXz1vzHEy/gG+YgOdWbZsqwINfght1Mvb8521z7KK+BGehO13rqHmTfj3xSJrn9I0jwMZkns7Xo6+eG+3FI7IWRN/uKQujvvgyCvF63ZgiwK7lUWGP7DlXf0Q6ai7l8DG36oZJR4BP1D6eN+6R61G/6dvML59PgJsvyVkG/WbEfdHTNprf/h1s4wpdiRTghq/n6fp5PDx1wqOpHlX1Msm5ZSEBbt50+WcBnz0Ugqci+MuGfm0Z7nP+lMHTg+abIuTXFn/E75Fkf0rkN73jLM0bAfc1f+IxvPjLrv4Yf74MRx1jhW6cLyuPflvivPo5Mbx4vrjfAM33Sdh8j2mb7uiSAG9Ve/x8Gv5FH7+u+vXVo/mDX1j24/IUHj8H/Doy3+u1c/DUCuflTy+Q3/l6xIzdPsmL1Iyh4eFOQKB5IR0lwJ4X6I98PcrW/Kvk4Y/7/WUyfynJdXzS8kd6XjzfzyOY/rjaS20B9oneL7hNeyzhFg9/TD38jWoLiD+ut5T6JO2PZIfFzdLg+dDet1m26kKqALtG8/uvHnX2KHrTVo+6e+qIR7YifwbN8wF9ovZJxO1uflnCJyJ/OcpzVL0MyohPsm6b5716tGpwaUbLPF/cv/7QLP4GejOX0t82H/x5Km/j/uRvvnsaQcN5vS7vTYA9/cCjie5rw4LbHMvt869nNL98MNTcn7q6VdcmFeBG7n0c/4RX86Uvi7fnM/sNlJf55MnTDJrfL/Vj9WjWfKPxK3RfpAD7DYpHPy2OHq3zyFsjE34s/hUSj0J6meTcspAA+6fG/LyzrPo1xlNAvPhLcP7t4GZu7rAAu99tm9u+mTIyt+uNf/wJhPugv0zqqRTDX8LzY/b8Y4/0Nsf1Lzx43rjfAPi+wf8+5ud+83vEUQJs8VupdfCXKAYfh2Xbnwx4/rT7g6dhDUqeszC35rd7m33NpqYAm3OT42D73afd9z0A4qlAnqvrT2Kaxa+7/oTN0z2Gf+mjef3z9CnnMvi4/abGGfi12X3Db1ZGzXcfbAuXZ4jAJC9SM4SFhzohgeaFdL5fQBj+ssmwAPtEZknzl878JRpLlW9zPb8Q+sXPglJTgP3RsqXOUuYvOPkndiw7/tKJJcAjqsNfmPLj8sepFneLqKXUP63kE4+/fewXYp+c/HuuzbJ1ru4wk4FN9nrRouuP1Fdq9UiW2+oToecEe4qBR6hde/hLgDnHtXT8gVZLosXBMmexs5RayiysgzLib+37BGWG/nKhpczCZ7Z+U+A6lhx/Oa1ZfFL0yJaZe2TWH61v0+qPfD3a54/bnY/fcDRzrtfPHX++0efmS1qeL+lf7XC/8gnRo0eWCJ88PQVh3F/j2DrXvvmyO133P1nrcL/1pyGeC+2fGbPc+It47ut+c2F5GvUbx7r5xsUjyB5Jbhb3rVFzpVfo9kgB9vH8Rsbt98ir37Q4T4uJpyh5lM4C6DybX2gYbPd8lxcSYGdu4fTrgwVpq1Zn7vnbt9TqN0HDfa45ln920Pu5rf5Uwcw9Ymhx8uKRf0+D8Jsp9ws/Hj9X3KYVWj11y491+Bcq/EbPn255O8vnf2t1Du7Pfn64PVEC7Fr+NR0/dk8Xa0aq/XOL3597HH5N8ci0nw9ui0fFPXfWr1d+/vlTDX9htxmh927btNYUYB/PfdxtcwbOwiOzbp+f7358fhyDbyjmHt6e1wG/zvnxOUc/d52Nc/F3CPx67JqDS5O9j+M33/PJr38TeG+/PjJUlqvTQgABnpYk230c23R4v5DOJ8CWNL9gNfNURwmDpdEjSh5R8Yu2BdIjpado9Yl1lEicPs/tDY2mXR4J8OXBZYWujJKDlbrdUuKTlz9S84icvxjl+WMeNfRH1xu0+kV31GIZ8Ed23tdi5ROsRdnH95er/Hucg98c36rrextFnOcwP3Wzj+GRTc9J9gnB1308fzHE8yObk+TgTjnHtbz6i3weUTFbC7CZeRTHI/jDo7AeFfRHjyu1WhAs5j4Zee6yf5LIJ/dR/3zCgmvR8ycEFuxGYP2myG+S/PgGf590/YhjDz5mi5TnEbodPum6HWbldliw3M/8E2rjLlu14aQjwK5tObQoOi/3Ec/b9Bsuz632Cb7pf27nqMXTXZrffN7bF39WaLtoAXZ7nMUGrX6TZTm0eHiOrgXFb7j83B38ua15HsaNNy8kwN7Qfcj9y2+E/VrjN8pb59rhOdHDfa4pbgYWP+fkkX33qVFi6ikE7qOevuPtLGN+HJ7O4H7mKT/Dnwr4TZufBxYxfwrhnz90hu7bC2XYtG+wnfNl5eebp4F4zrKfb2buZfh1zX3Jsuw3KWbkxa89njbh9vvN+eDI6ra57SZ5fWzau14X5mM+/Nia634u+9M8v9n066TfvJizzw1+Hr91qH3DdfzpmT958Hxgv9n2iLxl2a/RzSdfg/s0j2++9jS3pw4+LFSX+ztOAAHueEA0DwIQgEBPCFjoPe3GI/kWShYIQAACnSWAAHc2GhoGAQhAoHME/FF68zH7YOP8SxT+dMTzg/2fxzzXkwUCEIBAZwkgwJ2NhoZBAAIQ6ByBZvqF5xz7I3vP6/ac7OafxvgLhk/qXKtpEAQgAIEhAggwXQICEIAABMYl4Hn8no/qObWeQ+25uZ4D7i+Pna7VXyhr5vSOW5PtIAABCFQngABXR84BIQABCEAAAhCAAATaJIAAt0mfY0MAAhCAAAQgAAEIVCeAAFdHzgEhAAEIQAACEIAABNokgAC3SZ9jQwACEIAABCAAAQhUJ4AAF0R+ww03+JvSB2sd/McHBY9IaQhAAAIQgAAEIHAjAf+DlO8vXrz4XjD5aQIIcMEeIQH+3927d//Cjh3D/0Co4EErldaTadGyZcsWbd++fZEeZ6WjcpgcAmSWQ6+dfcmsHe45RyWzHHrt7DvNme27776L9tlnn8v0GP2rLSwDBBDggt1BYvjx66+//kHf//6o/0Rb8MAVSusJtegXfuEXFl122WWLJPkVjsghcgmQWS7B+vuTWX3muUcks1yC9fef5swOPvjgRfvtt98nJMAPrk+220dEgAvmgwAXhEvpiQlM84v8xDB6sgOZ9SSogWaSGZl1iQACPH8aCHDBnooAF4RL6YkJcGKeGFnrO5BZ6xFM3AAymxhZ6ztMc2YIMALcyhMMAW4FOwedh8A0v8hPa+hk1r9kyYzMukQAAUaAW+mPCHAr2DkoAjw1fQCZ6l+UZEZmXSKAACPArfRHBLgV7BwUAZ6aPoBM9S9KMiOzLhFAgBHgVvojAtwKdg6KAE9NH0Cm+hclmZFZlwggwAhwK/0RAW4FOwdFgKemDyBT/YuSzMisSwQQYAS4lf6IALeCnYMiwFPTB5Cp/kVJZmTWJQIIMALcSn9EgFvBzkER4KnpA8hU/6IkMzLrEgEEGAFupT8iwK1g56AI8NT0AWSqf1GSGZl1iQACjAC30h8R4Fawc1AEeGr6ADLVvyjJjMy6RAABRoBb6Y8IcCvYOSgCPDV9AJnqX5RkRmZdIoAAI8Ct9EcEuBXsHBQBnpo+gEz1L0oyI7MuEUCAEeBW+iMC3Ap2DooAT00fQKb6FyWZkVmXCCDACHAr/REBbgU7B0WAp6YPIFP9i5LMyKxLBBBgBLiV/ogAt4KdgyLAU9MHkKn+RUlmZNYlAggwAtxKf0SAW8HOQRHgqekDyFT/oiQzMusSAQQYAW6lPyLArWDnoAjw1PQBZKp/UZIZmXWJAAKMALfSHxHgVrBzUAR4avoAMtW/KMksLrNdv/u4uGIdqrTk7e+r1hoEGAGu1tkGD4QAt4KdgyLAU9MHkKn+RUlmcZkhwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgHpzan8AACAASURBVBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEeAZEODjjjvuFxcvXvw8Sef99XDvpcuXbN68+V7DD13bnaT7nq/b76j10t27d5+8ZcuW9w9up21uqeuv13qM1n21/v2uXbuecf755//vJN0RAZ6EFtuWJsCJuTTh+PpkFs+0dEUyiyOMAOezRIBnQIBXr179eL3wvFnS+Wk93LtJcvcZFmCJ7fG6/Szd/3L9/bC2XavLFuKHnHPOOZ9qMGm7D+i2e+r6c7XNdd5e667vfve7R2zdunXnuF0SAR6XFNvVIMCJuQbl2GOQWSzPGtXILI4yApzPEgGeAQHesGHDPlp3+6FKYE+XwB4xQoAv1d2fO/fcc08ckN2Lte2V2vZRc/s+QH8vlrz+lkaGPzh32921zVd0+Xhtt3ncLokAj0uK7WoQ4MRcg3LsMcgslmeNamQWRxkBzmeJAM+AAA8+xFECvGrVqrvohenrWo/RaO97m+3XrFnzTInqa6655poDL7roouu170bJ7jPkuQdpmxsGtvu8tvtXyfP6cbskAjwuKbarQYATcw3Ksccgs1ieNaqRWRxlBDifJQKMAC9au3btozTf90Kt9zjvvPMuGRgBfrguf7C5XULsEd47SoA9l/jGRWJ8psT40OHb99Y9EeD8Jy8V4ghwYo5jWasSmdUiHXccMotjiQDns0SAEWBPi3iCMJyh9bYaxb2sQaK5w0dIbD8jWX2QpjxcrO3+Qfft0jaPHBLgN2u7R0iA7zYfznXr1h147bXXHtjcv2nTpvMl1ve78sor83txxyr4Rf6QQw5ZdPnlly/SY+xY62jOKAJk1r9+QWZk1j8CcS3ecdJj4op1qNK+p/3U9+6Ltuyggw5atGzZsk/IXx5c9EA9LL64h21esMmjpkDUEGCNHm+QSJ/SNHDjxo2L/O5r+fLlC7aZDSAAAQhAAAIQuInANx99xFTiuMOFn639uBDgEcRnRoCbKRBicJhGd/1luD2LxPhnpkBIYu+gbfxluBuXcaZAMAJc+znN8SYhwGjiJLS6sS2ZdSOHSVpBZpPQ2vu2jADns2QEeH6GMyPAzZfgJLdHa6rDBQMC/Axdfq3WAyS92/0lOF3+Q10+WH9v/BKcbv+crv8bX4L7CTnmueW/MNWuQGa1iecfj8zyGdauQGZxxJkDnM+SOcAI8B4CkthLPd9X83jXDQjwx3XbVcM/g6YXsYfr1yI+5O2OP/74u2meq784x8+gzYHjRT7/hal2BTKrTTz/eGSWz7B2BTKLI44A57NEgGdAgB/72Mfe4mY3u9me3/KV0P6BRnoP1cXnzD30j2rk9ruao3uCrp+p+16m9SPabq3Wp+jyQ3X/Jwek+AO6fLhuf+6SJUuuk/z6H2Hs5h9h3NSReJHPf2GqXYHMahPPPx6Z5TOsXYHM4ogjwPksEeAZEGCN0q7Qvyv+r1EPVSJ7pKY9bPV9/lfI+vMCrXv+FbLue9F8/wpZcnys7l+qvx+UCD9Dv+rw7Um6Iz+DNgktti1NgBNzacLx9cksnmnpimQWRxgBzmeJAM+AAOd3k/gKCHA8UyqmE+DEnM6urT3JrC3y6ccls3R2w3siwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjMiqEtVpjM4tAiwPksEWAEOL8XJVRAgBOgsUsxApyYi6EtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8D5vSihAgKcAI1dihFApoqhLVaYzOLQIlNxLGtVIrN80ggwApzfixIqIMAJ0NilGAFkqhjaYoXJLA4tMhXHslYlMssnjQAjwPm9KKECApwAjV2KEUCmiqEtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8D5vSihAgKcAI1dihFApoqhLVaYzOLQIlNxLGtVIrN80ggwApzfixIqIMAJ0NilGAFkqhjaYoXJLA4tMhXHslYlMssnjQAjwPm9KKECApwAjV2KEUCmiqEtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8D5vSihAgKcAI1dihFApoqhLVaYzOLQIlNxLGtVIrN80ggwApzfixIqIMAJ0NilGAFkqhjaYoXJLA4tMhXHslYlMssnjQAjwPm9KKECApwAjV2KEUCmiqEtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8D5vSihAgKcAI1dihFApoqhLVaYzOLQIlNxLGtVIrN80ggwApzfixIqIMAJ0NilGAFkqhjaYoXJLA4tMhXHslYlMssnjQAjwPm9KKECApwAjV2KEUCmiqEtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8D5vSihAgKcAI1dihFApoqhLVaYzOLQIlNxLGtVIrN80ggwApzfixIqIMAJ0NilGAFkqhjaYoXJLA4tMhXHslYlMssnjQAjwPm9KKECApwAjV2KEUCmiqEtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8D5vSihAgKcAI1dihFApoqhLVaYzOLQIlNxLGtVIrN80ggwApzfixIqIMAJ0NilGAFkqhjaYoXJLA4tMhXHslYlMssnjQAjwPm9KKECApwAjV2KEUCmiqEtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8D5vSihAgKcAI1dihFApoqhLVaYzOLQIlNxLGtVIrN80ggwApzfixIqIMAJ0NilGAFkqhjaYoXJLA4tMhXHslYlMssnjQAjwPm9KKECApwAjV2KEUCmiqEtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8A3EjjuuOMepysnaz1c6zWLFy/+p127dr3gvPPO+89BTNruJN33fN12R62X7t69++QtW7a8f5LuiABPQottSxNApkoTjq9PZnFMkak4lrUqkVk+aQQYAd5DYPXq1Ssltf+oi+/SieVMSe3BurxR6xKt9z733HN/7O0kv8dru7N08eX6+2GJ7FpdthA/5JxzzvnUuF0SAR6XFNvVIIBM1aAcewwyi+OJTMWxrFWJzPJJI8AI8B4Ca9as+StJ6SMkuofq6g2+be3atUdKhC25D9UI7z/NCfCl+vs5bXdig05SfLEE+MrNmzc/atwuiQCPS4rtahBApmpQjj0GmcXxRKbiWNaqRGb5pBFgBHgPAUnsaZLYIySxv9QgkQDfVwL8OZ1oHqbR3Y+tWrXqLrr8da3H6Pp7m+0kz8+U0L7mmmuuOfCiiy66fpxuiQCPQ4ltahFApmqRjjsOmcWxRKbiWNaqRGb5pBFgBHgPAU2BeIhOKB7t/SNd3TMFQtffKik+RLfdTyO+uyTEj9LtF2q9h+YFXzIwAvxwXf7g8O17654IcP6TlwpxBJCpOJa1KpFZHGlkKo5lrUpklk8aAUaAbyQgCX6MTipnSU4P8I2S3y8uWbLkkZs2bfqOr2uU+An6c4bW20qIL2t21H5HaNvPaL8HaarExaOQrlu37sBrr732wOY+1Txfwny/K6+8Mr8Xd6yCT8yHHHLIossvv3yRHmPHWkdzRhEgs/71CzKLy2zHSY+JK9ahSvueNtF3szvU8oWbQmYLM1poi4MOOmjRsmXLPiF/efBC287a/Ytn6QFLYh+oE8qFkti/0d/3ewRYneLFur5DHB7iL8HlCLCmSWxQrVMaphs3blzkd1/Lly+fJcw8VghAAAKdI/DNRx/RuTZFNOgOF342okwna5BZWCwI8AiUMyXAktvPSnj/W3OAVzUsjj322NsvXbr0GxLX35cAv62ZAqH7D9N1fxluz6J9F5wCwQhw2JOVQgUIMJpYAGrhkmQWB5jRxDiWtSqRWT5pRoDnZzhrAnytBPiVEuCXDSKR3F6u29+h25/ffAlOQny0pjpcMCDAz9Dl12o9QGK8fZxuyRzgcSixTS0CzCetRTruOGQWx5L5pHEsa1Uis3zSzAFGgPcQ0BSFr0hKL5HAHtMgkfDeSXOA/0u3/4Fu/8u50d5LPd9XQrxuQIA/rtuu4mfQfkKEE3P+C1PtCmRWm3j+8cgsn2FTAZmKY1mrEpnlk0aAEeA9BDTS619/eIPWN+rE8rdz/wjjT3V9+c6dO+/5nve85/tzonyC/p4pKX6Z1o9IfNdqfYp/K1iS/MlxuyQjwOOSYrsaBJCpGpRjj0FmcTyRqTiWtSqRWT5pBBgBbggs1ijwU3XlaZJT/zOMq7V+UiL8osGfPJuT5ZP09wVa9/wrZG3/Iv4V8k0diRNz/gtT7QpkVpt4/vHILJ9hUwGZimNZqxKZ5ZNGgBHg/F6UUIER4ARo7FKMADJVDG2xwmQWhxaZimNZqxKZ5ZNGgBHg/F6UUAEBToDGLsUIIFPF0BYrTGZxaJGpOJa1KpFZPmkEGAHO70UJFRDgBGjsUowAMlUMbbHCZBaHFpmKY1mrEpnlk0aAEeD8XpRQAQFOgMYuxQggU8XQFitMZnFokak4lrUqkVk+aQQYAc7vRQkVEOAEaOxSjAAyVQxtscJkFocWmYpjWasSmeWTRoAR4PxelFABAU6Axi7FCCBTxdAWK0xmcWiRqTiWtSqRWT5pBBgBzu9FCRUQ4ARo7FKMADJVDG2xwmQWhxaZimNZqxKZ5ZNGgBHg/F6UUAEBToDGLsUIIFPF0BYrTGZxaJGpOJa1KpFZPmkEGAHO70UJFRDgBGjsUowAMlUMbbHCZBaHFpmKY1mrEpnlk0aAEeD8XpRQAQFOgMYuxQggU8XQFitMZnFokak4lrUqkVk+aQQYAc7vRQkVEOAEaOxSjAAyVQxtscJkFocWmYpjWasSmeWTRoAR4PxelFABAU6Axi7FCCBTxdAWK0xmcWiRqTiWtSqRWT5pBBgBzu9FCRUQ4ARo7FKMADJVDG2xwmQWhxaZimNZqxKZ5ZNGgBHg/F6UUAEBToDGLsUIIFPF0BYrTGZxaJGpOJa1KpFZPmkEGAHO70UJFRDgBGjsUowAMlUMbbHCZBaHFpmKY1mrEpnlk0aAEeD8XpRQAQFOgMYuxQggU8XQFitMZnFokak4lrUqkVk+aQQYAc7vRQkVEOAEaOxSjAAyVQxtscJkFocWmYpjWasSmeWTRoA7LsBr16596O7duw/evn37hy644IKr8yPvRgUEuBs50IqfEECm+tcTyCwuM2QqjmWtSmSWTxoB7ogAH3fccS9UU44899xzH9E0Sbedr8uPn7v+P0uXLn3Apk2bvp0fe/sVEOD2M6AFNxFApvrXG8gsLjNkKo5lrUpklk8aAe6OAH928eLFn968efMfuEka+f1NSeIHtZ6pq/+q9RTd/3bd/+z82NuvgAC3nwEtQID73AcQ4Lj0kKk4lrUqkVk+aQS4OwL8XTVlo0aA3+QmafT3zRLeYw8//PDbb9iwYbeuv043P0b33z0/9vYrIMDtZ0ALEOA+9wEEOC49ZCqOZa1KZJZPGgHujgD/WE15ugT3HXMC/EX9/Tddf6Kvr1mz5nckjW/U9f3zY2+/AgLcfga0AAHucx9AgOPSQ6biWNaqRGb5pBHg7gjwf6opmyW4LzjhhBN+fufOnZ7r+zRdf9ucED9HI8Iv1hSIW+fH3n4FBLj9DGgBAtznPoAAx6WHTMWxrFWJzPJJI8DdEeC3SXCPlxi+TH+PVLMerhf4u5x99tnfnBPgU/X3gRLie+fH3n4FBLj9DGgBAtznPoAAx6WHTMWxrFWJzPJJI8DdEeDbSXw/pObsmeMrQdwg2d3oyytXrly6fPnyb+v+c5svyeVH324FBLhd/hz9pwkgU/3rEWQWlxkyFceyViUyyyeNAHdEgOdGeZfo7+Fafyj5/UbTtHXr1h143XXXHamfQfsXjQhvy4+9/QoIcPsZ0AJGgPvcBxDguPSQqTiWtSqRWT5pBLgDAqxfeNhfo7tvVFM+oBHezfmxdr8CAtz9jGaphchU/9Ims7jMkKk4lrUqkVk+aQS4AwI8N/rrX4H4Q438npYfa/crIMDdz2iWWohM9S9tMovLDJmKY1mrEpnlk0aAOyLA+pmzf5EUni8Bfml+rN2vgAB3P6NZaiEy1b+0ySwuM2QqjmWtSmSWTxoB7ogAaxrEU9WUF2v9ZUmw/ynGVC8I8FTH27sHh0z1LrJFZBaXGTIVx7JWJTLLJ40Ad0eAn6R5wM+SGN5JTTpdl7+my9cON09y/K782NuvgAC3nwEtuIkAMtW/3kBmcZkhU3Esa1Uis3zSCHBHBFhTIHYvFKek8QYJsH8povcLAtz7CKfqASBT/YuTzOIyQ6biWNaqRGb5pBHgjgiwpkA8bJw4JcAfHWe7rm+DAHc9odlqHzLVv7zJLC4zZCqOZa1KZJZPGgHuiADnR9mvCghwv/Ka9tYiU/1LmMziMkOm4ljWqkRm+aQR4A4K8FFHHbXf/vvvfxs17bsa8d2eH3P3KiDA3ctklluETPUvfTKLywyZimNZqxKZ5ZNGgDskwJoGcR8153VaH6LVc30fLgH+8LHHHnvIkiVLNukF/5XnnHOO/11y7xcEuPcRTtUDQKb6FyeZxWWGTMWxrFWJzPJJI8AdEWDJ773VlE9qvULrB7X+diPAbqLu931fkxA/KT/29isgwO1nQAtuIoBM9a83kFlcZshUHMtalcgsnzQC3B0Bfo+acu/99tvvvrt37162c+fOyyWJv+kR4DkB/jN7sK7fPT/29isgwO1nQAsQ4D73AQQ4Lj1kKo5lrUpklk8aAe6OAH9fv/376s2bN7/qmGOOOXjffff97pAA/57uf63uPzA/9vYrIMDtZ0ALEOA+9wEEOC49ZCqOZa1KZJZPGgHuiADrd4CvkxQ+UyO8bxslwLr/2br/Zbp///zY26+AALefAS1AgPvcBxDguPSQqTiWtSqRWT5pBLgjAqw5vpdohPcfNcL7B/OMAJ+v+1fo/vvmx95+BQS4/QxoAQLc5z6AAMelh0zFsaxViczySSPA3RHgl6spfyQxXLlr167/8hQICe9v6FcfPiI59hff3qHrL/IUifzY26+AALefAS1AgPvcBxDguPSQqTiWtSqRWT5pBLg7AuypDRdLcu+mv5+UID5Ulz+mv7fW9Xvr8uevvvrqB1900UXX58fefgUEuP0MaAEC3Oc+gADHpYdMxbGsVYnM8kkjwB0RYDfj8Y9//AH6FYiNksMnSHj9jzAW6fKVunzG9ddff/IFF1xwdX7k3aiAAHcjB1rxEwLIVP96ApnFZYZMxbGsVYnM8kkjwB0S4MGmnHjiibe57rrr9jn//PO/aw/Oj7pbFRDgbuUx661BpvrXA8gsLjNkKo5lrUpklk8aAe6oAOdH2+0KCHC385m11iFT/UuczOIyQ6biWNaqRGb5pBHgjgjw2rVrH6R/gPHL+pmzNzdNWr169XGa/uAvvR2s9R2671n5kXejAgLcjRxoxU8IIFP96wlkFpcZMhXHslYlMssnjQB3RID1O79/JyncKcl9nJt0/PHHr9CvQVyqiz/U+h2th2t9qu7/6/zY26+AALefAS24iQAy1b/eQGZxmSFTcSxrVSKzfNIIcHcE+JuSwrdIcP/cTZIQv0h/XqLbDtVt39JPoV2k67fS5Qfkx95+BQS4/QxoAQLc5z6AAMelh0zFsaxViczySSPAHRFgCe6P1ZSnSXBPd5N0/YP6s1jXHz53/emaDrFRvwO859ch+r4gwH1PcLraj0z1L08yi8sMmYpjWasSmeWTRoA7IsAa8f2OpPDVEt7XrVy5cuny5ct/oKa9Rtc3zgnw7+nvG3T9Fvmxt18BAW4/A1pwEwFkqn+9gcziMkOm4ljWqkRm+aQR4I4IsEZ8/1FNOVj/Ae43d+7cuVaC+EatD9myZcvFbqIE+RX6c6JGgFfkx95+BQS4/QxoAQLc5z6AAMelh0zFsaxViczySSPA3RHgR2qKw99KDPeZa9JnNdr7a03zJMif1eVv6LZj82NvvwIC3H4GtAAB7nMfQIDj0kOm4ljWqkRm+aQR4I4IsJuhnz17iCT4aK1XLl269M1nnXWWp0Es8j/F2LFjx9v0gv+uc8455735sbdfAQFuPwNagAD3uQ8gwHHpIVNxLGtVIrN80ghwhwQ4P87+VECA+5PVLLQUmepfymQWlxkyFceyViUyyyeNACPA+b0ooQICnACNXYoRQKaKoS1WmMzi0CJTcSxrVSKzfNIIcEcEWHN8PzxGnDdoDvBvjLFd5zdBgDsf0Uw1EJnqX9xkFpcZMhXHslYlMssnjQB3RID1Kw/bJIU3DDZHc4GX6qbb6u8++vs93fcjCfCd82NvvwIC3H4GtOAmAshU/3oDmcVlhkzFsaxViczySSPAHRHg+Zqxfv36m/3oRz96niT4SZLGh0qAL8uPvf0KCHD7GdACBLjPfQABjksPmYpjWasSmeWTRoA7LsBN8zRF4mxJ8E79DvC6/Njbr4AAt58BLUCA+9wHEOC49JCpOJa1KpFZPmkEuD8C/DQJ8Mv4V8j5nb50BU7MpQnH1yezeKalK5JZHGFkKo5lrUpklk8aAe6JAGuO8AY19Y8lwD+XH3v7FRgBbj8DWsAIcJ/7AAIclx4yFceyViUyyyeNAHdcgI8++uhb+d8ja/T37WrqFyXAR+bH3n4FBLj9DGgBAtznPoAAx6WHTMWxrFWJzPJJI8AdEWCN8O4e/hWIpmmS38X+FQi94D9S/wnu8/mxz19B7Xiy7n2W1ntovUbH/Yz+Hqsv3/3Ye61du/axuu3PdPHuWr+hy6/Ufe+YtE0I8KTE2L4kAWSqJN0ytcksjisyFceyViUyyyeNAHdEgPUlt9PVlOGfQfP1K7ReKmHcJNG8Jj/y+SuoDSfLtZ+vY71CW31SJ5jb7N692787/Cc+tu5/sC5v1TZ/rfUcbffrun6y/q7R/VsmaRsCPAktti1NAJkqTTi+PpnFMUWm4ljWqkRm+aQR4I4IcH6UeRUkt3eX1P67hPdxW7ZsuWhUNY0O/71u31/TMB7U3K/9ztLl+0iAD5+kBQjwJLTYtjQBZKo04fj6ZBbHFJmKY1mrEpnlk0aAEeA9BCSyfy4BPlZye7dRSI466qj99t9//6t1n0eD3zAgwI/T5QuWLFly57PPPnvbuF0SAR6XFNvVIIBM1aAcewwyi+OJTMWxrFWJzPJJI8AIcCPAntrwfYnpF3TDM7XeStc/oxHh52hE+NMSZI/wfknrURLgDzTYVq1adVedvVTyAwAAIABJREFUiL46fPtCXRMBXogQ99ckgEzVpB1zLDKL4egqyFQcy1qVyCyfNAKMADcCfIku3E7S+7+S0xfp5HKt5PdFuu3eu3btuqt+ieKuuv5x3f4AfRHvUw22E0888TY7duz4rq4/QWLs6RAjl3Xr1h147bXXHtjcuWnTpvNV735XXnllfi/uWAWfmA855JBFl19++SI9xo61juaMIkBm/esXZBaX2Y6THhNXrEOV9j3t/R1qTWxTyCyf50EHHbRo2bJln5D3+PtNLAMEFs8SDc3v/arE965af0kjvv/qx65R34PUMbbptjfoZPP3OQLs3zFWnVMaphs3blzkd1/Lly+fJcw8VghAAAKdI/DNRx/RuTZFNOgOF342okwna5BZWCwI8AiUMyXAkt1PS3YPHf5Pc7r9o7r9e5LXF4vRl+Z+is1fhtuzjDsFghHgsCcrhQoQYDSxANTCJcksDjCjiXEsa1Uis3zSjADPz7CoAEssn6Qvjn1ski+O5cc9fwWN0P6N7n3cKAHW7ddoOXbuS3B/rKkO/6+p5N8F1sjw+/gS3E1smZtYsqeWqU1mZbiWrEpmcXSZTxrHslYlMssnzRzg9gR4lw79xGberIT4p67nRztZhdWrVx+rkd7ztNcvq01f9N7HHHPMwUuXLt2mi3+h217in0HTSPAtdPkhTXXddoZuuy8/g4YAT9bjurU1MtWtPMZpDZmNQ2m8bZCp8Th1aSsyy08DAW5JgCWOV0kcnyNx/Gs3Ye4/wa3b2xfJ8uOev8KGDRv2+dKXvuQvtx2k9WSt/s9vL5QUe17wvdSuy5p/hKHb36bbNuu+I7W+WCPAazVv+NxJ2sevQExCi21LE0CmShOOr09mcUyRqTiWtSqRWT5pBLglAZZMflLyeAvJ40s0feAHEsKt/hfDelH/0N5i1S8wfCw/9tEV5n7R4S9072O1LlP7/klterbk98vNHmq3f/f3xn+FrG1eqWkTnj4x0YIAT4SLjQsTQKYKAy5QnszioCJTcSxrVSKzfNIIcEsCrLmzR0p+PeXglm6CRHKxpPCn/hXyYNOa+yWjS/Jjb78CAtx+BrTgJgLIVP96A5nFZYZMxbGsVYnM8kkjwC0JsA979NFH30q/r3s/XbytBPd0SeGp+nvjb+yOappGW9+ZH3v7FRDg9jOgBQhwn/sAAhyXHjIVx7JWJTLLJ40AtyjAg4duew5wflearAICPBkvti5LAJkqy7dEdTKLo4pMxbGsVYnM8kkjwB0R4Pwo+1UBAe5XXtPeWmSqfwmTWVxmyFQcy1qVyCyfNALcMQHWl8zuqCY9Xuuhc037uv5eoLm/38iPuzsVEODuZEFLFi1CpvrXC8gsLjNkKo5lrUpklk8aAe6QAEt+X6DmbNS6xF96a5omWdzpnxvT/N9X5UfejQoIcDdyoBU/IYBM9a8nkFlcZshUHMtalcgsnzQC3BEBlvyuleRukhj+u5r0Gq3/Nte0e+vvH2u9p+4/QRK8OT/29isgwO1nQAtuIoBM9a83kFlcZshUHMtalcgsnzQC3B0B3vO7wBLD+2u6g/8JxY2L5Pjm/nUI3fcj3ffA/Njbr4AAt58BLUCA+9wHEOC49JCpOJa1KpFZPmkEuDsCfI2a8lIJrkd/f2aRBHsU+BTdv39+7O1XQIDbz4AWIMB97gMIcFx6yFQcy1qVyCyfNALcIQHWKO8GzXB47agm6WfSnidp3IAA53f60hU4MZcmHF+fzOKZlq5IZnGEkak4lrUqkVk+aQS4IwIswfUUh5v93M/93P1PP/306wabddRRR+13wAEH+P7rJMAPyI+9/QqMALefAS1gBLjPfQABjksPmYpjWasSmeWTRoA7IsCa4vAEjQC/W2L4Bf191dyX4Rbpr7/89jw18witT5QAn5Ufe/sVEOD2M6AFCHCf+wACHJceMhXHslYlMssnjQB3RIDdDEmwfwLtRVpv/Am0uebdoL8vl/yekh95NyogwN3IgVb8hAAy1b+eQGZxmSFTcSxrVSKzfNIIcIcEeE6Cf1EjvkdLEO8y17SvL1my5L1nn322/yHG1CwI8NREORUPBJnqX4xkFpcZMhXHslYlMssnjQB3TIDzI+1HBQS4HznNSiuRqf4lTWZxmSFTcSxrVSKzfNIIMAKc34sSKiDACdDYpRgBZKoY2mKFySwOLTIVx7JWJTLLJ40AI8D5vSihAgKcAI1dihFApoqhLVaYzOLQIlNxLGtVIrN80ggwApzfixIqIMAJ0NilGAFkqhjaYoXJLA4tMhXHslYlMssnjQAjwPm9KKECApwAjV2KEUCmiqEtVpjM4tAiU3Esa1Uis3zSCDACnN+LEiogwAnQ2KUYAWSqGNpihcksDi0yFceyViUyyyeNAHdAgPX7vzdXM46TFF66ZcuWT+fH2v0KCHD3M5qlFiJT/UubzOIyQ6biWNaqRGb5pBHgDgjwhg0b9vnSl750nX7/95mbN2/+q/xYu18BAe5+RrPUQmSqf2mTWVxmyFQcy1qVyCyfNALcAQF2E9asWbNNf94sAX5tfqzdr4AAdz+jWWohMtW/tMksLjNkKo5lrUpklk8aAe6IAGsaxKvVlIdpfaD+5fGu/Gi7XQEB7nY+s9Y6ZKp/iZNZXGbIVBzLWpXILJ80AtwRAT7++OPvsXv37jMlhlfphf11O3fu/Jr+XjvcPMnxN/Jjb78CAtx+BrTgJgLIVP96A5nFZYZMxbGsVYnM8kkjwB0RYE2B2C0pvEHzgBf773zNkgAvyY+9/QoIcPsZ0AIEuM99AAGOSw+ZimNZqxKZ5ZNGgLsjwBv2Jr5NMyXAL82Pvf0KCHD7GdACBLjPfQABjksPmYpjWasSmeWTRoA7IsD5UfarAgLcr7ymvbXIVP8SJrO4zJCpOJa1KpFZPmkEGAHO70UJFRDgBGjsUowAMlUMbbHCZBaHFpmKY1mrEpnlk0aAOyTAj3/84w/Yb7/9niU5/C016+e1PklTHj554okn3mbHjh1P15fkNp933nmX5MfefgUEuP0MaMFNBJCp/vUGMovLDJmKY1mrEpnlk0aAOyLAxxxzzMH77rvvx9WcX9T6HxLEu+nvwyXAH3YT9TNp/6k/79H15+bH3n4FBLj9DGgBAtznPoAAx6WHTMWxrFWJzPJJI8AdEWD9CsRb1JQnapT315ctW7ZNP4N2uSTxNwcE+PW6/9d1/T75sbdfAQFuPwNagAD3uQ8gwHHpIVNxLGtVIrN80ghwdwT4m5LCMyW4L5gbDf7uoABLkJ+p66fo/oPzY2+/AgLcfga0AAHucx9AgOPSQ6biWNaqRGb5pBHgjgiwpjhcr6Y8XYJ72igB1v1P0/2v1/03z4+9/QoIcPsZ0AIEuM99AAGOSw+ZimNZqxKZ5ZNGgLsjwN9SU06T4L5kHgF+q+73nOC75sfefgUEuP0MaAEC3Oc+gADHpYdMxbGsVYnM8kkjwN0R4NPVlN/Uek/N/12qL8TdOAVi1apVh+nF/vP6J3F/vXnz5mfmx95+BQS4/QxoAQLc5z6AAMelh0zFsaxViczySSPAHRFgSe5dlixZ8jmJ4ffUpHO0vlDrm+aad5L+/njp0qX32bRp07fzY2+/AgLcfga0AAHucx9AgOPSQ6biWNaqRGb5pBHgjgiwm6F5vvfRKO87dPGXhpr1bxLGdZr+8G/5kXejAgLcjRxoxU8IIFP96wlkFpcZMhXHslYlMssnjQB3SICbpqxevfqeEuF7aN1HovhVie8X86PuVgUEuFt5zHprkKn+9QAyi8sMmYpjWasSmeWTRoA7KMD5sXa/AgLc/YxmqYXIVP/SJrO4zJCpOJa1KpFZPmkEuGMCrGkQd9bI79Fqlv8jnJf/2LVr1wX6F8j+T3BTsyDAUxPlVDwQZKp/MZJZXGbIVBzLWpXILJ80AtwhAZb8bpT8+stvS4aatUvC+CpNhfjT/Mi7UQEB7kYOtOInBJCp/vUEMovLDJmKY1mrEpnlk0aAOyLAkt8/lPy+Uc35Z/075Nfp75fnTsz3lCw+V5eP0PpHkuA358fefgUEuP0MaMFNBJCp/vUGMovLDJmKY1mrEpnlk0aAuyPAl6gpVx100EEPOvXUU3cMNktyvEzXL9a6vwT4sPzY26+AALefAS1AgPvcBxDguPSQqTiWtSqRWT5pBLgjArxmzZrr1JQX6h9d/MWoJkmCn6MR4lfo/pvlx95+BQS4/QxoAQLc5z6AAMelh0zFsaxViczySSPAHRFgCa6/5PY2jfD++TwC/AIJ8O9KgA/Nj739Cghw+xnQAgS4z30AAY5LD5mKY1mrEpnlk0aAuyPA/oLbE7dv337EBRdccPVgsyTHt5T8fkbS+E4J8svzY2+/AgLcfga0AAHucx9AgOPSQ6biWNaqRGb5pBHglgR47dq1Dx08tL74tlSS+yqJ4SG6/S16cf+K79f1w7U+XRe/o/UFEuAP58fefgUEuP0MaAEC3Oc+gADHpYdMxbGsVYnM8kkjwC0JsOb87pYE3jB4eAnw4uZ6c9/wbRLg4Z9Iy+8FLVRAgFuAziHnJYBM9a9zkFlcZshUHMtalcgsnzQC3J4APzklPs0BfmfKfl3bBwHuWiKz3R5kqn/5k1lcZshUHMtalcgsnzQC3JIA50fX7woIcL/zm7bWI1P9S5TM4jJDpuJY1qpEZvmkEWAEOL8XJVRAgBOgsUsxAshUMbTFCpNZHFpkKo5lrUpklk8aAe6YAOsXH35RL+x305fiDlbTbpwT3DRTc4DflR97+xUQ4PYzoAU3EUCm+tcbyCwuM2QqjmWtSmSWTxoB7ogAn3DCCT+/c+fO09WcR7hJg19+a5roL8bxJbj8Tl+6Aifm0oTj65NZPNPSFcksjjAyFceyViUyyyeNAHdEgDXy+x5J72PUnDfr70c1AvyDUU2TAH80P/b2KzAC3H4GtIAR4D73AQQ4Lj1kKo5lrUpklk8aAe6OAF8j8X27fuXh2fmxdr8CAtz9jGaphchU/9Ims7jMkKk4lrUqkVk+aQS4IwKs3wX+nqTwZI3wnpofa/crIMDdz2iWWohM9S9tMovLDJmKY1mrEpnlk0aAuyPAm9SU7RoBTvp94PyuULcCAlyXN0fbOwFkqn89hMziMkOm4ljWqkRm+aQR4I4IsOYA305N+bjWN2t9k0aCt+fH290KCHB3s5nFliFT/UudzOIyQ6biWNaqRGb5pBHgjgiwmyEJPl5/ztRcYP+b5G/r8q7B5un2GzRCfGh+7O1XQIDbz4AW3EQAmepfbyCzuMyQqTiWtSqRWT5pBLgjAiz5faKacrpWj/xeKtkd+SsQEuAj82NvvwIC3H4GtAAB7nMfQIDj0kOm4ljWqkRm+aQR4O4I8KVqyo937dr1iPPPP//y/Gi7XQEB7nY+s9Y6ZKp/iZNZXGbIVBzLWpXILJ80AtwdAf6xRn2fpxHet+TH2v0KCHD3M5qlFiJT/UubzOIyQ6biWNaqRGb5pBHgjgiwfgbtS5LCM/Tlt1fmx9r9Cghw9zOapRYiU/1Lm8ziMkOm4ljWqkRm+aQR4I4IsOYA/55GgJ+/bNmyXz7jjDOuyo82r4Las78qXKL1dpLV+23ZsuWzTUXdd5Lbqut31Hqp/mvdybr//ZMcEQGehBbbliaATJUmHF+fzOKYIlNxLGtVIrN80ghwdwT4SWrKH2i9vdbTtP6X1p/6FQg3VSPE78qPfeEKGpF+lSTVv0n884MC7F+qkPyepdtfrr8f1n1rddlC/JBzzjnnUwtX/skWCPC4pNiuBgFkqgbl2GOQWRxPZCqOZa1KZJZPGgHuiABLOHcvFKek8QYJ8JKFtsu9f9WqVYfp5OIR3+dq/ashAfaX9T6ndpzYHEdSfLEE+ErNX37UuMdGgMclxXY1CCBTNSjHHoPM4ngiU3Esa1Uis3zSCHBHBFgS+bBx4pR4fnSc7XK2UVv+QUL7L5ra8H79/UgjwBLju+ik83Wtx2i0973NMSTvz9Q2r7nmmmsOvOiii64f59gI8DiU2KYWAWSqFum445BZHEtkKo5lrUpklk8aAe6IAOdHGVNB8rtald6833773e26666776AAr1279lGS4gu13uO8887z/OA9i/Z5uP58cPj2vbUIAY7JiyoxBJCpGI41q5BZHG1kKo5lrUpklk8aAUaAbyTw2Mc+9hY3u9nNLpH0btB0hr9ZvXr1ykEBlug+QRufofW2Gom+rNlR2x2h7T4jqX2Qvgx38Sik69atO/Daa689sLlv06ZN50uY73fllVfm9+KOVfCJ+ZBDDll0+eWXL9Jj7FjraM4oAmTWv35BZnGZ7TjpMXHFOlRp39Mm+m52h1q+cFPIbGFGC21x0EEHLdIPD3xC/vLghbadtfsX13zAksuXLHS8uX+F/LKFtku9X1MZXqF9Hy75/VX9vSFSgFV7gwT5lKZtGzduXOR3X8uXL09tLvtBAAIQgEAAgW8++oiAKt0rcYcLb/zxou41LrNFZJYJ8KbdEeARKKsK8N6+BOcvv0l+F5f8Epzm995JIypf9fze66+/fs8o7tKlSx+sw/6tjnuk/n5W9z3UUyB012EaAfaX4fYs40yBYAQ47MlKoQIEGE0sALVwSTKLA8xoYhzLWpXILJ80I8DzM6wqwBbQ4absu+++S3fu3HmoXuj9awz7698kr9fc26/lx/6zFZrR3vlqS4A/reOf6C/BSYiP1lSHCwYE+Bm6/FqtB0iMt4/TPuYAj0OJbWoRYD5pLdJxxyGzOJbMJ41jWasSmeWTZg5wRwR4gSgXz/3U2Ic0PeHF+bH/bIWjjz76Vhrxvc/gPZJeX/8Lrb+vk81n9MsPn1c7LvV8X7Vj3YAAf1y3XcXPoP2ECCfmEj20bE0yK8u3RHUyi6OKTMWxrFWJzPJJI8D9EOBFmiLxbI2aPlsjrP7va1WW4TnAPqjacYL+nKm2vEzrRyS+a7U+RZcfqrZ9ctyGMQI8Lim2q0EAmapBOfYYZBbHE5mKY1mrEpnlk0aAeyLAGnl9lkTzzzXKerP82MerMEqAvaf/FbL+vEDrnn+FLJl9Ef8K+SamnJjH619d2orMupTGeG0hs/E4jbMVMjUOpW5tQ2b5eSDAPRDgY4899rZLlizxaOtOCfC98mNvvwIjwO1nQAt409LnPoAAx6WHTMWxrFWJzPJJI8AdEWCNqn54nqYcJPE9TPctkzSeqGkGZ+fH3n4FBLj9DGgBAlyiD3BiLkG1bE0yK8u3RHUyy6eKAHdEgDW3dpt/5myoOb5+hVZPM3ijphl8Oj/yblRAgLuRA634CQFGE+N6AifmOJa1KpFZLdJxxyGzfJYIcEcEOD/KflVAgPuV17S3FgGOS5gTcxzLWpXIrBbpuOOQWT5LBBgBzu9FCRUQ4ARo7FKMAAIch5YTcxzLWpXIrBbpuOOQWT5LBBgBzu9FCRUQ4ARo7FKMAAIch5YTcxzLWpXIrBbpuOOQWT5LBLhFAdYX3/5zkgj935D1KxCHTrJPV7dFgLuazGy2CwGOy50TcxzLWpXIrBbpuOOQWT5LBLhdAf4PHX74i2+jWnRzye//8Zfk9CsQS/Jjb78CAtx+BrTgJgIIcFxv4MQcx7JWJTKrRTruOGSWzxIBblGAx4jP/wJ5veR3o7a9ndYvagT4vmPs1/lNEODORzRTDUSA4+LmxBzHslYlMqtFOu44ZJbPEgHuqACvXbv2tySJr9bqf3zxLa1/qtHfd485YpzfMwpXQIALA6b8RAQQ4Ilw7XVjTsxxLGtVIrNapOOOQ2b5LBHgjgmwRnzvoya9WutvaL1ao7+vvPrqq99w0UUXXZ8fd3cqIMDdyYKW8DvAkX2AE3MkzTq1yKwO58ijkFk+TQS4IwJ8/PHH32HXrl0vV3NO1LpL61/u3LnzZe95z3u+nx9z9yogwN3LZJZbxAhwXPqcmONY1qpEZrVIxx2HzPJZIsAtC/C6desO3L59+8kSwmdotPdm/p7b7t27X3jeeedN9AsR+V2hbgUEuC5vjrZ3AghwXA/hxBzHslYlMqtFOu44ZJbPEgFuUYA13eFZOvzJWg+S/H5C63PPOeecz+TH2v0KCHD3M5qlFiLAcWlzYo5jWasSmdUiHXccMstniQC3KMBr1qzZ7Z82k/haet+3UJxzP4P2yoW268P9CHAfUpqdNiLAcVlzYo5jWasSmdUiHXccMstniQC3LMCTRMjvAE9Cq71tkan22KcemcxSyf3sfpyY41jWqkRmtUjHHYfM8lkiwC0KsKZAPGzSCPVTaB+ddJ8ubs8IcBdTmd02IcBx2XNijmNZqxKZ1SIddxwyy2eJALcowPnx9bcCAtzf7Kax5QhwXKqcmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4vSqiAACdAY5diBBDgOLScmONY1qpEZrVIxx2HzPJZIsAIcH4v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\" width=\"639.9999861283738\">"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "<matplotlib.axes._subplots.AxesSubplot at 0x7f073c40a760>"
+                            "<matplotlib.text.Text at 0x7f27f7410208>"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# How different are the predictions from both algorithms ?\n",
-                "# Let's count the number of predictions for each rating value\n",
+                "from collections import Counter\n",
                 "\n",
                 "import matplotlib.pyplot as plt\n",
                 "import matplotlib\n",
                 "%matplotlib notebook\n",
                 "matplotlib.style.use('ggplot')\n",
                 "\n",
-                "figure, (ax1, ax2) = plt.subplots(1, 2)\n",
-                "\n",
-                "df_svd.est.plot(kind='hist', title='SVD', ax=ax1)\n",
-                "df_knn.est.plot(kind='hist', title='KNN', ax=ax2)\n",
-                "\n",
-                "# As expected, one of the drawbacks of the NN algorithms is that their predictions are often\n",
-                "#\u00a0quite concentrated around the mean. The SVD algorithm seems more confortable predicting extreme rating values."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 17,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "(nan, nan)"
-                        ]
-                    },
-                    "execution_count": 17,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "# Question: when a user has rated only a small number of items (less than 10), which algorithm\n",
-                "# gives the best predictions on average?\n",
-                "\n",
-                "def get_Iu(uid):\n",
-                "    \"\"\"Return the number of items rated by given user\n",
-                "    \n",
-                "    Args:\n",
-                "        uid: The raw id of the user.\n",
-                "    Returns:\n",
-                "        The number of items rated by the user.\n",
-                "    \"\"\"\n",
-                "    \n",
-                "    try:\n",
-                "        return len(trainset.ur[trainset.to_inner_uid(uid)])\n",
-                "    except ValueError:  # user was not part of the trainset\n",
-                "        return 0\n",
-                "    \n",
-                "df_knn['Iu'] = df_knn.uid.apply(get_Iu)\n",
-                "df_svd['Iu'] = df_svd.uid.apply(get_Iu)\n",
-                "\n",
-                "df_knn[df_knn.Iu < 10].err.mean(), df_svd[df_svd.Iu < 10].err.mean()"
+                "counter = Counter([r for (_, r) in trainset.ir[trainset.to_inner_iid('302')]])\n",
+                "pd.DataFrame.from_dict(counter, orient='index').plot(kind='bar', legend=False)\n",
+                "plt.xlabel('Rating value')\n",
+                "plt.ylabel('Number of users')\n",
+                "plt.title('Number of users having rated item 302')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "collapsed": true
+            },
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
@@ -1494,13 +1468,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.2"
+            "version": "3.5.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `scikit_surprise-1.1.4/examples/notebooks/KNNBasic_analysis.ipynb` & `scikit-surprise-1.1rc0/examples/notebooks/Compare.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9516326096035094%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#\\xa0Comparison of two algorithms\\n'), (2, 'We will "*

 * *            'see in this notebook how we can compare the prediction accuracy of two '*

 * *            "algorithms.')], delete: [2, 0]}}, 1: {'metadata': {replace: "*

 * *            "OrderedDict([('collapsed', True)])}, 'source': {insert: [(7, 'from surprise import "*

 * *            "SVD\\n')], delete: [10]}}, 2: {'outputs': {0: {'text': {insert: [(2, 'RMSE: "*

 * *            "0.9500\\n')]}}}, 'source': {insert: [(11, '        […]*

```diff
@@ -1,35 +1,37 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Analysis of the KNNBasic algorithm\n",
+                "#\u00a0Comparison of two algorithms\n",
                 "\n",
-                "In this notebook, we will run a basic neighborhood algorithm on the movielens dataset, dump the results, and use pandas to make some data analysis."
+                "We will see in this notebook how we can compare the prediction accuracy of two algorithms."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "metadata": {},
+            "metadata": {
+                "collapsed": true
+            },
             "outputs": [],
             "source": [
                 "from __future__ import (absolute_import, division, print_function,             \n",
                 "                        unicode_literals)                                      \n",
                 "import pickle\n",
                 "import os\n",
                 "\n",
                 "import pandas as pd\n",
                 "\n",
+                "from surprise import SVD\n",
                 "from surprise import KNNBasic\n",
                 "from surprise import Dataset                                                     \n",
                 "from surprise import Reader                                                      \n",
-                "from surprise.model_selection import PredefinedKFold\n",
                 "from surprise import dump\n",
                 "from surprise.accuracy import rmse"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
@@ -37,14 +39,15 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Computing the msd similarity matrix...\n",
                         "Done computing similarity matrix.\n",
+                        "RMSE: 0.9500\n",
                         "RMSE: 0.9889\n"
                     ]
                 }
             ],
             "source": [
                 "#\u00a0We will train and test on the u1.base and u1.test files of the movielens-100k dataset.\n",
                 "# if you haven't already, you need to download the movielens-100k dataset\n",
@@ -53,627 +56,488 @@
                 "#Dataset.load_builtin('ml-100k')\n",
                 "\n",
                 "# Now, let's load the dataset\n",
                 "train_file = os.path.expanduser('~') + '/.surprise_data/ml-100k/ml-100k/u1.base'\n",
                 "test_file = os.path.expanduser('~') + '/.surprise_data/ml-100k/ml-100k/u1.test'\n",
                 "data = Dataset.load_from_folds([(train_file, test_file)], Reader('ml-100k'))\n",
                 "\n",
-                "pkf = PredefinedKFold()\n",
+                "                \n",
+                "#\u00a0We'll use the well-known SVD algorithm and a basic nearest neighbors approach.\n",
+                "algo_svd = SVD()                                                       \n",
+                "algo_knn = KNNBasic()\n",
                 "\n",
-                "#\u00a0We'll use a basic nearest neighbor approach, where similarities are computed\n",
-                "# between users.\n",
-                "algo = KNNBasic()                                                       \n",
-                "\n",
-                "for trainset, testset in pkf.split(data):\n",
-                "    algo.fit(trainset)                             \n",
-                "    predictions = algo.test(testset)\n",
-                "    rmse(predictions)\n",
-                "                                                                               \n",
-                "    dump.dump('./dump_file', predictions, algo)"
+                "for trainset, testset in data.folds(): \n",
+                "    algo_svd.fit(trainset)                             \n",
+                "    predictions_svd = algo_svd.test(testset)\n",
+                "    \n",
+                "    algo_knn.fit(trainset)\n",
+                "    predictions_knn = algo_knn.test(testset)\n",
+                "    \n",
+                "    rmse(predictions_svd)\n",
+                "    rmse(predictions_knn)                                                                           \n",
+                "    \n",
+                "    dump.dump('./dump_SVD', predictions_svd, algo_svd)\n",
+                "    dump.dump('./dump_KNN', predictions_knn, algo_knn)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# The dump has been saved and we can now use it whenever we want.\n",
-                "# Let's load it and see what we can do\n",
-                "predictions, algo = dump.load('./dump_file')"
+                "# The dumps have been saved and we can now use them whenever we want.\n",
+                "\n",
+                "predictions_svd, algo_svd = dump.load('./dump_SVD')\n",
+                "predictions_knn, algo_knn = dump.load('./dump_KNN')\n",
+                "\n",
+                "df_svd = pd.DataFrame(predictions_svd, columns=['uid', 'iid', 'rui', 'est', 'details'])    \n",
+                "df_knn = pd.DataFrame(predictions_knn, columns=['uid', 'iid', 'rui', 'est', 'details'])    \n",
+                "\n",
+                "df_svd['err'] = abs(df_svd.est - df_svd.rui)\n",
+                "df_knn['err'] = abs(df_knn.est - df_knn.rui)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 4,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "algo: KNNBasic, k = 40, min_k = 1\n"
-                    ]
-                }
-            ],
             "source": [
-                "trainset = algo.trainset\n",
-                "print('algo: {0}, k = {1}, min_k = {2}'.format(algo.__class__.__name__, algo.k, algo.min_k))"
+                "We now have two dataframes with the all the predictions for each algorithm. The cool thing is that, as both algorithm have been tested on the same testset, the indexes of the two dataframes are the same!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>uid</th>\n",
+                            "      <th>iid</th>\n",
+                            "      <th>rui</th>\n",
+                            "      <th>est</th>\n",
+                            "      <th>details</th>\n",
+                            "      <th>err</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>1</td>\n",
+                            "      <td>6</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>3.300098</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>1.699902</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>1</td>\n",
+                            "      <td>10</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>3.673812</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>0.673812</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>1</td>\n",
+                            "      <td>12</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>4.746471</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>0.253529</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>1</td>\n",
+                            "      <td>14</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>4.031972</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>0.968028</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>1</td>\n",
+                            "      <td>17</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>2.744526</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>0.255474</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "  uid iid  rui       est                    details       err\n",
+                            "0   1   6  5.0  3.300098  {'was_impossible': False}  1.699902\n",
+                            "1   1  10  3.0  3.673812  {'was_impossible': False}  0.673812\n",
+                            "2   1  12  5.0  4.746471  {'was_impossible': False}  0.253529\n",
+                            "3   1  14  5.0  4.031972  {'was_impossible': False}  0.968028\n",
+                            "4   1  17  3.0  2.744526  {'was_impossible': False}  0.255474"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "# Let's build a pandas dataframe with all the predictions\n",
-                "\n",
-                "def get_Iu(uid):\n",
-                "    \"\"\"Return the number of items rated by given user\n",
-                "    \n",
-                "    Args:\n",
-                "        uid: The raw id of the user.\n",
-                "    Returns:\n",
-                "        The number of items rated by the user.\n",
-                "    \"\"\"\n",
-                "    \n",
-                "    try:\n",
-                "        return len(trainset.ur[trainset.to_inner_uid(uid)])\n",
-                "    except ValueError:  # user was not part of the trainset\n",
-                "        return 0\n",
-                "    \n",
-                "def get_Ui(iid):\n",
-                "    \"\"\"Return the number of users that have rated given item\n",
-                "    \n",
-                "    Args:\n",
-                "        iid: The raw id of the item.\n",
-                "    Returns:\n",
-                "        The number of users that have rated the item.\n",
-                "    \"\"\"\n",
-                "    \n",
-                "    try:\n",
-                "        return len(trainset.ir[trainset.to_inner_iid(iid)])\n",
-                "    except ValueError:  # item was not part of the trainset\n",
-                "        return 0\n",
-                "\n",
-                "df = pd.DataFrame(predictions, columns=['uid', 'iid', 'rui', 'est', 'details'])    \n",
-                "df['Iu'] = df.uid.apply(get_Iu)\n",
-                "df['Ui'] = df.iid.apply(get_Ui)\n",
-                "df['err'] = abs(df.est - df.rui)"
+                "df_svd.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>uid</th>\n",
                             "      <th>iid</th>\n",
                             "      <th>rui</th>\n",
                             "      <th>est</th>\n",
                             "      <th>details</th>\n",
-                            "      <th>Iu</th>\n",
-                            "      <th>Ui</th>\n",
                             "      <th>err</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1</td>\n",
                             "      <td>6</td>\n",
                             "      <td>5.0</td>\n",
                             "      <td>3.468613</td>\n",
-                            "      <td>{'actual_k': 20, 'was_impossible': False}</td>\n",
-                            "      <td>135</td>\n",
-                            "      <td>20</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 20}</td>\n",
                             "      <td>1.531387</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>1</td>\n",
                             "      <td>10</td>\n",
                             "      <td>3.0</td>\n",
                             "      <td>3.866290</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>135</td>\n",
-                            "      <td>73</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
                             "      <td>0.866290</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>1</td>\n",
                             "      <td>12</td>\n",
                             "      <td>5.0</td>\n",
                             "      <td>4.538194</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>135</td>\n",
-                            "      <td>211</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
                             "      <td>0.461806</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>1</td>\n",
                             "      <td>14</td>\n",
                             "      <td>5.0</td>\n",
                             "      <td>4.235741</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>135</td>\n",
-                            "      <td>140</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
                             "      <td>0.764259</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>1</td>\n",
                             "      <td>17</td>\n",
                             "      <td>3.0</td>\n",
                             "      <td>3.228002</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>135</td>\n",
-                            "      <td>72</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
                             "      <td>0.228002</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  uid iid  rui       est                                    details   Iu   Ui  \\\n",
-                            "0   1   6  5.0  3.468613  {'actual_k': 20, 'was_impossible': False}  135   20   \n",
-                            "1   1  10  3.0  3.866290  {'actual_k': 40, 'was_impossible': False}  135   73   \n",
-                            "2   1  12  5.0  4.538194  {'actual_k': 40, 'was_impossible': False}  135  211   \n",
-                            "3   1  14  5.0  4.235741  {'actual_k': 40, 'was_impossible': False}  135  140   \n",
-                            "4   1  17  3.0  3.228002  {'actual_k': 40, 'was_impossible': False}  135   72   \n",
-                            "\n",
-                            "        err  \n",
-                            "0  1.531387  \n",
-                            "1  0.866290  \n",
-                            "2  0.461806  \n",
-                            "3  0.764259  \n",
-                            "4  0.228002  "
+                            "  uid iid  rui       est                                    details       err\n",
+                            "0   1   6  5.0  3.468613  {'was_impossible': False, 'actual_k': 20}  1.531387\n",
+                            "1   1  10  3.0  3.866290  {'was_impossible': False, 'actual_k': 40}  0.866290\n",
+                            "2   1  12  5.0  4.538194  {'was_impossible': False, 'actual_k': 40}  0.461806\n",
+                            "3   1  14  5.0  4.235741  {'was_impossible': False, 'actual_k': 40}  0.764259\n",
+                            "4   1  17  3.0  3.228002  {'was_impossible': False, 'actual_k': 40}  0.228002"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df.head()"
+                "df_knn.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
-            "outputs": [],
-            "source": [
-                "best_predictions = df.sort_values(by='err')[:10]\n",
-                "worst_predictions = df.sort_values(by='err')[-10:]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>uid</th>\n",
                             "      <th>iid</th>\n",
                             "      <th>rui</th>\n",
                             "      <th>est</th>\n",
                             "      <th>details</th>\n",
-                            "      <th>Iu</th>\n",
-                            "      <th>Ui</th>\n",
                             "      <th>err</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>272</th>\n",
-                            "      <td>5</td>\n",
-                            "      <td>439</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <th>4198</th>\n",
+                            "      <td>89</td>\n",
+                            "      <td>221</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>{'actual_k': 3, 'was_impossible': False}</td>\n",
-                            "      <td>91</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>3.766186</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
+                            "      <td>2.766186</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>886</th>\n",
-                            "      <td>13</td>\n",
-                            "      <td>314</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <th>7385</th>\n",
+                            "      <td>167</td>\n",
+                            "      <td>48</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>{'actual_k': 2, 'was_impossible': False}</td>\n",
-                            "      <td>373</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>4.259556</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
+                            "      <td>3.259556</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>156</th>\n",
-                            "      <td>2</td>\n",
-                            "      <td>314</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <th>7390</th>\n",
+                            "      <td>167</td>\n",
+                            "      <td>169</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>{'actual_k': 2, 'was_impossible': False}</td>\n",
-                            "      <td>40</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>4.664991</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
+                            "      <td>3.664991</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>926</th>\n",
-                            "      <td>13</td>\n",
-                            "      <td>437</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <th>13972</th>\n",
+                            "      <td>295</td>\n",
+                            "      <td>183</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>{'actual_k': 3, 'was_impossible': False}</td>\n",
-                            "      <td>373</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>4.202611</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
+                            "      <td>3.202611</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>9276</th>\n",
-                            "      <td>206</td>\n",
-                            "      <td>314</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <th>15306</th>\n",
+                            "      <td>312</td>\n",
+                            "      <td>265</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
-                            "      <td>33</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>4.131875</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 40}</td>\n",
+                            "      <td>3.131875</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>19118</th>\n",
+                            "      <th>19140</th>\n",
                             "      <td>405</td>\n",
-                            "      <td>437</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>{'actual_k': 3, 'was_impossible': False}</td>\n",
-                            "      <td>582</td>\n",
-                            "      <td>3</td>\n",
-                            "      <td>0.0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>8032</th>\n",
-                            "      <td>181</td>\n",
-                            "      <td>1334</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
-                            "      <td>218</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0.0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>8041</th>\n",
-                            "      <td>181</td>\n",
-                            "      <td>1354</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
-                            "      <td>218</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0.0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9202</th>\n",
-                            "      <td>201</td>\n",
-                            "      <td>1424</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
-                            "      <td>215</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0.0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3018</th>\n",
-                            "      <td>60</td>\n",
-                            "      <td>1123</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
-                            "      <td>119</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>575</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>2.410506</td>\n",
+                            "      <td>{'was_impossible': False, 'actual_k': 36}</td>\n",
+                            "      <td>2.589494</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "       uid   iid  rui  est                                   details   Iu  Ui  \\\n",
-                            "272      5   439  1.0  1.0  {'actual_k': 3, 'was_impossible': False}   91   3   \n",
-                            "886     13   314  1.0  1.0  {'actual_k': 2, 'was_impossible': False}  373   2   \n",
-                            "156      2   314  1.0  1.0  {'actual_k': 2, 'was_impossible': False}   40   2   \n",
-                            "926     13   437  1.0  1.0  {'actual_k': 3, 'was_impossible': False}  373   3   \n",
-                            "9276   206   314  1.0  1.0  {'actual_k': 1, 'was_impossible': False}   33   2   \n",
-                            "19118  405   437  1.0  1.0  {'actual_k': 3, 'was_impossible': False}  582   3   \n",
-                            "8032   181  1334  1.0  1.0  {'actual_k': 1, 'was_impossible': False}  218   1   \n",
-                            "8041   181  1354  1.0  1.0  {'actual_k': 1, 'was_impossible': False}  218   1   \n",
-                            "9202   201  1424  3.0  3.0  {'actual_k': 1, 'was_impossible': False}  215   1   \n",
-                            "3018    60  1123  4.0  4.0  {'actual_k': 1, 'was_impossible': False}  119   1   \n",
-                            "\n",
-                            "       err  \n",
-                            "272    0.0  \n",
-                            "886    0.0  \n",
-                            "156    0.0  \n",
-                            "926    0.0  \n",
-                            "9276   0.0  \n",
-                            "19118  0.0  \n",
-                            "8032   0.0  \n",
-                            "8041   0.0  \n",
-                            "9202   0.0  \n",
-                            "3018   0.0  "
+                            "       uid  iid  rui       est                                    details  \\\n",
+                            "4198    89  221  1.0  3.766186  {'was_impossible': False, 'actual_k': 40}   \n",
+                            "7385   167   48  1.0  4.259556  {'was_impossible': False, 'actual_k': 40}   \n",
+                            "7390   167  169  1.0  4.664991  {'was_impossible': False, 'actual_k': 40}   \n",
+                            "13972  295  183  1.0  4.202611  {'was_impossible': False, 'actual_k': 40}   \n",
+                            "15306  312  265  1.0  4.131875  {'was_impossible': False, 'actual_k': 40}   \n",
+                            "19140  405  575  5.0  2.410506  {'was_impossible': False, 'actual_k': 36}   \n",
+                            "\n",
+                            "            err  \n",
+                            "4198   2.766186  \n",
+                            "7385   3.259556  \n",
+                            "7390   3.664991  \n",
+                            "13972  3.202611  \n",
+                            "15306  3.131875  \n",
+                            "19140  2.589494  "
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# Let's take a look at the best predictions of the algorithm\n",
-                "best_predictions"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "It's interesting to note that these perfect predictions are actually lucky shots: $|U_i|$ is always very small, meaning that very few users have rated the target item. This implies that the set of neighbors is very small (see the ``actual_k`` field)... And, it just happens that all the ratings from the neighbors are the same (and mostly, are equal to that of the target user).\n",
-                "\n",
-                "This may be a bit surprising but these lucky shots are actually very important to the accuracy of the algorithm... Try running the same algorithm with a value of ``min_k`` equal to $10$. This means that if there are less than $10$ neighbors, the prediction is set to the mean of all ratings. You'll see your accuracy decrease!"
+                "# Let's check how good are the KNN predictions when the SVD has a huge error:\n",
+                "df_knn[df_svd.err >= 3.5]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>uid</th>\n",
                             "      <th>iid</th>\n",
                             "      <th>rui</th>\n",
                             "      <th>est</th>\n",
                             "      <th>details</th>\n",
-                            "      <th>Iu</th>\n",
-                            "      <th>Ui</th>\n",
                             "      <th>err</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>9406</th>\n",
                             "      <td>208</td>\n",
                             "      <td>302</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.308447</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>11</td>\n",
-                            "      <td>245</td>\n",
-                            "      <td>3.308447</td>\n",
+                            "      <td>4.326863</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>3.326863</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>19089</th>\n",
                             "      <td>405</td>\n",
                             "      <td>169</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.364728</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>582</td>\n",
-                            "      <td>97</td>\n",
-                            "      <td>3.364728</td>\n",
+                            "      <td>3.039247</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>2.039247</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>19785</th>\n",
                             "      <td>436</td>\n",
                             "      <td>132</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.365369</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>126</td>\n",
-                            "      <td>200</td>\n",
-                            "      <td>3.365369</td>\n",
+                            "      <td>4.243595</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>3.243595</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>157</th>\n",
                             "      <td>2</td>\n",
                             "      <td>315</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.381308</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>40</td>\n",
-                            "      <td>136</td>\n",
-                            "      <td>3.381308</td>\n",
+                            "      <td>4.260016</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>3.260016</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8503</th>\n",
                             "      <td>193</td>\n",
                             "      <td>56</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.386478</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>61</td>\n",
-                            "      <td>312</td>\n",
-                            "      <td>3.386478</td>\n",
+                            "      <td>4.129742</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>3.129742</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5531</th>\n",
                             "      <td>113</td>\n",
                             "      <td>976</td>\n",
                             "      <td>5.0</td>\n",
-                            "      <td>1.610771</td>\n",
-                            "      <td>{'actual_k': 7, 'was_impossible': False}</td>\n",
-                            "      <td>31</td>\n",
-                            "      <td>7</td>\n",
-                            "      <td>3.389229</td>\n",
+                            "      <td>3.320028</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>1.679972</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7917</th>\n",
                             "      <td>181</td>\n",
                             "      <td>408</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.421499</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>218</td>\n",
-                            "      <td>93</td>\n",
-                            "      <td>3.421499</td>\n",
+                            "      <td>2.962557</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>1.962557</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7390</th>\n",
                             "      <td>167</td>\n",
                             "      <td>169</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>4.664991</td>\n",
-                            "      <td>{'actual_k': 40, 'was_impossible': False}</td>\n",
-                            "      <td>38</td>\n",
-                            "      <td>97</td>\n",
-                            "      <td>3.664991</td>\n",
+                            "      <td>4.720954</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>3.720954</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7412</th>\n",
                             "      <td>167</td>\n",
                             "      <td>1306</td>\n",
                             "      <td>5.0</td>\n",
-                            "      <td>1.000000</td>\n",
-                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
-                            "      <td>38</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>4.000000</td>\n",
+                            "      <td>3.350088</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>1.649912</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5553</th>\n",
                             "      <td>114</td>\n",
                             "      <td>1104</td>\n",
                             "      <td>5.0</td>\n",
-                            "      <td>1.000000</td>\n",
-                            "      <td>{'actual_k': 1, 'was_impossible': False}</td>\n",
-                            "      <td>27</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>4.000000</td>\n",
+                            "      <td>3.070772</td>\n",
+                            "      <td>{'was_impossible': False}</td>\n",
+                            "      <td>1.929228</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "       uid   iid  rui       est                                    details  \\\n",
-                            "9406   208   302  1.0  4.308447  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "19089  405   169  1.0  4.364728  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "19785  436   132  1.0  4.365369  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "157      2   315  1.0  4.381308  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "8503   193    56  1.0  4.386478  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "5531   113   976  5.0  1.610771   {'actual_k': 7, 'was_impossible': False}   \n",
-                            "7917   181   408  1.0  4.421499  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "7390   167   169  1.0  4.664991  {'actual_k': 40, 'was_impossible': False}   \n",
-                            "7412   167  1306  5.0  1.000000   {'actual_k': 1, 'was_impossible': False}   \n",
-                            "5553   114  1104  5.0  1.000000   {'actual_k': 1, 'was_impossible': False}   \n",
-                            "\n",
-                            "        Iu   Ui       err  \n",
-                            "9406    11  245  3.308447  \n",
-                            "19089  582   97  3.364728  \n",
-                            "19785  126  200  3.365369  \n",
-                            "157     40  136  3.381308  \n",
-                            "8503    61  312  3.386478  \n",
-                            "5531    31    7  3.389229  \n",
-                            "7917   218   93  3.421499  \n",
-                            "7390    38   97  3.664991  \n",
-                            "7412    38    1  4.000000  \n",
-                            "5553    27    1  4.000000  "
+                            "       uid   iid  rui       est                    details       err\n",
+                            "9406   208   302  1.0  4.326863  {'was_impossible': False}  3.326863\n",
+                            "19089  405   169  1.0  3.039247  {'was_impossible': False}  2.039247\n",
+                            "19785  436   132  1.0  4.243595  {'was_impossible': False}  3.243595\n",
+                            "157      2   315  1.0  4.260016  {'was_impossible': False}  3.260016\n",
+                            "8503   193    56  1.0  4.129742  {'was_impossible': False}  3.129742\n",
+                            "5531   113   976  5.0  3.320028  {'was_impossible': False}  1.679972\n",
+                            "7917   181   408  1.0  2.962557  {'was_impossible': False}  1.962557\n",
+                            "7390   167   169  1.0  4.720954  {'was_impossible': False}  3.720954\n",
+                            "7412   167  1306  5.0  3.350088  {'was_impossible': False}  1.649912\n",
+                            "5553   114  1104  5.0  3.070772  {'was_impossible': False}  1.929228"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# Now, let's look at the prediction with the biggest error\n",
-                "worst_predictions"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Let's focus first on the last two predictions. Well, we can't do much about them. We should have predicted $5$, but the only available neighbor had a rating of $1$, so we were screwed. The only way to avoid this kind of errors would be to increase the ``min_k`` parameter, but it would actually worsen the accuracy (see note above).\n",
-                "\n",
-                "How about the other ones? It seems that for each prediction, the users are some kind of outsiders: they rated their item with a rating of $1$ when the most of the ratings for the item where high (or inversely, rated a *bad* item with a rating of $5$). See the plot below as an illustration for the first rating.\n",
-                "\n",
-                "These are situations where baseline estimates would be quite helpful, in order to deal with highly biased users (and items)."
+                "# Well... Not much better.\n",
+                "# Now, let's look at the predictions of SVD on the 10 worst predictions for KNN\n",
+                "df_svd.iloc[df_knn.sort_values(by='err')[-10:].index]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/javascript": [
                             "/* Put everything inside the global mpl namespace */\n",
                             "window.mpl = {};\n",
@@ -681,15 +545,15 @@
                             "\n",
                             "mpl.get_websocket_type = function() {\n",
                             "    if (typeof(WebSocket) !== 'undefined') {\n",
                             "        return WebSocket;\n",
                             "    } else if (typeof(MozWebSocket) !== 'undefined') {\n",
                             "        return MozWebSocket;\n",
                             "    } else {\n",
-                            "        alert('Your browser does not have WebSocket support. ' +\n",
+                            "        alert('Your browser does not have WebSocket support.' +\n",
                             "              'Please try Chrome, Safari or Firefox \u2265 6. ' +\n",
                             "              'Firefox 4 and 5 are also supported but you ' +\n",
                             "              'have to enable WebSockets in about:config.');\n",
                             "    };\n",
                             "}\n",
                             "\n",
                             "mpl.figure = function(figure_id, websocket, ondownload, parent_element) {\n",
@@ -750,15 +614,15 @@
                             "                // there is no ghosting.\n",
                             "                fig.context.clearRect(0, 0, fig.canvas.width, fig.canvas.height);\n",
                             "            }\n",
                             "            fig.context.drawImage(fig.imageObj, 0, 0);\n",
                             "        };\n",
                             "\n",
                             "    this.imageObj.onunload = function() {\n",
-                            "        fig.ws.close();\n",
+                            "        this.ws.close();\n",
                             "    }\n",
                             "\n",
                             "    this.ws.onmessage = this._make_on_message_function(this);\n",
                             "\n",
                             "    this.ondownload = ondownload;\n",
                             "}\n",
                             "\n",
@@ -898,15 +762,15 @@
                             "\n",
                             "    window.setTimeout(set_focus, 100);\n",
                             "}\n",
                             "\n",
                             "mpl.figure.prototype._init_toolbar = function() {\n",
                             "    var fig = this;\n",
                             "\n",
-                            "    var nav_element = $('<div/>');\n",
+                            "    var nav_element = $('<div/>')\n",
                             "    nav_element.attr('style', 'width: 100%');\n",
                             "    this.root.append(nav_element);\n",
                             "\n",
                             "    // Define a callback function for later on.\n",
                             "    function toolbar_event(event) {\n",
                             "        return fig.toolbar_button_onclick(event['data']);\n",
                             "    }\n",
@@ -955,15 +819,15 @@
                             "    nav_element.append(fmt_picker_span);\n",
                             "    this.format_dropdown = fmt_picker[0];\n",
                             "\n",
                             "    for (var ind in mpl.extensions) {\n",
                             "        var fmt = mpl.extensions[ind];\n",
                             "        var option = $(\n",
                             "            '<option/>', {selected: fmt === mpl.default_extension}).html(fmt);\n",
-                            "        fmt_picker.append(option);\n",
+                            "        fmt_picker.append(option)\n",
                             "    }\n",
                             "\n",
                             "    // Add hover states to the ui-buttons\n",
                             "    $( \".ui-button\" ).hover(\n",
                             "        function() { $(this).addClass(\"ui-state-hover\");},\n",
                             "        function() { $(this).removeClass(\"ui-state-hover\");}\n",
                             "    );\n",
@@ -1019,15 +883,15 @@
                             "    y1 = Math.floor(y1) + 0.5;\n",
                             "    var min_x = Math.min(x0, x1);\n",
                             "    var min_y = Math.min(y0, y1);\n",
                             "    var width = Math.abs(x1 - x0);\n",
                             "    var height = Math.abs(y1 - y0);\n",
                             "\n",
                             "    fig.rubberband_context.clearRect(\n",
-                            "        0, 0, fig.canvas.width / mpl.ratio, fig.canvas.height / mpl.ratio);\n",
+                            "        0, 0, fig.canvas.width, fig.canvas.height);\n",
                             "\n",
                             "    fig.rubberband_context.strokeRect(min_x, min_y, width, height);\n",
                             "}\n",
                             "\n",
                             "mpl.figure.prototype.handle_figure_label = function(fig, msg) {\n",
                             "    // Updates the figure title.\n",
                             "    fig.header.textContent = msg['label'];\n",
@@ -1120,17 +984,17 @@
                             "            } catch (e) {\n",
                             "                console.log(\"Exception inside the 'handler_\" + msg_type + \"' callback:\", e, e.stack, msg);\n",
                             "            }\n",
                             "        }\n",
                             "    };\n",
                             "}\n",
                             "\n",
-                            "// from https://stackoverflow.com/questions/1114465/getting-mouse-location-in-canvas\n",
+                            "// from http://stackoverflow.com/questions/1114465/getting-mouse-location-in-canvas\n",
                             "mpl.findpos = function(e) {\n",
-                            "    //this section is from https://www.quirksmode.org/js/events_properties.html\n",
+                            "    //this section is from http://www.quirksmode.org/js/events_properties.html\n",
                             "    var targ;\n",
                             "    if (!e)\n",
                             "        e = window.event;\n",
                             "    if (e.target)\n",
                             "        targ = e.target;\n",
                             "    else if (e.srcElement)\n",
                             "        targ = e.srcElement;\n",
@@ -1145,15 +1009,15 @@
                             "\n",
                             "    return {\"x\": x, \"y\": y};\n",
                             "};\n",
                             "\n",
                             "/*\n",
                             " * return a copy of an object with only non-object keys\n",
                             " * we need this to avoid circular references\n",
-                            " * https://stackoverflow.com/a/24161582/3208463\n",
+                            " * http://stackoverflow.com/a/24161582/3208463\n",
                             " */\n",
                             "function simpleKeys (original) {\n",
                             "  return Object.keys(original).reduce(function (obj, key) {\n",
                             "    if (typeof original[key] !== 'object')\n",
                             "        obj[key] = original[key]\n",
                             "    return obj;\n",
                             "  }, {});\n",
@@ -1225,17 +1089,17 @@
                             "        this.send_message(\"toolbar_button\", {name: name});\n",
                             "    }\n",
                             "};\n",
                             "\n",
                             "mpl.figure.prototype.toolbar_button_onmouseover = function(tooltip) {\n",
                             "    this.message.textContent = tooltip;\n",
                             "};\n",
-                            "mpl.toolbar_items = [[\"Home\", \"Reset original view\", \"fa fa-home icon-home\", \"home\"], [\"Back\", \"Back to previous view\", \"fa fa-arrow-left icon-arrow-left\", \"back\"], [\"Forward\", \"Forward to next view\", \"fa fa-arrow-right icon-arrow-right\", \"forward\"], [\"\", \"\", \"\", \"\"], [\"Pan\", \"Pan axes with left mouse, zoom with right\", \"fa fa-arrows icon-move\", \"pan\"], [\"Zoom\", \"Zoom to rectangle\", \"fa fa-square-o icon-check-empty\", \"zoom\"], [\"\", \"\", \"\", \"\"], [\"Download\", \"Download plot\", \"fa fa-floppy-o icon-save\", \"download\"]];\n",
+                            "mpl.toolbar_items = [[\"Home\", \"Reset original view\", \"fa fa-home icon-home\", \"home\"], [\"Back\", \"Back to  previous view\", \"fa fa-arrow-left icon-arrow-left\", \"back\"], [\"Forward\", \"Forward to next view\", \"fa fa-arrow-right icon-arrow-right\", \"forward\"], [\"\", \"\", \"\", \"\"], [\"Pan\", \"Pan axes with left mouse, zoom with right\", \"fa fa-arrows icon-move\", \"pan\"], [\"Zoom\", \"Zoom to rectangle\", \"fa fa-square-o icon-check-empty\", \"zoom\"], [\"\", \"\", \"\", \"\"], [\"Download\", \"Download plot\", \"fa fa-floppy-o icon-save\", \"download\"]];\n",
                             "\n",
-                            "mpl.extensions = [\"eps\", \"jpeg\", \"pdf\", \"png\", \"ps\", \"raw\", \"svg\", \"tif\"];\n",
+                            "mpl.extensions = [\"eps\", \"pdf\", \"png\", \"ps\", \"raw\", \"svg\"];\n",
                             "\n",
                             "mpl.default_extension = \"png\";var comm_websocket_adapter = function(comm) {\n",
                             "    // Create a \"websocket\"-like object which calls the given IPython comm\n",
                             "    // object with the appropriate methods. Currently this is a non binary\n",
                             "    // socket, so there is still some room for performance tuning.\n",
                             "    var ws = {};\n",
                             "\n",
@@ -1245,15 +1109,15 @@
                             "    ws.send = function(m) {\n",
                             "        //console.log('sending', m);\n",
                             "        comm.send(m);\n",
                             "    };\n",
                             "    // Register the callback with on_msg.\n",
                             "    comm.on_msg(function(msg) {\n",
                             "        //console.log('receiving', msg['content']['data'], msg);\n",
-                            "        // Pass the mpl event to the overridden (by mpl) onmessage function.\n",
+                            "        // Pass the mpl event to the overriden (by mpl) onmessage function.\n",
                             "        ws.onmessage(msg['content']['data'])\n",
                             "    });\n",
                             "    return ws;\n",
                             "}\n",
                             "\n",
                             "mpl.mpl_figure_comm = function(comm, msg) {\n",
                             "    // This is the function which gets called when the mpl process\n",
@@ -1324,15 +1188,15 @@
                             "    // that it is saved nicely (might be nice to debounce this).\n",
                             "    setTimeout(function () { fig.push_to_output() }, 1000);\n",
                             "}\n",
                             "\n",
                             "mpl.figure.prototype._init_toolbar = function() {\n",
                             "    var fig = this;\n",
                             "\n",
-                            "    var nav_element = $('<div/>');\n",
+                            "    var nav_element = $('<div/>')\n",
                             "    nav_element.attr('style', 'width: 100%');\n",
                             "    this.root.append(nav_element);\n",
                             "\n",
                             "    // Define a callback function for later on.\n",
                             "    function toolbar_event(event) {\n",
                             "        return fig.toolbar_button_onclick(event['data']);\n",
                             "    }\n",
@@ -1448,55 +1312,91 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<img src=\"data:image/png;base64,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\" width=\"640\">"
+                            "<img src=\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAsAAAAIQCAYAAACPEdjAAAAgAElEQVR4XuydCbgUxdm2m+WAUSEKghiExCWgYIiJuOCuCWCIJuzngJDfhJiIioli1IiJBJUobjEqilvyRWU/J5rIB4I/ki+AKxrXiNEvxJUcgqIgsnjgf975Z87pGWbOdM3U21Pd/cx11TU9PdW1PPXWW/fUVFe38PiiAlSAClABKkAFqAAVoAIJUqBFgurKqlIBKkAFqAAVoAJUgApQAY8ATCOgAlSAClABKkAFqAAVSJQCBOBENTcrSwWoABWgAlSAClABKkAApg1QASpABagAFaACVIAKJEoBAnCimpuVpQJUgApQASpABagAFSAA0waoABWgAlSAClABKkAFEqUAAThRzc3KUgEqQAWoABWgAlSAChCAaQNUgApQASpABagAFaACiVKAAJyo5mZlqQAVoAJUgApQASpABQjAtAEqQAWoABWgAlSAClCBRClAAE5Uc7OyVIAKUAEqQAWoABWgAgRg2gAVoAJUgApQASpABahAohQgACequVlZKkAFqAAVoAJUgApQAQIwbYAKUAEqQAWoABWgAlQgUQoQgBPV3KwsFaACVIAKUAEqQAWoAAGYNkAFqAAVoAJUgApQASqQKAUIwIlqblaWClABKkAFqAAVoAJUgABMG6ACVIAKUAEqQAWoABVIlAIE4EQ1NytLBagAFaACVIAKUAEqQACmDVABKkAFqAAVoAJUgAokSgECcKKam5WlAlSAClABKkAFqAAVIADTBqgAFaACVIAKUAEqQAUSpQABOFHNzcpSASpABagAFaACVIAKEIBpA1SAClABKkAFqAAVoAKJUoAAnKjmZmWpABWgAlSAClABKkAFCMC0ASpABagAFaACVIAKUIFEKUAATlRzs7JUgApQASpABagAFaACBGDaABWgAlSAClABKkAFqECiFCAAJ6q5WVkqQAWoABWgAlSAClABAjBtgApQASpABagAFaACVCBRChCAE9XcrCwVoAJUgApQASpABagAAZg2QAWoABWgAlSAClABKpAoBQjAiWpuVpYKUAEqQAWoABWgAlSAAEwboAJUgApQASpABagAFUiUAgTgRDU3K0sFqAAVoAJUgApQASpAAKYNUAEqQAWoABWgAlSACiRKAQJwopqblaUCVIAKUAEqQAWoABUgANMG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\" width=\"639.9999861283738\">"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "Text(0.5, 1.0, 'Number of users having rated item 302')"
+                            "<matplotlib.axes._subplots.AxesSubplot at 0x7ff756a46ef0>"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from collections import Counter\n",
+                "# How different are the predictions from both algorithms ?\n",
+                "# Let's count the number of predictions for each rating value\n",
                 "\n",
                 "import matplotlib.pyplot as plt\n",
                 "import matplotlib\n",
                 "%matplotlib notebook\n",
                 "matplotlib.style.use('ggplot')\n",
                 "\n",
-                "counter = Counter([r for (_, r) in trainset.ir[trainset.to_inner_iid('302')]])\n",
-                "pd.DataFrame.from_dict(counter, orient='index').plot(kind='bar', legend=False)\n",
-                "plt.xlabel('Rating value')\n",
-                "plt.ylabel('Number of users')\n",
-                "plt.title('Number of users having rated item 302')"
+                "figure, (ax1, ax2) = plt.subplots(1, 2)\n",
+                "\n",
+                "df_svd.est.plot(kind='hist', title='SVD', ax=ax1)\n",
+                "df_knn.est.plot(kind='hist', title='KNN', ax=ax2)\n",
+                "\n",
+                "# As expected, one of the drawbacks of the NN algorithms is that their predictions are often\n",
+                "#\u00a0quite concentrated around the mean. The SVD algorithm seems more confortable predicting extreme rating values."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 11,
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "(1.0382962702232326, 1.0130235152149263)"
+                        ]
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Question: when a user has rated only a small number of items (less than 10), which algorithm\n",
+                "# gives the best predictions on average?\n",
+                "\n",
+                "def get_Iu(uid):\n",
+                "    \"\"\"Return the number of items rated by given user\n",
+                "    \n",
+                "    Args:\n",
+                "        uid: The raw id of the user.\n",
+                "    Returns:\n",
+                "        The number of items rated by the user.\n",
+                "    \"\"\"\n",
+                "    \n",
+                "    try:\n",
+                "        return len(trainset.ur[trainset.to_inner_uid(uid)])\n",
+                "    except ValueError:  # user was not part of the trainset\n",
+                "        return 0\n",
+                "    \n",
+                "df_knn['Iu'] = df_knn.uid.apply(get_Iu)\n",
+                "df_svd['Iu'] = df_svd.uid.apply(get_Iu)\n",
+                "\n",
+                "df_knn[df_knn.Iu < 10].err.mean(), df_svd[df_svd.Iu < 10].err.mean()"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
@@ -1507,13 +1407,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.2"
+            "version": "3.5.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `scikit_surprise-1.1.4/examples/precision_recall_at_k.py` & `scikit-surprise-1.1rc0/examples/precision_recall_at_k.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 This module illustrates how to compute Precision at k and Recall at k metrics.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 from collections import defaultdict
 
-from surprise import Dataset, SVD
+from surprise import Dataset
+from surprise import SVD
 from surprise.model_selection import KFold
 
 
 def precision_recall_at_k(predictions, k=10, threshold=3.5):
-    """Return precision and recall at k metrics for each user"""
+    '''Return precision and recall at k metrics for each user.'''
 
     # First map the predictions to each user.
     user_est_true = defaultdict(list)
     for uid, _, true_r, est, _ in predictions:
         user_est_true[uid].append((est, true_r))
 
     precisions = dict()
@@ -26,33 +29,27 @@
         # Number of relevant items
         n_rel = sum((true_r >= threshold) for (_, true_r) in user_ratings)
 
         # Number of recommended items in top k
         n_rec_k = sum((est >= threshold) for (est, _) in user_ratings[:k])
 
         # Number of relevant and recommended items in top k
-        n_rel_and_rec_k = sum(
-            ((true_r >= threshold) and (est >= threshold))
-            for (est, true_r) in user_ratings[:k]
-        )
+        n_rel_and_rec_k = sum(((true_r >= threshold) and (est >= threshold))
+                              for (est, true_r) in user_ratings[:k])
 
         # Precision@K: Proportion of recommended items that are relevant
-        # When n_rec_k is 0, Precision is undefined. We here set it to 0.
-
-        precisions[uid] = n_rel_and_rec_k / n_rec_k if n_rec_k != 0 else 0
+        precisions[uid] = n_rel_and_rec_k / n_rec_k if n_rec_k != 0 else 1
 
         # Recall@K: Proportion of relevant items that are recommended
-        # When n_rel is 0, Recall is undefined. We here set it to 0.
-
-        recalls[uid] = n_rel_and_rec_k / n_rel if n_rel != 0 else 0
+        recalls[uid] = n_rel_and_rec_k / n_rel if n_rel != 0 else 1
 
     return precisions, recalls
 
 
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 kf = KFold(n_splits=5)
 algo = SVD()
 
 for trainset, testset in kf.split(data):
     algo.fit(trainset)
     predictions = algo.test(testset)
     precisions, recalls = precision_recall_at_k(predictions, k=5, threshold=4)
```

### Comparing `scikit_surprise-1.1.4/examples/predict_ratings.py` & `scikit-surprise-1.1rc0/examples/predict_ratings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 This module descibes how to train on a full dataset (when no testset is
 built/specified) and how to use the predict() method.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
-from surprise import Dataset, KNNBasic
+from surprise import KNNBasic
+from surprise import Dataset
 
 # Load the movielens-100k dataset
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 
 # Retrieve the trainset.
 trainset = data.build_full_trainset()
 
 # Build an algorithm, and train it.
 algo = KNNBasic()
 algo.fit(trainset)
```

### Comparing `scikit_surprise-1.1.4/examples/run_all_examples.py` & `scikit-surprise-1.1rc0/examples/run_all_examples.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """Run all the examples (except for benchmark.py). Just used as some kind of
 functional test... If no warning / errors is output, it should be fine.
 """
 
-# flake8: noqa
-
-import os
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 import sys
+import os
 import warnings
 
 # redirect stout to /dev/null to avoid printing
-sys.stdout = open(os.devnull, "w")
+sys.stdout = open(os.devnull, 'w')
 
+from building_custom_algorithms import mean_rating_user_item
+from building_custom_algorithms import most_basic_algorithm2
+from building_custom_algorithms import most_basic_algorithm
+from building_custom_algorithms import with_baselines_or_sim
+import load_custom_dataset_predefined_folds
+import load_from_dataframe
 import baselines_conf
-import basic_usage
-import evaluate_on_trainset
 import generate_grid_search_cv_results_example
-import grid_search_usage
-import k_nearest_neighbors
-import load_custom_dataset
-import load_custom_dataset_predefined_folds
 import load_from_dataframe
-import precision_recall_at_k
-import predict_ratings
+import train_test_split
+import basic_usage
+import grid_search_usage
 import serialize_algorithm
+import use_cross_validation_iterators
+import k_nearest_neighbors
 import similarity_conf
+import precision_recall_at_k
 import split_data_for_unbiased_estimation
+import evaluate_on_trainset
+import load_custom_dataset
+import predict_ratings
 import top_n_recommendations
-import train_test_split
-import use_cross_validation_iterators
-from building_custom_algorithms import (
-    mean_rating_user_item,
-    most_basic_algorithm,
-    most_basic_algorithm2,
-    with_baselines_or_sim,
-)
```

### Comparing `scikit_surprise-1.1.4/examples/serialize_algorithm.py` & `scikit-surprise-1.1rc0/examples/serialize_algorithm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 This module illustrates the use of the dump and load methods for serializing an
 algorithm. The SVD algorithm is trained on a dataset and then serialized. It is
 then reloaded and can be used again for making predictions.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 import os
 
-from surprise import Dataset, dump, SVD
+from surprise import SVD
+from surprise import Dataset
+from surprise import dump
 
 
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 trainset = data.build_full_trainset()
 
 algo = SVD()
 algo.fit(trainset)
 
 # Compute predictions of the 'original' algorithm.
 predictions = algo.test(trainset.build_testset())
 
 # Dump algorithm and reload it.
-file_name = os.path.expanduser("~/dump_file")
+file_name = os.path.expanduser('~/dump_file')
 dump.dump(file_name, algo=algo)
 _, loaded_algo = dump.load(file_name)
 
 # We now ensure that the algo is still the same by checking the predictions.
 predictions_loaded_algo = loaded_algo.test(trainset.build_testset())
 assert predictions == predictions_loaded_algo
-print("Predictions are the same")
+print('Predictions are the same')
```

### Comparing `scikit_surprise-1.1.4/examples/split_data_for_unbiased_estimation.py` & `scikit-surprise-1.1rc0/examples/split_data_for_unbiased_estimation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 """
 This module descibes how to split a dataset into two parts A and B: A is for
 tuning the algorithm parameters, and B is for having an unbiased estimation of
 its performances. The tuning is done by Grid Search.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 import random
 
-from surprise import accuracy, Dataset, SVD
+from surprise import SVD
+from surprise import Dataset
+from surprise import accuracy
 from surprise.model_selection import GridSearchCV
 
 
 # Load the full dataset.
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 raw_ratings = data.raw_ratings
 
 # shuffle ratings if you want
 random.shuffle(raw_ratings)
 
 # A = 90% of the data, B = 10% of the data
-threshold = int(0.9 * len(raw_ratings))
+threshold = int(.9 * len(raw_ratings))
 A_raw_ratings = raw_ratings[:threshold]
 B_raw_ratings = raw_ratings[threshold:]
 
 data.raw_ratings = A_raw_ratings  # data is now the set A
 
 # Select your best algo with grid search.
-print("Grid Search...")
-param_grid = {"n_epochs": [5, 10], "lr_all": [0.002, 0.005]}
-grid_search = GridSearchCV(SVD, param_grid, measures=["rmse"], cv=3)
+print('Grid Search...')
+param_grid = {'n_epochs': [5, 10], 'lr_all': [0.002, 0.005]}
+grid_search = GridSearchCV(SVD, param_grid, measures=['rmse'], cv=3)
 grid_search.fit(data)
 
-algo = grid_search.best_estimator["rmse"]
+algo = grid_search.best_estimator['rmse']
 
 # retrain on the whole set A
 trainset = data.build_full_trainset()
 algo.fit(trainset)
 
 # Compute biased accuracy on A
 predictions = algo.test(trainset.build_testset())
-print("Biased accuracy on A,", end="   ")
+print('Biased accuracy on A,', end='   ')
 accuracy.rmse(predictions)
 
 # Compute unbiased accuracy on B
 testset = data.construct_testset(B_raw_ratings)  # testset is now the set B
 predictions = algo.test(testset)
-print("Unbiased accuracy on B,", end=" ")
+print('Unbiased accuracy on B,', end=' ')
 accuracy.rmse(predictions)
```

### Comparing `scikit_surprise-1.1.4/examples/top_n_recommendations.py` & `scikit-surprise-1.1rc0/examples/top_n_recommendations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """
 This module illustrates how to retrieve the top-10 items with highest rating
 prediction. We first train an SVD algorithm on the MovieLens dataset, and then
 predict all the ratings for the pairs (user, item) that are not in the training
 set. We then retrieve the top-10 prediction for each user.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 from collections import defaultdict
 
-from surprise import Dataset, SVD
+from surprise import SVD
+from surprise import Dataset
 
 
 def get_top_n(predictions, n=10):
-    """Return the top-N recommendation for each user from a set of predictions.
+    '''Return the top-N recommendation for each user from a set of predictions.
 
     Args:
         predictions(list of Prediction objects): The list of predictions, as
             returned by the test method of an algorithm.
         n(int): The number of recommendation to output for each user. Default
             is 10.
 
     Returns:
     A dict where keys are user (raw) ids and values are lists of tuples:
         [(raw item id, rating estimation), ...] of size n.
-    """
+    '''
 
     # First map the predictions to each user.
     top_n = defaultdict(list)
     for uid, iid, true_r, est, _ in predictions:
         top_n[uid].append((iid, est))
 
     # Then sort the predictions for each user and retrieve the k highest ones.
@@ -34,15 +37,15 @@
         user_ratings.sort(key=lambda x: x[1], reverse=True)
         top_n[uid] = user_ratings[:n]
 
     return top_n
 
 
 # First train an SVD algorithm on the movielens dataset.
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 trainset = data.build_full_trainset()
 algo = SVD()
 algo.fit(trainset)
 
 # Than predict ratings for all pairs (u, i) that are NOT in the training set.
 testset = trainset.build_anti_testset()
 predictions = algo.test(testset)
```

### Comparing `scikit_surprise-1.1.4/examples/use_cross_validation_iterators.py` & `scikit-surprise-1.1rc0/examples/use_cross_validation_iterators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 This module descibes how to use cross-validation iterators.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
-from surprise import accuracy, Dataset, SVD
+from surprise import SVD
+from surprise import Dataset
+from surprise import accuracy
 from surprise.model_selection import KFold
 
 # Load the movielens-100k dataset
-data = Dataset.load_builtin("ml-100k")
+data = Dataset.load_builtin('ml-100k')
 
 # define a cross-validation iterator
 kf = KFold(n_splits=3)
 
 algo = SVD()
 
 for trainset, testset in kf.split(data):
```

### Comparing `scikit_surprise-1.1.4/surprise/accuracy.py` & `scikit-surprise-1.1rc0/surprise/accuracy.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 
     rmse
     mse
     mae
     fcp
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 from collections import defaultdict
-
 import numpy as np
+from six import iteritems
 
 
 def rmse(predictions, verbose=True):
     """Compute RMSE (Root Mean Squared Error).
 
     .. math::
-        \\text{RMSE} = \\sqrt{\\frac{1}{|\\hat{R}|} \\sum_{\\hat{r}_{ui} \\in
+        \\text{RMSE} = \\sqrt{\\frac{1}{|\\hat{R}|} \\sum_{\\hat{r}_{ui} \in
         \\hat{R}}(r_{ui} - \\hat{r}_{ui})^2}.
 
     Args:
         predictions (:obj:`list` of :obj:`Prediction\
             <surprise.prediction_algorithms.predictions.Prediction>`):
             A list of predictions, as returned by the :meth:`test()
             <surprise.prediction_algorithms.algo_base.AlgoBase.test>` method.
@@ -37,32 +39,31 @@
         The Root Mean Squared Error of predictions.
 
     Raises:
         ValueError: When ``predictions`` is empty.
     """
 
     if not predictions:
-        raise ValueError("Prediction list is empty.")
+        raise ValueError('Prediction list is empty.')
 
-    mse = np.mean(
-        [float((true_r - est) ** 2) for (_, _, true_r, est, _) in predictions]
-    )
+    mse = np.mean([float((true_r - est)**2)
+                   for (_, _, true_r, est, _) in predictions])
     rmse_ = np.sqrt(mse)
 
     if verbose:
-        print(f"RMSE: {rmse_:1.4f}")
+        print('RMSE: {0:1.4f}'.format(rmse_))
 
     return rmse_
 
 
 def mse(predictions, verbose=True):
     """Compute MSE (Mean Squared Error).
 
     .. math::
-        \\text{MSE} = \\frac{1}{|\\hat{R}|} \\sum_{\\hat{r}_{ui} \\in
+        \\text{RMSE} = \\frac{1}{|\\hat{R}|} \\sum_{\\hat{r}_{ui} \in
         \\hat{R}}(r_{ui} - \\hat{r}_{ui})^2.
 
     Args:
         predictions (:obj:`list` of :obj:`Prediction\
             <surprise.prediction_algorithms.predictions.Prediction>`):
             A list of predictions, as returned by the :meth:`test()
             <surprise.prediction_algorithms.algo_base.AlgoBase.test>` method.
@@ -73,31 +74,30 @@
         The Mean Squared Error of predictions.
 
     Raises:
         ValueError: When ``predictions`` is empty.
     """
 
     if not predictions:
-        raise ValueError("Prediction list is empty.")
+        raise ValueError('Prediction list is empty.')
 
-    mse_ = np.mean(
-        [float((true_r - est) ** 2) for (_, _, true_r, est, _) in predictions]
-    )
+    mse_ = np.mean([float((true_r - est)**2)
+                    for (_, _, true_r, est, _) in predictions])
 
     if verbose:
-        print(f"MSE: {mse_:1.4f}")
+        print('MSE: {0:1.4f}'.format(mse_))
 
     return mse_
 
 
 def mae(predictions, verbose=True):
     """Compute MAE (Mean Absolute Error).
 
     .. math::
-        \\text{MAE} = \\frac{1}{|\\hat{R}|} \\sum_{\\hat{r}_{ui} \\in
+        \\text{MAE} = \\frac{1}{|\\hat{R}|} \\sum_{\\hat{r}_{ui} \in
         \\hat{R}}|r_{ui} - \\hat{r}_{ui}|
 
     Args:
         predictions (:obj:`list` of :obj:`Prediction\
             <surprise.prediction_algorithms.predictions.Prediction>`):
             A list of predictions, as returned by the :meth:`test()
             <surprise.prediction_algorithms.algo_base.AlgoBase.test>` method.
@@ -108,29 +108,30 @@
         The Mean Absolute Error of predictions.
 
     Raises:
         ValueError: When ``predictions`` is empty.
     """
 
     if not predictions:
-        raise ValueError("Prediction list is empty.")
+        raise ValueError('Prediction list is empty.')
 
-    mae_ = np.mean([float(abs(true_r - est)) for (_, _, true_r, est, _) in predictions])
+    mae_ = np.mean([float(abs(true_r - est))
+                    for (_, _, true_r, est, _) in predictions])
 
     if verbose:
-        print(f"MAE:  {mae_:1.4f}")
+        print('MAE:  {0:1.4f}'.format(mae_))
 
     return mae_
 
 
 def fcp(predictions, verbose=True):
     """Compute FCP (Fraction of Concordant Pairs).
 
     Computed as described in paper `Collaborative Filtering on Ordinal User
-    Feedback <https://www.ijcai.org/Proceedings/13/Papers/449.pdf>`_ by Koren
+    Feedback <http://www.ijcai.org/Proceedings/13/Papers/449.pdf>`_ by Koren
     and Sill, section 5.2.
 
     Args:
         predictions (:obj:`list` of :obj:`Prediction\
             <surprise.prediction_algorithms.predictions.Prediction>`):
             A list of predictions, as returned by the :meth:`test()
             <surprise.prediction_algorithms.algo_base.AlgoBase.test>` method.
@@ -141,39 +142,37 @@
         The Fraction of Concordant Pairs.
 
     Raises:
         ValueError: When ``predictions`` is empty.
     """
 
     if not predictions:
-        raise ValueError("Prediction list is empty.")
+        raise ValueError('Prediction list is empty.')
 
     predictions_u = defaultdict(list)
     nc_u = defaultdict(int)
     nd_u = defaultdict(int)
 
     for u0, _, r0, est, _ in predictions:
         predictions_u[u0].append((r0, est))
 
-    for u0, preds in predictions_u.items():
+    for u0, preds in iteritems(predictions_u):
         for r0i, esti in preds:
             for r0j, estj in preds:
                 if esti > estj and r0i > r0j:
                     nc_u[u0] += 1
                 if esti >= estj and r0i < r0j:
                     nd_u[u0] += 1
 
     nc = np.mean(list(nc_u.values())) if nc_u else 0
     nd = np.mean(list(nd_u.values())) if nd_u else 0
 
     try:
         fcp = nc / (nc + nd)
     except ZeroDivisionError:
-        raise ValueError(
-            "cannot compute fcp on this list of prediction. "
-            + "Does every user have at least two predictions?"
-        )
+        raise ValueError('cannot compute fcp on this list of prediction. ' +
+                         'Does every user have at least two predictions?')
 
     if verbose:
-        print(f"FCP:  {fcp:1.4f}")
+        print('FCP:  {0:1.4f}'.format(fcp))
 
     return fcp
```

### Comparing `scikit_surprise-1.1.4/surprise/builtin_datasets.py` & `scikit-surprise-1.1rc0/surprise/builtin_datasets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-"""This module contains built-in datasets that can be automatically
-downloaded."""
+'''This module contains built-in datasets that can be automatically
+downloaded.'''
 
-import errno
-import os
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+
+from six.moves.urllib.request import urlretrieve
 import zipfile
 from collections import namedtuple
-
+import os
 from os.path import join
-from urllib.request import urlretrieve
 
 
 def get_dataset_dir():
-    """Return folder where downloaded datasets and other data are stored.
+    '''Return folder where downloaded datasets and other data are stored.
     Default folder is ~/.surprise_data/, but it can also be set by the
     environment variable ``SURPRISE_DATA_FOLDER``.
-    """
+    '''
 
-    folder = os.environ.get(
-        "SURPRISE_DATA_FOLDER", os.path.expanduser("~") + "/.surprise_data/"
-    )
-    try:
+    folder = os.environ.get('SURPRISE_DATA_FOLDER', os.path.expanduser('~') +
+                            '/.surprise_data/')
+    if not os.path.exists(folder):
         os.makedirs(folder)
-    except OSError as e:
-        if e.errno != errno.EEXIST:
-            # reraise exception if folder does not exist and creation failed.
-            raise
 
     return folder
 
 
 # a builtin dataset has
 # - an url (where to download it)
 # - a path (where it is located on the filesystem)
 # - the parameters of the corresponding reader
-BuiltinDataset = namedtuple("BuiltinDataset", ["url", "path", "reader_params"])
+BuiltinDataset = namedtuple('BuiltinDataset', ['url', 'path', 'reader_params'])
 
 BUILTIN_DATASETS = {
-    "ml-100k": BuiltinDataset(
-        url="https://files.grouplens.org/datasets/movielens/ml-100k.zip",
-        path=join(get_dataset_dir(), "ml-100k/ml-100k/u.data"),
-        reader_params=dict(
-            line_format="user item rating timestamp", rating_scale=(1, 5), sep="\t"
+    'ml-100k':
+        BuiltinDataset(
+            url='http://files.grouplens.org/datasets/movielens/ml-100k.zip',
+            path=join(get_dataset_dir(), 'ml-100k/ml-100k/u.data'),
+            reader_params=dict(line_format='user item rating timestamp',
+                               rating_scale=(1, 5),
+                               sep='\t')
         ),
-    ),
-    "ml-1m": BuiltinDataset(
-        url="https://files.grouplens.org/datasets/movielens/ml-1m.zip",
-        path=join(get_dataset_dir(), "ml-1m/ml-1m/ratings.dat"),
-        reader_params=dict(
-            line_format="user item rating timestamp", rating_scale=(1, 5), sep="::"
+    'ml-1m':
+        BuiltinDataset(
+            url='http://files.grouplens.org/datasets/movielens/ml-1m.zip',
+            path=join(get_dataset_dir(), 'ml-1m/ml-1m/ratings.dat'),
+            reader_params=dict(line_format='user item rating timestamp',
+                               rating_scale=(1, 5),
+                               sep='::')
         ),
-    ),
-    "jester": BuiltinDataset(
-        url="https://eigentaste.berkeley.edu/dataset/archive/jester_dataset_2.zip",
-        path=join(get_dataset_dir(), "jester/jester_ratings.dat"),
-        reader_params=dict(line_format="user item rating", rating_scale=(-10, 10)),
-    ),
+    'jester':
+        BuiltinDataset(
+            url='http://eigentaste.berkeley.edu/dataset/jester_dataset_2.zip',
+            path=join(get_dataset_dir(), 'jester/jester_ratings.dat'),
+            reader_params=dict(line_format='user item rating',
+                               rating_scale=(-10, 10))
+        )
 }
 
 
 def download_builtin_dataset(name):
 
     dataset = BUILTIN_DATASETS[name]
 
-    print("Trying to download dataset from " + dataset.url + "...")
-    tmp_file_path = join(get_dataset_dir(), "tmp.zip")
+    print('Trying to download dataset from ' + dataset.url + '...')
+    tmp_file_path = join(get_dataset_dir(), 'tmp.zip')
     urlretrieve(dataset.url, tmp_file_path)
 
-    with zipfile.ZipFile(tmp_file_path, "r") as tmp_zip:
+    with zipfile.ZipFile(tmp_file_path, 'r') as tmp_zip:
         tmp_zip.extractall(join(get_dataset_dir(), name))
 
     os.remove(tmp_file_path)
-    print("Done! Dataset", name, "has been saved to", join(get_dataset_dir(), name))
+    print('Done! Dataset', name, 'has been saved to',
+          join(get_dataset_dir(), name))
```

### Comparing `scikit_surprise-1.1.4/surprise/dataset.py` & `scikit-surprise-1.1rc0/surprise/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,39 +2,43 @@
 The :mod:`dataset <surprise.dataset>` module defines the :class:`Dataset` class
 and other subclasses which are used for managing datasets.
 
 Users may use both *built-in* and user-defined datasets (see the
 :ref:`getting_started` page for examples). Right now, three built-in datasets
 are available:
 
-* The `movielens-100k <https://grouplens.org/datasets/movielens/>`_ dataset.
-* The `movielens-1m <https://grouplens.org/datasets/movielens/>`_ dataset.
-* The `Jester <https://eigentaste.berkeley.edu/dataset/>`_ dataset 2.
+* The `movielens-100k <http://grouplens.org/datasets/movielens/>`_ dataset.
+* The `movielens-1m <http://grouplens.org/datasets/movielens/>`_ dataset.
+* The `Jester <http://eigentaste.berkeley.edu/dataset/>`_ dataset 2.
 
 Built-in datasets can all be loaded (or downloaded if you haven't already)
 using the :meth:`Dataset.load_builtin` method.
 Summary:
 
 .. autosummary::
     :nosignatures:
 
     Dataset.load_builtin
     Dataset.load_from_file
     Dataset.load_from_folds
 """
 
 
-import itertools
-import os
-import sys
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 from collections import defaultdict
+import sys
+import os
+import itertools
 
-from .builtin_datasets import BUILTIN_DATASETS, download_builtin_dataset
+from six.moves import input
 
 from .reader import Reader
+from .builtin_datasets import download_builtin_dataset
+from .builtin_datasets import BUILTIN_DATASETS
 from .trainset import Trainset
 
 
 class Dataset:
     """Base class for loading datasets.
 
     Note that you should never instantiate the :class:`Dataset` class directly
@@ -42,15 +46,15 @@
     available methods for loading datasets."""
 
     def __init__(self, reader):
 
         self.reader = reader
 
     @classmethod
-    def load_builtin(cls, name="ml-100k", prompt=True):
+    def load_builtin(cls, name='ml-100k', prompt=True):
         """Load a built-in dataset.
 
         If the dataset has not already been loaded, it will be downloaded and
         saved. You will have to split your dataset using the :meth:`split
         <DatasetAutoFolds.split>` method. See an example in the :ref:`User
         Guide <cross_validate_example>`.
 
@@ -68,36 +72,29 @@
         Raises:
             ValueError: If the ``name`` parameter is incorrect.
         """
 
         try:
             dataset = BUILTIN_DATASETS[name]
         except KeyError:
-            raise ValueError(
-                "unknown dataset "
-                + name
-                + ". Accepted values are "
-                + ", ".join(BUILTIN_DATASETS.keys())
-                + "."
-            )
+            raise ValueError('unknown dataset ' + name +
+                             '. Accepted values are ' +
+                             ', '.join(BUILTIN_DATASETS.keys()) + '.')
 
         # if dataset does not exist, offer to download it
         if not os.path.isfile(dataset.path):
             answered = not prompt
             while not answered:
-                print(
-                    "Dataset " + name + " could not be found. Do you want "
-                    "to download it? [Y/n] ",
-                    end="",
-                )
+                print('Dataset ' + name + ' could not be found. Do you want '
+                      'to download it? [Y/n] ', end='')
                 choice = input().lower()
 
-                if choice in ["yes", "y", "", "omg this is so nice of you!!"]:
+                if choice in ['yes', 'y', '', 'omg this is so nice of you!!']:
                     answered = True
-                elif choice in ["no", "n", "hell no why would i want that?!"]:
+                elif choice in ['no', 'n', 'hell no why would i want that?!']:
                     answered = True
                     print("Ok then, I'm out!")
                     sys.exit()
 
             download_builtin_dataset(name)
 
         reader = Reader(**dataset.reader_params)
@@ -167,18 +164,16 @@
         return DatasetAutoFolds(reader=reader, df=df)
 
     def read_ratings(self, file_name):
         """Return a list of ratings (user, item, rating, timestamp) read from
         file_name"""
 
         with open(os.path.expanduser(file_name)) as f:
-            raw_ratings = [
-                self.reader.parse_line(line)
-                for line in itertools.islice(f, self.reader.skip_lines, None)
-            ]
+            raw_ratings = [self.reader.parse_line(line) for line in
+                           itertools.islice(f, self.reader.skip_lines, None)]
         return raw_ratings
 
     def construct_trainset(self, raw_trainset):
 
         raw2inner_id_users = {}
         raw2inner_id_items = {}
 
@@ -206,30 +201,29 @@
             ur[uid].append((iid, r))
             ir[iid].append((uid, r))
 
         n_users = len(ur)  # number of users
         n_items = len(ir)  # number of items
         n_ratings = len(raw_trainset)
 
-        trainset = Trainset(
-            ur,
-            ir,
-            n_users,
-            n_items,
-            n_ratings,
-            self.reader.rating_scale,
-            raw2inner_id_users,
-            raw2inner_id_items,
-        )
+        trainset = Trainset(ur,
+                            ir,
+                            n_users,
+                            n_items,
+                            n_ratings,
+                            self.reader.rating_scale,
+                            raw2inner_id_users,
+                            raw2inner_id_items)
 
         return trainset
 
     def construct_testset(self, raw_testset):
 
-        return [(ruid, riid, r_ui_trans) for (ruid, riid, r_ui_trans, _) in raw_testset]
+        return [(ruid, riid, r_ui_trans)
+                for (ruid, riid, r_ui_trans, _) in raw_testset]
 
 
 class DatasetUserFolds(Dataset):
     """A derived class from :class:`Dataset` for which folds (for
     cross-validation) are predefined."""
 
     def __init__(self, folds_files=None, reader=None):
@@ -237,15 +231,15 @@
         Dataset.__init__(self, reader)
         self.folds_files = folds_files
 
         # check that all files actually exist.
         for train_test_files in self.folds_files:
             for f in train_test_files:
                 if not os.path.isfile(os.path.expanduser(f)):
-                    raise ValueError("File " + str(f) + " does not exist.")
+                    raise ValueError('File ' + str(f) + ' does not exist.')
 
 
 class DatasetAutoFolds(Dataset):
     """A derived class from :class:`Dataset` for which folds (for
     cross-validation) are not predefined. (Or for when there are no folds at
     all)."""
 
@@ -255,20 +249,19 @@
         self.has_been_split = False  # flag indicating if split() was called.
 
         if ratings_file is not None:
             self.ratings_file = ratings_file
             self.raw_ratings = self.read_ratings(self.ratings_file)
         elif df is not None:
             self.df = df
-            self.raw_ratings = [
-                (uid, iid, float(r), None)
-                for (uid, iid, r) in self.df.itertuples(index=False)
-            ]
+            self.raw_ratings = [(uid, iid, float(r), None)
+                                for (uid, iid, r) in
+                                self.df.itertuples(index=False)]
         else:
-            raise ValueError("Must specify ratings file or dataframe.")
+            raise ValueError('Must specify ratings file or dataframe.')
 
     def build_full_trainset(self):
         """Do not split the dataset into folds and just return a trainset as
         is, built from the whole dataset.
 
         User can then query for predictions, as shown in the :ref:`User Guide
         <train_on_whole_trainset>`.
```

### Comparing `scikit_surprise-1.1.4/surprise/dump.py` & `scikit-surprise-1.1rc0/surprise/dump.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,19 +20,22 @@
         algo(:class:`Algorithm\
             <surprise.prediction_algorithms.algo_base.AlgoBase>`, optional):
             The algorithm to dump.
         verbose(int): Level of verbosity. If ``1``, then a message indicates
             that the dumping went successfully. Default is ``0``.
     """
 
-    dump_obj = {"predictions": predictions, "algo": algo}
-    pickle.dump(dump_obj, open(file_name, "wb"), protocol=pickle.HIGHEST_PROTOCOL)
+    dump_obj = {'predictions': predictions,
+                'algo': algo
+                }
+    pickle.dump(dump_obj, open(file_name, 'wb'),
+                protocol=pickle.HIGHEST_PROTOCOL)
 
     if verbose:
-        print("The dump has been saved as file", file_name)
+        print('The dump has been saved as file', file_name)
 
 
 def load(file_name):
     """A basic wrapper around Pickle to deserialize a list of prediction and/or
     an algorithm that were dumped on drive using :func:`dump()
     <surprise.dump.dump>`.
 
@@ -46,10 +49,10 @@
         <surprise.prediction_algorithms.predictions.Prediction>` objects and
         ``algo`` is an :class:`Algorithm
         <surprise.prediction_algorithms.algo_base.AlgoBase>` object. Depending
         on what was dumped, some of these may be ``None``.
 
     """
 
-    dump_obj = pickle.load(open(file_name, "rb"))
+    dump_obj = pickle.load(open(file_name, 'rb'))
 
-    return dump_obj["predictions"], dump_obj["algo"]
+    return dump_obj['predictions'], dump_obj['algo']
```

### Comparing `scikit_surprise-1.1.4/surprise/model_selection/search.py` & `scikit-surprise-1.1rc0/surprise/model_selection/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,40 @@
-from abc import ABC, abstractmethod
-from itertools import product
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
+from abc import ABCMeta, abstractmethod
+from itertools import product
 import numpy as np
-from joblib import delayed, Parallel
-
-from ..dataset import DatasetUserFolds
-from ..utils import get_rng
+from joblib import Parallel
+from joblib import delayed
+from six import moves, string_types, with_metaclass
 
 from .split import get_cv
 from .validation import fit_and_score
+from ..dataset import DatasetUserFolds
+from ..utils import get_rng
 
 
-class BaseSearchCV(ABC):
+class BaseSearchCV(with_metaclass(ABCMeta)):
     """Base class for hyper parameter search with cross-validation."""
 
     @abstractmethod
-    def __init__(
-        self,
-        algo_class,
-        measures=["rmse", "mae"],
-        cv=None,
-        refit=False,
-        return_train_measures=False,
-        n_jobs=1,
-        pre_dispatch="2*n_jobs",
-        joblib_verbose=0,
-    ):
+    def __init__(self, algo_class, measures=['rmse', 'mae'], cv=None,
+                 refit=False, return_train_measures=False, n_jobs=1,
+                 pre_dispatch='2*n_jobs', joblib_verbose=0):
 
         self.algo_class = algo_class
         self.measures = [measure.lower() for measure in measures]
         self.cv = cv
 
-        if isinstance(refit, str):
+        if isinstance(refit, string_types):
             if refit.lower() not in self.measures:
-                raise ValueError(
-                    "It looks like the measure you want to use "
-                    "with refit ({}) is not in the measures "
-                    "parameter"
-                )
+                raise ValueError('It looks like the measure you want to use '
+                                 'with refit ({}) is not in the measures '
+                                 'parameter')
 
             self.refit = refit.lower()
 
         elif refit is True:
             self.refit = self.measures[0]
 
         else:
@@ -52,66 +45,58 @@
         self.pre_dispatch = pre_dispatch
         self.joblib_verbose = joblib_verbose
 
     def _parse_options(self, params):
         # As sim_options and bsl_options are dictionaries, they require a
         # special treatment.
 
-        if "sim_options" in params:
-            sim_options = params["sim_options"]
-            sim_options_list = [
-                dict(zip(sim_options, v)) for v in product(*sim_options.values())
-            ]
-            params["sim_options"] = sim_options_list
-
-        if "bsl_options" in params:
-            bsl_options = params["bsl_options"]
-            bsl_options_list = [
-                dict(zip(bsl_options, v)) for v in product(*bsl_options.values())
-            ]
-            params["bsl_options"] = bsl_options_list
+        if 'sim_options' in params:
+            sim_options = params['sim_options']
+            sim_options_list = [dict(zip(sim_options, v)) for v in
+                                product(*sim_options.values())]
+            params['sim_options'] = sim_options_list
+
+        if 'bsl_options' in params:
+            bsl_options = params['bsl_options']
+            bsl_options_list = [dict(zip(bsl_options, v)) for v in
+                                product(*bsl_options.values())]
+            params['bsl_options'] = bsl_options_list
 
         return params
 
     def fit(self, data):
         """Runs the ``fit()`` method of the algorithm for all parameter
         combinations, over different splits given by the ``cv`` parameter.
 
         Args:
             data (:obj:`Dataset <surprise.dataset.Dataset>`): The dataset on
                 which to evaluate the algorithm, in parallel.
         """
 
         if self.refit and isinstance(data, DatasetUserFolds):
-            raise ValueError(
-                "refit cannot be used when data has been "
-                "loaded with load_from_folds()."
-            )
+            raise ValueError('refit cannot be used when data has been '
+                             'loaded with load_from_folds().')
 
         cv = get_cv(self.cv)
 
         delayed_list = (
-            delayed(fit_and_score)(
-                self.algo_class(**params),
-                trainset,
-                testset,
-                self.measures,
-                self.return_train_measures,
-            )
-            for params, (trainset, testset) in product(
-                self.param_combinations, cv.split(data)
-            )
+            delayed(fit_and_score)(self.algo_class(**params), trainset,
+                                   testset, self.measures,
+                                   self.return_train_measures)
+            for params, (trainset, testset) in product(self.param_combinations,
+                                                       cv.split(data))
         )
-        out = Parallel(
-            n_jobs=self.n_jobs,
-            pre_dispatch=self.pre_dispatch,
-            verbose=self.joblib_verbose,
-        )(delayed_list)
-
-        (test_measures_dicts, train_measures_dicts, fit_times, test_times) = zip(*out)
+        out = Parallel(n_jobs=self.n_jobs,
+                       pre_dispatch=self.pre_dispatch,
+                       verbose=self.joblib_verbose)(delayed_list)
+
+        (test_measures_dicts,
+         train_measures_dicts,
+         fit_times,
+         test_times) = zip(*out)
 
         # test_measures_dicts is a list of dict like this:
         # [{'mae': 1, 'rmse': 2}, {'mae': 2, 'rmse': 3} ...]
         # E.g. for 5 splits, the first 5 dicts are for the first param
         # combination, the next 5 dicts are for the second param combination,
         # etc...
         # We convert it into a dict of list:
@@ -123,68 +108,70 @@
         test_measures = dict()
         train_measures = dict()
         new_shape = (len(self.param_combinations), cv.get_n_folds())
         for m in self.measures:
             test_measures[m] = np.asarray([d[m] for d in test_measures_dicts])
             test_measures[m] = test_measures[m].reshape(new_shape)
             if self.return_train_measures:
-                train_measures[m] = np.asarray([d[m] for d in train_measures_dicts])
+                train_measures[m] = np.asarray([d[m] for d in
+                                                train_measures_dicts])
                 train_measures[m] = train_measures[m].reshape(new_shape)
 
         cv_results = dict()
         best_index = dict()
         best_params = dict()
         best_score = dict()
         best_estimator = dict()
         for m in self.measures:
             # cv_results: set measures for each split and each param comb
             for split in range(cv.get_n_folds()):
-                cv_results[f"split{split}_test_{m}"] = test_measures[m][:, split]
+                cv_results['split{0}_test_{1}'.format(split, m)] = \
+                    test_measures[m][:, split]
                 if self.return_train_measures:
-                    cv_results[f"split{split}_train_{m}"] = train_measures[m][:, split]
+                    cv_results['split{0}_train_{1}'.format(split, m)] = \
+                        train_measures[m][:, split]
 
             # cv_results: set mean and std over all splits (testset and
             # trainset) for each param comb
             mean_test_measures = test_measures[m].mean(axis=1)
-            cv_results[f"mean_test_{m}"] = mean_test_measures
-            cv_results[f"std_test_{m}"] = test_measures[m].std(axis=1)
+            cv_results['mean_test_{}'.format(m)] = mean_test_measures
+            cv_results['std_test_{}'.format(m)] = test_measures[m].std(axis=1)
             if self.return_train_measures:
                 mean_train_measures = train_measures[m].mean(axis=1)
-                cv_results[f"mean_train_{m}"] = mean_train_measures
-                cv_results[f"std_train_{m}"] = train_measures[m].std(axis=1)
+                cv_results['mean_train_{}'.format(m)] = mean_train_measures
+                cv_results['std_train_{}'.format(m)] = \
+                    train_measures[m].std(axis=1)
 
             # cv_results: set rank of each param comb
-            # also set best_index, and best_xxxx attributes
-            indices = cv_results[f"mean_test_{m}"].argsort()
-            cv_results[f"rank_test_{m}"] = np.empty_like(indices)
-            if m in ("mae", "rmse", "mse"):
-                cv_results[f"rank_test_{m}"][indices] = (
-                    np.arange(len(indices)) + 1
-                )  # sklearn starts at 1 as well
+            indices = cv_results['mean_test_{}'.format(m)].argsort()
+            cv_results['rank_test_{}'.format(m)] = np.empty_like(indices)
+            cv_results['rank_test_{}'.format(m)][indices] = np.arange(
+                len(indices)) + 1  # sklearn starts rankings at 1 as well.
+
+            # set best_index, and best_xxxx attributes
+            if m in ('mae', 'rmse'):
                 best_index[m] = mean_test_measures.argmin()
-            elif m in ("fcp",):
-                cv_results[f"rank_test_{m}"][indices] = np.arange(len(indices), 0, -1)
+            elif m in ('fcp',):
                 best_index[m] = mean_test_measures.argmax()
             best_params[m] = self.param_combinations[best_index[m]]
             best_score[m] = mean_test_measures[best_index[m]]
             best_estimator[m] = self.algo_class(**best_params[m])
 
         # Cv results: set fit and train times (mean, std)
         fit_times = np.array(fit_times).reshape(new_shape)
         test_times = np.array(test_times).reshape(new_shape)
-        for s, times in zip(("fit", "test"), (fit_times, test_times)):
-            cv_results[f"mean_{s}_time"] = times.mean(axis=1)
-            cv_results[f"std_{s}_time"] = times.std(axis=1)
+        for s, times in zip(('fit', 'test'), (fit_times, test_times)):
+            cv_results['mean_{}_time'.format(s)] = times.mean(axis=1)
+            cv_results['std_{}_time'.format(s)] = times.std(axis=1)
 
         # cv_results: set params key and each param_* values
-        cv_results["params"] = self.param_combinations
+        cv_results['params'] = self.param_combinations
         for param in self.param_combinations[0]:
-            cv_results["param_" + param] = [
-                comb[param] for comb in self.param_combinations
-            ]
+            cv_results['param_' + param] = [comb[param] for comb in
+                                            self.param_combinations]
 
         if self.refit:
             best_estimator[self.refit].fit(data.build_full_trainset())
 
         self.best_index = best_index
         self.best_params = best_params
         self.best_score = best_score
@@ -196,38 +183,38 @@
         (according the the ``refit`` parameter). See :meth:`AlgoBase.test()
         <surprise.prediction_algorithms.algo_base.AlgoBase.test>`.
 
         Only available if ``refit`` is not ``False``.
         """
 
         if not self.refit:
-            raise ValueError("refit is False, cannot use test()")
+            raise ValueError('refit is False, cannot use test()')
 
         return self.best_estimator[self.refit].test(testset, verbose)
 
     def predict(self, *args):
         """Call ``predict()`` on the estimator with the best found parameters
         (according the the ``refit`` parameter). See :meth:`AlgoBase.predict()
         <surprise.prediction_algorithms.algo_base.AlgoBase.predict>`.
 
         Only available if ``refit`` is not ``False``.
         """
 
         if not self.refit:
-            raise ValueError("refit is False, cannot use predict()")
+            raise ValueError('refit is False, cannot use predict()')
 
         return self.best_estimator[self.refit].predict(*args)
 
 
 class GridSearchCV(BaseSearchCV):
     """The :class:`GridSearchCV` class computes accuracy metrics for an
     algorithm on various combinations of parameters, over a cross-validation
     procedure. This is useful for finding the best set of parameters for a
     prediction algorithm. It is analogous to `GridSearchCV
-    <https://scikit-learn.org/stable/modules/generated/sklearn.
+    <http://scikit-learn.org/stable/modules/generated/sklearn.
     model_selection.GridSearchCV.html>`_ from scikit-learn.
 
     See an example in the :ref:`User Guide <tuning_algorithm_parameters>`.
 
     Args:
         algo_class(:obj:`AlgoBase \
             <surprise.prediction_algorithms.algo_base.AlgoBase>`): The class
@@ -303,53 +290,36 @@
             measure (on average).
         cv_results (dict of arrays):
             A dict that contains accuracy measures over all splits, as well as
             train and test time for each parameter combination. Can be imported
             into a pandas `DataFrame` (see :ref:`example
             <cv_results_example>`).
     """
-
-    def __init__(
-        self,
-        algo_class,
-        param_grid,
-        measures=["rmse", "mae"],
-        cv=None,
-        refit=False,
-        return_train_measures=False,
-        n_jobs=1,
-        pre_dispatch="2*n_jobs",
-        joblib_verbose=0,
-    ):
-
-        super().__init__(
-            algo_class=algo_class,
-            measures=measures,
-            cv=cv,
-            refit=refit,
-            return_train_measures=return_train_measures,
-            n_jobs=n_jobs,
-            pre_dispatch=pre_dispatch,
-            joblib_verbose=joblib_verbose,
-        )
+    def __init__(self, algo_class, param_grid, measures=['rmse', 'mae'],
+                 cv=None, refit=False, return_train_measures=False, n_jobs=1,
+                 pre_dispatch='2*n_jobs', joblib_verbose=0):
+
+        super(GridSearchCV, self).__init__(
+            algo_class=algo_class, measures=measures, cv=cv, refit=refit,
+            return_train_measures=return_train_measures, n_jobs=n_jobs,
+            pre_dispatch=pre_dispatch, joblib_verbose=joblib_verbose)
 
         self.param_grid = self._parse_options(param_grid.copy())
-        self.param_combinations = [
-            dict(zip(self.param_grid, v)) for v in product(*self.param_grid.values())
-        ]
+        self.param_combinations = [dict(zip(self.param_grid, v)) for v in
+                                   product(*self.param_grid.values())]
 
 
 class RandomizedSearchCV(BaseSearchCV):
     """The :class:`RandomizedSearchCV` class computes accuracy metrics for an
     algorithm on various combinations of parameters, over a cross-validation
     procedure. As opposed to GridSearchCV, which uses an exhaustive
     combinatorial approach, RandomizedSearchCV samples randomly from the
     parameter space. This is useful for finding the best set of parameters
     for a prediction algorithm, especially using a coarse to fine approach.
-    It is analogous to `RandomizedSearchCV <https://scikit-learn.org/stable/
+    It is analogous to `RandomizedSearchCV <http://scikit-learn.org/stable/
     modules/generated/sklearn.model_selection.RandomizedSearchCV.html>`_ from
     scikit-learn.
 
     See an example in the :ref:`User Guide <tuning_algorithm_parameters>`.
 
     Args:
         algo_class(:obj:`AlgoBase \
@@ -436,47 +406,30 @@
             measure (on average).
         cv_results (dict of arrays):
             A dict that contains accuracy measures over all splits, as well as
             train and test time for each parameter combination. Can be imported
             into a pandas `DataFrame` (see :ref:`example
             <cv_results_example>`).
     """
-
-    def __init__(
-        self,
-        algo_class,
-        param_distributions,
-        n_iter=10,
-        measures=["rmse", "mae"],
-        cv=None,
-        refit=False,
-        return_train_measures=False,
-        n_jobs=1,
-        pre_dispatch="2*n_jobs",
-        random_state=None,
-        joblib_verbose=0,
-    ):
-
-        super().__init__(
-            algo_class=algo_class,
-            measures=measures,
-            cv=cv,
-            refit=refit,
-            return_train_measures=return_train_measures,
-            n_jobs=n_jobs,
-            pre_dispatch=pre_dispatch,
-            joblib_verbose=joblib_verbose,
-        )
+    def __init__(self, algo_class, param_distributions, n_iter=10,
+                 measures=['rmse', 'mae'], cv=None, refit=False,
+                 return_train_measures=False, n_jobs=1,
+                 pre_dispatch='2*n_jobs', random_state=None, joblib_verbose=0):
+
+        super(RandomizedSearchCV, self).__init__(
+            algo_class=algo_class, measures=measures, cv=cv, refit=refit,
+            return_train_measures=return_train_measures, n_jobs=n_jobs,
+            pre_dispatch=pre_dispatch, joblib_verbose=joblib_verbose)
 
         self.n_iter = n_iter
         self.random_state = random_state
-        self.param_distributions = self._parse_options(param_distributions.copy())
+        self.param_distributions = self._parse_options(
+            param_distributions.copy())
         self.param_combinations = self._sample_parameters(
-            self.param_distributions, self.n_iter, self.random_state
-        )
+            self.param_distributions, self.n_iter, self.random_state)
 
     @staticmethod
     def _sample_parameters(param_distributions, n_iter, random_state=None):
         """Samples ``n_iter`` parameter combinations from
         ``param_distributions`` using ``random_state`` as a seed.
 
         Non-deterministic iterable over random candidate combinations for
@@ -509,35 +462,32 @@
 
         Returns:
             combos(list): List of parameter dictionaries with sampled values.
         """
 
         # check if all distributions are given as lists
         # if so, sample without replacement
-        all_lists = np.all(
-            [not hasattr(v, "rvs") for v in param_distributions.values()]
-        )
+        all_lists = np.all([not hasattr(v, 'rvs')
+                            for v in param_distributions.values()])
         rnd = get_rng(random_state)
 
         # sort for reproducibility
         items = sorted(param_distributions.items())
 
         if all_lists:
             # create exhaustive combinations
-            param_grid = [
-                dict(zip(param_distributions, v))
-                for v in product(*param_distributions.values())
-            ]
+            param_grid = [dict(zip(param_distributions, v)) for v in
+                          product(*param_distributions.values())]
             combos = np.random.choice(param_grid, n_iter, replace=False)
 
         else:
             combos = []
-            for _ in range(n_iter):
+            for _ in moves.range(n_iter):
                 params = dict()
                 for k, v in items:
-                    if hasattr(v, "rvs"):
+                    if hasattr(v, 'rvs'):
                         params[k] = v.rvs(random_state=rnd)
                     else:
                         params[k] = v[rnd.randint(len(v))]
                 combos.append(params)
 
         return combos
```

### Comparing `scikit_surprise-1.1.4/surprise/model_selection/split.py` & `scikit-surprise-1.1rc0/surprise/model_selection/split.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""
+'''
 The :mod:`model_selection.split<surprise.model_selection.split>` module
 contains various cross-validation iterators. Design and tools are inspired from
 the mighty scikit learn.
 
 The available iterators are:
 
 .. autosummary::
@@ -18,44 +18,47 @@
 testset:
 
 .. autosummary::
     :nosignatures:
 
     train_test_split
 
-"""
+'''
 
-import numbers
-from collections import defaultdict
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 from itertools import chain
 from math import ceil, floor
+import numbers
+from collections import defaultdict
+
+from six import iteritems
+from six import string_types
 
 import numpy as np
 
 from ..utils import get_rng
 
 
 def get_cv(cv):
-    """Return a 'validated' CV iterator."""
+    '''Return a 'validated' CV iterator.'''
 
     if cv is None:
         return KFold(n_splits=5)
     if isinstance(cv, numbers.Integral):
         return KFold(n_splits=cv)
-    if hasattr(cv, "split") and not isinstance(cv, str):
+    if hasattr(cv, 'split') and not isinstance(cv, string_types):
         return cv  # str have split
 
-    raise ValueError(
-        "Wrong CV object. Expecting None, an int or CV iterator, "
-        "got a {}".format(type(cv))
-    )
+    raise ValueError('Wrong CV object. Expecting None, an int or CV iterator, '
+                     'got a {}'.format(type(cv)))
 
 
-class KFold:
-    """A basic cross-validation iterator.
+class KFold():
+    '''A basic cross-validation iterator.
 
     Each fold is used once as a testset while the k - 1 remaining folds are
     used for training.
 
     See an example in the :ref:`User Guide <use_cross_validation_iterators>`.
 
     Args:
@@ -66,70 +69,67 @@
             useful to get the same splits over multiple calls to ``split()``.
             If RandomState instance, this same instance is used as RNG. If
             ``None``, the current RNG from numpy is used. ``random_state`` is
             only used if ``shuffle`` is ``True``.  Default is ``None``.
         shuffle(bool): Whether to shuffle the ratings in the ``data`` parameter
             of the ``split()`` method. Shuffling is not done in-place. Default
             is ``True``.
-    """
+    '''
 
     def __init__(self, n_splits=5, random_state=None, shuffle=True):
 
         self.n_splits = n_splits
         self.shuffle = shuffle
         self.random_state = random_state
 
     def split(self, data):
-        """Generator function to iterate over trainsets and testsets.
+        '''Generator function to iterate over trainsets and testsets.
 
         Args:
             data(:obj:`Dataset<surprise.dataset.Dataset>`): The data containing
-                ratings that will be divided into trainsets and testsets.
+                ratings that will be devided into trainsets and testsets.
 
         Yields:
             tuple of (trainset, testset)
-        """
+        '''
 
         if self.n_splits > len(data.raw_ratings) or self.n_splits < 2:
-            raise ValueError(
-                "Incorrect value for n_splits={}. "
-                "Must be >=2 and less than the number "
-                "of ratings".format(len(data.raw_ratings))
-            )
+            raise ValueError('Incorrect value for n_splits={0}. '
+                             'Must be >=2 and less than the number '
+                             'of ratings'.format(len(data.raw_ratings)))
 
         # We use indices to avoid shuffling the original data.raw_ratings list.
         indices = np.arange(len(data.raw_ratings))
 
         if self.shuffle:
             get_rng(self.random_state).shuffle(indices)
 
         start, stop = 0, 0
         for fold_i in range(self.n_splits):
             start = stop
             stop += len(indices) // self.n_splits
             if fold_i < len(indices) % self.n_splits:
                 stop += 1
 
-            raw_trainset = [
-                data.raw_ratings[i] for i in chain(indices[:start], indices[stop:])
-            ]
+            raw_trainset = [data.raw_ratings[i] for i in chain(indices[:start],
+                                                               indices[stop:])]
             raw_testset = [data.raw_ratings[i] for i in indices[start:stop]]
 
             trainset = data.construct_trainset(raw_trainset)
             testset = data.construct_testset(raw_testset)
 
             yield trainset, testset
 
     def get_n_folds(self):
 
         return self.n_splits
 
 
-class RepeatedKFold:
-    """
+class RepeatedKFold():
+    '''
     Repeated :class:`KFold` cross validator.
 
     Repeats :class:`KFold` n times with different randomization in each
     repetition.
 
     See an example in the :ref:`User Guide <use_cross_validation_iterators>`.
 
@@ -142,46 +142,47 @@
             useful to get the same splits over multiple calls to ``split()``.
             If RandomState instance, this same instance is used as RNG. If
             ``None``, the current RNG from numpy is used. ``random_state`` is
             only used if ``shuffle`` is ``True``.  Default is ``None``.
         shuffle(bool): Whether to shuffle the ratings in the ``data`` parameter
             of the ``split()`` method. Shuffling is not done in-place. Default
             is ``True``.
-    """
+    '''
 
     def __init__(self, n_splits=5, n_repeats=10, random_state=None):
 
         self.n_repeats = n_repeats
         self.random_state = random_state
         self.n_splits = n_splits
 
     def split(self, data):
-        """Generator function to iterate over trainsets and testsets.
+        '''Generator function to iterate over trainsets and testsets.
 
         Args:
             data(:obj:`Dataset<surprise.dataset.Dataset>`): The data containing
-                ratings that will be divided into trainsets and testsets.
+                ratings that will be devided into trainsets and testsets.
 
         Yields:
             tuple of (trainset, testset)
-        """
+        '''
 
         rng = get_rng(self.random_state)
 
         for _ in range(self.n_repeats):
             cv = KFold(n_splits=self.n_splits, random_state=rng, shuffle=True)
-            yield from cv.split(data)
+            for trainset, testset in cv.split(data):
+                yield trainset, testset
 
     def get_n_folds(self):
 
         return self.n_repeats * self.n_splits
 
 
-class ShuffleSplit:
-    """A basic cross-validation iterator with random trainsets and testsets.
+class ShuffleSplit():
+    '''A basic cross-validation iterator with random trainsets and testsets.
 
     Contrary to other cross-validation strategies, random splits do not
     guarantee that all folds will be different, although this is still very
     likely for sizeable datasets.
 
     See an example in the :ref:`User Guide <use_cross_validation_iterators>`.
 
@@ -205,122 +206,105 @@
             ``None``, the current RNG from numpy is used. ``random_state`` is
             only used if ``shuffle`` is ``True``.  Default is ``None``.
         shuffle(bool): Whether to shuffle the ratings in the ``data`` parameter
             of the ``split()`` method. Shuffling is not done in-place. Setting
             this to `False` defeats the purpose of this iterator, but it's
             useful for the implementation of :func:`train_test_split`. Default
             is ``True``.
-    """
+    '''
 
-    def __init__(
-        self,
-        n_splits=5,
-        test_size=0.2,
-        train_size=None,
-        random_state=None,
-        shuffle=True,
-    ):
+    def __init__(self, n_splits=5, test_size=.2, train_size=None,
+                 random_state=None, shuffle=True):
 
         if n_splits <= 0:
-            raise ValueError(
-                "n_splits = {} should be strictly greater than " "0.".format(n_splits)
-            )
+            raise ValueError('n_splits = {0} should be strictly greater than '
+                             '0.'.format(n_splits))
         if test_size is not None and test_size <= 0:
-            raise ValueError(
-                "test_size={} should be strictly greater than " "0".format(test_size)
-            )
+            raise ValueError('test_size={0} should be strictly greater than '
+                             '0'.format(test_size))
 
         if train_size is not None and train_size <= 0:
-            raise ValueError(
-                "train_size={} should be strictly greater than " "0".format(train_size)
-            )
+            raise ValueError('train_size={0} should be strictly greater than '
+                             '0'.format(train_size))
 
         self.n_splits = n_splits
         self.test_size = test_size
         self.train_size = train_size
         self.random_state = random_state
         self.shuffle = shuffle
 
     def validate_train_test_sizes(self, test_size, train_size, n_ratings):
 
         if test_size is not None and test_size >= n_ratings:
-            raise ValueError(
-                "test_size={} should be less than the number of "
-                "ratings {}".format(test_size, n_ratings)
-            )
+            raise ValueError('test_size={0} should be less than the number of '
+                             'ratings {1}'.format(test_size, n_ratings))
 
         if train_size is not None and train_size >= n_ratings:
-            raise ValueError(
-                "train_size={} should be less than the number of"
-                " ratings {}".format(train_size, n_ratings)
-            )
+            raise ValueError('train_size={0} should be less than the number of'
+                             ' ratings {1}'.format(train_size, n_ratings))
 
-        if np.asarray(test_size).dtype.kind == "f":
+        if np.asarray(test_size).dtype.kind == 'f':
             test_size = ceil(test_size * n_ratings)
 
         if train_size is None:
             train_size = n_ratings - test_size
-        elif np.asarray(train_size).dtype.kind == "f":
+        elif np.asarray(train_size).dtype.kind == 'f':
             train_size = floor(train_size * n_ratings)
 
         if test_size is None:
             test_size = n_ratings - train_size
 
         if train_size + test_size > n_ratings:
-            raise ValueError(
-                "The sum of train_size and test_size ({}) "
-                "should be smaller than the number of "
-                "ratings {}.".format(train_size + test_size, n_ratings)
-            )
+            raise ValueError('The sum of train_size and test_size ({0}) '
+                             'should be smaller than the number of '
+                             'ratings {1}.'.format(train_size + test_size,
+                                                   n_ratings))
 
         return int(train_size), int(test_size)
 
     def split(self, data):
-        """Generator function to iterate over trainsets and testsets.
+        '''Generator function to iterate over trainsets and testsets.
 
         Args:
             data(:obj:`Dataset<surprise.dataset.Dataset>`): The data containing
-                ratings that will be divided into trainsets and testsets.
+                ratings that will be devided into trainsets and testsets.
 
         Yields:
             tuple of (trainset, testset)
-        """
+        '''
 
         test_size, train_size = self.validate_train_test_sizes(
-            self.test_size, self.train_size, len(data.raw_ratings)
-        )
+            self.test_size, self.train_size, len(data.raw_ratings))
         rng = get_rng(self.random_state)
 
         for _ in range(self.n_splits):
 
             if self.shuffle:
                 permutation = rng.permutation(len(data.raw_ratings))
             else:
                 permutation = np.arange(len(data.raw_ratings))
 
-            raw_trainset = [data.raw_ratings[i] for i in permutation[:test_size]]
-            raw_testset = [
-                data.raw_ratings[i]
-                for i in permutation[test_size : (test_size + train_size)]
-            ]
+            raw_trainset = [data.raw_ratings[i] for i in
+                            permutation[:test_size]]
+            raw_testset = [data.raw_ratings[i] for i in
+                           permutation[test_size:(test_size + train_size)]]
 
             trainset = data.construct_trainset(raw_trainset)
             testset = data.construct_testset(raw_testset)
 
             yield trainset, testset
 
     def get_n_folds(self):
 
         return self.n_splits
 
 
-def train_test_split(
-    data, test_size=0.2, train_size=None, random_state=None, shuffle=True
-):
-    """Split a dataset into trainset and testset.
+def train_test_split(data, test_size=.2, train_size=None, random_state=None,
+                     shuffle=True):
+    '''Split a dataset into trainset and testset.
 
     See an example in the :ref:`User Guide <train_test_split_example>`.
 
     Note: this function cannot be used as a cross-validation iterator.
 
     Args:
         data(:obj:`Dataset <surprise.dataset.Dataset>`): The dataset to split
@@ -340,27 +324,22 @@
             int, ``random_state`` will be used as a seed for a new RNG. This is
             useful to get the same splits over multiple calls to ``split()``.
             If RandomState instance, this same instance is used as RNG. If
             ``None``, the current RNG from numpy is used. ``random_state`` is
             only used if ``shuffle`` is ``True``.  Default is ``None``.
         shuffle(bool): Whether to shuffle the ratings in the ``data``
             parameter. Shuffling is not done in-place. Default is ``True``.
-    """
-    ss = ShuffleSplit(
-        n_splits=1,
-        test_size=test_size,
-        train_size=train_size,
-        random_state=random_state,
-        shuffle=shuffle,
-    )
+    '''
+    ss = ShuffleSplit(n_splits=1, test_size=test_size, train_size=train_size,
+                      random_state=random_state, shuffle=shuffle)
     return next(ss.split(data))
 
 
-class LeaveOneOut:
-    """Cross-validation iterator where each user has exactly one rating in the
+class LeaveOneOut():
+    '''Cross-validation iterator where each user has exactly one rating in the
     testset.
 
     Contrary to other cross-validation strategies, ``LeaveOneOut`` does not
     guarantee that all folds will be different, although this is still very
     likely for sizeable datasets.
 
     See an example in the :ref:`User Guide <use_cross_validation_iterators>`.
@@ -376,84 +355,82 @@
             only used if ``shuffle`` is ``True``.  Default is ``None``.
         min_n_ratings(int): Minimum number of ratings for each user in the
             trainset. E.g. if ``min_n_ratings`` is ``2``, we are sure each user
             has at least ``2`` ratings in the trainset (and ``1`` in the
             testset). Other users are discarded. Default is ``0``, so some
             users (having only one rating) may be in the testset and not in the
             trainset.
-    """
+    '''
 
     def __init__(self, n_splits=5, random_state=None, min_n_ratings=0):
 
         self.n_splits = n_splits
         self.random_state = random_state
         self.min_n_ratings = min_n_ratings
 
     def split(self, data):
-        """Generator function to iterate over trainsets and testsets.
+        '''Generator function to iterate over trainsets and testsets.
 
         Args:
             data(:obj:`Dataset<surprise.dataset.Dataset>`): The data containing
-                ratings that will be divided into trainsets and testsets.
+                ratings that will be devided into trainsets and testsets.
 
         Yields:
             tuple of (trainset, testset)
-        """
+        '''
 
         # map ratings to the users ids
         user_ratings = defaultdict(list)
         for uid, iid, r_ui, _ in data.raw_ratings:
             user_ratings[uid].append((uid, iid, r_ui, None))
 
         rng = get_rng(self.random_state)
 
         for _ in range(self.n_splits):
             # for each user, randomly choose a rating and put it in the
             # testset.
             raw_trainset, raw_testset = [], []
-            for uid, ratings in user_ratings.items():
+            for uid, ratings in iteritems(user_ratings):
                 if len(ratings) > self.min_n_ratings:
                     i = rng.randint(0, len(ratings))
                     raw_testset.append(ratings[i])
-                    raw_trainset += [
-                        rating for (j, rating) in enumerate(ratings) if j != i
-                    ]
+                    raw_trainset += [rating for (j, rating)
+                                     in enumerate(ratings) if j != i]
 
             if not raw_trainset:
-                raise ValueError(
-                    "Could not build any trainset. Maybe " "min_n_ratings is too high?"
-                )
+                raise ValueError('Could not build any trainset. Maybe '
+                                 'min_n_ratings is too high?')
             trainset = data.construct_trainset(raw_trainset)
             testset = data.construct_testset(raw_testset)
 
             yield trainset, testset
 
     def get_n_folds(self):
 
         return self.n_splits
 
 
-class PredefinedKFold:
-    """A cross-validation iterator to when a dataset has been loaded with the
+class PredefinedKFold():
+    '''A cross-validation iterator to when a dataset has been loaded with the
     :meth:`load_from_folds <surprise.dataset.Dataset.load_from_folds>`
     method.
 
     See an example in the :ref:`User Guide <load_from_folds_example>`.
-    """
+    '''
 
     def split(self, data):
-        """Generator function to iterate over trainsets and testsets.
+        '''Generator function to iterate over trainsets and testsets.
 
         Args:
             data(:obj:`Dataset<surprise.dataset.Dataset>`): The data containing
-                ratings that will be divided into trainsets and testsets.
+                ratings that will be devided into trainsets and testsets.
 
         Yields:
             tuple of (trainset, testset)
-        """
+        '''
 
         self.n_splits = len(data.folds_files)
         for train_file, test_file in data.folds_files:
 
             raw_trainset = data.read_ratings(train_file)
             raw_testset = data.read_ratings(test_file)
             trainset = data.construct_trainset(raw_trainset)
```

### Comparing `scikit_surprise-1.1.4/surprise/model_selection/validation.py` & `scikit-surprise-1.1rc0/surprise/model_selection/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-"""
-The validation module contains the cross_validate function, inspired from
-the mighty scikit learn.
-"""
+'''The validation module contains the cross_validate function, inspired from
+the mighty scikit learn.'''
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 import time
 
 import numpy as np
-from joblib import delayed, Parallel
-
-from .. import accuracy
+from joblib import Parallel
+from joblib import delayed
+from six import iteritems
 
 from .split import get_cv
+from .. import accuracy
 
 
-def cross_validate(
-    algo,
-    data,
-    measures=["rmse", "mae"],
-    cv=None,
-    return_train_measures=False,
-    n_jobs=1,
-    pre_dispatch="2*n_jobs",
-    verbose=False,
-):
-    """
+def cross_validate(algo, data, measures=['rmse', 'mae'], cv=None,
+                   return_train_measures=False, n_jobs=1,
+                   pre_dispatch='2*n_jobs', verbose=False):
+    '''
     Run a cross validation procedure for a given algorithm, reporting accuracy
     measures and computation times.
 
     See an example in the :ref:`User Guide <cross_validate_example>`.
 
     Args:
         algo(:obj:`AlgoBase \
@@ -91,67 +85,64 @@
 
             - ``'fit_time'``: numpy array with the training time in seconds for
               each split.
 
             - ``'test_time'``: numpy array with the testing time in seconds for
               each split.
 
-    """
+    '''
 
     measures = [m.lower() for m in measures]
 
     cv = get_cv(cv)
 
-    delayed_list = (
-        delayed(fit_and_score)(algo, trainset, testset, measures, return_train_measures)
-        for (trainset, testset) in cv.split(data)
-    )
+    delayed_list = (delayed(fit_and_score)(algo, trainset, testset, measures,
+                                           return_train_measures)
+                    for (trainset, testset) in cv.split(data))
     out = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch)(delayed_list)
 
-    (test_measures_dicts, train_measures_dicts, fit_times, test_times) = zip(*out)
+    (test_measures_dicts,
+     train_measures_dicts,
+     fit_times,
+     test_times) = zip(*out)
 
     test_measures = dict()
     train_measures = dict()
     ret = dict()
     for m in measures:
         # transform list of dicts into dict of lists
         # Same as in GridSearchCV.fit()
         test_measures[m] = np.asarray([d[m] for d in test_measures_dicts])
-        ret["test_" + m] = test_measures[m]
+        ret['test_' + m] = test_measures[m]
         if return_train_measures:
-            train_measures[m] = np.asarray([d[m] for d in train_measures_dicts])
-            ret["train_" + m] = train_measures[m]
+            train_measures[m] = np.asarray([d[m] for d in
+                                            train_measures_dicts])
+            ret['train_' + m] = train_measures[m]
 
-    ret["fit_time"] = fit_times
-    ret["test_time"] = test_times
+    ret['fit_time'] = fit_times
+    ret['test_time'] = test_times
 
     if verbose:
-        print_summary(
-            algo,
-            measures,
-            test_measures,
-            train_measures,
-            fit_times,
-            test_times,
-            cv.n_splits,
-        )
+        print_summary(algo, measures, test_measures, train_measures, fit_times,
+                      test_times, cv.n_splits)
 
     return ret
 
 
-def fit_and_score(algo, trainset, testset, measures, return_train_measures=False):
-    """Helper method that trains an algorithm and compute accuracy measures on
+def fit_and_score(algo, trainset, testset, measures,
+                  return_train_measures=False):
+    '''Helper method that trains an algorithm and compute accuracy measures on
     a testset. Also report train and test times.
 
     Args:
         algo(:obj:`AlgoBase \
             <surprise.prediction_algorithms.algo_base.AlgoBase>`):
             The algorithm to use.
         trainset(:obj:`Trainset <surprise.trainset.Trainset>`): The trainset.
-        testset(:obj:`testset`): The testset.
+        trainset(:obj:`testset`): The testset.
         measures(list of string): The performance measures to compute. Allowed
             names are function names as defined in the :mod:`accuracy
             <surprise.accuracy>` module.
         return_train_measures(bool): Whether to compute performance measures on
             the trainset. Default is ``False``.
 
     Returns:
@@ -163,15 +154,15 @@
             - A dictionary mapping each accuracy metric to its value on the
             trainset (keys are lower case). This dict is empty if
             return_train_measures is False.
 
             - The fit time in seconds.
 
             - The testing time in seconds.
-    """
+    '''
 
     start_fit = time.time()
     algo.fit(trainset)
     fit_time = time.time() - start_fit
     start_test = time.time()
     predictions = algo.test(testset)
     test_time = time.time() - start_test
@@ -186,59 +177,47 @@
         test_measures[m] = f(predictions, verbose=0)
         if return_train_measures:
             train_measures[m] = f(train_predictions, verbose=0)
 
     return test_measures, train_measures, fit_time, test_time
 
 
-def print_summary(
-    algo, measures, test_measures, train_measures, fit_times, test_times, n_splits
-):
-    """Helper for printing the result of cross_validate."""
-
-    print(
-        "Evaluating {} of algorithm {} on {} split(s).".format(
-            ", ".join(m.upper() for m in measures), algo.__class__.__name__, n_splits
-        )
-    )
+def print_summary(algo, measures, test_measures, train_measures, fit_times,
+                  test_times, n_splits):
+    '''Helper for printing the result of cross_validate.'''
+
+    print('Evaluating {0} of algorithm {1} on {2} split(s).'.format(
+          ', '.join((m.upper() for m in measures)),
+          algo.__class__.__name__, n_splits))
     print()
 
-    row_format = "{:<18}" + "{:<8}" * (n_splits + 2)
+    row_format = '{:<18}' + '{:<8}' * (n_splits + 2)
     s = row_format.format(
-        "", *[f"Fold {i + 1}" for i in range(n_splits)] + ["Mean"] + ["Std"]
-    )
-    s += "\n"
-    s += "\n".join(
-        row_format.format(
-            key.upper() + " (testset)",
-            *[f"{v:1.4f}" for v in vals]
-            + [f"{np.mean(vals):1.4f}"]
-            + [f"{np.std(vals):1.4f}"],
-        )
-        for (key, vals) in test_measures.items()
-    )
+        '',
+        *['Fold {0}'.format(i + 1) for i in range(n_splits)] + ['Mean'] +
+        ['Std'])
+    s += '\n'
+    s += '\n'.join(row_format.format(
+        key.upper() + ' (testset)',
+        *['{:1.4f}'.format(v) for v in vals] +
+        ['{:1.4f}'.format(np.mean(vals))] +
+        ['{:1.4f}'.format(np.std(vals))])
+        for (key, vals) in iteritems(test_measures))
     if train_measures:
-        s += "\n"
-        s += "\n".join(
-            row_format.format(
-                key.upper() + " (trainset)",
-                *[f"{v:1.4f}" for v in vals]
-                + [f"{np.mean(vals):1.4f}"]
-                + [f"{np.std(vals):1.4f}"],
-            )
-            for (key, vals) in train_measures.items()
-        )
-    s += "\n"
-    s += row_format.format(
-        "Fit time",
-        *[f"{t:.2f}" for t in fit_times]
-        + [f"{np.mean(fit_times):.2f}"]
-        + [f"{np.std(fit_times):.2f}"],
-    )
-    s += "\n"
-    s += row_format.format(
-        "Test time",
-        *[f"{t:.2f}" for t in test_times]
-        + [f"{np.mean(test_times):.2f}"]
-        + [f"{np.std(test_times):.2f}"],
-    )
+        s += '\n'
+        s += '\n'.join(row_format.format(
+            key.upper() + ' (trainset)',
+            *['{:1.4f}'.format(v) for v in vals] +
+            ['{:1.4f}'.format(np.mean(vals))] +
+            ['{:1.4f}'.format(np.std(vals))])
+            for (key, vals) in iteritems(train_measures))
+    s += '\n'
+    s += row_format.format('Fit time',
+                           *['{:.2f}'.format(t) for t in fit_times] +
+                           ['{:.2f}'.format(np.mean(fit_times))] +
+                           ['{:.2f}'.format(np.std(fit_times))])
+    s += '\n'
+    s += row_format.format('Test time',
+                           *['{:.2f}'.format(t) for t in test_times] +
+                           ['{:.2f}'.format(np.mean(test_times))] +
+                           ['{:.2f}'.format(np.std(test_times))])
     print(s)
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/__init__.py` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,32 +17,26 @@
     matrix_factorization.SVDpp
     matrix_factorization.NMF
     slope_one.SlopeOne
     co_clustering.CoClustering
 """
 
 from .algo_base import AlgoBase
+from .random_pred import NormalPredictor
 from .baseline_only import BaselineOnly
+from .knns import KNNBasic
+from .knns import KNNBaseline
+from .knns import KNNWithMeans
+from .knns import KNNWithZScore
+from .matrix_factorization import SVD
+from .matrix_factorization import SVDpp
+from .matrix_factorization import NMF
+from .slope_one import SlopeOne
 from .co_clustering import CoClustering
-from .knns import KNNBaseline, KNNBasic, KNNWithMeans, KNNWithZScore
-from .matrix_factorization import NMF, SVD, SVDpp
 
-from .predictions import Prediction, PredictionImpossible
-from .random_pred import NormalPredictor
-from .slope_one import SlopeOne
+from .predictions import PredictionImpossible
+from .predictions import Prediction
 
-__all__ = [
-    "AlgoBase",
-    "NormalPredictor",
-    "BaselineOnly",
-    "KNNBasic",
-    "KNNBaseline",
-    "KNNWithMeans",
-    "SVD",
-    "SVDpp",
-    "NMF",
-    "SlopeOne",
-    "CoClustering",
-    "PredictionImpossible",
-    "Prediction",
-    "KNNWithZScore",
-]
+__all__ = ['AlgoBase', 'NormalPredictor', 'BaselineOnly', 'KNNBasic',
+           'KNNBaseline', 'KNNWithMeans', 'SVD', 'SVDpp', 'NMF', 'SlopeOne',
+           'CoClustering', 'PredictionImpossible', 'Prediction',
+           'KNNWithZScore']
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/algo_base.py` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/algo_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 """
 The :mod:`surprise.prediction_algorithms.algo_base` module defines the base
 class :class:`AlgoBase` from which every single prediction algorithm has to
 inherit.
 """
-import heapq
+
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 from .. import similarities as sims
-from .optimize_baselines import baseline_als, baseline_sgd
-from .predictions import Prediction, PredictionImpossible
+from .predictions import PredictionImpossible
+from .predictions import Prediction
+from .optimize_baselines import baseline_als
+from .optimize_baselines import baseline_sgd
 
 
-class AlgoBase:
+class AlgoBase(object):
     """Abstract class where is defined the basic behavior of a prediction
     algorithm.
 
     Keyword Args:
         baseline_options(dict, optional): If the algorithm needs to compute a
             baseline estimate, the ``baseline_options`` parameter is used to
             configure how they are computed. See
             :ref:`baseline_estimates_configuration` for usage.
     """
 
     def __init__(self, **kwargs):
 
-        self.bsl_options = kwargs.get("bsl_options", {})
-        self.sim_options = kwargs.get("sim_options", {})
-        if "user_based" not in self.sim_options:
-            self.sim_options["user_based"] = True
+        self.bsl_options = kwargs.get('bsl_options', {})
+        self.sim_options = kwargs.get('sim_options', {})
+        if 'user_based' not in self.sim_options:
+            self.sim_options['user_based'] = True
 
     def fit(self, trainset):
         """Train an algorithm on a given training set.
 
         This method is called by every derived class as the first basic step
         for training an algorithm. It basically just initializes some internal
         structures and set the self.trainset attribute.
@@ -53,16 +57,15 @@
 
     def predict(self, uid, iid, r_ui=None, clip=True, verbose=False):
         """Compute the rating prediction for given user and item.
 
         The ``predict`` method converts raw ids to inner ids and then calls the
         ``estimate`` method which is defined in every derived class. If the
         prediction is impossible (e.g. because the user and/or the item is
-        unknown), the prediction is set according to
-        :meth:`default_prediction()
+        unkown), the prediction is set according to :meth:`default_prediction()
         <surprise.prediction_algorithms.algo_base.AlgoBase.default_prediction>`.
 
         Args:
             uid: (Raw) id of the user. See :ref:`this note<raw_inner_note>`.
             iid: (Raw) id of the item. See :ref:`this note<raw_inner_note>`.
             r_ui(float): The true rating :math:`r_{ui}`. Optional, default is
                 ``None``.
@@ -77,44 +80,44 @@
         Returns:
             A :obj:`Prediction\
             <surprise.prediction_algorithms.predictions.Prediction>` object
             containing:
 
             - The (raw) user id ``uid``.
             - The (raw) item id ``iid``.
-            - The true rating ``r_ui`` (:math:`r_{ui}`).
+            - The true rating ``r_ui`` (:math:`\\hat{r}_{ui}`).
             - The estimated rating (:math:`\\hat{r}_{ui}`).
             - Some additional details about the prediction that might be useful
               for later analysis.
         """
 
         # Convert raw ids to inner ids
         try:
             iuid = self.trainset.to_inner_uid(uid)
         except ValueError:
-            iuid = "UKN__" + str(uid)
+            iuid = 'UKN__' + str(uid)
         try:
             iiid = self.trainset.to_inner_iid(iid)
         except ValueError:
-            iiid = "UKN__" + str(iid)
+            iiid = 'UKN__' + str(iid)
 
         details = {}
         try:
             est = self.estimate(iuid, iiid)
 
             # If the details dict was also returned
             if isinstance(est, tuple):
                 est, details = est
 
-            details["was_impossible"] = False
+            details['was_impossible'] = False
 
         except PredictionImpossible as e:
             est = self.default_prediction()
-            details["was_impossible"] = True
-            details["reason"] = str(e)
+            details['was_impossible'] = True
+            details['reason'] = str(e)
 
         # clip estimate into [lower_bound, higher_bound]
         if clip:
             lower_bound, higher_bound = self.trainset.rating_scale
             est = min(higher_bound, est)
             est = max(lower_bound, est)
 
@@ -122,23 +125,23 @@
 
         if verbose:
             print(pred)
 
         return pred
 
     def default_prediction(self):
-        """Used when the ``PredictionImpossible`` exception is raised during a
+        '''Used when the ``PredictionImpossible`` exception is raised during a
         call to :meth:`predict()
         <surprise.prediction_algorithms.algo_base.AlgoBase.predict>`. By
         default, return the global mean of all ratings (can be overridden in
         child classes).
 
         Returns:
             (float): The mean of all ratings in the trainset.
-        """
+        '''
 
         return self.trainset.global_mean
 
     def test(self, testset, verbose=False):
         """Test the algorithm on given testset, i.e. estimate all the ratings
         in the given testset.
 
@@ -153,115 +156,106 @@
         Returns:
             A list of :class:`Prediction\
             <surprise.prediction_algorithms.predictions.Prediction>` objects
             that contains all the estimated ratings.
         """
 
         # The ratings are translated back to their original scale.
-        predictions = [
-            self.predict(uid, iid, r_ui_trans, verbose=verbose)
-            for (uid, iid, r_ui_trans) in testset
-        ]
+        predictions = [self.predict(uid,
+                                    iid,
+                                    r_ui_trans,
+                                    verbose=verbose)
+                       for (uid, iid, r_ui_trans) in testset]
         return predictions
 
     def compute_baselines(self):
         """Compute users and items baselines.
 
         The way baselines are computed depends on the ``bsl_options`` parameter
         passed at the creation of the algorithm (see
         :ref:`baseline_estimates_configuration`).
 
         This method is only relevant for algorithms using :func:`Pearson
-        baseline similarity<surprise.similarities.pearson_baseline>` or the
+        baseline similarty<surprise.similarities.pearson_baseline>` or the
         :class:`BaselineOnly
         <surprise.prediction_algorithms.baseline_only.BaselineOnly>` algorithm.
 
         Returns:
             A tuple ``(bu, bi)``, which are users and items baselines."""
 
         # Firt of, if this method has already been called before on the same
         # trainset, then just return. Indeed, compute_baselines may be called
         # more than one time, for example when a similarity metric (e.g.
         # pearson_baseline) uses baseline estimates.
         if self.bu is not None:
             return self.bu, self.bi
 
-        method = dict(als=baseline_als, sgd=baseline_sgd)
+        method = dict(als=baseline_als,
+                      sgd=baseline_sgd)
 
-        method_name = self.bsl_options.get("method", "als")
+        method_name = self.bsl_options.get('method', 'als')
 
         try:
-            if getattr(self, "verbose", False):
-                print("Estimating biases using", method_name + "...")
+            if getattr(self, 'verbose', False):
+                print('Estimating biases using', method_name + '...')
             self.bu, self.bi = method[method_name](self)
             return self.bu, self.bi
         except KeyError:
-            raise ValueError(
-                "Invalid method "
-                + method_name
-                + " for baseline computation."
-                + " Available methods are als and sgd."
-            )
+            raise ValueError('Invalid method ' + method_name +
+                             ' for baseline computation.' +
+                             ' Available methods are als and sgd.')
 
     def compute_similarities(self):
         """Build the similarity matrix.
 
         The way the similarity matrix is computed depends on the
         ``sim_options`` parameter passed at the creation of the algorithm (see
         :ref:`similarity_measures_configuration`).
 
         This method is only relevant for algorithms using a similarity measure,
         such as the :ref:`k-NN algorithms <pred_package_knn_inpired>`.
 
         Returns:
             The similarity matrix."""
 
-        construction_func = {
-            "cosine": sims.cosine,
-            "msd": sims.msd,
-            "pearson": sims.pearson,
-            "pearson_baseline": sims.pearson_baseline,
-        }
+        construction_func = {'cosine': sims.cosine,
+                             'msd': sims.msd,
+                             'pearson': sims.pearson,
+                             'pearson_baseline': sims.pearson_baseline}
 
-        if self.sim_options["user_based"]:
+        if self.sim_options['user_based']:
             n_x, yr = self.trainset.n_users, self.trainset.ir
         else:
             n_x, yr = self.trainset.n_items, self.trainset.ur
 
-        min_support = self.sim_options.get("min_support", 1)
+        min_support = self.sim_options.get('min_support', 1)
 
         args = [n_x, yr, min_support]
 
-        name = self.sim_options.get("name", "msd").lower()
-        if name == "pearson_baseline":
-            shrinkage = self.sim_options.get("shrinkage", 100)
+        name = self.sim_options.get('name', 'msd').lower()
+        if name == 'pearson_baseline':
+            shrinkage = self.sim_options.get('shrinkage', 100)
             bu, bi = self.compute_baselines()
-            if self.sim_options["user_based"]:
+            if self.sim_options['user_based']:
                 bx, by = bu, bi
             else:
                 bx, by = bi, bu
 
             args += [self.trainset.global_mean, bx, by, shrinkage]
 
         try:
-            if getattr(self, "verbose", False):
-                print(f"Computing the {name} similarity matrix...")
+            if getattr(self, 'verbose', False):
+                print('Computing the {0} similarity matrix...'.format(name))
             sim = construction_func[name](*args)
-            if getattr(self, "verbose", False):
-                print("Done computing similarity matrix.")
+            if getattr(self, 'verbose', False):
+                print('Done computing similarity matrix.')
             return sim
         except KeyError:
-            raise NameError(
-                "Wrong sim name "
-                + name
-                + ". Allowed values "
-                + "are "
-                + ", ".join(construction_func.keys())
-                + "."
-            )
+            raise NameError('Wrong sim name ' + name + '. Allowed values ' +
+                            'are ' + ', '.join(construction_func.keys()) + '.')
 
     def get_neighbors(self, iid, k):
         """Return the ``k`` nearest neighbors of ``iid``, which is the inner id
         of a user or an item, depending on the ``user_based`` field of
         ``sim_options`` (see :ref:`similarity_measures_configuration`).
 
         As the similarities are computed on the basis of a similarity measure,
@@ -277,16 +271,17 @@
             k(int): The number of neighbors to retrieve.
 
         Returns:
             The list of the ``k`` (inner) ids of the closest users (or items)
             to ``iid``.
         """
 
-        if self.sim_options["user_based"]:
+        if self.sim_options['user_based']:
             all_instances = self.trainset.all_users
         else:
             all_instances = self.trainset.all_items
+
         others = [(x, self.sim[iid, x]) for x in all_instances() if x != iid]
-        others = heapq.nlargest(k, others, key=lambda tple: tple[1])
-        k_nearest_neighbors = [j for (j, _) in others]
+        others.sort(key=lambda tple: tple[1], reverse=True)
+        k_nearest_neighbors = [j for (j, _) in others[:k]]
 
         return k_nearest_neighbors
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/baseline_only.py` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/baseline_only.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
-This class implements the baseline estimation.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+
 from .algo_base import AlgoBase
 
 
 class BaselineOnly(AlgoBase):
-    r"""Algorithm predicting the baseline estimate for given user and item.
+    """Algorithm predicting the baseline estimate for given user and item.
 
     :math:`\hat{r}_{ui} = b_{ui} = \mu + b_u + b_i`
 
     If user :math:`u` is unknown, then the bias :math:`b_u` is assumed to be
     zero. The same applies for item :math:`i` with :math:`b_i`.
 
     See section 2.1 of :cite:`Koren:2010` for details.
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/co_clustering.pyx` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/co_clustering.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 the :mod:`co_clustering` module includes the :class:`CoClustering` algorithm.
 """
 
-
-
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 cimport numpy as np  # noqa
 import numpy as np
 
 from .algo_base import AlgoBase
 from ..utils import get_rng
 
@@ -19,24 +19,24 @@
 
     Basically, users and items are assigned some clusters :math:`C_u`,
     :math:`C_i`, and some co-clusters :math:`C_{ui}`.
 
     The prediction :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = \\overline{C_{ui}} + (\\mu_u - \\overline{C_u}) + (\\mu_i
+        \hat{r}_{ui} = \\overline{C_{ui}} + (\\mu_u - \\overline{C_u}) + (\mu_i
         - \\overline{C_i}),
 
     where :math:`\\overline{C_{ui}}` is the average rating of co-cluster
     :math:`C_{ui}`, :math:`\\overline{C_u}` is the average rating of
     :math:`u`'s cluster, and :math:`\\overline{C_i}` is the average rating of
     :math:`i`'s cluster. If the user is unknown, the prediction is
-    :math:`\\hat{r}_{ui} = \\mu_i`. If the item is unknown, the prediction is
-    :math:`\\hat{r}_{ui} = \\mu_u`. If both the user and the item are unknown,
-    the prediction is :math:`\\hat{r}_{ui} = \\mu`.
+    :math:`\hat{r}_{ui} = \\mu_i`. If the item is unknown, the prediction is
+    :math:`\hat{r}_{ui} = \\mu_u`. If both the user and the item are unknown,
+    the prediction is :math:`\hat{r}_{ui} = \\mu`.
 
     Clusters are assigned using a straightforward optimization method, much
     like k-means.
 
     Args:
        n_cltr_u(int): Number of user clusters. Default is ``3``.
        n_cltr_i(int): Number of item clusters. Default is ``3``.
@@ -182,21 +182,21 @@
         cdef np.ndarray[np.double_t] avg_cltr_i
         cdef np.ndarray[np.double_t, ndim=2] avg_cocltr
 
         cdef int u, i, r, uc, ic
         cdef double global_mean = self.trainset.global_mean
 
         # Initialize everything to zero
-        count_cltr_u = np.zeros(self.n_cltr_u, np.int_)
-        count_cltr_i = np.zeros(self.n_cltr_i, np.int_)
-        count_cocltr = np.zeros((self.n_cltr_u, self.n_cltr_i), np.int_)
-
-        sum_cltr_u = np.zeros(self.n_cltr_u, np.int_)
-        sum_cltr_i = np.zeros(self.n_cltr_i, np.int_)
-        sum_cocltr = np.zeros((self.n_cltr_u, self.n_cltr_i), np.int_)
+        count_cltr_u = np.zeros(self.n_cltr_u, np.int)
+        count_cltr_i = np.zeros(self.n_cltr_i, np.int)
+        count_cocltr = np.zeros((self.n_cltr_u, self.n_cltr_i), np.int)
+
+        sum_cltr_u = np.zeros(self.n_cltr_u, np.int)
+        sum_cltr_i = np.zeros(self.n_cltr_i, np.int)
+        sum_cocltr = np.zeros((self.n_cltr_u, self.n_cltr_i), np.int)
 
         avg_cltr_u = np.zeros(self.n_cltr_u, np.double)
         avg_cltr_i = np.zeros(self.n_cltr_i, np.double)
         avg_cocltr = np.zeros((self.n_cltr_u, self.n_cltr_i), np.double)
 
         # Compute counts and sums for every cluster.
         for u, i, r in self.trainset.all_ratings():
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/knns.py` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/knns.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 the :mod:`knns` module includes some k-NN inspired algorithms.
 """
 
-import heapq
-
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 import numpy as np
-
-from .algo_base import AlgoBase
+from six import iteritems
+import heapq
 
 from .predictions import PredictionImpossible
+from .algo_base import AlgoBase
 
 
 # Important note: as soon as an algorithm uses a similarity measure, it should
 # also allow the bsl_options parameter because of the pearson_baseline
-# similarity. It can be done explicitly (e.g. KNNBaseline), or implicetely
+# similarity. It can be done explicitely (e.g. KNNBaseline), or implicetely
 # using kwargs (e.g. KNNBasic).
 
-
 class SymmetricAlgo(AlgoBase):
     """This is an abstract class aimed to ease the use of symmetric algorithms.
 
-    A symmetric algorithm is an algorithm that can be based on users or on
+    A symmetric algorithm is an algorithm that can can be based on users or on
     items indifferently, e.g. all the algorithms in this module.
 
     When the algo is user-based x denotes a user and y an item. Else, it's
     reversed.
     """
 
     def __init__(self, sim_options={}, verbose=True, **kwargs):
@@ -32,47 +32,47 @@
         AlgoBase.__init__(self, sim_options=sim_options, **kwargs)
         self.verbose = verbose
 
     def fit(self, trainset):
 
         AlgoBase.fit(self, trainset)
 
-        ub = self.sim_options["user_based"]
+        ub = self.sim_options['user_based']
         self.n_x = self.trainset.n_users if ub else self.trainset.n_items
         self.n_y = self.trainset.n_items if ub else self.trainset.n_users
         self.xr = self.trainset.ur if ub else self.trainset.ir
         self.yr = self.trainset.ir if ub else self.trainset.ur
 
         return self
 
     def switch(self, u_stuff, i_stuff):
         """Return x_stuff and y_stuff depending on the user_based field."""
 
-        if self.sim_options["user_based"]:
+        if self.sim_options['user_based']:
             return u_stuff, i_stuff
         else:
             return i_stuff, u_stuff
 
 
 class KNNBasic(SymmetricAlgo):
     """A basic collaborative filtering algorithm.
 
     The prediction :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = \\frac{
-        \\sum\\limits_{v \\in N^k_i(u)} \\text{sim}(u, v) \\cdot r_{vi}}
-        {\\sum\\limits_{v \\in N^k_i(u)} \\text{sim}(u, v)}
+        \hat{r}_{ui} = \\frac{
+        \\sum\\limits_{v \in N^k_i(u)} \\text{sim}(u, v) \cdot r_{vi}}
+        {\\sum\\limits_{v \in N^k_i(u)} \\text{sim}(u, v)}
 
     or
 
     .. math::
-        \\hat{r}_{ui} = \\frac{
-        \\sum\\limits_{j \\in N^k_u(i)} \\text{sim}(i, j) \\cdot r_{uj}}
-        {\\sum\\limits_{j \\in N^k_u(i)} \\text{sim}(i, j)}
+        \hat{r}_{ui} = \\frac{
+        \\sum\\limits_{j \in N^k_u(i)} \\text{sim}(i, j) \cdot r_{uj}}
+        {\\sum\\limits_{j \in N^k_u(i)} \\text{sim}(i, j)}
 
     depending on the ``user_based`` field of the ``sim_options`` parameter.
 
     Args:
         k(int): The (max) number of neighbors to take into account for
             aggregation (see :ref:`this note <actual_k_note>`). Default is
             ``40``.
@@ -84,29 +84,30 @@
             options.
         verbose(bool): Whether to print trace messages of bias estimation,
             similarity, etc.  Default is True.
     """
 
     def __init__(self, k=40, min_k=1, sim_options={}, verbose=True, **kwargs):
 
-        SymmetricAlgo.__init__(self, sim_options=sim_options, verbose=verbose, **kwargs)
+        SymmetricAlgo.__init__(self, sim_options=sim_options, verbose=verbose,
+                               **kwargs)
         self.k = k
         self.min_k = min_k
 
     def fit(self, trainset):
 
         SymmetricAlgo.fit(self, trainset)
         self.sim = self.compute_similarities()
 
         return self
 
     def estimate(self, u, i):
 
         if not (self.trainset.knows_user(u) and self.trainset.knows_item(i)):
-            raise PredictionImpossible("User and/or item is unknown.")
+            raise PredictionImpossible('User and/or item is unkown.')
 
         x, y = self.switch(u, i)
 
         neighbors = [(self.sim[x, x2], r) for (x2, r) in self.yr[y]]
         k_neighbors = heapq.nlargest(self.k, neighbors, key=lambda t: t[0])
 
         # compute weighted average
@@ -114,81 +115,82 @@
         for (sim, r) in k_neighbors:
             if sim > 0:
                 sum_sim += sim
                 sum_ratings += sim * r
                 actual_k += 1
 
         if actual_k < self.min_k:
-            raise PredictionImpossible("Not enough neighbors.")
+            raise PredictionImpossible('Not enough neighbors.')
 
         est = sum_ratings / sum_sim
 
-        details = {"actual_k": actual_k}
+        details = {'actual_k': actual_k}
         return est, details
 
 
 class KNNWithMeans(SymmetricAlgo):
     """A basic collaborative filtering algorithm, taking into account the mean
     ratings of each user.
 
     The prediction :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = \\mu_u + \\frac{ \\sum\\limits_{v \\in N^k_i(u)}
-        \\text{sim}(u, v) \\cdot (r_{vi} - \\mu_v)} {\\sum\\limits_{v \\in
+        \hat{r}_{ui} = \mu_u + \\frac{ \\sum\\limits_{v \in N^k_i(u)}
+        \\text{sim}(u, v) \cdot (r_{vi} - \mu_v)} {\\sum\\limits_{v \in
         N^k_i(u)} \\text{sim}(u, v)}
 
     or
 
     .. math::
-        \\hat{r}_{ui} = \\mu_i + \\frac{ \\sum\\limits_{j \\in N^k_u(i)}
-        \\text{sim}(i, j) \\cdot (r_{uj} - \\mu_j)} {\\sum\\limits_{j \\in
+        \hat{r}_{ui} = \mu_i + \\frac{ \\sum\\limits_{j \in N^k_u(i)}
+        \\text{sim}(i, j) \cdot (r_{uj} - \mu_j)} {\\sum\\limits_{j \in
         N^k_u(i)} \\text{sim}(i, j)}
 
     depending on the ``user_based`` field of the ``sim_options`` parameter.
 
 
     Args:
         k(int): The (max) number of neighbors to take into account for
             aggregation (see :ref:`this note <actual_k_note>`). Default is
             ``40``.
         min_k(int): The minimum number of neighbors to take into account for
             aggregation. If there are not enough neighbors, the neighbor
             aggregation is set to zero (so the prediction ends up being
-            equivalent to the mean :math:`\\mu_u` or :math:`\\mu_i`). Default is
+            equivalent to the mean :math:`\mu_u` or :math:`\mu_i`). Default is
             ``1``.
         sim_options(dict): A dictionary of options for the similarity
             measure. See :ref:`similarity_measures_configuration` for accepted
             options.
         verbose(bool): Whether to print trace messages of bias estimation,
             similarity, etc.  Default is True.
     """
 
     def __init__(self, k=40, min_k=1, sim_options={}, verbose=True, **kwargs):
 
-        SymmetricAlgo.__init__(self, sim_options=sim_options, verbose=verbose, **kwargs)
+        SymmetricAlgo.__init__(self, sim_options=sim_options,
+                               verbose=verbose, **kwargs)
 
         self.k = k
         self.min_k = min_k
 
     def fit(self, trainset):
 
         SymmetricAlgo.fit(self, trainset)
         self.sim = self.compute_similarities()
 
         self.means = np.zeros(self.n_x)
-        for x, ratings in self.xr.items():
+        for x, ratings in iteritems(self.xr):
             self.means[x] = np.mean([r for (_, r) in ratings])
 
         return self
 
     def estimate(self, u, i):
 
         if not (self.trainset.knows_user(u) and self.trainset.knows_item(i)):
-            raise PredictionImpossible("User and/or item is unknown.")
+            raise PredictionImpossible('User and/or item is unkown.')
 
         x, y = self.switch(u, i)
 
         neighbors = [(x2, self.sim[x, x2], r) for (x2, r) in self.yr[y]]
         k_neighbors = heapq.nlargest(self.k, neighbors, key=lambda t: t[1])
 
         est = self.means[x]
@@ -205,36 +207,36 @@
             sum_ratings = 0
 
         try:
             est += sum_ratings / sum_sim
         except ZeroDivisionError:
             pass  # return mean
 
-        details = {"actual_k": actual_k}
+        details = {'actual_k': actual_k}
         return est, details
 
 
 class KNNBaseline(SymmetricAlgo):
     """A basic collaborative filtering algorithm taking into account a
     *baseline* rating.
 
 
     The prediction :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = b_{ui} + \\frac{ \\sum\\limits_{v \\in N^k_i(u)}
-        \\text{sim}(u, v) \\cdot (r_{vi} - b_{vi})} {\\sum\\limits_{v \\in
+        \hat{r}_{ui} = b_{ui} + \\frac{ \\sum\\limits_{v \in N^k_i(u)}
+        \\text{sim}(u, v) \cdot (r_{vi} - b_{vi})} {\\sum\\limits_{v \in
         N^k_i(u)} \\text{sim}(u, v)}
 
     or
 
 
     .. math::
-        \\hat{r}_{ui} = b_{ui} + \\frac{ \\sum\\limits_{j \\in N^k_u(i)}
-        \\text{sim}(i, j) \\cdot (r_{uj} - b_{uj})} {\\sum\\limits_{j \\in
+        \hat{r}_{ui} = b_{ui} + \\frac{ \\sum\\limits_{j \in N^k_u(i)}
+        \\text{sim}(i, j) \cdot (r_{uj} - b_{uj})} {\\sum\\limits_{j \in
         N^k_u(i)} \\text{sim}(i, j)}
 
     depending on the ``user_based`` field of the ``sim_options`` parameter. For
     the best predictions, use the :func:`pearson_baseline
     <surprise.similarities.pearson_baseline>` similarity measure.
 
     This algorithm corresponds to formula (3), section 2.2 of
@@ -257,25 +259,20 @@
             computation. See :ref:`baseline_estimates_configuration` for
             accepted options.
         verbose(bool): Whether to print trace messages of bias estimation,
             similarity, etc.  Default is True.
 
     """
 
-    def __init__(
-        self, k=40, min_k=1, sim_options={}, bsl_options={}, verbose=True, **kwargs
-    ):
-
-        SymmetricAlgo.__init__(
-            self,
-            sim_options=sim_options,
-            bsl_options=bsl_options,
-            verbose=verbose,
-            **kwargs
-        )
+    def __init__(self, k=40, min_k=1, sim_options={}, bsl_options={},
+                 verbose=True, **kwargs):
+
+        SymmetricAlgo.__init__(self, sim_options=sim_options,
+                               bsl_options=bsl_options, verbose=verbose,
+                               **kwargs)
 
         self.k = k
         self.min_k = min_k
 
     def fit(self, trainset):
 
         SymmetricAlgo.fit(self, trainset)
@@ -314,85 +311,87 @@
             sum_ratings = 0
 
         try:
             est += sum_ratings / sum_sim
         except ZeroDivisionError:
             pass  # just baseline again
 
-        details = {"actual_k": actual_k}
+        details = {'actual_k': actual_k}
         return est, details
 
 
 class KNNWithZScore(SymmetricAlgo):
     """A basic collaborative filtering algorithm, taking into account
-    the z-score normalization of each user.
+        the z-score normalization of each user.
 
     The prediction :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = \\mu_u + \\sigma_u \\frac{ \\sum\\limits_{v \\in N^k_i(u)}
-        \\text{sim}(u, v) \\cdot (r_{vi} - \\mu_v) / \\sigma_v} {\\sum\\limits_{v
-        \\in N^k_i(u)} \\text{sim}(u, v)}
+        \hat{r}_{ui} = \mu_u + \sigma_u \\frac{ \\sum\\limits_{v \in N^k_i(u)}
+        \\text{sim}(u, v) \cdot (r_{vi} - \mu_v) / \sigma_v} {\\sum\\limits_{v
+        \in N^k_i(u)} \\text{sim}(u, v)}
 
     or
 
     .. math::
-        \\hat{r}_{ui} = \\mu_i + \\sigma_i \\frac{ \\sum\\limits_{j \\in N^k_u(i)}
-        \\text{sim}(i, j) \\cdot (r_{uj} - \\mu_j) / \\sigma_j} {\\sum\\limits_{j
-        \\in N^k_u(i)} \\text{sim}(i, j)}
+        \hat{r}_{ui} = \mu_i + \sigma_i \\frac{ \\sum\\limits_{j \in N^k_u(i)}
+        \\text{sim}(i, j) \cdot (r_{uj} - \mu_j) / \sigma_j} {\\sum\\limits_{j
+        \in N^k_u(i)} \\text{sim}(i, j)}
 
     depending on the ``user_based`` field of the ``sim_options`` parameter.
 
-    If :math:`\\sigma` is 0, than the overall sigma is used in that case.
+    If :math:`\sigma` is 0, than the overall sigma is used in that case.
 
     Args:
         k(int): The (max) number of neighbors to take into account for
             aggregation (see :ref:`this note <actual_k_note>`). Default is
             ``40``.
         min_k(int): The minimum number of neighbors to take into account for
             aggregation. If there are not enough neighbors, the neighbor
             aggregation is set to zero (so the prediction ends up being
-            equivalent to the mean :math:`\\mu_u` or :math:`\\mu_i`). Default is
+            equivalent to the mean :math:`\mu_u` or :math:`\mu_i`). Default is
             ``1``.
         sim_options(dict): A dictionary of options for the similarity
             measure. See :ref:`similarity_measures_configuration` for accepted
             options.
         verbose(bool): Whether to print trace messages of bias estimation,
             similarity, etc.  Default is True.
     """
 
     def __init__(self, k=40, min_k=1, sim_options={}, verbose=True, **kwargs):
 
-        SymmetricAlgo.__init__(self, sim_options=sim_options, verbose=verbose, **kwargs)
+        SymmetricAlgo.__init__(self, sim_options=sim_options, verbose=verbose,
+                               **kwargs)
 
         self.k = k
         self.min_k = min_k
 
     def fit(self, trainset):
 
         SymmetricAlgo.fit(self, trainset)
 
         self.means = np.zeros(self.n_x)
         self.sigmas = np.zeros(self.n_x)
         # when certain sigma is 0, use overall sigma
-        self.overall_sigma = np.std([r for (_, _, r) in self.trainset.all_ratings()])
+        self.overall_sigma = np.std([r for (_, _, r)
+                                     in self.trainset.all_ratings()])
 
-        for x, ratings in self.xr.items():
+        for x, ratings in iteritems(self.xr):
             self.means[x] = np.mean([r for (_, r) in ratings])
             sigma = np.std([r for (_, r) in ratings])
             self.sigmas[x] = self.overall_sigma if sigma == 0.0 else sigma
 
         self.sim = self.compute_similarities()
 
         return self
 
     def estimate(self, u, i):
 
         if not (self.trainset.knows_user(u) and self.trainset.knows_item(i)):
-            raise PredictionImpossible("User and/or item is unknown.")
+            raise PredictionImpossible('User and/or item is unkown.')
 
         x, y = self.switch(u, i)
 
         neighbors = [(x2, self.sim[x, x2], r) for (x2, r) in self.yr[y]]
         k_neighbors = heapq.nlargest(self.k, neighbors, key=lambda t: t[1])
 
         est = self.means[x]
@@ -409,9 +408,9 @@
             sum_ratings = 0
 
         try:
             est += sum_ratings / sum_sim * self.sigmas[x]
         except ZeroDivisionError:
             pass  # return mean
 
-        details = {"actual_k": actual_k}
+        details = {'actual_k': actual_k}
         return est, details
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/matrix_factorization.pyx` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/matrix_factorization.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 """
 the :mod:`matrix_factorization` module includes some algorithms using matrix
 factorization.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+
 cimport numpy as np  # noqa
 import numpy as np
-from libc.math cimport sqrt
+from six.moves import range
 
 from .algo_base import AlgoBase
 from .predictions import PredictionImpossible
 from ..utils import get_rng
 
-import cython
-from libc.stdlib cimport malloc, free
-
 
 class SVD(AlgoBase):
     """The famous *SVD* algorithm, as popularized by `Simon Funk
-    <https://sifter.org/~simon/journal/20061211.html>`_ during the Netflix
+    <http://sifter.org/~simon/journal/20061211.html>`_ during the Netflix
     Prize. When baselines are not used, this is equivalent to Probabilistic
     Matrix Factorization :cite:`salakhutdinov2008a` (see :ref:`note
     <unbiased_note>` below).
 
     The prediction :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = \\mu + b_u + b_i + q_i^Tp_u
+        \hat{r}_{ui} = \mu + b_u + b_i + q_i^Tp_u
 
     If user :math:`u` is unknown, then the bias :math:`b_u` and the factors
     :math:`p_u` are assumed to be zero. The same applies for item :math:`i`
     with :math:`b_i` and :math:`q_i`.
 
     For details, see equation (5) from :cite:`Koren:2009`. See also
     :cite:`Ricci:2010`, section 5.3.1.
 
     To estimate all the unknown, we minimize the following regularized squared
     error:
 
     .. math::
-        \\sum_{r_{ui} \\in R_{train}} \\left(r_{ui} - \\hat{r}_{ui} \\right)^2 +
-        \\lambda\\left(b_i^2 + b_u^2 + ||q_i||^2 + ||p_u||^2\\right)
+        \sum_{r_{ui} \in R_{train}} \left(r_{ui} - \hat{r}_{ui} \\right)^2 +
+        \lambda\\left(b_i^2 + b_u^2 + ||q_i||^2 + ||p_u||^2\\right)
 
 
     The minimization is performed by a very straightforward stochastic gradient
     descent:
 
     .. math::
-        b_u &\\leftarrow b_u &+ \\gamma (e_{ui} - \\lambda b_u)\\\\
-        b_i &\\leftarrow b_i &+ \\gamma (e_{ui} - \\lambda b_i)\\\\
-        p_u &\\leftarrow p_u &+ \\gamma (e_{ui} \\cdot q_i - \\lambda p_u)\\\\
-        q_i &\\leftarrow q_i &+ \\gamma (e_{ui} \\cdot p_u - \\lambda q_i)
+        b_u &\\leftarrow b_u &+ \gamma (e_{ui} - \lambda b_u)\\\\
+        b_i &\\leftarrow b_i &+ \gamma (e_{ui} - \lambda b_i)\\\\
+        p_u &\\leftarrow p_u &+ \gamma (e_{ui} \\cdot q_i - \lambda p_u)\\\\
+        q_i &\\leftarrow q_i &+ \gamma (e_{ui} \\cdot p_u - \lambda q_i)
 
     where :math:`e_{ui} = r_{ui} - \\hat{r}_{ui}`. These steps are performed
     over all the ratings of the trainset and repeated ``n_epochs`` times.
     Baselines are initialized to ``0``. User and item factors are randomly
     initialized according to a normal distribution, which can be tuned using
     the ``init_mean`` and ``init_std_dev`` parameters.
 
-    You also have control over the learning rate :math:`\\gamma` and the
-    regularization term :math:`\\lambda`. Both can be different for each
+    You also have control over the learning rate :math:`\gamma` and the
+    regularization term :math:`\lambda`. Both can be different for each
     kind of parameter (see below). By default, learning rates are set to
     ``0.005`` and regularization terms are set to ``0.02``.
 
     .. _unbiased_note:
 
     .. note::
         You can choose to use an unbiased version of this algorithm, simply
         predicting:
 
         .. math::
-            \\hat{r}_{ui} = q_i^Tp_u
+            \hat{r}_{ui} = q_i^Tp_u
 
         This is equivalent to Probabilistic Matrix Factorization
         (:cite:`salakhutdinov2008a`, section 2) and can be achieved by setting
         the ``biased`` parameter to ``False``.
 
 
     Args:
@@ -186,73 +186,76 @@
 
         # A note on cythonization: I haven't dived into the details, but
         # accessing 2D arrays like pu using just one of the indices like pu[u]
         # is not efficient. That's why the old (cleaner) version can't be used
         # anymore, we need to compute the dot products by hand, and update
         # user and items factors by iterating over all factors...
 
-        rng = get_rng(self.random_state)
-
         # user biases
-        cdef double [::1] bu = np.zeros(trainset.n_users, dtype=np.double)
+        cdef np.ndarray[np.double_t] bu
         # item biases
-        cdef double [::1] bi = np.zeros(trainset.n_items, dtype=np.double)
+        cdef np.ndarray[np.double_t] bi
         # user factors
-        cdef double [:, ::1] pu = rng.normal(self.init_mean, self.init_std_dev, size=(trainset.n_users, self.n_factors))
+        cdef np.ndarray[np.double_t, ndim=2] pu
         # item factors
-        cdef double [:, ::1] qi = rng.normal(self.init_mean, self.init_std_dev, size=(trainset.n_items, self.n_factors))
+        cdef np.ndarray[np.double_t, ndim=2] qi
 
         cdef int u, i, f
-        cdef int n_factors = self.n_factors
-        cdef bint biased = self.biased
-
         cdef double r, err, dot, puf, qif
         cdef double global_mean = self.trainset.global_mean
 
         cdef double lr_bu = self.lr_bu
         cdef double lr_bi = self.lr_bi
         cdef double lr_pu = self.lr_pu
         cdef double lr_qi = self.lr_qi
 
         cdef double reg_bu = self.reg_bu
         cdef double reg_bi = self.reg_bi
         cdef double reg_pu = self.reg_pu
         cdef double reg_qi = self.reg_qi
 
-        if not biased:
+        rng = get_rng(self.random_state)
+
+        bu = np.zeros(trainset.n_users, np.double)
+        bi = np.zeros(trainset.n_items, np.double)
+        pu = rng.normal(self.init_mean, self.init_std_dev,
+                        (trainset.n_users, self.n_factors))
+        qi = rng.normal(self.init_mean, self.init_std_dev,
+                        (trainset.n_items, self.n_factors))
+
+        if not self.biased:
             global_mean = 0
 
         for current_epoch in range(self.n_epochs):
             if self.verbose:
                 print("Processing epoch {}".format(current_epoch))
-
             for u, i, r in trainset.all_ratings():
+
                 # compute current error
                 dot = 0  # <q_i, p_u>
-                for f in range(n_factors):
+                for f in range(self.n_factors):
                     dot += qi[i, f] * pu[u, f]
                 err = r - (global_mean + bu[u] + bi[i] + dot)
 
                 # update biases
-                if biased:
+                if self.biased:
                     bu[u] += lr_bu * (err - reg_bu * bu[u])
                     bi[i] += lr_bi * (err - reg_bi * bi[i])
 
                 # update factors
-                for f in range(n_factors):
+                for f in range(self.n_factors):
                     puf = pu[u, f]
                     qif = qi[i, f]
                     pu[u, f] += lr_pu * (err * qif - reg_pu * puf)
                     qi[i, f] += lr_qi * (err * puf - reg_qi * qif)
 
-        self.bu = np.asarray(bu)
-        self.bi = np.asarray(bi)
-        self.pu = np.asarray(pu)
-        self.qi = np.asarray(qi)
-    
+        self.bu = bu
+        self.bi = bi
+        self.pu = pu
+        self.qi = qi
 
     def estimate(self, u, i):
         # Should we cythonize this as well?
 
         known_user = self.trainset.knows_user(u)
         known_item = self.trainset.knows_item(i)
 
@@ -268,29 +271,28 @@
             if known_user and known_item:
                 est += np.dot(self.qi[i], self.pu[u])
 
         else:
             if known_user and known_item:
                 est = np.dot(self.qi[i], self.pu[u])
             else:
-                raise PredictionImpossible('User and item are unknown.')
+                raise PredictionImpossible('User and item are unkown.')
 
         return est
 
 
-@cython.cdivision(True)
 class SVDpp(AlgoBase):
     """The *SVD++* algorithm, an extension of :class:`SVD` taking into account
     implicit ratings.
 
     The prediction :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = \\mu + b_u + b_i + q_i^T\\left(p_u +
-        |I_u|^{-\\frac{1}{2}} \\sum_{j \\in I_u}y_j\\right)
+        \hat{r}_{ui} = \mu + b_u + b_i + q_i^T\\left(p_u +
+        |I_u|^{-\\frac{1}{2}} \sum_{j \\in I_u}y_j\\right)
 
     Where the :math:`y_j` terms are a new set of item factors that capture
     implicit ratings. Here, an implicit rating describes the fact that a user
     :math:`u` rated an item :math:`j`, regardless of the rating value.
 
     If user :math:`u` is unknown, then the bias :math:`b_u` and the factors
     :math:`p_u` are assumed to be zero. The same applies for item :math:`i`
@@ -303,26 +305,23 @@
     Just as for :class:`SVD`, the parameters are learned using a SGD on the
     regularized squared error objective.
 
     Baselines are initialized to ``0``. User and item factors are randomly
     initialized according to a normal distribution, which can be tuned using
     the ``init_mean`` and ``init_std_dev`` parameters.
 
-    You have control over the learning rate :math:`\\gamma` and the
-    regularization term :math:`\\lambda`. Both can be different for each
+    You have control over the learning rate :math:`\gamma` and the
+    regularization term :math:`\lambda`. Both can be different for each
     kind of parameter (see below). By default, learning rates are set to
     ``0.005`` and regularization terms are set to ``0.02``.
 
     Args:
         n_factors: The number of factors. Default is ``20``.
         n_epochs: The number of iteration of the SGD procedure. Default is
             ``20``.
-        cache_ratings: Whether or not to cache ratings during `fit()`.
-            This should speed-up the training, and has a higher
-            memory footprint. Default is False.
         init_mean: The mean of the normal distribution for factor vectors
             initialization. Default is ``0``.
         init_std_dev: The standard deviation of the normal distribution for
             factor vectors initialization. Default is ``0.1``.
         lr_all: The learning rate for all parameters. Default is ``0.007``.
         reg_all: The regularization term for all parameters. Default is
             ``0.02``.
@@ -367,16 +366,15 @@
         bi(numpy array of size (n_items)): The item biases (only
             exists if ``fit()`` has been called)
     """
 
     def __init__(self, n_factors=20, n_epochs=20, init_mean=0, init_std_dev=.1,
                  lr_all=.007, reg_all=.02, lr_bu=None, lr_bi=None, lr_pu=None,
                  lr_qi=None, lr_yj=None, reg_bu=None, reg_bi=None, reg_pu=None,
-                 reg_qi=None, reg_yj=None, random_state=None, verbose=False,
-                 cache_ratings=False):
+                 reg_qi=None, reg_yj=None, random_state=None, verbose=False):
 
         self.n_factors = n_factors
         self.n_epochs = n_epochs
         self.init_mean = init_mean
         self.init_std_dev = init_std_dev
         self.lr_bu = lr_bu if lr_bu is not None else lr_all
         self.lr_bi = lr_bi if lr_bi is not None else lr_all
@@ -386,142 +384,109 @@
         self.reg_bu = reg_bu if reg_bu is not None else reg_all
         self.reg_bi = reg_bi if reg_bi is not None else reg_all
         self.reg_pu = reg_pu if reg_pu is not None else reg_all
         self.reg_qi = reg_qi if reg_qi is not None else reg_all
         self.reg_yj = reg_yj if reg_yj is not None else reg_all
         self.random_state = random_state
         self.verbose = verbose
-        self.cache_ratings = cache_ratings
 
         AlgoBase.__init__(self)
 
     def fit(self, trainset):
 
         AlgoBase.fit(self, trainset)
         self.sgd(trainset)
 
         return self
 
     def sgd(self, trainset):
 
-        rng = get_rng(self.random_state)
-
         # user biases
-        cdef double [::1] bu = np.zeros(trainset.n_users, dtype=np.double)
+        cdef np.ndarray[np.double_t] bu
         # item biases
-        cdef double [::1] bi = np.zeros(trainset.n_items, dtype=np.double)
+        cdef np.ndarray[np.double_t] bi
         # user factors
-        cdef double [:, ::1] pu = rng.normal(self.init_mean, self.init_std_dev, size=(trainset.n_users, self.n_factors))
+        cdef np.ndarray[np.double_t, ndim=2] pu
         # item factors
-        cdef double [:, ::1] qi = rng.normal(self.init_mean, self.init_std_dev, size=(trainset.n_items, self.n_factors))
+        cdef np.ndarray[np.double_t, ndim=2] qi
         # item implicit factors
-        cdef double [:, ::1] yj = rng.normal(self.init_mean, self.init_std_dev, size=(trainset.n_items, self.n_factors))
+        cdef np.ndarray[np.double_t, ndim=2] yj
 
-        cdef double [::1] u_impl_fdb = np.zeros(self.n_factors, dtype=np.double)
-
-        cdef int u, i, j, f, k, Iu_length
-        cdef int max_Iu_length = 0
-        cdef int n_factors = self.n_factors
-        cdef bint cache_ratings = self.cache_ratings
+        cdef int u, i, j, f
         cdef double r, err, dot, puf, qif, sqrt_Iu, _
         cdef double global_mean = self.trainset.global_mean
+        cdef np.ndarray[np.double_t] u_impl_fdb
 
         cdef double lr_bu = self.lr_bu
         cdef double lr_bi = self.lr_bi
         cdef double lr_pu = self.lr_pu
         cdef double lr_qi = self.lr_qi
         cdef double lr_yj = self.lr_yj
 
         cdef double reg_bu = self.reg_bu
         cdef double reg_bi = self.reg_bi
         cdef double reg_pu = self.reg_pu
         cdef double reg_qi = self.reg_qi
         cdef double reg_yj = self.reg_yj
-        cdef double err_qif_sqrt = 0.0
 
-        cdef int ** Iu_cached = NULL
-        cdef int * Iu = NULL
-        cdef int * Iu_lengths = NULL
-
-        if cache_ratings:
-            Iu_cached = <int **>malloc(trainset.n_users * sizeof(int *))
-            Iu_lengths = <int *>malloc(trainset.n_users * sizeof(int))
-            for u in range(trainset.n_users):
-                Iu_lengths[u] = len(trainset.ur[u])
-                Iu_cached[u] = <int *>malloc(Iu_lengths[u] * sizeof(int))
-                for k, (j, _) in enumerate(trainset.ur[u]):
-                    Iu_cached[u][k] = j
-        else:
-            for u in range(trainset.n_users):
-                # Might as well allocate the max size once and for all
-                # instead of allocating the exact size each time
-                max_Iu_length = max(max_Iu_length, len(trainset.ur[u]))
-                Iu = <int *>malloc(max_Iu_length * sizeof(int))
+        bu = np.zeros(trainset.n_users, np.double)
+        bi = np.zeros(trainset.n_items, np.double)
+
+        rng = get_rng(self.random_state)
+
+        pu = rng.normal(self.init_mean, self.init_std_dev,
+                        (trainset.n_users, self.n_factors))
+        qi = rng.normal(self.init_mean, self.init_std_dev,
+                        (trainset.n_items, self.n_factors))
+        yj = rng.normal(self.init_mean, self.init_std_dev,
+                        (trainset.n_items, self.n_factors))
+        u_impl_fdb = np.zeros(self.n_factors, np.double)
 
         for current_epoch in range(self.n_epochs):
             if self.verbose:
                 print(" processing epoch {}".format(current_epoch))
-
             for u, i, r in trainset.all_ratings():
 
-                # items rated by u.
-                if cache_ratings:
-                    Iu = Iu_cached[u]
-                    Iu_length = Iu_lengths[u]
-                else:
-                    for k, (j, _) in enumerate(trainset.ur[u]):
-                        Iu[k] = j
-                    Iu_length = k + 1
-
-                sqrt_Iu = sqrt(Iu_length)
+                # items rated by u. This is COSTLY
+                Iu = [j for (j, _) in trainset.ur[u]]
+                sqrt_Iu = np.sqrt(len(Iu))
 
                 # compute user implicit feedback
-                # for f in range(n_factors):
-                u_impl_fdb[:] = 0
-
-                for k in range(Iu_length):
-                    j = Iu[k]
-                    for f in range(n_factors):
+                u_impl_fdb = np.zeros(self.n_factors, np.double)
+                for j in Iu:
+                    for f in range(self.n_factors):
                         u_impl_fdb[f] += yj[j, f] / sqrt_Iu
-                
+
                 # compute current error
-                dot = 0 
-                for f in range(n_factors):
+                dot = 0  # <q_i, (p_u + sum_{j in Iu} y_j / sqrt{Iu}>
+                for f in range(self.n_factors):
                     dot += qi[i, f] * (pu[u, f] + u_impl_fdb[f])
 
                 err = r - (global_mean + bu[u] + bi[i] + dot)
 
                 # update biases
                 bu[u] += lr_bu * (err - reg_bu * bu[u])
                 bi[i] += lr_bi * (err - reg_bi * bi[i])
 
                 # update factors
-                for f in range(n_factors):
+                for f in range(self.n_factors):
                     puf = pu[u, f]
                     qif = qi[i, f]
                     pu[u, f] += lr_pu * (err * qif - reg_pu * puf)
-                    qi[i, f] += lr_qi * (err * (puf + u_impl_fdb[f]) - reg_qi * qif)
-                    err_qif_sqrt = err * qif / sqrt_Iu
-                    for k in range(Iu_length):
-                        j = Iu[k]
-                        yj[j, f] += lr_yj * (err_qif_sqrt - reg_yj * yj[j, f])
-
-        if cache_ratings:
-            for u in range(trainset.n_users):
-                free(Iu_cached[u])
-            free(Iu_cached)
-            free(Iu_lengths)
-        else:
-            free(Iu)
-
-        self.bu = np.asarray(bu)
-        self.bi = np.asarray(bi)
-        self.pu = np.asarray(pu)
-        self.qi = np.asarray(qi)
-        self.yj = np.asarray(yj)
+                    qi[i, f] += lr_qi * (err * (puf + u_impl_fdb[f]) -
+                                         reg_qi * qif)
+                    for j in Iu:
+                        yj[j, f] += lr_yj * (err * qif / sqrt_Iu -
+                                             reg_yj * yj[j, f])
+
+        self.bu = bu
+        self.bi = bi
+        self.pu = pu
+        self.qi = qi
+        self.yj = yj
 
     def estimate(self, u, i):
 
         est = self.trainset.global_mean
 
         if self.trainset.knows_user(u):
             est += self.bu[u]
@@ -542,63 +507,63 @@
     """A collaborative filtering algorithm based on Non-negative Matrix
     Factorization.
 
     This algorithm is very similar to :class:`SVD`. The prediction
     :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = q_i^Tp_u,
+        \hat{r}_{ui} = q_i^Tp_u,
 
     where user and item factors are kept **positive**. Our implementation
     follows that suggested in :cite:`NMF:2014`, which is equivalent to
     :cite:`Zhang96` in its non-regularized form. Both are direct applications
     of NMF for dense matrices :cite:`NMF_algo`.
 
     The optimization procedure is a (regularized) stochastic gradient descent
     with a specific choice of step size that ensures non-negativity of factors,
     provided that their initial values are also positive.
 
     At each step of the SGD procedure, the factors :math:`f` or user :math:`u`
     and item :math:`i` are updated as follows:
 
     .. math::
-        p_{uf} &\\leftarrow p_{uf} &\\cdot \\frac{\\sum_{i \\in I_u} q_{if}
-        \\cdot r_{ui}}{\\sum_{i \\in I_u} q_{if} \\cdot \\hat{r_{ui}} +
+        p_{uf} &\\leftarrow p_{uf} &\cdot \\frac{\\sum_{i \in I_u} q_{if}
+        \\cdot r_{ui}}{\\sum_{i \in I_u} q_{if} \\cdot \\hat{r_{ui}} +
         \\lambda_u |I_u| p_{uf}}\\\\
-        q_{if} &\\leftarrow q_{if} &\\cdot \\frac{\\sum_{u \\in U_i} p_{uf}
-        \\cdot r_{ui}}{\\sum_{u \\in U_i} p_{uf} \\cdot \\hat{r_{ui}} +
-        \\lambda_i |U_i| q_{if}}\\\\
+        q_{if} &\\leftarrow q_{if} &\cdot \\frac{\\sum_{u \in U_i} p_{uf}
+        \\cdot r_{ui}}{\\sum_{u \in U_i} p_{uf} \\cdot \\hat{r_{ui}} +
+        \lambda_i |U_i| q_{if}}\\\\
 
-    where :math:`\\lambda_u` and :math:`\\lambda_i` are regularization
+    where :math:`\lambda_u` and :math:`\lambda_i` are regularization
     parameters.
 
     This algorithm is highly dependent on initial values. User and item factors
     are uniformly initialized between ``init_low`` and ``init_high``. Change
     them at your own risks!
 
     A biased version is available by setting the ``biased`` parameter to
     ``True``. In this case, the prediction is set as
 
     .. math::
-        \\hat{r}_{ui} = \\mu + b_u + b_i + q_i^Tp_u,
+        \hat{r}_{ui} = \mu + b_u + b_i + q_i^Tp_u,
 
     still ensuring positive factors. Baselines are optimized in the same way as
     in the :class:`SVD` algorithm. While yielding better accuracy, the biased
     version seems highly prone to overfitting so you may want to reduce the
     number of factors (or increase regularization).
 
     Args:
         n_factors: The number of factors. Default is ``15``.
         n_epochs: The number of iteration of the SGD procedure. Default is
             ``50``.
         biased(bool): Whether to use baselines (or biases). Default is
             ``False``.
-        reg_pu: The regularization term for users :math:`\\lambda_u`. Default is
+        reg_pu: The regularization term for users :math:`\lambda_u`. Default is
             ``0.06``.
-        reg_qi: The regularization term for items :math:`\\lambda_i`. Default is
+        reg_qi: The regularization term for items :math:`\lambda_i`. Default is
             ``0.06``.
         reg_bu: The regularization term for :math:`b_u`. Only relevant for
             biased version. Default is ``0.02``.
         reg_bi: The regularization term for :math:`b_i`. Only relevant for
             biased version. Default is ``0.02``.
         lr_bu: The learning rate for :math:`b_u`. Only relevant for biased
             version. Default is ``0.005``.
@@ -657,99 +622,102 @@
         AlgoBase.fit(self, trainset)
         self.sgd(trainset)
 
         return self
 
     def sgd(self, trainset):
 
-        rng = get_rng(self.random_state)
-
         # user and item factors
-        cdef double [:, ::1] pu = rng.uniform(self.init_low, self.init_high, size=(trainset.n_users, self.n_factors))
-        cdef double [:, ::1] qi = rng.uniform(self.init_low, self.init_high, size=(trainset.n_items, self.n_factors))
+        cdef np.ndarray[np.double_t, ndim=2] pu
+        cdef np.ndarray[np.double_t, ndim=2] qi
 
         # user and item biases
-        cdef double [::1] bu = np.zeros(trainset.n_users, dtype=np.double)
-        cdef double [::1] bi = np.zeros(trainset.n_items, dtype=np.double)
+        cdef np.ndarray[np.double_t] bu
+        cdef np.ndarray[np.double_t] bi
+
+        # auxiliary matrices used in optimization process
+        cdef np.ndarray[np.double_t, ndim=2] user_num
+        cdef np.ndarray[np.double_t, ndim=2] user_denom
+        cdef np.ndarray[np.double_t, ndim=2] item_num
+        cdef np.ndarray[np.double_t, ndim=2] item_denom
 
         cdef int u, i, f
-        cdef int n_factors = self.n_factors
         cdef double r, est, l, dot, err
         cdef double reg_pu = self.reg_pu
         cdef double reg_qi = self.reg_qi
         cdef double reg_bu = self.reg_bu
         cdef double reg_bi = self.reg_bi
         cdef double lr_bu = self.lr_bu
         cdef double lr_bi = self.lr_bi
         cdef double global_mean = self.trainset.global_mean
 
-        # auxiliary matrices used in optimization process
-        cdef double [:, ::1] user_num = np.zeros((trainset.n_users, n_factors))
-        cdef double [:, ::1] user_denom = np.zeros((trainset.n_users, n_factors))
-        cdef double [:, ::1] item_num = np.zeros((trainset.n_items, n_factors))
-        cdef double [:, ::1] item_denom = np.zeros((trainset.n_items, n_factors))
+        # Randomly initialize user and item factors
+        rng = get_rng(self.random_state)
+        pu = rng.uniform(self.init_low, self.init_high,
+                         size=(trainset.n_users, self.n_factors))
+        qi = rng.uniform(self.init_low, self.init_high,
+                         size=(trainset.n_items, self.n_factors))
 
+        bu = np.zeros(trainset.n_users, np.double)
+        bi = np.zeros(trainset.n_items, np.double)
 
         if not self.biased:
             global_mean = 0
 
         for current_epoch in range(self.n_epochs):
 
             if self.verbose:
                 print("Processing epoch {}".format(current_epoch))
 
             # (re)initialize nums and denoms to zero
-            # TODO: Use fill or memset??
-            user_num[:, :] = 0
-            user_denom[:, :] = 0
-            item_num[:, :] = 0
-            item_denom[:, :] = 0
+            user_num = np.zeros((trainset.n_users, self.n_factors))
+            user_denom = np.zeros((trainset.n_users, self.n_factors))
+            item_num = np.zeros((trainset.n_items, self.n_factors))
+            item_denom = np.zeros((trainset.n_items, self.n_factors))
 
             # Compute numerators and denominators for users and items factors
             for u, i, r in trainset.all_ratings():
 
                 # compute current estimation and error
                 dot = 0  # <q_i, p_u>
-                for f in range(n_factors):
+                for f in range(self.n_factors):
                     dot += qi[i, f] * pu[u, f]
                 est = global_mean + bu[u] + bi[i] + dot
                 err = r - est
 
                 # update biases
                 if self.biased:
                     bu[u] += lr_bu * (err - reg_bu * bu[u])
                     bi[i] += lr_bi * (err - reg_bi * bi[i])
 
                 # compute numerators and denominators
-                for f in range(n_factors):
+                for f in range(self.n_factors):
                     user_num[u, f] += qi[i, f] * r
                     user_denom[u, f] += qi[i, f] * est
                     item_num[i, f] += pu[u, f] * r
                     item_denom[i, f] += pu[u, f] * est
 
             # Update user factors
             for u in trainset.all_users():
                 n_ratings = len(trainset.ur[u])
-                for f in range(n_factors):
-                    if pu[u, f] != 0:  # Can happen if user only has 0 ratings
-                        user_denom[u, f] += n_ratings * reg_pu * pu[u, f]
-                        pu[u, f] *= user_num[u, f] / user_denom[u, f]
+                for f in range(self.n_factors):
+                    user_denom[u, f] += n_ratings * reg_pu * pu[u, f]
+                    pu[u, f] *= user_num[u, f] / user_denom[u, f]
 
             # Update item factors
             for i in trainset.all_items():
                 n_ratings = len(trainset.ir[i])
-                for f in range(n_factors):
-                    if qi[i, f] != 0:
-                        item_denom[i, f] += n_ratings * reg_qi * qi[i, f]
-                        qi[i, f] *= item_num[i, f] / item_denom[i, f]
-
-        self.bu = np.asarray(bu)
-        self.bi = np.asarray(bi)
-        self.pu = np.asarray(pu)
-        self.qi = np.asarray(qi)
+                for f in range(self.n_factors):
+                    item_denom[i, f] += n_ratings * reg_qi * qi[i, f]
+                    qi[i, f] *= item_num[i, f] / item_denom[i, f]
+
+        self.bu = bu
+        self.bi = bi
+        self.pu = pu
+        self.qi = qi
 
     def estimate(self, u, i):
         # Should we cythonize this as well?
 
         known_user = self.trainset.knows_user(u)
         known_item = self.trainset.knows_item(i)
 
@@ -765,10 +733,10 @@
             if known_user and known_item:
                 est += np.dot(self.qi[i], self.pu[u])
 
         else:
             if known_user and known_item:
                 est = np.dot(self.qi[i], self.pu[u])
             else:
-                raise PredictionImpossible('User and item are unknown.')
+                raise PredictionImpossible('User and item are unkown.')
 
         return est
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/optimize_baselines.pyx` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/optimize_baselines.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 This module includes the two methods for baseline computation: stochastic
 gradient descent and alternating least squares.
 """
 
-
-
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 cimport numpy as np  # noqa
 import numpy as np
+from six.moves import range
 
 
 def baseline_als(self):
     """Optimize biases using ALS.
 
     Args:
         self: The algorithm that needs to compute baselines.
@@ -21,16 +22,16 @@
     """
 
     # This piece of code is largely inspired by that of MyMediaLite:
     # https://github.com/zenogantner/MyMediaLite/blob/master/src/MyMediaLite/RatingPrediction/UserItemBaseline.cs
     # see also https://www.youtube.com/watch?v=gCaOa3W9kM0&t=32m55s
     # (Alex Smola on RS, ML Class 10-701)
 
-    cdef double [::1] bu = np.zeros(self.trainset.n_users)
-    cdef double [::1] bi = np.zeros(self.trainset.n_items)
+    cdef np.ndarray[np.double_t] bu = np.zeros(self.trainset.n_users)
+    cdef np.ndarray[np.double_t] bi = np.zeros(self.trainset.n_items)
 
     cdef int u, i
     cdef double r, err, dev_i, dev_u
     cdef double global_mean = self.trainset.global_mean
 
     cdef int n_epochs = self.bsl_options.get('n_epochs', 10)
     cdef double reg_u = self.bsl_options.get('reg_u', 15)
@@ -46,29 +47,29 @@
 
         for u in self.trainset.all_users():
             dev_u = 0
             for (i, r) in self.trainset.ur[u]:
                 dev_u += r - global_mean - bi[i]
             bu[u] = dev_u / (reg_u + len(self.trainset.ur[u]))
 
-    return np.asarray(bu), np.asarray(bi)
+    return bu, bi
 
 
 def baseline_sgd(self):
     """Optimize biases using SGD.
 
     Args:
         self: The algorithm that needs to compute baselines.
 
     Returns:
         A tuple ``(bu, bi)``, which are users and items baselines.
     """
 
-    cdef double [::1] bu = np.zeros(self.trainset.n_users)
-    cdef double [::1] bi = np.zeros(self.trainset.n_items)
+    cdef np.ndarray[np.double_t] bu = np.zeros(self.trainset.n_users)
+    cdef np.ndarray[np.double_t] bi = np.zeros(self.trainset.n_items)
 
     cdef int u, i
     cdef double r, err
     cdef double global_mean = self.trainset.global_mean
 
     cdef int n_epochs = self.bsl_options.get('n_epochs', 20)
     cdef double reg = self.bsl_options.get('reg', 0.02)
@@ -76,8 +77,8 @@
 
     for dummy in range(n_epochs):
         for u, i, r in self.trainset.all_ratings():
             err = (r - (global_mean + bu[u] + bi[i]))
             bu[u] += lr * (err - reg * bu[u])
             bi[i] += lr * (err - reg * bi[i])
 
-    return np.asarray(bu), np.asarray(bi)
+    return bu, bi
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/predictions.py` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/predictions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 The :mod:`surprise.prediction_algorithms.predictions` module defines the
 :class:`Prediction` named tuple and the :class:`PredictionImpossible`
 exception.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 from collections import namedtuple
 
 
 class PredictionImpossible(Exception):
-    r"""Exception raised when a prediction is impossible.
+    """Exception raised when a prediction is impossible.
 
     When raised, the estimation :math:`\hat{r}_{ui}` is set to the global mean
     of all ratings :math:`\mu`.
     """
 
     pass
 
 
-class Prediction(namedtuple("Prediction", ["uid", "iid", "r_ui", "est", "details"])):
+class Prediction(namedtuple('Prediction',
+                            ['uid', 'iid', 'r_ui', 'est', 'details'])):
     """A named tuple for storing the results of a prediction.
 
     It's wrapped in a class, but only for documentation and printing purposes.
 
     Args:
         uid: The (raw) user id. See :ref:`this note<raw_inner_note>`.
         iid: The (raw) item id. See :ref:`this note<raw_inner_note>`.
@@ -31,17 +34,17 @@
         details (dict): Stores additional details about the prediction that
             might be useful for later analysis.
     """
 
     __slots__ = ()  # for memory saving purpose.
 
     def __str__(self):
-        s = f"user: {self.uid:<10} "
-        s += f"item: {self.iid:<10} "
+        s = 'user: {uid:<10} '.format(uid=self.uid)
+        s += 'item: {iid:<10} '.format(iid=self.iid)
         if self.r_ui is not None:
-            s += f"r_ui = {self.r_ui:1.2f}   "
+            s += 'r_ui = {r_ui:1.2f}   '.format(r_ui=self.r_ui)
         else:
-            s += "r_ui = None   "
-        s += f"est = {self.est:1.2f}   "
+            s += 'r_ui = None   '
+        s += 'est = {est:1.2f}   '.format(est=self.est)
         s += str(self.details)
 
         return s
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/random_pred.py` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/random_pred.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """ Algorithm predicting a random rating.
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 import numpy as np
 
 from .algo_base import AlgoBase
 
 
 class NormalPredictor(AlgoBase):
     """Algorithm predicting a random rating based on the distribution of the
     training set, which is assumed to be normal.
 
-    The prediction :math:`\\hat{r}_{ui}` is generated from a normal distribution
-    :math:`\\mathcal{N}(\\hat{\\mu}, \\hat{\\sigma}^2)` where :math:`\\hat{\\mu}` and
-    :math:`\\hat{\\sigma}` are estimated from the training data using Maximum
+    The prediction :math:`\hat{r}_{ui}` is generated from a normal distribution
+    :math:`\mathcal{N}(\hat{\mu}, \hat{\sigma}^2)` where :math:`\hat{\mu}` and
+    :math:`\hat{\sigma}` are estimated from the training data using Maximum
     Likelihood Estimation:
 
     .. math::
-        \\hat{\\mu} &= \\frac{1}{|R_{train}|} \\sum_{r_{ui} \\in R_{train}}
+        \\hat{\mu} &= \\frac{1}{|R_{train}|} \\sum_{r_{ui} \\in R_{train}}
         r_{ui}\\\\\\\\\
-        \\hat{\\sigma} &= \\sqrt{\\sum_{r_{ui} \\in R_{train}}
-        \\frac{(r_{ui} - \\hat{\\mu})^2}{|R_{train}|}}
+        \\hat{\sigma} &= \\sqrt{\\sum_{r_{ui} \\in R_{train}}
+        \\frac{(r_{ui} - \\hat{\mu})^2}{|R_{train}|}}
     """
 
     def __init__(self):
 
         AlgoBase.__init__(self)
 
     def fit(self, trainset):
 
         AlgoBase.fit(self, trainset)
 
-        num = sum(
-            (r - self.trainset.global_mean) ** 2
-            for (_, _, r) in self.trainset.all_ratings()
-        )
+        num = sum((r - self.trainset.global_mean)**2
+                  for (_, _, r) in self.trainset.all_ratings())
         denum = self.trainset.n_ratings
         self.sigma = np.sqrt(num / denum)
 
         return self
 
     def estimate(self, *_):
```

### Comparing `scikit_surprise-1.1.4/surprise/prediction_algorithms/slope_one.pyx` & `scikit-surprise-1.1rc0/surprise/prediction_algorithms/slope_one.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,92 @@
 """
 the :mod:`slope_one` module includes the :class:`SlopeOne` algorithm.
 """
 
-
-
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 cimport numpy as np  # noqa
 import numpy as np
+from six.moves import range
+from six import iteritems
 
 from .algo_base import AlgoBase
 from .predictions import PredictionImpossible
 
 
 class SlopeOne(AlgoBase):
     """A simple yet accurate collaborative filtering algorithm.
 
     This is a straightforward implementation of the SlopeOne algorithm
     :cite:`lemire2007a`.
 
     The prediction :math:`\\hat{r}_{ui}` is set as:
 
     .. math::
-        \\hat{r}_{ui} = \\mu_u + \\frac{1}{
+        \hat{r}_{ui} = \\mu_u + \\frac{1}{
         |R_i(u)|}
-        \\sum\\limits_{j \\in R_i(u)} \\text{dev}(i, j),
+        \\sum\\limits_{j \in R_i(u)} \\text{dev}(i, j),
 
     where :math:`R_i(u)` is the set of relevant items, i.e. the set of items
     :math:`j` rated by :math:`u` that also have at least one common user with
     :math:`i`. :math:`\\text{dev}_(i, j)` is defined as the average difference
     between the ratings of :math:`i` and those of :math:`j`:
 
     .. math::
         \\text{dev}(i, j) = \\frac{1}{
-        |U_{ij}|}\\sum\\limits_{u \\in U_{ij}} r_{ui} - r_{uj}
+        |U_{ij}|}\\sum\\limits_{u \in U_{ij}} r_{ui} - r_{uj}
     """
 
     def __init__(self):
 
         AlgoBase.__init__(self)
 
     def fit(self, trainset):
 
-        cdef int n_items = trainset.n_items
+        n_items = trainset.n_items
 
         # Number of users having rated items i and j: |U_ij|
-        cdef long [:, ::1] freq = np.zeros((trainset.n_items, trainset.n_items), np.int_)
+        cdef np.ndarray[np.int_t, ndim=2] freq
         # Deviation from item i to item j: mean(r_ui - r_uj for u in U_ij)
-        cdef double [:, ::1] dev = np.zeros((trainset.n_items, trainset.n_items), np.double)
+        cdef np.ndarray[np.double_t, ndim=2] dev
+
         cdef int u, i, j, r_ui, r_uj
 
         AlgoBase.fit(self, trainset)
 
+        freq = np.zeros((trainset.n_items, trainset.n_items), np.int)
+        dev = np.zeros((trainset.n_items, trainset.n_items), np.double)
+
         # Computation of freq and dev arrays.
-        for u, u_ratings in trainset.ur.items():
+        for u, u_ratings in iteritems(trainset.ur):
             for i, r_ui in u_ratings:
                 for j, r_uj in u_ratings:
                     freq[i, j] += 1
                     dev[i, j] += r_ui - r_uj
 
         for i in range(n_items):
             dev[i, i] = 0
             for j in range(i + 1, n_items):
                 dev[i, j] /= freq[i, j]
                 dev[j, i] = -dev[i, j]
 
-        self.freq = np.asarray(freq)
-        self.dev = np.asarray(dev)
+        self.freq = freq
+        self.dev = dev
 
         # mean ratings of all users: mu_u
         self.user_mean = [np.mean([r for (_, r) in trainset.ur[u]])
                           for u in trainset.all_users()]
 
         return self
 
     def estimate(self, u, i):
 
         if not (self.trainset.knows_user(u) and self.trainset.knows_item(i)):
-            raise PredictionImpossible('User and/or item is unknown.')
+            raise PredictionImpossible('User and/or item is unkown.')
 
         # Ri: relevant items for i. This is the set of items j rated by u that
         # also have common users with i (i.e. at least one user has rated both
         # i and j).
         Ri = [j for (j, _) in self.trainset.ur[u] if self.freq[i, j] > 0]
         est = self.user_mean[u]
         if Ri:
```

### Comparing `scikit_surprise-1.1.4/surprise/reader.py` & `scikit-surprise-1.1rc0/surprise/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-"""This module contains the Reader class."""
+'''This module contains the Reader class.'''
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 from .builtin_datasets import BUILTIN_DATASETS
 
 
-class Reader:
+class Reader():
     """The Reader class is used to parse a file containing ratings.
 
     Such a file is assumed to specify only one rating per line, and each line
     needs to respect the following structure: ::
 
         user ; item ; rating ; [timestamp]
 
@@ -34,76 +36,68 @@
         rating_scale(:obj:`tuple`, optional): The rating scale used for every
             rating.  Default is ``(1, 5)``.
         skip_lines(:obj:`int`, optional): Number of lines to skip at the
             beginning of the file. Default is ``0``.
 
     """
 
-    def __init__(
-        self,
-        name=None,
-        line_format="user item rating",
-        sep=None,
-        rating_scale=(1, 5),
-        skip_lines=0,
-    ):
+    def __init__(self, name=None, line_format='user item rating', sep=None,
+                 rating_scale=(1, 5), skip_lines=0):
 
         if name:
             try:
                 self.__init__(**BUILTIN_DATASETS[name].reader_params)
             except KeyError:
-                raise ValueError(
-                    "unknown reader "
-                    + name
-                    + ". Accepted values are "
-                    + ", ".join(BUILTIN_DATASETS.keys())
-                    + "."
-                )
+                raise ValueError('unknown reader ' + name +
+                                 '. Accepted values are ' +
+                                 ', '.join(BUILTIN_DATASETS.keys()) + '.')
         else:
             self.sep = sep
             self.skip_lines = skip_lines
             self.rating_scale = rating_scale
 
             lower_bound, higher_bound = rating_scale
 
             splitted_format = line_format.split()
 
-            entities = ["user", "item", "rating"]
-            if "timestamp" in splitted_format:
+            entities = ['user', 'item', 'rating']
+            if 'timestamp' in splitted_format:
                 self.with_timestamp = True
-                entities.append("timestamp")
+                entities.append('timestamp')
             else:
                 self.with_timestamp = False
 
             # check that all fields are correct
             if any(field not in entities for field in splitted_format):
-                raise ValueError("line_format parameter is incorrect.")
+                raise ValueError('line_format parameter is incorrect.')
 
-            self.indexes = [splitted_format.index(entity) for entity in entities]
+            self.indexes = [splitted_format.index(entity) for entity in
+                            entities]
 
     def parse_line(self, line):
-        """Parse a line.
+        '''Parse a line.
 
         Ratings are translated so that they are all strictly positive.
 
         Args:
             line(str): The line to parse
 
         Returns:
             tuple: User id, item id, rating and timestamp. The timestamp is set
             to ``None`` if it does no exist.
-        """
+            '''
 
         line = line.split(self.sep)
         try:
             if self.with_timestamp:
-                uid, iid, r, timestamp = (line[i].strip() for i in self.indexes)
+                uid, iid, r, timestamp = (line[i].strip()
+                                          for i in self.indexes)
             else:
-                uid, iid, r = (line[i].strip() for i in self.indexes)
+                uid, iid, r = (line[i].strip()
+                               for i in self.indexes)
                 timestamp = None
 
         except IndexError:
-            raise ValueError(
-                "Impossible to parse line. Check the line_format" " and sep parameters."
-            )
+            raise ValueError('Impossible to parse line. Check the line_format'
+                             ' and sep parameters.')
 
         return uid, iid, float(r), timestamp
```

### Comparing `scikit_surprise-1.1.4/surprise/similarities.pyx` & `scikit-surprise-1.1rc0/surprise/similarities.pyx`

 * *Files 25% similar despite different names*

```diff
@@ -11,102 +11,112 @@
 
     cosine
     msd
     pearson
     pearson_baseline
 """
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 cimport numpy as np  # noqa
 import numpy as np
-from libc.math cimport sqrt
 
+from six.moves import range
+from six import iteritems
 
-def cosine(int n_x, yr, int min_support):
+
+def cosine(n_x, yr, min_support):
     """Compute the cosine similarity between all pairs of users (or items).
 
     Only **common** users (or items) are taken into account. The cosine
     similarity is defined as:
 
     .. math::
         \\text{cosine_sim}(u, v) = \\frac{
-        \\sum\\limits_{i \\in I_{uv}} r_{ui} \\cdot r_{vi}}
-        {\\sqrt{\\sum\\limits_{i \\in I_{uv}} r_{ui}^2} \\cdot
-        \\sqrt{\\sum\\limits_{i \\in I_{uv}} r_{vi}^2}
+        \\sum\\limits_{i \in I_{uv}} r_{ui} \cdot r_{vi}}
+        {\\sqrt{\\sum\\limits_{i \in I_{uv}} r_{ui}^2} \cdot
+        \\sqrt{\\sum\\limits_{i \in I_{uv}} r_{vi}^2}
         }
 
     or
 
     .. math::
         \\text{cosine_sim}(i, j) = \\frac{
-        \\sum\\limits_{u \\in U_{ij}} r_{ui} \\cdot r_{uj}}
-        {\\sqrt{\\sum\\limits_{u \\in U_{ij}} r_{ui}^2} \\cdot
-        \\sqrt{\\sum\\limits_{u \\in U_{ij}} r_{uj}^2}
+        \\sum\\limits_{u \in U_{ij}} r_{ui} \cdot r_{uj}}
+        {\\sqrt{\\sum\\limits_{u \in U_{ij}} r_{ui}^2} \cdot
+        \\sqrt{\\sum\\limits_{u \in U_{ij}} r_{uj}^2}
         }
 
     depending on the ``user_based`` field of ``sim_options`` (see
     :ref:`similarity_measures_configuration`).
 
     For details on cosine similarity, see on `Wikipedia
     <https://en.wikipedia.org/wiki/Cosine_similarity#Definition>`__.
     """
 
     # sum (r_xy * r_x'y) for common ys
-    cdef double [:, ::1] prods = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] prods
     # number of common ys
-    cdef long [:, ::1] freq = np.zeros((n_x, n_x), np.int_)
+    cdef np.ndarray[np.int_t, ndim=2] freq
     # sum (r_xy ^ 2) for common ys
-    cdef double [:, ::1] sqi = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sqi
     # sum (r_x'y ^ 2) for common ys
-    cdef double [:, ::1] sqj = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sqj
     # the similarity matrix
-    cdef double [:, ::1] sim = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sim
 
-    cdef int xi, xj, y
+    cdef int xi, xj
     cdef double ri, rj
     cdef int min_sprt = min_support
 
-    for y, y_ratings in yr.items():
+    prods = np.zeros((n_x, n_x), np.double)
+    freq = np.zeros((n_x, n_x), np.int)
+    sqi = np.zeros((n_x, n_x), np.double)
+    sqj = np.zeros((n_x, n_x), np.double)
+    sim = np.zeros((n_x, n_x), np.double)
+
+    for y, y_ratings in iteritems(yr):
         for xi, ri in y_ratings:
             for xj, rj in y_ratings:
                 freq[xi, xj] += 1
                 prods[xi, xj] += ri * rj
                 sqi[xi, xj] += ri**2
                 sqj[xi, xj] += rj**2
 
     for xi in range(n_x):
         sim[xi, xi] = 1
         for xj in range(xi + 1, n_x):
             if freq[xi, xj] < min_sprt:
                 sim[xi, xj] = 0
             else:
-                denum = sqrt(sqi[xi, xj] * sqj[xi, xj])
+                denum = np.sqrt(sqi[xi, xj] * sqj[xi, xj])
                 sim[xi, xj] = prods[xi, xj] / denum
 
             sim[xj, xi] = sim[xi, xj]
 
-    return np.asarray(sim)
+    return sim
 
 
-def msd(int n_x, yr, int min_support):
+def msd(n_x, yr, min_support):
     """Compute the Mean Squared Difference similarity between all pairs of
     users (or items).
 
     Only **common** users (or items) are taken into account. The Mean Squared
     Difference is defined as:
 
     .. math ::
-        \\text{msd}(u, v) = \\frac{1}{|I_{uv}|} \\cdot
-        \\sum\\limits_{i \\in I_{uv}} (r_{ui} - r_{vi})^2
+        \\text{msd}(u, v) = \\frac{1}{|I_{uv}|} \cdot
+        \\sum\\limits_{i \in I_{uv}} (r_{ui} - r_{vi})^2
 
     or
 
     .. math ::
-        \\text{msd}(i, j) = \\frac{1}{|U_{ij}|} \\cdot
-        \\sum\\limits_{u \\in U_{ij}} (r_{ui} - r_{uj})^2
+        \\text{msd}(i, j) = \\frac{1}{|U_{ij}|} \cdot
+        \\sum\\limits_{u \in U_{ij}} (r_{ui} - r_{uj})^2
 
     depending on the ``user_based`` field of ``sim_options`` (see
     :ref:`similarity_measures_configuration`).
 
     The MSD-similarity is then defined as:
 
     .. math ::
@@ -118,25 +128,29 @@
 
     For details on MSD, see third definition on `Wikipedia
     <https://en.wikipedia.org/wiki/Root-mean-square_deviation#Formula>`__.
 
     """
 
     # sum (r_xy - r_x'y)**2 for common ys
-    cdef double [:, ::1] sq_diff = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sq_diff
     # number of common ys
-    cdef long [:, ::1] freq = np.zeros((n_x, n_x), np.int_)
+    cdef np.ndarray[np.int_t, ndim=2] freq
     # the similarity matrix
-    cdef double [:, ::1] sim = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sim
 
     cdef int xi, xj
     cdef double ri, rj
     cdef int min_sprt = min_support
 
-    for y, y_ratings in yr.items():
+    sq_diff = np.zeros((n_x, n_x), np.double)
+    freq = np.zeros((n_x, n_x), np.int)
+    sim = np.zeros((n_x, n_x), np.double)
+
+    for y, y_ratings in iteritems(yr):
         for xi, ri in y_ratings:
             for xj, rj in y_ratings:
                 sq_diff[xi, xj] += (ri - rj)**2
                 freq[xi, xj] += 1
 
     for xi in range(n_x):
         sim[xi, xi] = 1  # completely arbitrary and useless anyway
@@ -145,70 +159,79 @@
                 sim[xi, xj] = 0
             else:
                 # return inverse of (msd + 1) (+ 1 to avoid dividing by zero)
                 sim[xi, xj] = 1 / (sq_diff[xi, xj] / freq[xi, xj] + 1)
 
             sim[xj, xi] = sim[xi, xj]
 
-    return np.asarray(sim)
+    return sim
 
 
-def pearson(int n_x, yr, int min_support):
+def pearson(n_x, yr, min_support):
     """Compute the Pearson correlation coefficient between all pairs of users
     (or items).
 
     Only **common** users (or items) are taken into account. The Pearson
     correlation coefficient can be seen as a mean-centered cosine similarity,
     and is defined as:
 
     .. math ::
-        \\text{pearson_sim}(u, v) = \\frac{ \\sum\\limits_{i \\in I_{uv}}
-        (r_{ui} -  \\mu_u) \\cdot (r_{vi} - \\mu_{v})} {\\sqrt{\\sum\\limits_{i
-        \\in I_{uv}} (r_{ui} -  \\mu_u)^2} \\cdot \\sqrt{\\sum\\limits_{i \\in
-        I_{uv}} (r_{vi} -  \\mu_{v})^2} }
+        \\text{pearson_sim}(u, v) = \\frac{ \\sum\\limits_{i \in I_{uv}}
+        (r_{ui} -  \mu_u) \cdot (r_{vi} - \mu_{v})} {\\sqrt{\\sum\\limits_{i
+        \in I_{uv}} (r_{ui} -  \mu_u)^2} \cdot \\sqrt{\\sum\\limits_{i \in
+        I_{uv}} (r_{vi} -  \mu_{v})^2} }
 
     or
 
     .. math ::
-        \\text{pearson_sim}(i, j) = \\frac{ \\sum\\limits_{u \\in U_{ij}}
-        (r_{ui} -  \\mu_i) \\cdot (r_{uj} - \\mu_{j})} {\\sqrt{\\sum\\limits_{u
-        \\in U_{ij}} (r_{ui} -  \\mu_i)^2} \\cdot \\sqrt{\\sum\\limits_{u \\in
-        U_{ij}} (r_{uj} -  \\mu_{j})^2} }
+        \\text{pearson_sim}(i, j) = \\frac{ \\sum\\limits_{u \in U_{ij}}
+        (r_{ui} -  \mu_i) \cdot (r_{uj} - \mu_{j})} {\\sqrt{\\sum\\limits_{u
+        \in U_{ij}} (r_{ui} -  \mu_i)^2} \cdot \\sqrt{\\sum\\limits_{u \in
+        U_{ij}} (r_{uj} -  \mu_{j})^2} }
 
     depending on the ``user_based`` field of ``sim_options`` (see
     :ref:`similarity_measures_configuration`).
 
 
     Note: if there are no common users or items, similarity will be 0 (and not
     -1).
 
     For details on Pearson coefficient, see `Wikipedia
     <https://en.wikipedia.org/wiki/Pearson_product-moment_correlation_coefficient#For_a_sample>`__.
 
     """
+
     # number of common ys
-    cdef long [:, ::1] freq = np.zeros((n_x, n_x), np.int_)
+    cdef np.ndarray[np.int_t, ndim=2] freq
     # sum (r_xy * r_x'y) for common ys
-    cdef double [:, ::1] prods = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] prods
     # sum (rxy ^ 2) for common ys
-    cdef double [:, ::1] sqi = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sqi
     # sum (rx'y ^ 2) for common ys
-    cdef double [:, ::1] sqj = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sqj
     # sum (rxy) for common ys
-    cdef double [:, ::1] si = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] si
     # sum (rx'y) for common ys
-    cdef double [:, ::1] sj = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sj
     # the similarity matrix
-    cdef double [:, ::1] sim = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sim
 
-    cdef int xi, xj, y, n
-    cdef double ri, rj, num, denum
+    cdef int xi, xj
+    cdef double ri, rj
     cdef int min_sprt = min_support
 
-    for y, y_ratings in yr.items():
+    freq = np.zeros((n_x, n_x), np.int)
+    prods = np.zeros((n_x, n_x), np.double)
+    sqi = np.zeros((n_x, n_x), np.double)
+    sqj = np.zeros((n_x, n_x), np.double)
+    si = np.zeros((n_x, n_x), np.double)
+    sj = np.zeros((n_x, n_x), np.double)
+    sim = np.zeros((n_x, n_x), np.double)
+
+    for y, y_ratings in iteritems(yr):
         for xi, ri in y_ratings:
             for xj, rj in y_ratings:
                 prods[xi, xj] += ri * rj
                 freq[xi, xj] += 1
                 sqi[xi, xj] += ri**2
                 sqj[xi, xj] += rj**2
                 si[xi, xj] += ri
@@ -219,113 +242,120 @@
         for xj in range(xi + 1, n_x):
 
             if freq[xi, xj] < min_sprt:
                 sim[xi, xj] = 0
             else:
                 n = freq[xi, xj]
                 num = n * prods[xi, xj] - si[xi, xj] * sj[xi, xj]
-                denum = sqrt((n * sqi[xi, xj] - si[xi, xj]**2) *
-                             (n * sqj[xi, xj] - sj[xi, xj]**2))
+                denum = np.sqrt((n * sqi[xi, xj] - si[xi, xj]**2) *
+                                (n * sqj[xi, xj] - sj[xi, xj]**2))
                 if denum == 0:
                     sim[xi, xj] = 0
                 else:
                     sim[xi, xj] = num / denum
 
             sim[xj, xi] = sim[xi, xj]
 
-    return np.asarray(sim)
+    return sim
 
 
-def pearson_baseline(
-    int n_x,
-    yr,
-    int min_support,
-    double global_mean,
-    double [::1] x_biases,
-    double [::1] y_biases,
-    double shrinkage=100,
-):
+def pearson_baseline(n_x, yr, min_support, global_mean, x_biases, y_biases,
+                     shrinkage=100):
     """Compute the (shrunk) Pearson correlation coefficient between all pairs
     of users (or items) using baselines for centering instead of means.
 
     The shrinkage parameter helps to avoid overfitting when only few ratings
     are available (see :ref:`similarity_measures_configuration`).
 
     The Pearson-baseline correlation coefficient is defined as:
 
     .. math::
-        \\text{pearson_baseline_sim}(u, v) = \\hat{\\rho}_{uv} = \\frac{
-            \\sum\\limits_{i \\in I_{uv}} (r_{ui} -  b_{ui}) \\cdot (r_{vi} -
-            b_{vi})} {\\sqrt{\\sum\\limits_{i \\in I_{uv}} (r_{ui} -  b_{ui})^2}
-            \\cdot \\sqrt{\\sum\\limits_{i \\in I_{uv}} (r_{vi} -  b_{vi})^2}}
+        \\text{pearson_baseline_sim}(u, v) = \hat{\\rho}_{uv} = \\frac{
+            \\sum\\limits_{i \in I_{uv}} (r_{ui} -  b_{ui}) \cdot (r_{vi} -
+            b_{vi})} {\\sqrt{\\sum\\limits_{i \in I_{uv}} (r_{ui} -  b_{ui})^2}
+            \cdot \\sqrt{\\sum\\limits_{i \in I_{uv}} (r_{vi} -  b_{vi})^2}}
 
     or
 
     .. math::
-        \\text{pearson_baseline_sim}(i, j) = \\hat{\\rho}_{ij} = \\frac{
-            \\sum\\limits_{u \\in U_{ij}} (r_{ui} -  b_{ui}) \\cdot (r_{uj} -
-            b_{uj})} {\\sqrt{\\sum\\limits_{u \\in U_{ij}} (r_{ui} -  b_{ui})^2}
-            \\cdot \\sqrt{\\sum\\limits_{u \\in U_{ij}} (r_{uj} -  b_{uj})^2}}
+        \\text{pearson_baseline_sim}(i, j) = \hat{\\rho}_{ij} = \\frac{
+            \\sum\\limits_{u \in U_{ij}} (r_{ui} -  b_{ui}) \cdot (r_{uj} -
+            b_{uj})} {\\sqrt{\\sum\\limits_{u \in U_{ij}} (r_{ui} -  b_{ui})^2}
+            \cdot \\sqrt{\\sum\\limits_{u \in U_{ij}} (r_{uj} -  b_{uj})^2}}
 
     The shrunk Pearson-baseline correlation coefficient is then defined as:
 
     .. math::
         \\text{pearson_baseline_shrunk_sim}(u, v) &= \\frac{|I_{uv}| - 1}
-        {|I_{uv}| - 1 + \\text{shrinkage}} \\cdot \\hat{\\rho}_{uv}
+        {|I_{uv}| - 1 + \\text{shrinkage}} \\cdot \hat{\\rho}_{uv}
 
         \\text{pearson_baseline_shrunk_sim}(i, j) &= \\frac{|U_{ij}| - 1}
-        {|U_{ij}| - 1 + \\text{shrinkage}} \\cdot \\hat{\\rho}_{ij}
+        {|U_{ij}| - 1 + \\text{shrinkage}} \\cdot \hat{\\rho}_{ij}
 
 
     Obviously, a shrinkage parameter of 0 amounts to no shrinkage at all.
 
     Note: here again, if there are no common users/items, similarity will be 0
     (and not -1).
 
     Motivations for such a similarity measure can be found on the *Recommender
     System Handbook*, section 5.4.1.
     """
 
     # number of common ys
-    cdef long [:, ::1] freq = np.zeros((n_x, n_x), np.int_)
+    cdef np.ndarray[np.int_t, ndim=2] freq
     # sum (r_xy - b_xy) * (r_x'y - b_x'y) for common ys
-    cdef double [:, ::1] prods = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] prods
     # sum (r_xy - b_xy)**2 for common ys
-    cdef double [:, ::1] sq_diff_i = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sq_diff_i
     # sum (r_x'y - b_x'y)**2 for common ys
-    cdef double [:, ::1] sq_diff_j = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sq_diff_j
     # the similarity matrix
-    cdef double [:, ::1] sim = np.zeros((n_x, n_x), np.double)
+    cdef np.ndarray[np.double_t, ndim=2] sim
+
+    cdef np.ndarray[np.double_t, ndim=1] x_biases_
+    cdef np.ndarray[np.double_t, ndim=1] y_biases_
 
-    cdef int y, xi, xj
+    cdef int xi, xj
     cdef double ri, rj, diff_i, diff_j, partial_bias
     cdef int min_sprt = min_support
     cdef double global_mean_ = global_mean
 
+    freq = np.zeros((n_x, n_x), np.int)
+    prods = np.zeros((n_x, n_x), np.double)
+    sq_diff_i = np.zeros((n_x, n_x), np.double)
+    sq_diff_j = np.zeros((n_x, n_x), np.double)
+    sim = np.zeros((n_x, n_x), np.double)
+
+    x_biases_ = x_biases
+    y_biases_ = y_biases
+
     # Need this because of shrinkage. When pearson coeff is zero when support
     # is 1, so that's OK.
     min_sprt = max(2, min_sprt)
 
-    for y, y_ratings in yr.items():
-        partial_bias = global_mean_ + y_biases[y]
+    for y, y_ratings in iteritems(yr):
+        partial_bias = global_mean_ + y_biases_[y]
         for xi, ri in y_ratings:
             for xj, rj in y_ratings:
                 freq[xi, xj] += 1
-                diff_i = (ri - (partial_bias + x_biases[xi]))
-                diff_j = (rj - (partial_bias + x_biases[xj]))
+                diff_i = (ri - (partial_bias + x_biases_[xi]))
+                diff_j = (rj - (partial_bias + x_biases_[xj]))
                 prods[xi, xj] += diff_i * diff_j
                 sq_diff_i[xi, xj] += diff_i**2
                 sq_diff_j[xi, xj] += diff_j**2
 
     for xi in range(n_x):
         sim[xi, xi] = 1
         for xj in range(xi + 1, n_x):
             if freq[xi, xj] < min_sprt:
                 sim[xi, xj] = 0
             else:
-                sim[xi, xj] = prods[xi, xj] / (sqrt(sq_diff_i[xi, xj] * sq_diff_j[xi, xj]))
+                sim[xi, xj] = prods[xi, xj] / (np.sqrt(sq_diff_i[xi, xj] *
+                                                       sq_diff_j[xi, xj]))
                 # the shrinkage part
-                sim[xi, xj] *= (freq[xi, xj] - 1) / (freq[xi, xj] - 1 + shrinkage)
+                sim[xi, xj] *= (freq[xi, xj] - 1) / (freq[xi, xj] - 1 +
+                                                     shrinkage)
 
             sim[xj, xi] = sim[xi, xj]
 
-    return np.asarray(sim)
+    return sim
```

### Comparing `scikit_surprise-1.1.4/surprise/trainset.py` & `scikit-surprise-1.1rc0/surprise/trainset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-"""This module contains the Trainset class."""
+'''This module contains the Trainset class.'''
 
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+
 import numpy as np
+from six import iteritems
 
 
 class Trainset:
     """A trainset contains all useful data that constitute a training set.
 
     It is used by the :meth:`fit()
     <surprise.prediction_algorithms.algo_base.AlgoBase.fit>` method of every
@@ -33,25 +37,16 @@
         n_items: Total number of items :math:`|I|`.
         n_ratings: Total number of ratings :math:`|R_{train}|`.
         rating_scale(tuple): The minimum and maximal rating of the rating
             scale.
         global_mean: The mean of all ratings :math:`\\mu`.
     """
 
-    def __init__(
-        self,
-        ur,
-        ir,
-        n_users,
-        n_items,
-        n_ratings,
-        rating_scale,
-        raw2inner_id_users,
-        raw2inner_id_items,
-    ):
+    def __init__(self, ur, ir, n_users, n_items, n_ratings, rating_scale,
+                 raw2inner_id_users, raw2inner_id_items):
 
         self.ur = ur
         self.ir = ir
         self.n_users = n_users
         self.n_items = n_items
         self.n_ratings = n_ratings
         self.rating_scale = rating_scale
@@ -105,15 +100,16 @@
         Raises:
             ValueError: When user is not part of the trainset.
         """
 
         try:
             return self._raw2inner_id_users[ruid]
         except KeyError:
-            raise ValueError("User " + str(ruid) + " is not part of the trainset.")
+            raise ValueError('User ' + str(ruid) +
+                             ' is not part of the trainset.')
 
     def to_raw_uid(self, iuid):
         """Convert a **user** inner id to a raw id.
 
         See :ref:`this note<raw_inner_note>`.
 
         Args:
@@ -123,22 +119,21 @@
             str: The user raw id.
 
         Raises:
             ValueError: When ``iuid`` is not an inner id.
         """
 
         if self._inner2raw_id_users is None:
-            self._inner2raw_id_users = {
-                inner: raw for (raw, inner) in self._raw2inner_id_users.items()
-            }
+            self._inner2raw_id_users = {inner: raw for (raw, inner) in
+                                        iteritems(self._raw2inner_id_users)}
 
         try:
             return self._inner2raw_id_users[iuid]
         except KeyError:
-            raise ValueError(str(iuid) + " is not a valid inner id.")
+            raise ValueError(str(iuid) + ' is not a valid inner id.')
 
     def to_inner_iid(self, riid):
         """Convert an **item** raw id to an inner id.
 
         See :ref:`this note<raw_inner_note>`.
 
         Args:
@@ -150,15 +145,16 @@
         Raises:
             ValueError: When item is not part of the trainset.
         """
 
         try:
             return self._raw2inner_id_items[riid]
         except KeyError:
-            raise ValueError("Item " + str(riid) + " is not part of the trainset.")
+            raise ValueError('Item ' + str(riid) +
+                             ' is not part of the trainset.')
 
     def to_raw_iid(self, iiid):
         """Convert an **item** inner id to a raw id.
 
         See :ref:`this note<raw_inner_note>`.
 
         Args:
@@ -168,50 +164,47 @@
             str: The item raw id.
 
         Raises:
             ValueError: When ``iiid`` is not an inner id.
         """
 
         if self._inner2raw_id_items is None:
-            self._inner2raw_id_items = {
-                inner: raw for (raw, inner) in self._raw2inner_id_items.items()
-            }
+            self._inner2raw_id_items = {inner: raw for (raw, inner) in
+                                        iteritems(self._raw2inner_id_items)}
 
         try:
             return self._inner2raw_id_items[iiid]
         except KeyError:
-            raise ValueError(str(iiid) + " is not a valid inner id.")
+            raise ValueError(str(iiid) + ' is not a valid inner id.')
 
     def all_ratings(self):
         """Generator function to iterate over all ratings.
 
         Yields:
             A tuple ``(uid, iid, rating)`` where ids are inner ids (see
             :ref:`this note <raw_inner_note>`).
         """
 
-        for u, u_ratings in self.ur.items():
+        for u, u_ratings in iteritems(self.ur):
             for i, r in u_ratings:
                 yield u, i, r
 
     def build_testset(self):
         """Return a list of ratings that can be used as a testset in the
         :meth:`test() <surprise.prediction_algorithms.algo_base.AlgoBase.test>`
         method.
 
         The ratings are all the ratings that are in the trainset, i.e. all the
         ratings returned by the :meth:`all_ratings()
         <surprise.Trainset.all_ratings>` generator. This is useful in
         cases where you want to to test your algorithm on the trainset.
         """
 
-        return [
-            (self.to_raw_uid(u), self.to_raw_iid(i), r)
-            for (u, i, r) in self.all_ratings()
-        ]
+        return [(self.to_raw_uid(u), self.to_raw_iid(i), r)
+                for (u, i, r) in self.all_ratings()]
 
     def build_anti_testset(self, fill=None):
         """Return a list of ratings that can be used as a testset in the
         :meth:`test() <surprise.prediction_algorithms.algo_base.AlgoBase.test>`
         method.
 
         The ratings are all the ratings that are **not** in the trainset, i.e.
@@ -229,20 +222,18 @@
         Returns:
             A list of tuples ``(uid, iid, fill)`` where ids are raw ids.
         """
         fill = self.global_mean if fill is None else float(fill)
 
         anti_testset = []
         for u in self.all_users():
-            user_items = {j for (j, _) in self.ur[u]}
-            anti_testset += [
-                (self.to_raw_uid(u), self.to_raw_iid(i), fill)
-                for i in self.all_items()
-                if i not in user_items
-            ]
+            user_items = set([j for (j, _) in self.ur[u]])
+            anti_testset += [(self.to_raw_uid(u), self.to_raw_iid(i), fill) for
+                             i in self.all_items() if
+                             i not in user_items]
         return anti_testset
 
     def all_users(self):
         """Generator function to iterate over all users.
 
         Yields:
             Inner id of users.
@@ -255,11 +246,15 @@
         Yields:
             Inner id of items.
         """
         return range(self.n_items)
 
     @property
     def global_mean(self):
+        """Return the mean of all ratings.
+
+        It's only computed once."""
         if self._global_mean is None:
-            self._global_mean = np.mean([r for (_, _, r) in self.all_ratings()])
+            self._global_mean = np.mean([r for (_, _, r) in
+                                         self.all_ratings()])
 
         return self._global_mean
```

### Comparing `scikit_surprise-1.1.4/surprise/utils.py` & `scikit-surprise-1.1rc0/surprise/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-"""The utils module contains the get_rng function."""
-
+'''The utils module contains the get_rng function.'''
 
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 import numbers
 
 import numpy as np
 
 
 def get_rng(random_state):
-    """Return a 'validated' RNG.
+    '''Return a 'validated' RNG.
 
     If random_state is None, use RandomState singleton from numpy.  Else if
     it's an integer, consider it's a seed and initialized an rng with that
     seed. If it's already an rng, return it.
-    """
+    '''
     if random_state is None:
         return np.random.mtrand._rand
     elif isinstance(random_state, (numbers.Integral, np.integer)):
         return np.random.RandomState(random_state)
     if isinstance(random_state, np.random.RandomState):
         return random_state
-    raise ValueError(
-        "Wrong random state. Expecting None, an int or a numpy "
-        "RandomState instance, got a "
-        "{}".format(type(random_state))
-    )
+    raise ValueError('Wrong random state. Expecting None, an int or a numpy '
+                     'RandomState instance, got a '
+                     '{}'.format(type(random_state)))
```

