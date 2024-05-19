# Comparing `tmp/autogluon.tabular-1.1.1b20240517.tar.gz` & `tmp/autogluon.tabular-1.1.1b20240518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-1.1.1b20240517.tar", last modified: Fri May 17 09:05:33 2024, max compression
+gzip compressed data, was "autogluon.tabular-1.1.1b20240518.tar", last modified: Sat May 18 09:04:54 2024, max compression
```

## Comparing `autogluon.tabular-1.1.1b20240517.tar` & `autogluon.tabular-1.1.1b20240518.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.965486 autogluon.tabular-1.1.1b20240517/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.965486 autogluon.tabular-1.1.1b20240517/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.969487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.969487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.969487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/zeroshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/zeroshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.973487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/experimental/_scikit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/experimental/_tabular_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/experimental/_tabular_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.973487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51900 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)    23537 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.973487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.973487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.973487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.973487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.973487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1379 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27704 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.977486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.981486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.981486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.981486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.981486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    36460 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.981486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24707 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabpfn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabpfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.985486 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/predictor/_deprecated_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)   316069 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17843 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.989487 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-17 09:04:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 09:05:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:05:33.969487 autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-17 09:05:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-17 09:05:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:05:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 09:05:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-17 09:05:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 09:05:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:05:33.000000 autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.222182 autogluon.tabular-1.1.1b20240518/
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-18 09:04:54.222182 autogluon.tabular-1.1.1b20240518/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:04:54.222182 autogluon.tabular-1.1.1b20240518/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.202182 autogluon.tabular-1.1.1b20240518/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.202182 autogluon.tabular-1.1.1b20240518/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.206182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.206182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.206182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/zeroshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/zeroshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/experimental/_scikit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/experimental/_tabular_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/experimental/_tabular_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51900 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23537 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1379 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27704 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.210182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36460 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.214182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24707 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.218182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/predictor/_deprecated_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)   317268 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.222182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.222182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17843 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.222182 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-18 09:03:55.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-18 09:04:54.000000 autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:04:54.206182 autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-18 09:04:54.000000 autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-18 09:04:54.000000 autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:04:54.000000 autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 09:04:54.000000 autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-18 09:04:54.000000 autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 09:04:54.000000 autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:04:54.000000 autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-1.1.1b20240517/PKG-INFO` & `autogluon.tabular-1.1.1b20240518/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 1.1.1b20240517
+Version: 1.1.1b20240518
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-1.1.1b20240517/setup.py` & `autogluon.tabular-1.1.1b20240518/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/experimental/_scikit_mixin.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/experimental/_scikit_mixin.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/experimental/_tabular_classifier.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/experimental/_tabular_classifier.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/experimental/_tabular_regressor.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/experimental/_tabular_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabpfn/tabpfn_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabpfn/tabpfn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/predictor/_deprecated_methods.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/predictor/_deprecated_methods.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/predictor/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         For other problem types, will equal None.
         For multiclass, it is possible for not all of the label values to have a mapping.
             This indicates that the internal models will never predict those missing labels, and training rows associated with the missing labels were dropped.
     """
 
     Dataset = TabularDataset
     predictor_file_name = "predictor.pkl"
-    _predictor_version_file_name = "__version__"
+    _predictor_version_file_name = "version.txt"
     _predictor_metadata_file_name = "metadata.json"
     _predictor_log_file_name = "predictor_log.txt"
 
     def __init__(
         self,
         label: str,
         problem_type: str = None,
@@ -402,15 +402,15 @@
         fit_full_last_level_weighted_ensemble: bool = True,
         full_weighted_ensemble_additionally: bool = False,
         dynamic_stacking: bool | str = False,
         calibrate_decision_threshold: bool | str = False,
         num_cpus: int | str = "auto",
         num_gpus: int | str = "auto",
         **kwargs,
-    ):
+    ) -> "TabularPredictor":
         """
         Fit models to predict a column of a data table (label) based on the other columns (features).
 
         Parameters
         ----------
         train_data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
             Table of the training data, which is similar to a pandas DataFrame.
@@ -4143,45 +4143,65 @@
             self._learner: AbstractTabularLearner = learner
         self._learner_type = type(self._learner)
         if self._learner.trainer_path is not None:
             self._learner.persist_trainer(low_memory=True)
             self._trainer: AbstractTrainer = self._learner.load_trainer()  # Trainer object
 
     @classmethod
-    def _load_version_file(cls, path) -> str:
+    def _load_version_file(cls, path: str) -> str:
+        """
+        Loads the version file that is part of the saved predictor artifact.
+        The version file contains a string matching `predictor._learner.version`.
+
+        Parameters
+        ----------
+        path: str
+            The path that would be used to load the predictor via `predictor.load(path)`
+
+        Returns
+        -------
+        The version of AutoGluon used to fit the predictor, as a string.
+
+        """
         version_file_path = os.path.join(path, cls._predictor_version_file_name)
-        version = load_str.load(path=version_file_path)
+        try:
+            version = load_str.load(path=version_file_path)
+        except:
+            # Loads the old version file used in `autogluon.tabular<=1.1.0`, named `__version__`.
+            # This file name was changed because Kaggle does not allow uploading files named `__version__`.
+            version_file_path = os.path.join(path, "__version__")
+            version = load_str.load(path=version_file_path)
         return version
 
     @classmethod
-    def _load_metadata_file(cls, path: str, silent=True):
+    def _load_metadata_file(cls, path: str, silent: bool = True):
         metadata_file_path = os.path.join(path, cls._predictor_metadata_file_name)
         return load_json.load(path=metadata_file_path, verbose=not silent)
 
-    def _save_version_file(self, silent=False):
+    def _save_version_file(self, silent: bool = False):
         from ..version import __version__
 
         version_file_contents = f"{__version__}"
         version_file_path = os.path.join(self.path, self._predictor_version_file_name)
         save_str.save(path=version_file_path, data=version_file_contents, verbose=not silent)
 
-    def _save_metadata_file(self, silent=False):
+    def _save_metadata_file(self, silent: bool = False):
         """
         Save metadata json file to disk containing information such as
         python version, autogluon version, installed packages, operating system, etc.
         """
         metadata_file_path = os.path.join(self.path, self._predictor_metadata_file_name)
 
         metadata = get_autogluon_metadata()
 
         save_json.save(path=metadata_file_path, obj=metadata)
         if not silent:
             logger.log(15, f"Saving {metadata_file_path}")
 
-    def save(self, silent=False):
+    def save(self, silent: bool = False):
         """
         Save this Predictor to file in directory specified by this Predictor's `path`.
         Note that :meth:`TabularPredictor.fit` already saves the predictor object automatically
         (we do not recommend modifying the Predictor object yourself as it tracks many trained models).
 
         Parameters
         ----------
@@ -4202,25 +4222,32 @@
             self._save_metadata_file(silent=silent)
         except Exception as e:
             logger.log(30, f"Failed to save metadata file due to exception {e}, skipping...")
         if not silent:
             logger.log(20, f'TabularPredictor saved. To load, use: predictor = TabularPredictor.load("{self.path}")')
 
     @classmethod
-    def _load(cls, path: str):
+    def _load(cls, path: str) -> "TabularPredictor":
         """
         Inner load method, called in `load`.
         """
         predictor: TabularPredictor = load_pkl.load(path=os.path.join(path, cls.predictor_file_name))
         learner = predictor._learner_type.load(path)
         predictor._set_post_fit_vars(learner=learner)
         return predictor
 
     @classmethod
-    def load(cls, path: str, verbosity: int = None, require_version_match: bool = True, require_py_version_match: bool = True, check_packages: bool = False):
+    def load(
+        cls,
+        path: str,
+        verbosity: int = None,
+        require_version_match: bool = True,
+        require_py_version_match: bool = True,
+        check_packages: bool = False,
+    ) -> "TabularPredictor":
         """
         Load a TabularPredictor object previously produced by `fit()` from file and returns this object. It is highly recommended the predictor be loaded with the exact AutoGluon version it was fit with.
 
         Parameters
         ----------
         path : str
             The path to directory in which this Predictor was previously saved.
@@ -4236,14 +4263,23 @@
         require_py_version_match : bool, default = True
             If True, will raise an AssertionError if the Python version of the loaded predictor does not match the installed Python version.
                 Micro version differences such as 3.9.2 and 3.9.7 will log a warning but will not raise an exception.
             If False, will allow loading of models trained on incompatible python versions, but is NOT recommended. Users may run into numerous issues if attempting this.
         check_packages : bool, default = False
             If True, checks package versions of the loaded predictor against the package versions of the current environment.
             Warnings will be logged for each mismatch of package version.
+
+        Returns
+        -------
+        predictor : TabularPredictor
+
+        Examples
+        --------
+        >>> predictor = TabularPredictor.load(path_to_predictor)
+
         """
         if verbosity is not None:
             set_logger_verbosity(verbosity)  # Reset logging after load (may be in new Python session)
         if path is None:
             raise ValueError("path cannot be None in load()")
 
         try:
@@ -4255,15 +4291,15 @@
 
         path = setup_outputdir(path, warn_if_exist=False)  # replace ~ with absolute path if it exists
         try:
             version_saved = cls._load_version_file(path=path)
         except:
             logger.warning(
                 f'WARNING: Could not find version file at "{os.path.join(path, cls._predictor_version_file_name)}".\n'
-                f"This means that the predictor was fit in a version `<=0.3.1`."
+                f"This means that the predictor was fit in an AutoGluon version `<=0.3.1`."
             )
             version_saved = None
 
         if version_saved is None:
             predictor = cls._load(path=path)
             try:
                 version_saved = predictor._learner.version
@@ -4322,16 +4358,16 @@
             Path to the predictor to load the log.
             This can be used when the predictor was initialized with `log_file_path="auto"` to fetch the log file automatically
         log_file_path: Optional[str], default = None
             Path to the log file.
             If you specified a `log_file_path` while initializing the predictor, you should use `log_file_path` to load the log file instead.
             At least one of `predictor_path` or `log_file_path` must to be specified
 
-        Return
-        ------
+        Returns
+        -------
         List[str]
             A list containing lines of the log file
         """
         file_path = log_file_path
         if file_path is None:
             assert predictor_path is not None, "Please either provide `predictor_path` or `log_file_path` to load the log file"
             file_path = os.path.join(predictor_path, "logs", cls._predictor_log_file_name)
@@ -4717,15 +4753,15 @@
             logger.log(20, f"Setting dynamic_stacking from 'auto' to {dynamic_stacking}. {log_extra_ds}")
 
         return num_bag_folds, num_bag_sets, num_stack_levels, dynamic_stacking, use_bag_holdout
 
     # TODO: Add .delete() method to easily clean-up clones?
     #  Would need to be careful that user doesn't delete important things accidentally.
     # TODO: Add .save_zip() and load_zip() methods to pack and unpack artifacts into a single file to simplify deployment code?
-    def clone(self, path: str, *, return_clone: bool = False, dirs_exist_ok: bool = False):
+    def clone(self, path: str, *, return_clone: bool = False, dirs_exist_ok: bool = False) -> str | "TabularPredictor":
         """
         Clone the predictor and all of its artifacts to a new location on local disk.
         This is ideal for use-cases where saving a snapshot of the predictor is desired before performing
         more advanced operations (such as fit_extra and refit_full).
 
         Parameters
         ----------
@@ -4749,15 +4785,15 @@
         logger.log(
             30,
             f"Cloned {self.__class__.__name__} located in '{self.path}' to '{path_clone}'.\n"
             f'\tTo load the cloned predictor: predictor_clone = {self.__class__.__name__}.load(path="{path_clone}")',
         )
         return self.__class__.load(path=path_clone) if return_clone else path_clone
 
-    def clone_for_deployment(self, path: str, *, model: str = "best", return_clone: bool = False, dirs_exist_ok: bool = False):
+    def clone_for_deployment(self, path: str, *, model: str = "best", return_clone: bool = False, dirs_exist_ok: bool = False) -> str | "TabularPredictor":
         """
         Clone the predictor and all of its artifacts to a new location on local disk,
         then delete the clones artifacts unnecessary during prediction.
         This is ideal for use-cases where saving a snapshot of the predictor is desired before performing
         more advanced operations (such as fit_extra and refit_full).
 
         Note that the clone can no longer fit new models,
@@ -5042,15 +5078,15 @@
         if predictor.model_best in predictor.model_refit_map(inverse=True):
             leaderboard_kwargs = dict(refit_full=True, set_refit_score_to_parent=True)
         # Determine stacked overfitting
         ho_leaderboard = predictor.leaderboard(data=val_data, **leaderboard_kwargs).reset_index(drop=True)
         logger.info("Leaderboard on holdout data from dynamic stacking:")
         with pd.option_context("display.max_rows", None, "display.max_columns", None, "display.width", 1000):
             # Rename to avoid confusion for the user
-            logger.info(ho_leaderboard.rename({"score_test": "holdout_score"}, axis=1))
+            logger.info(ho_leaderboard.rename({"score_test": "score_holdout"}, axis=1))
         stacked_overfitting = check_stacked_overfitting_from_leaderboard(ho_leaderboard)
 
     logger.info(f"Stacked overfitting occurred: {stacked_overfitting}.")
     del predictor._learner
     predictor._learner = learner_og
 
     if clean_up_fits:
```

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-1.1.1b20240518/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 1.1.1b20240517
+Version: 1.1.1b20240518
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240517/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-1.1.1b20240518/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 numpy<1.29,>=1.21
 scipy<1.13,>=1.5.4
 pandas<2.3.0,>=2.0.0
 scikit-learn<1.4.1,>=1.3.0
 networkx<4,>=3.0
-autogluon.core==1.1.1b20240517
-autogluon.features==1.1.1b20240517
+autogluon.core==1.1.1b20240518
+autogluon.features==1.1.1b20240518
 
 [all]
-autogluon.core[all]==1.1.1b20240517
-fastai<2.8,>=2.3.1
-torch<2.2,>=2.1
+autogluon.core[all]==1.1.1b20240518
 xgboost<2.1,>=1.6
+torch<2.2,>=2.1
+fastai<2.8,>=2.3.1
 lightgbm<4.4,>=3.3
 
 [all:sys_platform != "darwin"]
 catboost<1.3,>=1.1
 
 [all:sys_platform == "darwin" and python_version < "3.11"]
 catboost<1.2,>=1.1
@@ -34,15 +34,15 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<4.4,>=3.3
 
 [ray]
-autogluon.core[all]==1.1.1b20240517
+autogluon.core[all]==1.1.1b20240518
 
 [skex]
 scikit-learn-intelex<2024.3,>=2023.0
 
 [skl2onnx]
 skl2onnx<1.17.0,>=1.15.0
 onnxruntime-gpu<1.18.0,>=1.15.0
```

