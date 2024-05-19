# Comparing `tmp/fairbench-0.2.9-py3-none-any.whl.zip` & `tmp/fairbench-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,49 +1,53 @@
-Zip file size: 38308 bytes, number of entries: 47
--rw-rw-rw-  2.0 fat      411 b- defN 23-Jun-23 14:12 fairbench/__init__.py
--rw-rw-rw-  2.0 fat     1952 b- defN 23-Jun-01 09:25 fairbench/export.py
--rw-rw-rw-  2.0 fat     5762 b- defN 23-Jun-28 17:37 fairbench/stamps.py
+Zip file size: 42536 bytes, number of entries: 51
+-rw-rw-rw-  2.0 fat      497 b- defN 24-Apr-18 11:38 fairbench/__init__.py
+-rw-rw-rw-  2.0 fat     6985 b- defN 24-May-18 11:02 fairbench/verification.py
 -rw-rw-rw-  2.0 fat       38 b- defN 23-Jun-14 13:57 fairbench/bench/__init__.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-15 21:51 fairbench/bench/demos.py
--rw-rw-rw-  2.0 fat     1660 b- defN 23-Jun-15 09:42 fairbench/bench/loader.py
+-rw-rw-rw-  2.0 fat     5853 b- defN 24-May-16 19:02 fairbench/bench/demos.py
+-rw-rw-rw-  2.0 fat     1660 b- defN 23-Jul-19 12:04 fairbench/bench/loader.py
+-rw-rw-rw-  2.0 fat      179 b- defN 23-Nov-10 23:11 fairbench/blocks/__init__.py
+-rw-rw-rw-  2.0 fat     3823 b- defN 24-Feb-28 07:00 fairbench/blocks/framework.py
+-rw-rw-rw-  2.0 fat       52 b- defN 23-Nov-10 23:11 fairbench/blocks/expanders/__init__.py
+-rw-rw-rw-  2.0 fat     4309 b- defN 24-May-16 14:21 fairbench/blocks/expanders/expanders.py
+-rw-rw-rw-  2.0 fat      274 b- defN 23-Nov-10 22:56 fairbench/blocks/metrics/__init__.py
+-rw-rw-rw-  2.0 fat     4016 b- defN 23-Nov-09 17:25 fairbench/blocks/metrics/classification.py
+-rw-rw-rw-  2.0 fat     2769 b- defN 23-Nov-09 17:25 fairbench/blocks/metrics/disparate_impact.py
+-rw-rw-rw-  2.0 fat     1583 b- defN 23-Nov-09 17:25 fairbench/blocks/metrics/disparate_mistreatment.py
+-rw-rw-rw-  2.0 fat     5162 b- defN 24-May-19 11:14 fairbench/blocks/metrics/ranking.py
+-rw-rw-rw-  2.0 fat     3006 b- defN 24-Feb-13 17:27 fairbench/blocks/metrics/regression.py
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Nov-10 23:11 fairbench/blocks/reducers/__init__.py
+-rw-rw-rw-  2.0 fat     4283 b- defN 24-May-16 14:21 fairbench/blocks/reducers/reducers.py
+-rw-rw-rw-  2.0 fat      157 b- defN 23-Nov-09 17:25 fairbench/core/__init__.py
+-rw-rw-rw-  2.0 fat     2463 b- defN 24-Feb-13 17:27 fairbench/core/categorical.py
+-rw-rw-rw-  2.0 fat    15076 b- defN 24-May-16 14:21 fairbench/core/fork.py
+-rw-rw-rw-  2.0 fat       49 b- defN 23-Nov-09 17:25 fairbench/core/compute/__init__.py
+-rw-rw-rw-  2.0 fat     3935 b- defN 23-Nov-09 20:07 fairbench/core/compute/backends.py
+-rw-rw-rw-  2.0 fat     5563 b- defN 24-Apr-18 11:38 fairbench/core/compute/delegation.py
+-rw-rw-rw-  2.0 fat      183 b- defN 23-Nov-09 17:25 fairbench/core/explanation/__init__.py
+-rw-rw-rw-  2.0 fat     1999 b- defN 23-Nov-10 16:55 fairbench/core/explanation/base.py
+-rw-rw-rw-  2.0 fat      674 b- defN 23-Nov-09 17:25 fairbench/core/explanation/curve.py
+-rw-rw-rw-  2.0 fat      388 b- defN 23-Nov-09 17:25 fairbench/core/explanation/error.py
 -rw-rw-rw-  2.0 fat      134 b- defN 23-Jun-28 12:59 fairbench/export/__init__.py
--rw-rw-rw-  2.0 fat    16566 b- defN 23-Jul-11 12:04 fairbench/export/interactive.py
--rw-rw-rw-  2.0 fat     3022 b- defN 23-Jul-07 09:37 fairbench/export/native.py
+-rw-rw-rw-  2.0 fat    19106 b- defN 24-May-16 08:55 fairbench/export/interactive.py
+-rw-rw-rw-  2.0 fat     3200 b- defN 24-Feb-13 17:25 fairbench/export/native.py
 -rw-rw-rw-  2.0 fat      173 b- defN 23-Jun-28 12:05 fairbench/export/modelcards/__init__.py
--rw-rw-rw-  2.0 fat     2856 b- defN 23-Jun-28 13:13 fairbench/export/modelcards/tohtml.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-Jun-28 13:12 fairbench/export/modelcards/tomarkdown.py
--rw-rw-rw-  2.0 fat      562 b- defN 23-Jun-28 12:59 fairbench/export/modelcards/toyaml.py
--rw-rw-rw-  2.0 fat      122 b- defN 23-May-13 22:58 fairbench/forks/__init__.py
--rw-rw-rw-  2.0 fat     2130 b- defN 23-May-25 07:44 fairbench/forks/categorical.py
--rw-rw-rw-  2.0 fat     2936 b- defN 23-Jun-28 12:59 fairbench/forks/explanation.py
--rw-rw-rw-  2.0 fat    26940 b- defN 23-Jul-10 09:08 fairbench/forks/fork.py
--rw-rw-rw-  2.0 fat      239 b- defN 23-Jun-20 08:51 fairbench/metrics/__init__.py
--rw-rw-rw-  2.0 fat     4016 b- defN 23-Jul-07 09:37 fairbench/metrics/classification.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-May-31 07:41 fairbench/metrics/disparate_impact.py
--rw-rw-rw-  2.0 fat     1494 b- defN 23-May-31 07:41 fairbench/metrics/disparate_mistreatment.py
--rw-rw-rw-  2.0 fat     3760 b- defN 23-Jul-10 11:32 fairbench/metrics/ranking.py
--rw-rw-rw-  2.0 fat     2970 b- defN 23-Jul-06 06:59 fairbench/metrics/regression.py
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-31 10:15 fairbench/mitigation/__init__.py
--rw-rw-rw-  2.0 fat     1790 b- defN 23-May-31 10:16 fairbench/mitigation/postprocessing.py
--rw-rw-rw-  2.0 fat      207 b- defN 23-Jan-15 14:06 fairbench/reports/__init__.py
--rw-rw-rw-  2.0 fat     1491 b- defN 23-Jun-07 08:52 fairbench/reports/accumulate.py
--rw-rw-rw-  2.0 fat     2075 b- defN 23-Jul-10 10:19 fairbench/reports/adhoc.py
--rw-rw-rw-  2.0 fat     2590 b- defN 23-Jun-20 08:05 fairbench/reports/base.py
--rw-rw-rw-  2.0 fat      883 b- defN 23-May-14 15:09 fairbench/reports/surrogate.py
--rw-rw-rw-  2.0 fat      155 b- defN 23-Feb-20 08:42 fairbench/reports/reduction/__init__.py
--rw-rw-rw-  2.0 fat     2260 b- defN 23-Jun-16 09:23 fairbench/reports/reduction/expanders.py
--rw-rw-rw-  2.0 fat     2637 b- defN 23-Jun-20 14:07 fairbench/reports/reduction/reduce.py
--rw-rw-rw-  2.0 fat     2834 b- defN 23-Jun-16 06:45 fairbench/reports/reduction/reducers.py
+-rw-rw-rw-  2.0 fat     2978 b- defN 24-Feb-28 09:48 fairbench/export/modelcards/tohtml.py
+-rw-rw-rw-  2.0 fat     2569 b- defN 24-Feb-28 09:32 fairbench/export/modelcards/tomarkdown.py
+-rw-rw-rw-  2.0 fat     1229 b- defN 24-May-18 13:17 fairbench/export/modelcards/toyaml.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-Nov-10 22:54 fairbench/reports/__init__.py
+-rw-rw-rw-  2.0 fat     1437 b- defN 24-Feb-13 17:25 fairbench/reports/accumulate.py
+-rw-rw-rw-  2.0 fat     3954 b- defN 24-May-19 10:45 fairbench/reports/adhoc.py
+-rw-rw-rw-  2.0 fat     2969 b- defN 24-May-18 21:56 fairbench/reports/base.py
+-rw-rw-rw-  2.0 fat      912 b- defN 24-Feb-13 10:59 fairbench/reports/surrogate.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-26 21:15 tests/__init__.py
--rw-rw-rw-  2.0 fat     1394 b- defN 23-Jun-12 10:06 tests/test_batching.py
--rw-rw-rw-  2.0 fat     1278 b- defN 23-Jun-01 09:09 tests/test_benchmarks.py
--rw-rw-rw-  2.0 fat     1103 b- defN 23-Jun-16 09:20 tests/test_demos.py
--rw-rw-rw-  2.0 fat     5807 b- defN 23-Jun-15 09:42 tests/test_forks.py
--rw-rw-rw-  2.0 fat     3391 b- defN 23-Jul-07 09:35 tests/test_metrics.py
--rw-rw-rw-  2.0 fat     1150 b- defN 23-Jun-29 09:15 tests/test_modelcards.py
--rw-rw-rw-  2.0 fat     1624 b- defN 23-Jun-14 06:40 tests/test_reduction.py
--rw-rw-rw-  2.0 fat     6556 b- defN 23-May-31 14:04 tests/test_reports.py
--rw-rw-rw-  2.0 fat      877 b- defN 23-Jul-11 12:06 fairbench-0.2.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 12:06 fairbench-0.2.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jul-11 12:06 fairbench-0.2.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3986 b- defN 23-Jul-11 12:06 fairbench-0.2.9.dist-info/RECORD
-47 files, 128869 bytes uncompressed, 31956 bytes compressed:  75.2%
+-rw-rw-rw-  2.0 fat     1613 b- defN 24-Feb-11 00:25 tests/test_batching.py
+-rw-rw-rw-  2.0 fat     1370 b- defN 24-May-16 19:11 tests/test_demos.py
+-rw-rw-rw-  2.0 fat     7095 b- defN 23-Nov-10 23:01 tests/test_forks.py
+-rw-rw-rw-  2.0 fat     4391 b- defN 24-Mar-21 21:33 tests/test_metrics.py
+-rw-rw-rw-  2.0 fat     1101 b- defN 24-May-18 11:04 tests/test_modelcards.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 23-Nov-10 16:55 tests/test_reduction.py
+-rw-rw-rw-  2.0 fat     8347 b- defN 24-May-19 11:18 tests/test_reports.py
+-rw-rw-rw-  2.0 fat      901 b- defN 24-May-19 11:35 fairbench-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-19 11:35 fairbench-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-19 11:35 fairbench-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     4408 b- defN 24-May-19 11:35 fairbench-0.3.0.dist-info/RECORD
+51 files, 145427 bytes uncompressed, 35478 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,116 +1,128 @@
 Filename: fairbench/__init__.py
 Comment: 
 
-Filename: fairbench/export.py
-Comment: 
-
-Filename: fairbench/stamps.py
+Filename: fairbench/verification.py
 Comment: 
 
 Filename: fairbench/bench/__init__.py
 Comment: 
 
 Filename: fairbench/bench/demos.py
 Comment: 
 
 Filename: fairbench/bench/loader.py
 Comment: 
 
-Filename: fairbench/export/__init__.py
+Filename: fairbench/blocks/__init__.py
 Comment: 
 
-Filename: fairbench/export/interactive.py
+Filename: fairbench/blocks/framework.py
 Comment: 
 
-Filename: fairbench/export/native.py
+Filename: fairbench/blocks/expanders/__init__.py
 Comment: 
 
-Filename: fairbench/export/modelcards/__init__.py
+Filename: fairbench/blocks/expanders/expanders.py
 Comment: 
 
-Filename: fairbench/export/modelcards/tohtml.py
+Filename: fairbench/blocks/metrics/__init__.py
 Comment: 
 
-Filename: fairbench/export/modelcards/tomarkdown.py
+Filename: fairbench/blocks/metrics/classification.py
 Comment: 
 
-Filename: fairbench/export/modelcards/toyaml.py
+Filename: fairbench/blocks/metrics/disparate_impact.py
 Comment: 
 
-Filename: fairbench/forks/__init__.py
+Filename: fairbench/blocks/metrics/disparate_mistreatment.py
 Comment: 
 
-Filename: fairbench/forks/categorical.py
+Filename: fairbench/blocks/metrics/ranking.py
 Comment: 
 
-Filename: fairbench/forks/explanation.py
+Filename: fairbench/blocks/metrics/regression.py
 Comment: 
 
-Filename: fairbench/forks/fork.py
+Filename: fairbench/blocks/reducers/__init__.py
 Comment: 
 
-Filename: fairbench/metrics/__init__.py
+Filename: fairbench/blocks/reducers/reducers.py
 Comment: 
 
-Filename: fairbench/metrics/classification.py
+Filename: fairbench/core/__init__.py
 Comment: 
 
-Filename: fairbench/metrics/disparate_impact.py
+Filename: fairbench/core/categorical.py
 Comment: 
 
-Filename: fairbench/metrics/disparate_mistreatment.py
+Filename: fairbench/core/fork.py
 Comment: 
 
-Filename: fairbench/metrics/ranking.py
+Filename: fairbench/core/compute/__init__.py
 Comment: 
 
-Filename: fairbench/metrics/regression.py
+Filename: fairbench/core/compute/backends.py
 Comment: 
 
-Filename: fairbench/mitigation/__init__.py
+Filename: fairbench/core/compute/delegation.py
 Comment: 
 
-Filename: fairbench/mitigation/postprocessing.py
+Filename: fairbench/core/explanation/__init__.py
 Comment: 
 
-Filename: fairbench/reports/__init__.py
+Filename: fairbench/core/explanation/base.py
 Comment: 
 
-Filename: fairbench/reports/accumulate.py
+Filename: fairbench/core/explanation/curve.py
 Comment: 
 
-Filename: fairbench/reports/adhoc.py
+Filename: fairbench/core/explanation/error.py
 Comment: 
 
-Filename: fairbench/reports/base.py
+Filename: fairbench/export/__init__.py
 Comment: 
 
-Filename: fairbench/reports/surrogate.py
+Filename: fairbench/export/interactive.py
+Comment: 
+
+Filename: fairbench/export/native.py
+Comment: 
+
+Filename: fairbench/export/modelcards/__init__.py
 Comment: 
 
-Filename: fairbench/reports/reduction/__init__.py
+Filename: fairbench/export/modelcards/tohtml.py
 Comment: 
 
-Filename: fairbench/reports/reduction/expanders.py
+Filename: fairbench/export/modelcards/tomarkdown.py
 Comment: 
 
-Filename: fairbench/reports/reduction/reduce.py
+Filename: fairbench/export/modelcards/toyaml.py
 Comment: 
 
-Filename: fairbench/reports/reduction/reducers.py
+Filename: fairbench/reports/__init__.py
 Comment: 
 
-Filename: tests/__init__.py
+Filename: fairbench/reports/accumulate.py
 Comment: 
 
-Filename: tests/test_batching.py
+Filename: fairbench/reports/adhoc.py
 Comment: 
 
-Filename: tests/test_benchmarks.py
+Filename: fairbench/reports/base.py
+Comment: 
+
+Filename: fairbench/reports/surrogate.py
+Comment: 
+
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/test_batching.py
 Comment: 
 
 Filename: tests/test_demos.py
 Comment: 
 
 Filename: tests/test_forks.py
 Comment: 
@@ -123,20 +135,20 @@
 
 Filename: tests/test_reduction.py
 Comment: 
 
 Filename: tests/test_reports.py
 Comment: 
 
-Filename: fairbench-0.2.9.dist-info/METADATA
+Filename: fairbench-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fairbench-0.2.9.dist-info/WHEEL
+Filename: fairbench-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fairbench-0.2.9.dist-info/top_level.txt
+Filename: fairbench-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fairbench-0.2.9.dist-info/RECORD
+Filename: fairbench-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fairbench/__init__.py

```diff
@@ -1,14 +1,21 @@
-from fairbench.forks import *
-from fairbench.metrics import *
+from fairbench.core import (
+    Fork,
+    categories,
+    binary,
+    Categories,
+    setbackend,
+    individuals,
+    simplify,
+)
+from fairbench.blocks import *
 from fairbench.reports import *
 from fairbench.export import *
 from fairbench.bench import *
 
-from fairbench import forks
-from fairbench import metrics
+from fairbench import core
+from fairbench import blocks
 from fairbench import reports
 from fairbench import export
-from fairbench import mitigation
 from fairbench import bench
-from fairbench import stamps
 from fairbench.bench import demos
+from fairbench.verification import stamps
```

## fairbench/bench/demos.py

```diff
@@ -3,53 +3,74 @@
 
 
 def adult(
     classifier=sklearn.linear_model.LogisticRegression(max_iter=1000).fit,
     scaler=sklearn.preprocessing.MinMaxScaler().fit_transform,
     predict="predict",
 ):
+    """
+    Creates demonstration outputs for the *adult* dataset.
+
+    :param classifier: A method returning a trained classifier from X, y training pairs.
+        Default is the `fit` method of sklearn's logistic regression for max_iter=1000.
+    :param scaler: A method to preprocess features X. Default is the `fit_transform` of sklearn's `MinMaxScaler`.
+    :param predict: Either "predict" (default) or "probabilities". The second option returns classification scores.
+    :return: A tuple of the test set, desired binary labels, and predicted binary labels or their probabilities.
+    """
     train = read_csv(
         "https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data",
         header=None,
         skipinitialspace=True,
     )
     test = read_csv(
         "https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.test",
         header=None,
         skipinitialspace=True,
         skiprows=[0],
     )
     numeric = [0, 4, 11, 12]
-    categorical = [1, 3, 5, 6]
+    categorical = [1, 3, 5, 6, 8, 9]
     x_train = features(train, numeric, categorical)
     y_train = (train[14] == ">50K").values
     x = features(test, numeric, categorical)
     y = (test[14] == ">50K.").values
     x_train = scaler(x_train)
     x = scaler(x)
+    if predict == "data":
+        return x_train, y_train, x, y, train, test
     classifier = classifier(x_train, y_train)
     if predict == "predict":
         yhat = classifier.predict(x)
     elif predict == "probabilities":
         yhat = classifier.predict_proba(x)[:, 1]
     else:
         raise NotImplementedError()
     return test, y, yhat
 
 
 def bank(
     classifier=sklearn.linear_model.LogisticRegression(max_iter=1000).fit,
     scaler=sklearn.preprocessing.MinMaxScaler().fit_transform,
     predict="predict",
+    seed=None,
 ):
+    """
+    Creates demonstration outputs for the *bank* dataset.
+
+    :param classifier: A method returning a trained classifier from X, y training pairs.
+        Default is the `fit` method of sklearn's logistic regression for max_iter=1000.
+    :param scaler: A method to preprocess features X. Default is the `fit_transform` of sklearn's `MinMaxScaler`.
+    :param predict: Either "predict" (default) or "probabilities". The second option returns classification scores.
+    :return: A tuple of the test set, desired binary labels, and predicted binary labels or their probabilities.
+    """
     data = read_csv(
         "https://archive.ics.uci.edu/static/public/222/bank+marketing.zip/bank/bank.csv",
         delimiter=";",
     )
-    train, test = sklearn.model_selection.train_test_split(data)
+    train, test = sklearn.model_selection.train_test_split(data, random_state=seed)
     numeric = ["age", "duration", "campaign", "pdays", "previous"]
     categorical = [
         "job",
         "marital",
         "education",
         "default",
         "housing",
@@ -59,14 +80,73 @@
     ]
     x_train = features(train, numeric, categorical)
     y_train = (train["y"] == "yes").values
     x = features(test, numeric, categorical)
     y = (test["y"] == "yes").values
     x_train = scaler(x_train)
     x = scaler(x)
+    if predict == "data":
+        return x_train, y_train, x, y, train, test
+    classifier = classifier(x_train, y_train)
+    if predict == "predict":
+        yhat = classifier.predict(x)
+    elif predict == "probabilities":
+        yhat = classifier.predict_proba(x)[:, 0]
+    else:
+        raise NotImplementedError()
+    return test, y, yhat
+
+
+def compas(
+    classifier=sklearn.linear_model.LogisticRegression(max_iter=1000).fit,
+    scaler=sklearn.preprocessing.MinMaxScaler().fit_transform,
+    predict="predict",
+    seed=None,
+):
+    """
+    Creates demonstration outputs for the *compas* dataset.
+
+    :param classifier: A method returning a trained classifier from X, y training pairs.
+        Default is the `fit` method of sklearn's logistic regression for max_iter=1000.
+    :param scaler: A method to preprocess features X. Default is the `fit_transform` of sklearn's `MinMaxScaler`.
+    :param predict: Either "predict" (default) or "probabilities". The second option returns classification scores.
+    :return: A tuple of the test set, desired binary labels, and predicted binary labels or their probabilities.
+    """
+    data = read_csv(
+        "https://raw.githubusercontent.com/propublica/compas-analysis/master/compas-scores-two-years.csv",
+        delimiter=",",
+    )
+    train, test = sklearn.model_selection.train_test_split(data, random_state=seed)
+    numeric = [
+        "age",
+        # "juv_fel_count",
+        # "decile_score",
+        # "juv_misd_count",
+        # "juv_other_count",
+        # "priors_count",
+        # "days_b_screening_arrest",
+    ]
+    categorical = [
+        "sex",
+        "c_charge_degree",
+        "race",
+        "is_recid",
+        # "violent_recid",
+        # "is_violent_recid",
+        # "vr_charge_degree",
+        # "v_decile_score"
+    ]
+    x_train = features(train, numeric, categorical)
+    y_train = (train["two_year_recid"] == 1).values
+    x = features(test, numeric, categorical)
+    y = (test["two_year_recid"] == 1).values
+    x_train = scaler(x_train)
+    x = scaler(x)
+    if predict == "data":
+        return x_train, y_train, x, y, train, test
     classifier = classifier(x_train, y_train)
     if predict == "predict":
         yhat = classifier.predict(x)
     elif predict == "probabilities":
         yhat = classifier.predict_proba(x)[:, 0]
     else:
         raise NotImplementedError()
```

## fairbench/bench/loader.py

```diff
@@ -31,15 +31,15 @@
         url += ".zip"
         temp = "data/" + url.split("/")[-1]
         if not os.path.exists(path):
             os.makedirs(os.path.join(*path.split("/")[:-1]), exist_ok=True)
             wget.download(url, temp)
             _extract_nested_zip(temp, extract_to)
     else:
-        shortened = "/".join(url.split("/")[-2:])
+        shortened = "/".join(url.split("/")[-4:])
         path = "data/" + shortened
         if not os.path.exists(path):
             os.makedirs("/".join(path.split("/")[:-1]), exist_ok=True)
             wget.download(url, path)
     return pd.read_csv(path, *args, **kwargs)
```

## fairbench/export/interactive.py

```diff
@@ -1,9 +1,11 @@
-from fairbench.forks.fork import Fork, Forklike
-from fairbench.forks.explanation import tofloat, ExplainableError
+import fairbench
+from fairbench.core.fork import Fork, Forklike
+from fairbench.core.explanation.base import tofloat
+from fairbench.core.explanation import ExplainableError
 
 
 def _clean(fork):  # pragma: no cover
     if isinstance(fork, Fork):
         branches = {k: _clean(v) for k, v in fork.branches().items()}
         branches = {k: v for k, v in branches.items() if v is not None}
         if not branches:
@@ -34,15 +36,22 @@
         else:
             return False  # Other type (?)
     except NameError:
         return False  # Probably standard Python interpreter
 
 
 def interactive(
-    report, name="report", width=800, height=400, spacing=None, horizontal=True
+    report,
+    name="report",
+    width=800,
+    height=400,
+    spacing=None,
+    horizontal=True,
+    port=8888,
+    browser=None,
 ):  # pragma: no cover
     """
     Creates an interactive visualization over a fairness report.
     :param report: A fairness report.
     :param name: Default is 'report'.
     :param width: The minimum width of interactive plot screens.
     :param height: The minimum height of interactive plot screens.
@@ -78,27 +87,33 @@
         if horizontal:
             plot = figure(
                 y_range=["1", "2"], width=width, height=height, x_axis_location="above"
             )
         else:
             plot = figure(x_range=["1", "2"], width=width, height=height)
         plot.add_tools(HoverTool(tooltips=[("Name", "@keys"), ("Value", "@values")]))
+        curves = figure(width=width, height=height)
         select_branch = RadioButtonGroup(
             labels=["ALL"] + list(report.branches().keys()), active=0
         )
         select_view = Select(
             value="Branches", options=["Branches", "Entries"], width=100, height=30
         )
         explain = Button(label="Explain", width=100, button_type="success")
         back = Button(label="Back", button_type="danger")
         explain.sizing_mode = "stretch_width"
         back.sizing_mode = "stretch_width"
         previous = [report]
         previous_title = [name]
         label = Div()
+        cannot_observe = Div()
+        cannot_observe.text = (
+            "Data too complicated to visualize. Focus on one branch or entry."
+        )
+        cannot_observe.visible = False
 
         def _asdict(obj):
             if isinstance(obj, Fork):
                 obj = obj.branches()
             if isinstance(obj, dict):
                 obj = {
                     k: v
@@ -112,25 +127,35 @@
             if selected_branch in branches:
                 return branches[selected_branch]
             return getattr(Forklike(branches), selected_branch)
 
         def _depth(obj):
             if obj is None:
                 return 0
-            if isinstance(obj, Fork):
-                return max(_depth(x) for x in obj.branches().values()) + 1
-            if isinstance(obj, dict):
-                if obj.values():
+            elif isinstance(obj, Fork):
+                branches = obj.branches()
+                if branches:
+                    return max(_depth(x) for x in branches.values()) + 1
+            elif isinstance(obj, dict):
+                if obj:
                     return max(_depth(x) for x in obj.values()) + 1
             return 0
 
         def _update_branches():
             branches = _asdict(previous[-1])
+            if not branches:
+                select_branch.labels = ["ALL"]
+                return
+
             if isinstance(previous[-1], Forklike) or isinstance(previous[-1], Fork):
-                val = list(branches.values())[0].role()
+                val = (
+                    ""
+                    if not hasattr(list(branches.values())[0], "role")
+                    else list(branches.values())[0].role()
+                )
                 prev_selection = select_view.value
                 options = ["Branch", "Entries" if val is None else val]
                 select_view.options = options
                 if prev_selection not in options:
                     select_view.value = options[0]
 
             if _depth(previous[-1]) <= 1:
@@ -157,52 +182,62 @@
             if horizontal:
                 plot.y_range.factors = []
             else:
                 plot.x_range.factors = []
             select_view.disabled = not True
             plot.title.text = "" if selected_branch == "ALL" else selected_branch
             plot.title_location = "above"
+            plot.visible = True
+            curves.visible = False
+            cannot_observe.visible = False
             if selected_branch == "ALL":
                 if horizontal:
                     plot.ygrid.grid_line_color = None
                 else:
                     plot.xgrid.grid_line_color = None
                 explain.visible = False
                 label.text = f"<h1>{'.'.join([t for t in previous_title if t!='ALL'])}</h1>Select a branch or entry to focus and explain it."
                 _source = dict()
                 if (select_view.value == select_view.options[0]) != isinstance(
                     previous[-1], Fork
                 ):
-                    for branch in branches.keys():
-                        for k, v in _asdict(branches[branch]).items():
-                            if k not in _source:
-                                _source[k] = list()
-                            _source[k].append(branch)
+                    if branches:
+                        for branch in branches.keys():
+                            for k, v in _asdict(branches[branch]).items():
+                                if k not in _source:
+                                    _source[k] = list()
+                                _source[k].append(branch)
                     try:
                         values = [
                             tofloat(_asdict(branches[branch])[metric])
                             for metric in order(_source)
                             for branch in order(_source[metric])
                         ]
                     except TypeError:
+                        cannot_observe.visible = True
+                        plot.visible = False
                         return
                 else:
                     for branch in branches.keys():
                         for k, v in _asdict(branches[branch]).items():
                             if branch not in _source:
                                 _source[branch] = list()
                             _source[branch].append(k)
                     try:
                         values = [
                             tofloat(_asdict(branches[branch])[metric])
                             for branch in order(_source)
                             for metric in order(_source[branch])
                         ]
                     except TypeError:
+                        cannot_observe.visible = True
+                        plot.visible = False
                         return
+                if not _source:
+                    pass
                 keys = [
                     (metric, branch)
                     for metric in order(_source)
                     for branch in order(_source[metric])
                 ]
                 if horizontal:
                     plot.height = max(height, spacing * len(keys))
@@ -252,14 +287,37 @@
                 select_view.disabled = not True
             else:
                 select_view.disabled = not False
                 label.text = f"<h1>{'.'.join([t for t in previous_title if t!='ALL'])}.<em>{selected_branch}</em></h1>Select ALL to switch between branch and entry views."
                 plot_data = _branch(selected_branch)
                 explain.visible = hasattr(plot_data, "explain")
                 plot_data = _asdict(plot_data)
+                if hasattr(plot_data, "keys") and (
+                    not list(plot_data.keys())
+                    or isinstance(
+                        plot_data[list(plot_data.keys())[0]], fairbench.ExplanationCurve
+                    )
+                ):
+                    plot.visible = False
+                    curves.visible = True
+                    curves.renderers = []
+                    curves.legend.items = []
+                    for i, k in enumerate(plot_data):
+                        curve = plot_data[k]
+                        curves.line(
+                            curve.x,
+                            curve.y,
+                            line_color=Category20[20][i],
+                            line_width=2,
+                            legend_label=curve.name + " of " + k,
+                        )
+                    if plot_data:
+                        curves.legend.location = "bottom_right"
+                    # curves.legend.title = selected_branch
+                    return
                 plot_data = {k: plot_data[k] for k in order(plot_data)}
                 keys = list(plot_data.keys())
                 if horizontal:
                     plot.height = max(height, spacing * len(keys))
                     plot.y_range.factors = keys
                 else:
                     plot.width = max(width, spacing * len(keys))
@@ -340,15 +398,19 @@
                     if label == branch_name:
                         select_branch.active = i
             # if select_branch.active in branches and _depth(branches[select_branch.active ]) > 1:
             #    previous_title.pop()
             update_plot(doc)
 
         def update_value(doc):
-            selected_branch = select_branch.labels[select_branch.active]
+            selected_branch = (
+                select_branch.labels[select_branch.active]
+                if select_branch.labels
+                else "ALL"
+            )
             if selected_branch != "ALL" and _depth(_branch(selected_branch)) > 1:
                 previous_title.append(selected_branch)
                 branch = _branch(selected_branch)
                 previous.append(_clean(branch))
                 _update_branches()
                 select_branch.active = 0
             update_plot(doc)
@@ -361,24 +423,28 @@
         _update_branches()
         select_branch.on_change("active", lambda attr, old, new: update_value(doc))
         select_view.on_change("value", lambda attr, old, new: update_view(doc))
         explain.on_click(explain_button)
         back.on_click(back_button)
         update_plot(doc)
         controls = row(select_view, select_branch, back, explain)
-        doc.add_root(column(label, controls, plot))
+        doc.add_root(column(label, controls, plot, curves, cannot_observe))
 
     app = Application(FunctionHandler(modify_doc))
-    if _in_jupyter():
+    if browser is not None and not browser and _in_jupyter():
         from bokeh.io import show
         from bokeh.plotting import output_notebook
+        import os
 
+        os.environ["BOKEH_ALLOW_WS_ORIGIN"] = "localhost:" + str(port)
         output_notebook()
         show(app)
         return
+    if browser is not None and browser == False:
+        raise Exception("Cannot set broswer=False when not using Jupyter,")
     server = Server({"/": app}, num_procs=1)
     server.start()
     address = server.address.split(":")[0] if server.address else "localhost"
     server_url = f"http://{address}:{server.port}/"
     print(f"Bokeh server started at {server_url}")
 
     try:
```

## fairbench/export/native.py

```diff
@@ -1,13 +1,13 @@
-from fairbench.forks.fork import Fork, Forklike
+from fairbench.core.fork import Fork, Forklike
 from fairbench.reports.accumulate import todict
 from matplotlib import pyplot as plt
 import json
-from fairbench.forks.explanation import tofloat
-from fairbench.forks import ExplanationCurve
+from fairbench.core.explanation.base import tofloat
+from fairbench.core import ExplanationCurve
 
 
 def _is_fork_of_dicts(report):
     return isinstance(report[next(iter(report))], dict)
 
 
 def tojson(report: Fork):
@@ -53,35 +53,39 @@
                     + [f"{entry:.3f}".ljust(spacing) for entry in report[metric]]
                 )
                 + "\n"
             )
     print(ret)
 
 
-def visualize(report: Fork, hold: bool = False, xrotation: int = 0):
+def visualize(
+    report: Fork, hold: bool = False, xrotation: int = 0, legend: bool = True
+):
     report = json.loads(tojson(report))
-
+    num_metrics = len([metric for metric in report if metric != "header"])
     i = 1
     for metric in report:
         if metric != "header":
-            plt.subplot(2, len(report) // 2, i)
+            if num_metrics > 1:
+                plt.subplot(2, len(report) // 2, i)
             barplots = False
             for j, case in enumerate(report["header"][1:]):
                 if isinstance(report[metric][j], float):
                     plt.bar(j, report[metric][j])
                     barplots = True
                 else:
                     plt.plot(
                         report[metric][j]["x"],
                         report[metric][j]["y"],
                         label=report["header"][1 + j],
                     )
             if barplots:
                 plt.xticks(list(range(len(report["header"][1:]))), report["header"][1:])
                 plt.xticks(rotation=-xrotation, ha="right" if xrotation < 0 else "left")
-            else:
+            elif legend:
                 plt.legend()
             plt.title(metric)
             i += 1
-    plt.tight_layout()
+    if num_metrics > 1:
+        plt.tight_layout()
     if not hold:
         plt.show()
```

## fairbench/export/modelcards/tohtml.py

```diff
@@ -1,11 +1,11 @@
 from fairbench.export.modelcards.toyaml import toyamlprimitives
 import webbrowser
 import tempfile
-from fairbench.forks import Fork, Explainable
+from fairbench.core import Fork, Explainable, ExplainableError
 
 
 def _resulttohtml(value, inline=False):
     if value == "False":
         return "&#10060;"
     if value == "True":
         return "&#9989;"
@@ -30,14 +30,16 @@
             if not isinstance(report, Fork)
             else getattr(report, row["name"])
         )
         while isinstance(metric_fork, Explainable):
             metric_fork = metric_fork.explain
         if isinstance(metric_fork, Fork):
             metric_fork = metric_fork.branches()
+        if isinstance(metric_fork, ExplainableError):
+            raise Exception(metric_fork.explain)
         factors.extend(metric_fork.keys())
         if table:
             caveats.extend(row["caveats"])
             if not prepend:
                 prepend += "\n<h2>Evaluation Results</h2>\n<table>\n"
                 prepend += "<tr><th>Metric</th><th>Value</th></tr>\n"
             prepend += f'<tr><td>{row["name"]}</td><td>{results}</td></tr>\n'
```

## fairbench/export/modelcards/tomarkdown.py

```diff
@@ -1,11 +1,11 @@
 from fairbench.export.modelcards.toyaml import toyamlprimitives
 import webbrowser
 import tempfile
-from fairbench.forks import Fork, Explainable
+from fairbench.core import Fork, Explainable, ExplainableError
 
 
 def _resulttomarkdown(value, inline=False):
     if value == "False":
         return ":x:"
     if value == "True":
         return ":heavy_check_mark:"
@@ -29,14 +29,17 @@
             if not isinstance(report, Fork)
             else getattr(report, row["name"])
         )
         while isinstance(metric_fork, Explainable):
             metric_fork = metric_fork.explain
         if isinstance(metric_fork, Fork):
             metric_fork = metric_fork.branches()
+        if isinstance(metric_fork, ExplainableError):
+            raise Exception(metric_fork.explain)
+            # continue
         factors.extend(metric_fork.keys())
         if table:
             caveats.extend(row["caveats"])
             if not prepend:
                 prepend += "\n\n## Evaluation Results\n"
                 prepend += "| Metric | Value |\n"
                 prepend += "| ------ | ----- |\n"
```

## fairbench/export/modelcards/toyaml.py

```diff
@@ -5,19 +5,34 @@
 
 
 def toyamlprimitives(report):
     if isinstance(report, Fork):
         report = report.branches()
     result = list()
     for metric, value in report.items():
+        stamp = value.stamp
+        symbols = stamp.symbols
+        description = stamp.desc
+        caveats = stamp.caveats
+        value = str(value)
+        if value == "True" and stamp.caveats_accept is not None:
+            caveats = caveats + stamp.caveats_accept
+        if value == "False" and stamp.caveats_reject is not None:
+            caveats = caveats + stamp.caveats_reject
+        if symbols:
+            for symbol, replace in symbols.items():
+                description = description.replace("{" + symbol + "}", replace)
+                caveats = [
+                    caveat.replace("{" + symbol + "}", replace) for caveat in caveats
+                ]
         metric_dict = {
             "name": metric,
-            "description": value.desc.desc,
-            "results": str(value),
-            "caveats": value.desc.caveats,
+            "description": description,
+            "results": value,
+            "caveats": caveats,
         }
         result.append(metric_dict)
     return result
 
 
 def toyaml(report):
     return yaml.dump({"Metrics": toyamlprimitives(report)})
```

## fairbench/reports/__init__.py

```diff
@@ -1,5 +1,4 @@
 from fairbench.reports.accumulate import *
 from fairbench.reports.base import *
-from fairbench.reports.reduction import *
 from fairbench.reports.surrogate import *
 from fairbench.reports.adhoc import *
```

## fairbench/reports/accumulate.py

```diff
@@ -1,9 +1,8 @@
-from fairbench.forks.fork import comparator, parallel_primitive, astensor, merge
-from fairbench.forks.explanation import Explainable
+from fairbench.core.fork import comparator, parallel_primitive, astensor, merge
 import eagerpy as ep
 
 
 """
 This module provides helper methods to concatenate tensors stored within Forks of tensor or Forks of dicts of tensors
 and use the final output in one report at the end.
 """
```

## fairbench/reports/adhoc.py

```diff
@@ -1,71 +1,126 @@
 from fairbench.reports.base import report
-from fairbench.reports import reduction as fb
+from fairbench.blocks import framework, reducers, expanders, metrics
 from fairbench.reports.accumulate import todict as tokwargs
-from fairbench.forks.fork import combine, merge, role
+from fairbench.core.fork import combine, merge, role, tobackend, Fork
 from fairbench.reports.surrogate import surrogate_positives
-from fairbench import metrics
-from fairbench.reports import reduction
+from fairbench.blocks.reducers import identical
+import numpy as np
+from makefun import wraps
 
+# TODO: create a differentiable report (and maybe separate metrics into subpackages of diffs vs normal)
+# TODO: have to check which values are differentiable
 
-common_metrics = (metrics.accuracy, metrics.prule, metrics.dfpr, metrics.dfnr)
-acc_metrics = (
+common_adhoc_metrics = (
+    metrics.accuracy,
+    metrics.prule,
+    metrics.dfpr,
+    metrics.dfnr,
+)
+
+common_performance_metrics = (
     metrics.accuracy,
     metrics.pr,
     metrics.tpr,
     metrics.tnr,
     metrics.auc,
-    metrics.phi,
-    metrics.hr,
-    metrics.reck,
-    metrics.ap,
+    metrics.avgscore,
+    metrics.tophr,
+    metrics.toprec,
+    metrics.mae,
+    metrics.rmse,
+    metrics.avghr,
+    metrics.avgrepr,
     metrics.r2,
 )
+
 common_reduction = (
-    {"reducer": reduction.min},
-    {"reducer": reduction.wmean},
-    {"reducer": reduction.min, "expand": reduction.ratio},
-    {"reducer": reduction.max, "expand": reduction.diff},
-    {"reducer": reduction.max, "expand": reduction.barea},
+    {"reducer": reducers.min},
+    {"reducer": reducers.wmean},
+    {"reducer": reducers.gini},
+    {"reducer": reducers.min, "expand": expanders.ratio},
+    {"reducer": reducers.max, "expand": expanders.diff},
+    {"reducer": reducers.max, "expand": expanders.barea},
+    {"reducer": reducers.max, "expand": expanders.rarea},
+    {"reducer": reducers.max, "expand": expanders.bdcg},
+    # {"reducer": reducers.max, "expand": expanders.jsdcg},
 )
 
 
-def accreport(*args, metrics=acc_metrics, **kwargs):
+def accreport(*args, metrics=common_performance_metrics, **kwargs):
     return report(*args, metrics=metrics, **kwargs)
 
 
-def binreport(*args, metrics=common_metrics, **kwargs):
+def binreport(*args, metrics=common_adhoc_metrics, **kwargs):
     return report(*args, metrics=metrics, **kwargs)
 
 
 @role("report")
 def multireport(
-    *args, metrics=acc_metrics, reduction_schemes=common_reduction, **kwargs
+    *args,
+    metrics=common_performance_metrics,
+    reduction_schemes=common_reduction,
+    compare_all_to=None,
+    **kwargs
 ):
     base = report(*args, metrics=metrics, **kwargs)
-    return combine(*[fb.reduce(base, **scheme) for scheme in reduction_schemes])
+    return combine(
+        *[
+            framework.reduce(base, **scheme, base=compare_all_to)
+            for scheme in reduction_schemes
+        ]
+    )
+
+
+@role("report")
+def unireport(
+    *args,
+    metrics=common_performance_metrics,
+    reduction_schemes=common_reduction,
+    **kwargs
+):
+    def modify_kwargs(kwargs):
+        # adds an additional branch for the whole population called Any
+        if "sensitive" in kwargs and "Any" not in kwargs["sensitive"]._branches:
+            length = framework.areduce(
+                kwargs["sensitive"].shape[0], identical
+            )  # asserts that everything has the same identical shape and returns it
+            length = int(length.value)  # retrieve int value from the explainable
+            kwargs["sensitive"]._branches["Any"] = tobackend(np.ones((length,)))
+        return kwargs
+
+    base = report(*args, metrics=metrics, modify_kwargs=modify_kwargs, **kwargs)
+    # perform the reduction while accounting for the
+    return combine(
+        *[
+            framework.reduce(
+                base, **scheme, base="Any" if "expand" in scheme else None
+            )  # the bas kwarg refers to the base fork branch of the base report
+            for scheme in reduction_schemes
+        ]
+    )
 
 
 @role("report")
 def isecreport(*args, **kwargs):
     if len(args) == 0:
         params = tokwargs(**kwargs)
     else:
         params = dict()
         for arg in args:
             params = merge(params, arg)
         params = merge(params, kwargs)
 
-    bayesian = fb.reduce(
+    bayesian = framework.reduce(
         surrogate_positives(params["predictions"], params["sensitive"]),
-        fb.min,
-        fb.ratio,
+        reducers.min,
+        expanders.ratio,
         name="bayesian",
     )
 
-    empirical = fb.reduce(
+    empirical = framework.reduce(
         metrics.pr(predictions=params["predictions"], sensitive=params["sensitive"]),
-        fb.min,
-        fb.ratio,
+        reducers.min,
+        expanders.ratio,
         name="empirical",
     )
     return combine(tokwargs(minprule=empirical), tokwargs(minprule=bayesian))
```

## fairbench/reports/base.py

```diff
@@ -1,31 +1,42 @@
-from fairbench.forks.fork import parallel_primitive, comparator, role
-from fairbench.forks.explanation import Explainable
+from fairbench.core.fork import parallel_primitive, comparator, role, Fork
+from fairbench.core.explanation import Explainable
 import inspect
 from typing import Union, Iterable, Callable
 
 
 def reportargsparse(*args, **kwargs):
     for arg in args:
-        if not isinstance(arg, dict):
+        if not isinstance(arg, dict) and not isinstance(arg, Fork):
             raise TypeError(
                 "Reports only support dicts of arguments as positional arguments"
             )
         for k, v in arg.items():
             if k in kwargs:
                 raise TypeError(f"Report argument {k} provided multiple times")
             kwargs[k] = v
     return kwargs
 
 
+def report(
+    *args, metrics: Union[Callable, Iterable, dict] = None, modify_kwargs=None, **kwargs
+):
+    """
+    This is a wrapper method of the true _report method, which also adds the prospect of modifying kwargs.
+    """
+    kwargs = reportargsparse(*args, **kwargs)
+    if modify_kwargs is not None:
+        kwargs = modify_kwargs(kwargs)
+    return _report(metrics, **kwargs)
+
+
 @role("report")
 @comparator
 @parallel_primitive
-def report(*args, metrics: Union[Callable, Iterable, dict] = None, **kwargs):
-    kwargs = reportargsparse(*args, **kwargs)
+def _report(metrics: Union[Callable, Iterable, dict] = None, **kwargs):
     assert (
         metrics is not None
     ), "Cannot use fairbench.report() without explicitly declared metrics.\nUse accreport, binreport, multireport, or isecreport as ad-hoc report generation mechanisms."
     if not isinstance(metrics, Iterable):
         metrics = [metrics]
     if not isinstance(metrics, dict):
         metrics = {metric.__name__: metric for metric in metrics}
```

## fairbench/reports/surrogate.py

```diff
@@ -1,21 +1,21 @@
-from fairbench.reports import reduce, todata, identical
-from fairbench.forks.fork import Fork, multibranch_tensors
+from fairbench.blocks import framework, todata, identical
+from fairbench.core.fork import Fork, multibranch_tensors
 from sklearn.linear_model import LogisticRegression
 import numpy as np
 
 
 @multibranch_tensors
 def surrogate_positives(
     predictions, sensitive, surrogate_model=LogisticRegression(max_iter=1000)
 ):
-    predictions = np.round(reduce(predictions, identical, name=None).numpy())
-    X = reduce(sensitive, todata, name=None).numpy()
+    predictions = np.round(framework.reduce(predictions, identical, name=None).numpy())
+    X = framework.reduce(sensitive, todata, name=None).numpy()
     surrogate_model = surrogate_model.fit(X, predictions)
     prediction_branches = dict()
-    for branches in sensitive.intersections():
+    for branches in sensitive.iterate_intersections():
         Xbranch = np.array(
             [[1 if branch in branches else 0 for branch in sensitive._branches]]
         )
         yhat = float(surrogate_model.predict_proba(Xbranch)[:, 1])
         prediction_branches["&".join(branches)] = yhat
     return Fork(prediction_branches)
```

## tests/test_batching.py

```diff
@@ -3,33 +3,51 @@
 from .test_forks import environment
 
 
 def test_batch_accumulation():
     for _ in environment():
         import torch
         import sklearn
+
         fb.setbackend("torch")
-        x = [[0, 0.1], [0.9, 0], [0, 0.1], [1.1, -0.1], [0.1, 0.1], [0.9, 0.1], [0.4, 0.5], [0.6, 0.3]]
+        x = [
+            [0, 0.1],
+            [0.9, 0],
+            [0, 0.1],
+            [1.1, -0.1],
+            [0.1, 0.1],
+            [0.9, 0.1],
+            [0.4, 0.5],
+            [0.6, 0.3],
+        ]
         y = [0, 1, 0, 1, 0, 1, 1, 1]
         s = [0, 0, 0, 0, 1, 1, 1, 1]
 
-        x, y, s = torch.from_numpy(np.array(x)), torch.from_numpy(np.array(y)), torch.from_numpy(np.array(s))
+        x, y, s = (
+            torch.from_numpy(np.array(x)),
+            torch.from_numpy(np.array(y)),
+            torch.from_numpy(np.array(s)),
+        )
         s2 = [0, 1, 1, 1, 1, 1, 1, 1]
         s3 = np.array(s2)
         # s = 1-s2  # really hard imbalance in the sensitive (isecreport handles this)
         s2 = 1 - s
         sensitive = fb.Fork(gender=s, ehtnicity=s2, ethinicity2=s3)
 
         classifier = sklearn.linear_model.LogisticRegression()
         classifier = classifier.fit(x, y)
         yhat = classifier.predict(x)
 
         vals = None
-        vals = fb.concatenate(vals, fb.todict(predictions=yhat, labels=y, sensitive=sensitive))
-        vals = fb.concatenate(vals, fb.todict(predictions=yhat, labels=y, sensitive=sensitive))
+        vals = fb.concatenate(
+            vals, fb.todict(predictions=yhat, labels=y, sensitive=sensitive)
+        )
+        vals = fb.concatenate(
+            vals, fb.todict(predictions=yhat, labels=y, sensitive=sensitive)
+        )
 
         report = fb.isecreport(vals)
         fb.describe(report)
         assert report.minprule.bayesian.value > 0.4
         fb.setbackend("numpy")
         report = fb.multireport(vals)
         fb.describe(report)
```

## tests/test_demos.py

```diff
@@ -1,26 +1,37 @@
 import fairbench as fb
 from .test_forks import environment
 
 
 def test_settings(monkeypatch):
     from matplotlib import pyplot as plt
-    monkeypatch.setattr(plt, 'show', lambda: None)
+
+    monkeypatch.setattr(plt, "show", lambda: None)
     for _ in environment():
-        for setting, protected in [(fb.demos.adult, 8), (fb.demos.bank, "marital")]:
+        for setting, protected in [
+            (fb.demos.adult, 8),
+            (fb.demos.bank, "marital"),
+            (fb.demos.compas, "sex"),
+        ]:
             test, y, yhat = setting()
-            sensitive = fb.Fork(fb.categories@test[protected])
+            sensitive = fb.Fork(fb.categories @ test[protected])
             report = fb.multireport(predictions=yhat, labels=y, sensitive=sensitive)
             fb.visualize(report)
             fb.visualize(report.min.accuracy.explain.explain)
             fb.visualize(report.min.accuracy.explain)
             fb.visualize(report.min.explain)
 
 
 def test_curve_visualization(monkeypatch):
     from matplotlib import pyplot as plt
+
     for _ in environment():
-        monkeypatch.setattr(plt, 'show', lambda: None)
-        test, y, yhat = fb.demos.adult(predict="probabilities")
-        s = fb.Fork(fb.categories @ test[9])
-        report = fb.multireport(scores=yhat, labels=y, sensitive=s)
-        fb.visualize(report.min.auc.explain.explain)
+        for setting, protected in [
+            (fb.demos.adult, 9),
+            (fb.demos.bank, "marital"),
+            (fb.demos.compas, "sex"),
+        ]:
+            monkeypatch.setattr(plt, "show", lambda: None)
+            test, y, yhat = setting(predict="probabilities")
+            s = fb.Fork(fb.categories @ test[protected])
+            report = fb.multireport(scores=yhat, labels=y, sensitive=s)
+            fb.visualize(report.min.auc.explain.explain)
```

## tests/test_forks.py

```diff
@@ -1,83 +1,103 @@
 import fairbench as fb
 import numpy as np
 
 
 def environment():
-    for _ in ["torch", "numpy"]:
-        fb.distributed()
-        yield "distributed"
-        fb.serial()
-        yield "serial"
+    for env in ["torch", "tensorflow", "jax", "numpy"]:
+        fb.setbackend(env)
+        yield env
 
 
 def test_conversion_number():
     for _ in environment():
         x = np.float64(2)
         y = fb.astensor(x).log()
-        x2 = fb.fromtensor(y)
-        assert isinstance(x2, np.float64)
+        x2 = fb.core.asprimitive(y)
+        fb.setbackend("numpy")
+        x2 = fb.core.asprimitive(x2)
+        assert abs(x2 - np.float64(0.69314718)) < 0.0000001
 
 
 def test_explainble():
     x = fb.Explainable(fb.astensor(1))
     y = fb.Explainable(fb.astensor(np.float32(2)))
-    assert x/y == 0.5
+    assert x / y == 0.5
 
 
 def test_fork_generation():
     for _ in environment():
         fork = fb.Fork(a=1)
         assert fork.a == 1
         fork = fb.Fork(a=1, b=2, c=3)
         assert fork.a == 1
         assert fork.b == 2
         assert fork.c == 3
 
 
 def test_categories():
     for _ in environment():
-        branches = fb.Fork(fb.categories@["Man", "Woman", "Man", "Woman"]).branches()
+        branches = fb.Fork(fb.categories @ ["Man", "Woman", "Man", "Woman"]).branches()
         assert "Man" in branches
         assert "Woman" in branches
 
-        branches = fb.Fork(gender=fb.categories@{"Man": [0, 1], "Woman": [0, 1]}).branches()
+        branches = fb.Fork(
+            gender=fb.categories @ {"Man": [0, 1], "Woman": [0, 1]}
+        ).branches()
         assert "genderMan" in branches
         assert "genderWoman" in branches
 
         branches = fb.Fork({"Man": [0, 1], "Woman": [0, 1]}).branches()
         assert "Man" in branches
         assert "Woman" in branches
 
-        branches = fb.Fork(attr=fb.Categories(range(4))@[0, 1, 2, 0, 1]).branches()
+        branches = fb.Fork(attr=fb.Categories(range(4)) @ [0, 1, 2, 0, 1]).branches()
         assert "attr0" in branches
         assert "attr1" in branches
         assert "attr2" in branches
         assert "attr3" in branches
 
         branches = fb.Fork(attr=fb.Categories(range(4))([0, 1, 2, 0, 1])).branches()
         assert "attr0" in branches
         assert "attr1" in branches
         assert "attr2" in branches
         assert "attr3" in branches
 
 
 def test_intersectional():
-    branches = fb.Fork(gender=fb.binary(np.array([0, 1, 0, 1])),  # same notation as bellow
-                       race=fb.binary@np.array([1, 1, 0, 0])).intersectional().branches()
+    branches = (
+        fb.Fork(
+            gender=fb.binary(np.array([0, 1, 0, 1])),  # same notation as bellow
+            race=fb.binary @ np.array([1, 1, 0, 0]),
+        )
+        .intersectional()
+        .branches()
+    )
     assert len(branches) == 8
 
-    branches = fb.Fork(gender=fb.binary(np.array([0, 1, 0, 1])),  # same notation as bellow
-                       race=fb.binary@np.array([0, 1, 0, 1])).intersectional().branches()
+    branches = (
+        fb.Fork(
+            gender=fb.binary(np.array([0, 1, 0, 1])),  # same notation as bellow
+            race=fb.binary @ np.array([0, 1, 0, 1]),
+        )
+        .intersectional()
+        .branches()
+    )
     assert len(branches) == 6
 
-    branches = fb.Fork(sensitive=fb.binary@np.array([0, 1, 0, 1]) & fb.binary@np.array([0, 1, 0, 1])).branches()
+    branches = fb.Fork(
+        sensitive=fb.binary @ np.array([0, 1, 0, 1])
+        & fb.binary @ np.array([0, 1, 0, 1])
+    ).branches()
     assert len(branches) == 4
 
-    branches = fb.Fork(sensitive=fb.binary@[0, 1, 0, 1] | fb.categories@["Man", "Woman", "Man", "Woman"]).branches()
+    branches = fb.Fork(
+        sensitive=fb.binary @ [0, 1, 0, 1]
+        | fb.categories @ ["Man", "Woman", "Man", "Woman"]
+    ).branches()
     assert len(branches) == 4
 
 
 def test_fork_operations():
     for _ in environment():
         fork = fb.Fork(a=1)
         assert (fork == 1).a
@@ -87,38 +107,42 @@
         assert (fork >= 1).a
         assert (fork >= 0).a
         assert not (fork <= 0).a
         assert (fork <= 1).a
         assert not (fork < 0).a
         assert not (fork < 1).a
         assert not (fork > 1).a
-        assert (fork+2).a == 3
-        assert (2+fork).a == 3
-        assert (fork-2).a == -1
-        assert (2-fork).a == 1
-        assert (fork/2).a == 0.5
-        assert (2/fork).a == 2
-        assert (fork//2).a == 0
-        assert (2//fork).a == 2
-        assert (fork*2).a == 2
-        assert (2*fork).a == 2
+        assert (fork + 2).a == 3
+        assert (2 + fork).a == 3
+        assert (fork - 2).a == -1
+        assert (2 - fork).a == 1
+        assert (fork / 2).a == 0.5
+        assert (2 / fork).a == 2
+        assert (fork // 2).a == 0
+        assert (2 // fork).a == 2
+        assert (fork * 2).a == 2
+        assert (2 * fork).a == 2
+        assert ((1 + fork) ** 3).a == 8
+        assert (3 ** (1 + fork)).a == 9
         assert (abs(-fork) == 1).a
 
 
 def test_fork_getattr():
     for _ in environment():
-        fork = fb.Fork(a=np.array([1, 2, 3]), b=np.array([2, 3, 4]), c=np.array([3, 4, 5]))
+        fork = fb.Fork(
+            a=np.array([1, 2, 3]), b=np.array([2, 3, 4]), c=np.array([3, 4, 5])
+        )
         sums = fork.sum()
         assert sums.a == 6
         assert sums.b == 9
         assert sums.c == 12
 
 
 def test_fork_of_dicts():
-    #for _ in environment():  # TODO: the following don't work for distributed
+    # for _ in environment():  # TODO: the following don't work for distributed
     fork = fb.Fork(a={"x": 1, "y": 2}, b={"x": 2, "y": 4})
     fork["z"] = fork.x + fork.y
     del fork["x"]
     del fork["y"]
     assert len(fork.a) == 1
     assert len(fork.b) == 1
     assert fork.a["z"] == 3
@@ -149,27 +173,66 @@
         assert fork.x.b == fork.b.x
         assert fork.y.a == fork.a.y
         assert fork.y.b == fork.b.y
         assert isinstance(fork.y.b, int)
 
 
 def test_fork_to_array():
-    import fairbench as fb
-    import numpy as np
+    sensitive = fb.Fork(
+        gender=fb.categories @ np.array([1, 0, 0, 1]),
+        race=fb.categories @ np.array([0, 1, 2, 3]),
+        age=fb.categories @ np.array([3, 1, 2, 0]),
+    )
+
+    report = fb.multireport(
+        predictions=np.array([0, 0, 1, 1]),
+        labels=np.array([0, 1, 1, 0]),
+        sensitive=sensitive,
+    )
+    print(report)
 
-    sensitive = fb.Fork(gender=fb.categories@np.array([1, 0, 0, 1]),
-                        race=fb.categories@np.array([0, 1, 2, 3]),
-                        age=fb.categories@np.array([3, 1, 2, 0]))
 
-    report = fb.multireport(predictions=np.array([0, 0, 1, 1]), labels=np.array([0, 1, 1, 0]), sensitive=sensitive)
-    print(report)
+def test_fork_to_str():
+    fork = fb.Fork(a={"c": 1.0, "d": 2.0}, b={"c": 3.0, "d": 4.0})
+    converted = str(fork)
+    assert "1.0" in converted
+    assert "2.0" in converted
+    assert "3.0" in converted
+    assert "4.0" in converted
+
+
+def test_fork_to_html():
+    fork = fb.Fork(
+        a={"c": 1.0, "d": {"value": "2.0b"}}, b={"c": 3.0, "d": 4.0}
+    )  # just something complex
+    converted = fork._repr_html_()
+    assert "1.0" in converted
+    assert "2.0b" in converted
+    assert "3.0" in converted
+    assert "4.0" in converted
+    assert "<table>" in converted
+    assert "<tr><td><strong>c" in converted
+    assert "<tr><td><strong>d" in converted
+
+
+def test_fork_of_iterables():
+    fork = fb.Fork(a={"c": 1.0, "d": 2.0}, b={"c": 3.0, "d": 4.0})
+    assert len(fork) == 2
+    for k, v in fork.items():
+        assert k in ["c", "d"]
+        assert "a" in v.branches()
+        assert "b" in v.branches()
 
 
 def test_fork_direct_explain():
-    import fairbench as fb
-    import numpy as np
-    sensitive = fb.Fork(gender=fb.categories@np.array([1, 0, 0, 1]),
-                        race=fb.categories@np.array([0, 1, 2, 3]),
-                        age=fb.categories@np.array([3, 1, 2, 0]))
-    report = fb.multireport(predictions=np.array([0, 0, 1, 1]), labels=np.array([0, 1, 1, 0]), sensitive=sensitive)
+    sensitive = fb.Fork(
+        gender=fb.categories @ np.array([1, 0, 0, 1]),
+        race=fb.categories @ np.array([0, 1, 2, 3]),
+        age=fb.categories @ np.array([3, 1, 2, 0]),
+    )
+    report = fb.multireport(
+        predictions=np.array([0, 0, 1, 1]),
+        labels=np.array([0, 1, 1, 0]),
+        sensitive=sensitive,
+    )
     explanation = report.explain
     assert "min" in explanation.branches()
```

## tests/test_metrics.py

```diff
@@ -1,88 +1,161 @@
 import fairbench as fb
 from .test_forks import environment
 
 
 def test_accuracy():
     for _ in environment():
         assert fb.accuracy(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 1, 0])) < 1
-        assert fb.accuracy(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 1, 0]), fb.astensor([1, 1, 0, 1])) == 1
+        assert (
+            fb.accuracy(
+                fb.astensor([1, 1, 0, 0]),
+                fb.astensor([1, 1, 1, 0]),
+                fb.astensor([1, 1, 0, 1]),
+            )
+            == 1
+        )
 
 
 def test_tpr():
     for _ in environment():
         assert fb.tpr(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 1, 0])) == 1
         assert fb.tpr(fb.astensor([1, 1, 1, 0]), fb.astensor([1, 1, 0, 0])) < 1
-        assert fb.tpr(fb.astensor([1, 1, 1, 0]), fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 0, 1])) == 1
+        assert (
+            fb.tpr(
+                fb.astensor([1, 1, 1, 0]),
+                fb.astensor([1, 1, 0, 0]),
+                fb.astensor([1, 1, 0, 1]),
+            )
+            == 1
+        )
 
 
 def test_tnr():
     for _ in environment():
         assert fb.tnr(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 1, 0])) < 1
         assert fb.tnr(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 0, 0, 0])) == 1
-        assert fb.tnr(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 1, 0]), fb.astensor([1, 1, 0, 1])) == 1
+        assert (
+            fb.tnr(
+                fb.astensor([1, 1, 0, 0]),
+                fb.astensor([1, 1, 1, 0]),
+                fb.astensor([1, 1, 0, 1]),
+            )
+            == 1
+        )
 
 
 def test_fpr():
     for _ in environment():
         assert fb.fpr(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 1, 0])) == 0
         assert fb.fpr(fb.astensor([1, 1, 1, 0]), fb.astensor([1, 1, 0, 0])) > 0
-        assert fb.fpr(fb.astensor([1, 1, 1, 0]), fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 0, 1])) == 0
+        assert (
+            fb.fpr(
+                fb.astensor([1, 1, 1, 0]),
+                fb.astensor([1, 1, 0, 0]),
+                fb.astensor([1, 1, 0, 1]),
+            )
+            == 0
+        )
 
 
 def test_fnr():
     for _ in environment():
         assert fb.fnr(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 1, 0])) > 0
         assert fb.fnr(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 0, 0, 0])) == 0
-        assert fb.fnr(fb.astensor([1, 1, 0, 0]), fb.astensor([1, 1, 1, 0]), fb.astensor([1, 1, 0, 1])) == 0
+        assert (
+            fb.fnr(
+                fb.astensor([1, 1, 0, 0]),
+                fb.astensor([1, 1, 1, 0]),
+                fb.astensor([1, 1, 0, 1]),
+            )
+            == 0
+        )
 
 
 def test_auc():
     for _ in environment():
-        assert fb.auc(scores=fb.astensor([0.5, 0.8, 0.3, 0.2]), labels=fb.astensor([1, 1, 1, 0])) > 0.5
+        assert (
+            fb.auc(
+                scores=fb.astensor([0.5, 0.8, 0.3, 0.2]),
+                labels=fb.astensor([1, 1, 1, 0]),
+            )
+            > 0.5
+        )
 
 
 def test_f1k():
     for _ in environment():
-        assert fb.f1k(scores=fb.astensor([0.5, 0.8, 0.3, 0.2, 0, 0.1, 0.12]), labels=fb.astensor([1, 1, 1, 0, 0, 0, 0])) == 1
+        assert (
+            fb.metrics.topf1(
+                scores=fb.astensor([0.5, 0.8, 0.3, 0.2, 0, 0.1, 0.12]),
+                labels=fb.astensor([1, 1, 1, 0, 0, 0, 0]),
+            )
+            == 1
+        )
 
 
 def test_hr():
     for _ in environment():
-        assert fb.hr(scores=fb.astensor([0.5, 0.8, 0.3, 0.2, 0, 0.1, 0.12]), labels=fb.astensor([1, 1, 1, 0, 0, 0, 0])) == 1
+        assert (
+            fb.metrics.tophr(
+                scores=fb.astensor([0.5, 0.8, 0.3, 0.2, 0, 0.1, 0.12]),
+                labels=fb.astensor([1, 1, 1, 0, 0, 0, 0]),
+            )
+            == 1
+        )
 
 
 def test_reck():
     for _ in environment():
-        assert fb.reck(scores=fb.astensor([0.5, 0.8, 0.3, 0.2, 0, 0.1, 0.12]), labels=fb.astensor([1, 1, 1, 0, 0, 0, 0])) == 1
-
-
-def test_ap():
-    for _ in environment():
-        assert fb.ap(scores=fb.astensor([0.5, 0.8, 0.3, 0.2, 0, 0.1, 0.12]), labels=fb.astensor([1, 1, 1, 0, 0, 0, 0])) == 1
+        assert (
+            fb.metrics.toprec(
+                scores=fb.astensor([0.5, 0.8, 0.3, 0.2, 0, 0.1, 0.12]),
+                labels=fb.astensor([1, 1, 1, 0, 0, 0, 0]),
+            )
+            == 1
+        )
 
 
 def test_pinball():
     for _ in environment():
-        mae = fb.metrics.mae(scores=fb.astensor([0.5, 0.8, 0.3, 0.2]), targets=fb.astensor([1, 1, 1, 0]))
-        pinball = fb.metrics.pinball(scores=fb.astensor([0.5, 0.8, 0.3, 0.2]), targets=fb.astensor([1, 1, 1, 0]), alpha=0.5)
-        assert pinball == 0.5*mae
+        mae = fb.metrics.mae(
+            scores=fb.astensor([0.5, 0.8, 0.3, 0.2]), targets=fb.astensor([1, 1, 1, 0])
+        )
+        pinball = fb.metrics.pinball(
+            scores=fb.astensor([0.5, 0.8, 0.3, 0.2]),
+            targets=fb.astensor([1, 1, 1, 0]),
+            alpha=0.5,
+        )
+        assert pinball == 0.5 * mae
 
 
 def test_r2():
     for _ in environment():
-        assert fb.r2(scores=fb.astensor([0.5, 0.8, 0.3, 0.2]), targets=fb.astensor([0.45, 0.85, 0.4, 0.1])) > 0
+        assert (
+            fb.r2(
+                scores=fb.astensor([0.5, 0.8, 0.3, 0.2]),
+                targets=fb.astensor([0.45, 0.85, 0.4, 0.1]),
+            )
+            > 0
+        )
 
 
 def test_mae():
     for _ in environment():
-        assert fb.mae(scores=fb.astensor([0.5, 0.8]), targets=fb.astensor([0, 1])) == 0.35
+        assert (
+            fb.mae(scores=fb.astensor([0.5, 0.8]), targets=fb.astensor([0, 1])) == 0.35
+        )
 
 
 def test_mse():
     for _ in environment():
-        assert fb.mse(scores=fb.astensor([0.5, 0.8]), targets=fb.astensor([0, 1])) == 0.145
+        assert (
+            fb.mse(scores=fb.astensor([0.5, 0.8]), targets=fb.astensor([0, 1])) == 0.145
+        )
 
 
 def test_rmse():
     for _ in environment():
-        assert fb.rmse(scores=fb.astensor([0.5, 0.8]), targets=fb.astensor([0, 1])) == .3807886552931954
+        assert (
+            fb.rmse(scores=fb.astensor([0.5, 0.8]), targets=fb.astensor([0, 1]))
+            == 0.3807886552931954
+        )
```

## tests/test_modelcards.py

```diff
@@ -1,30 +1,28 @@
 import fairbench as fb
 from .test_forks import environment
 
 
 def test_modelcards(monkeypatch):
     import webbrowser
+
     for _ in environment():
-        monkeypatch.setattr(webbrowser, 'open_new', lambda: None)
+        monkeypatch.setattr(webbrowser, "open_new", lambda: None)
         for setting, protected in [(fb.demos.adult, 8), (fb.demos.bank, "marital")]:
             test, y, yhat = setting()
-            sensitive = fb.Fork(fb.categories@test[protected])
+            sensitive = fb.Fork(fb.categories @ test[protected])
             report = fb.multireport(predictions=yhat, labels=y, sensitive=sensitive)
             stamps = fb.combine(
                 fb.stamps.prule(report),
                 fb.stamps.accuracy(report),
                 fb.stamps.dfpr(report),
                 fb.stamps.dfnr(report),
-                fb.stamps.four_fifths_rule(report)
+                fb.stamps.four_fifths(report),
             )
 
             fb.modelcards.toyaml(stamps)  # TODO: add this to texts
-            texts = [
-                fb.modelcards.tohtml(stamps),
-                fb.modelcards.tomarkdown(stamps)
-            ]
+            texts = [fb.modelcards.tohtml(stamps), fb.modelcards.tomarkdown(stamps)]
 
             for text in texts:
                 assert "Metrics" in text
                 assert "Caveats and Recommendations" in text
                 assert "Factors" in text
```

## tests/test_reduction.py

```diff
@@ -13,21 +13,69 @@
     report = fb.binreport(sensitive=sensitive, predictions=predictions, labels=labels)
     return report
 
 
 def test_reduce():
     for _ in environment():
         reduction = fb.reduce(produce_report(), reducer=fb.min, expand=fb.ratio)
-        assert reduction.minratio.accuracy.value == 0.6666666666666667
+        assert abs(reduction.minratio.accuracy.value - 0.666666) < 1.0e-6
         assert reduction.minratio.dfnr.value == -2
 
 
 def test_areduce():
     report = produce_report()
-    assert fb.areduce(report.accuracy, reducer=fb.min, expand=fb.ratio) == 0.6666666666666667
-    assert fb.areduce(report.accuracy, reducer=fb.max, expand=fb.diff) == 0.33333333333333326
-    assert fb.areduce(report.accuracy, reducer=fb.mean, expand=fb.diff) == 0.1481481481481481
-    assert fb.areduce(report.accuracy, reducer=fb.budget, expand=fb.diff) == -1.09861228866811
-    assert fb.areduce(report.accuracy, reducer=fb.min, expand=fb.ratio).value == 0.6666666666666667
-    assert fb.areduce(report.accuracy, reducer=fb.max, expand=fb.diff).value == 0.33333333333333326
-    assert fb.areduce(report.accuracy, reducer=fb.mean, expand=fb.diff).value == 0.1481481481481481
-    assert fb.areduce(report.accuracy, reducer=fb.budget, expand=fb.diff).value == -1.09861228866811
+    assert (
+        abs(
+            fb.areduce(report.accuracy, reducer=fb.min, expand=fb.ratio)
+            - 0.6666666666666667
+        )
+        < 1.0e-6
+    )
+    assert (
+        abs(
+            fb.areduce(report.accuracy, reducer=fb.max, expand=fb.diff)
+            - 0.33333333333333326
+        )
+        < 1.0e-6
+    )
+    assert (
+        abs(
+            fb.areduce(report.accuracy, reducer=fb.mean, expand=fb.diff)
+            - 0.1481481481481481
+        )
+        < 1.0e-6
+    )
+    assert (
+        abs(
+            fb.areduce(report.accuracy, reducer=fb.budget, expand=fb.diff)
+            + 1.09861228866811
+        )
+        < 1.0e-6
+    )
+    assert (
+        abs(
+            fb.areduce(report.accuracy, reducer=fb.min, expand=fb.ratio).value
+            - 0.6666666666666667
+        )
+        < 1.0e-6
+    )
+    assert (
+        abs(
+            fb.areduce(report.accuracy, reducer=fb.max, expand=fb.diff).value
+            - 0.33333333333333326
+        )
+        < 1.0e-6
+    )
+    assert (
+        abs(
+            fb.areduce(report.accuracy, reducer=fb.mean, expand=fb.diff).value
+            - 0.1481481481481481
+        )
+        < 1.0e-6
+    )
+    assert (
+        abs(
+            fb.areduce(report.accuracy, reducer=fb.budget, expand=fb.diff).value
+            - -1.09861228866811
+        )
+        < 1.0e-6
+    )
```

## tests/test_reports.py

```diff
@@ -7,129 +7,219 @@
     for _ in environment():
         men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
         women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
         nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
         sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
         predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
         labels = np.array([1, 0, 1, 0, 1, 0, 1, 0])
-        report = fb.report(predictions=predictions, labels=labels, sensitive=sensitive, metrics=[fb.accuracy, fb.pr])
-        assert report.pr.men == fb.areport(predictions=predictions, labels=labels, sensitive=sensitive, metrics=fb.pr).men
-        assert report.pr.women == fb.areport(predictions=predictions, labels=labels, sensitive=sensitive, metrics=fb.pr).women
-        assert report.pr.nonbin == fb.areport(predictions=predictions, labels=labels, sensitive=sensitive, metrics=fb.pr).nonbin
-        assert len(fb.areport(predictions=predictions, labels=labels, sensitive=sensitive, metrics=[fb.accuracy, fb.pr])) == 2
-        assert len(fb.areport(predictions=predictions, labels=labels, sensitive=sensitive, metrics={"acc": fb.accuracy, "pr": fb.pr})) == 2
+        report = fb.report(
+            predictions=predictions,
+            labels=labels,
+            sensitive=sensitive,
+            metrics=[fb.accuracy, fb.pr],
+        )
+        assert (
+            report.pr.men
+            == fb.areport(
+                predictions=predictions,
+                labels=labels,
+                sensitive=sensitive,
+                metrics=fb.pr,
+            ).men
+        )
+        assert (
+            report.pr.women
+            == fb.areport(
+                predictions=predictions,
+                labels=labels,
+                sensitive=sensitive,
+                metrics=fb.pr,
+            ).women
+        )
+        assert (
+            report.pr.nonbin
+            == fb.areport(
+                predictions=predictions,
+                labels=labels,
+                sensitive=sensitive,
+                metrics=fb.pr,
+            ).nonbin
+        )
+        assert (
+            len(
+                fb.areport(
+                    predictions=predictions,
+                    labels=labels,
+                    sensitive=sensitive,
+                    metrics=[fb.accuracy, fb.pr],
+                )
+            )
+            == 2
+        )
+        assert (
+            len(
+                fb.areport(
+                    predictions=predictions,
+                    labels=labels,
+                    sensitive=sensitive,
+                    metrics={"acc": fb.accuracy, "pr": fb.pr},
+                )
+            )
+            == 2
+        )
 
 
 def test_multireport():
     for _ in environment():
         men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
         women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
         nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
         sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
         predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
         labels = np.array([1, 0, 1, 0, 1, 0, 1, 0])
-        report = fb.multireport(predictions=predictions, labels=labels, sensitive=sensitive)
+        report = fb.multireport(
+            predictions=predictions, labels=labels, sensitive=sensitive
+        )
         assert report.min.accuracy.value == 0
         assert report.min.accuracy.explain.men == 1
         assert report.minratio.pr.value == 0
 
 
 def test_binreport():
     for _ in environment():
         men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
         women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
         nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
         sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
         predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
         labels = np.array([1, 0, 1, 0, 1, 0, 1, 0])
-        report = fb.binreport(predictions=predictions, labels=labels, sensitive=sensitive)
+        report = fb.binreport(
+            predictions=predictions, labels=labels, sensitive=sensitive
+        )
         assert report.men.accuracy == 1
         assert report.nonbin.prule == 0
         assert report.accuracy.men == 1
         assert report.prule.nonbin == 0
 
 
 def test_accreport():
     for _ in environment():
         men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
         women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
         nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
         sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
         predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
         labels = np.array([1, 0, 1, 0, 1, 0, 1, 0])
-        report = fb.accreport(predictions=predictions, labels=labels, sensitive=sensitive)
+        report = fb.accreport(
+            predictions=predictions, labels=labels, sensitive=sensitive
+        )
         assert report.men.accuracy == 1
         assert report.nonbin.pr == 0
 
 
+def test_unireport():
+    for _ in environment():
+        men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
+        women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
+        nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
+        sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
+        predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
+        labels = np.array([1, 0, 1, 0, 1, 0, 1, 0])
+        report = fb.unireport(
+            predictions=predictions, labels=labels, sensitive=sensitive
+        )
+        assert report.branches()["min"].accuracy.value == 0
+        assert report.branches()["min"].accuracy.explain.men == 1
+        assert report.branches()["minratio[vsAny]"].pr.value == 0
+
+
 def test_report_combination():
     for _ in environment():
         men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
         women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
         nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
         sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
         predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
         labels = np.array([1, 0, 1, 0, 1, 0, 1, 0])
-        report1 = fb.binreport(predictions=predictions, labels=labels, sensitive=sensitive)
-        report2 = fb.multireport(predictions=predictions, labels=labels, sensitive=sensitive)
+        report1 = fb.binreport(
+            predictions=predictions, labels=labels, sensitive=sensitive
+        )
+        report2 = fb.multireport(
+            predictions=predictions, labels=labels, sensitive=sensitive
+        )
         report = fb.combine(report1, report2)
         assert "min" in report.branches()
         assert "women" in report.branches()
 
 
 def test_extract():
     for _ in environment():
         men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
         women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
         nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
         sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
         predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
         labels = np.array([1, 0, 1, 0, 1, 0, 1, 0])
-        report = fb.multireport(predictions=predictions, labels=labels, sensitive=sensitive)
+        report = fb.multireport(
+            predictions=predictions, labels=labels, sensitive=sensitive
+        )
         extracted = fb.Fork(acc=report.min.accuracy, prule=report.pr.minratio)
         assert report.min.accuracy == extracted.acc
         assert report.minratio.pr == extracted.prule
 
 
 def test_extract_comparison():
-    #for _ in environment():  # TODO: fix extract for distributed environment
+    # for _ in environment():  # TODO: fix extract for distributed environment
     men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
     women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
     nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
     sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
     predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
     labels = np.array([1, 0, 1, 0, 1, 0, 1, 0])
-    report1 = fb.multireport(predictions=predictions, labels=labels, sensitive=sensitive)
-    report2 = fb.multireport(predictions=predictions, labels=labels, sensitive=fb.Fork(men=men, women=1-men))
+    report1 = fb.multireport(
+        predictions=predictions, labels=labels, sensitive=sensitive
+    )
+    report2 = fb.multireport(
+        predictions=predictions,
+        labels=labels,
+        sensitive=fb.Fork(men=men, women=1 - men),
+    )
     report = fb.Fork(report1=report1, report2=report2)
     extracted = fb.extract(acc=report.min.accuracy, prule=report.pr.minratio)
     assert report1.min.accuracy.value == extracted.acc.report1.value
     assert report2.minratio.pr.value == extracted.prule.report2.value
 
 
 def test_disparity_metrics():
     for _ in environment():
         men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
         women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
         nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
         sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
         predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
-        report = fb.report(predictions=predictions, sensitive=sensitive, metrics=[fb.cvdisparity, fb.eqrep])
+        report = fb.report(
+            predictions=predictions,
+            sensitive=sensitive,
+            metrics=[fb.cvdisparity, fb.eqrep],
+        )
         assert report.men.eqrep <= 1
         assert report.men.cvdisparity >= 0
 
 
 def test_rates():
     for _ in environment():
         men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
         women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
         nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
         sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
         predictions = np.array([1, 0, 1, 1, 0, 1, 0, 0])
         labels = np.array([1, 0, 1, 1, 0, 1, 0, 0])
-        report = fb.report(predictions=predictions, labels=labels, sensitive=sensitive, metrics=[fb.tpr, fb.tnr, fb.fpr, fb.fnr])
+        report = fb.report(
+            predictions=predictions,
+            labels=labels,
+            sensitive=sensitive,
+            metrics=[fb.tpr, fb.tnr, fb.fpr, fb.fnr],
+        )
         assert report.men.tpr == 1
         assert report.men.tnr == 1
         assert report.men.fpr == 0
         assert report.men.fnr == 0
-
-
```

## Comparing `fairbench/forks/categorical.py` & `fairbench/core/categorical.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from fairbench.forks.fork import tobackend, istensor, Fork
+from fairbench.core.fork import tobackend, istensor, Fork
 from typing import Iterable, Mapping
+import numpy as np
 
 
 class Categorical(dict):
     def __and__(self, other):
         ret = Categorical()
         for k, v in self.items():
             for k2, v2 in other.items():
@@ -36,14 +37,29 @@
 
     def __call__(
         self, other
     ):  # allow traditional call in case someone finds it easier to read
         return self.__matmul__(other)
 
 
+def _onehot(num, position):
+    ret = np.zeros((num))
+    ret[position] = 1
+    ret = tobackend(ret)
+    return ret
+
+
+@Transform
+def individuals(x):
+    if not isinstance(x, int):
+        assert isinstance(x, Iterable)
+        x = len(x)
+    return {str(i): _onehot(x, i) for i in range(x)}
+
+
 @Transform
 def binary(x):
     x = tobackend(x)
     return {"1": x, "0": 1 - x}
 
 
 class Categories:
@@ -69,12 +85,12 @@
 @Transform
 def categories(x):
     assert isinstance(x, Iterable)
     if isinstance(x, Mapping):
         return Categorical(x)
     vals = list(set(x))
     return {
-        str(val.numpy())
-        if istensor(val)
-        else str(val): tobackend([1 if val == xval else 0 for xval in x])
+        str(val.numpy()) if istensor(val) else str(val): tobackend(
+            [1 if val == xval else 0 for xval in x]
+        )
         for val in vals
     }
```

## Comparing `fairbench/forks/explanation.py` & `fairbench/core/explanation/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,38 @@
 from typing import Any
-import eagerpy as ep
 from objwrap import ClosedWrapper
 import numpy as np
-from scipy import interpolate
+import eagerpy as ep
 
 
-def tofloat(value):
+def tofloat(value: Any) -> float:
     if isinstance(value, ep.Tensor):
         return float(value.raw)
     return float(value)
 
 
-class ExplainableError(Exception):
-    def __init__(self, message):
-        super().__init__(message)
-        self.explain = message
-        self.value = float("NaN")
-        self.distribution = None
-        self.desc = None
-
-    def __float__(self):
-        return self.value
-
-    def __int__(self):
-        return self.value
-
-    def __str__(self):
-        return "---"
-
-
-class ExplanationCurve:
-    def __init__(self, x, y, name="Curve"):
-        assert isinstance(x, np.ndarray)
-        assert isinstance(y, np.ndarray)
-        self.x = x
-        self.y = y
-        self.name = name
-        assert x.shape == y.shape
-
-    def togrid(self, grid):
-        new_x = np.linspace(self.x.min(), self.x.max(), num=grid)
-        approx = interpolate.interp1d(x=self.x, y=self.y)
-        return ExplanationCurve(new_x, approx(new_x))
-
-    @property
-    def points(self):
-        return self.x.shape[0]
-
-    def __str__(self):
-        return f"{self.name} ({self.points} points)"
-
-
 class Explainable(ClosedWrapper):
     def __init__(
         self, value, explain: Any = None, desc: str = None, units: Any = None, **kwargs
     ):
-        from fairbench.forks import Fork
+        from fairbench.core import Fork
 
         if value.__class__.__name__ == "Future":
             value = value.result()
         if isinstance(value, np.bool_):
             value = bool(value)
         if isinstance(value, int) or isinstance(value, float):
             value = np.float64(value)
         assert (
             isinstance(value, float)
             or isinstance(value, int)
             or isinstance(value, np.floating)
-            or "tensor" in value.__class__.__name__.lower()
-            or "array" in value.__class__.__name__
+            or "tensor" in value.__class__.__name__.lower()  # torch and tensorflow
+            or "array" in value.__class__.__name__  # numpy
+            or "ArrayImpl" in value.__class__.__name__  # jax
         ), f"Can not set data type as explainable: {type(value)}"
         assert (
             explain is None or not kwargs
         ), "Cannot create explainable with both todict and a Fork"
         super().__init__(value)
         self.explain = Fork(kwargs) if explain is None else explain
         self.desc = desc
```

## Comparing `fairbench/metrics/classification.py` & `fairbench/blocks/metrics/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fairbench.forks import parallel, unit_bounded, role
-from fairbench.forks.explanation import Explainable
+from fairbench.core import parallel, unit_bounded, role
+from fairbench.core.explanation import Explainable
 from eagerpy import Tensor
 from typing import Optional
 
 
 @role("metric")
 @parallel
 @unit_bounded
@@ -52,14 +52,15 @@
     predictions: Tensor,
     labels: Tensor,
     sensitive: Optional[Tensor] = None,
     max_prediction: float = 1,
 ):
     if sensitive is None:
         sensitive = predictions.ones_like()
+
     error = (max_prediction - (predictions - labels).abs()) * predictions
     error_sensitive = error * sensitive
     num_sensitive = (sensitive * predictions).sum()
     return Explainable(
         0 if num_sensitive == 0 else (error_sensitive.sum() / num_sensitive),
         positives=num_sensitive,
         true_positives=error_sensitive.sum(),
```

## Comparing `fairbench/metrics/disparate_impact.py` & `fairbench/blocks/metrics/disparate_impact.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from fairbench.forks.fork import parallel, unit_bounded
+from fairbench.core import parallel, unit_bounded
 from eagerpy import Tensor
 from typing import Optional
 
 
 @parallel
 @unit_bounded
 def prule(
     predictions: Tensor,
     sensitive: Tensor,
     non_sensitive: Optional[Tensor] = None,
-    max_sensitive: float = 1,
+    # max_sensitive: float = 1,
 ):
+    max_sensitive = 1
     if non_sensitive is None:
         non_sensitive = max_sensitive - sensitive
     sum_sensitive = sensitive.sum()
     sum_non_sensitive = non_sensitive.sum()
     if sum_sensitive == 0:
         return sum_sensitive
     if sum_non_sensitive == 0:
@@ -29,27 +30,49 @@
 
 @parallel
 @unit_bounded
 def cvdisparity(
     predictions: Tensor,
     sensitive: Tensor,
     non_sensitive: Optional[Tensor] = None,
+    # max_sensitive: float = 1,
+):
+    max_sensitive = 1
+    if non_sensitive is None:
+        non_sensitive = max_sensitive - sensitive
+    sum_sensitive = sensitive.sum()
+    sum_non_sensitive = non_sensitive.sum()
+    if sum_sensitive == 0:
+        return sum_sensitive
+    if sum_non_sensitive == 0:
+        return sum_non_sensitive
+    r1 = (predictions * sensitive).sum() / sum_sensitive
+    r2 = (predictions * non_sensitive).sum() / sum_non_sensitive
+    return r1.maximum(r2) - r1.minimum(r2)
+
+
+@parallel
+@unit_bounded
+def _cvdisparity(
+    predictions: Tensor,
+    sensitive: Tensor,
+    non_sensitive: Optional[Tensor] = None,
     max_sensitive: float = 1,
 ):
     if non_sensitive is None:
         non_sensitive = max_sensitive - sensitive
     sum_sensitive = sensitive.sum()
     sum_non_sensitive = non_sensitive.sum()
     if sum_sensitive == 0:
         return sum_sensitive
     if sum_non_sensitive == 0:
         return sum_non_sensitive
     r1 = (predictions * sensitive).sum() / sum_sensitive
     r2 = (predictions * non_sensitive).sum() / sum_non_sensitive
-    return r1 - r2
+    return r1.maximum(r2) - r1.minimum(r2)
 
 
 @parallel
 @unit_bounded
 def eqrep(
     predictions: Tensor,
     sensitive: Tensor,
```

## Comparing `fairbench/metrics/disparate_mistreatment.py` & `fairbench/blocks/metrics/disparate_mistreatment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fairbench.forks.fork import parallel, unit_bounded
+from fairbench.core import parallel, unit_bounded
 from eagerpy import Tensor
 from typing import Optional
 
 
 @parallel
 @unit_bounded
 def dfpr(
@@ -14,36 +14,38 @@
     if non_sensitive is None:
         non_sensitive = 1.0 - sensitive
     error = (predictions - labels).abs() * predictions
     error_sensitive = error * sensitive
     error_non_sensitive = error * non_sensitive
     num_sensitive = (sensitive * predictions).sum()
     num_non_sensitive = (non_sensitive * predictions).sum()
+    if num_sensitive == 0 or num_non_sensitive == 0:
+        return num_sensitive * 0
     return (
         error_sensitive.sum() / num_sensitive
         - error_non_sensitive.sum() / num_non_sensitive
     )
 
 
 @parallel
 @unit_bounded
 def dfnr(
     predictions: Tensor,
     labels: Tensor,
     sensitive: Tensor,
     non_sensitive: Optional[Tensor] = None,
-    max_prediction: float = 1,
+    # max_prediction: float = 1,
 ):
-    negatives = max_prediction - predictions
+    negatives = 1.0 - predictions
     if non_sensitive is None:
         non_sensitive = 1.0 - sensitive
     error = (predictions - labels).abs() * negatives
     error_sensitive = error * sensitive
     error_non_sensitive = error * non_sensitive
     num_sensitive = (sensitive * negatives).sum()
     num_non_sensitive = (non_sensitive * negatives).sum()
     if num_sensitive == 0 or num_non_sensitive == 0:
-        return 0
+        return num_sensitive * 0
     return (
         error_sensitive.sum() / num_sensitive
         - error_non_sensitive.sum() / num_non_sensitive
     )
```

## Comparing `fairbench/metrics/regression.py` & `fairbench/blocks/metrics/regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fairbench.forks import parallel, unit_bounded, role
-from fairbench.forks.explanation import Explainable, ExplanationCurve
+from fairbench.core import parallel, unit_bounded, role
+from fairbench.core.explanation import Explainable, ExplanationCurve
 from eagerpy import Tensor
 
 
 @role("metric")
 @parallel
 def max_error(scores: Tensor, targets: Tensor, sensitive: Tensor = None):
     return Explainable(((scores - targets) * sensitive).abs().sum())
@@ -59,18 +59,20 @@
         sensitive = scores.ones_like()
     num_sensitive = sensitive.sum()
     true = ((scores - targets) ** 2 * sensitive).sum()
     target_mean_squares = (targets**2 * sensitive).sum() / num_sensitive
     target_mean = (targets**2 * sensitive).sum() / num_sensitive
     target_variance = target_mean_squares - target_mean**2
     return Explainable(
-        0
-        if num_sensitive == 0
-        else (1 - (true / target_variance))
-        * ((num_sensitive - 1) / (num_sensitive - 1 - deg_freedom)),
+        (
+            0
+            if num_sensitive == 0
+            else (1 - (true / target_variance))
+            * ((num_sensitive - 1) / (num_sensitive - 1 - deg_freedom))
+        ),
         samples=num_sensitive,
         # target_mean=target_mean,
         # target_variance=target_variance,
         deg_freedom=deg_freedom,
         sse=true,
     )
```

## Comparing `fairbench/reports/reduction/reduce.py` & `fairbench/blocks/framework.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from fairbench.forks.fork import Fork, astensor, comparator, fromtensor, role
-from fairbench.forks.explanation import Explainable, ExplainableError
+from fairbench.core.fork import Fork, astensor, asprimitive, role
+from fairbench.core.compute import comparator
+from fairbench.core.explanation import Explainable, ExplainableError
 from typing import Optional
 
 # from fairbench.reports.accumulate import todict as tokwargs
 
 
 def areduce(fork: Fork, reducer, expand=None, transform=None, branches=None):
     return reduce(fork, reducer, expand, transform, branches, name=None)
@@ -18,65 +19,98 @@
             return arg
     try:
         return method(*args, **kwargs)
     except ExplainableError as e:
         return e
 
 
-@role("reduction")
+def reduce_namefinder(
+    reducer, expand=None, transform=None, branches=None, base=None
+) -> str:
+    name = reducer.__name__
+    if expand is not None:
+        name += expand.__name__
+    if transform is not None:
+        name += transform.__name__
+    if branches is not None:
+        name += "[" + ",".join(branches) + "]"
+    if base is not None:
+        name += "[vs" + base + "]"
+    return name
+
+
+@role("reducers")
 @comparator
 def reduce(
     fork: Fork,
     reducer,
     expand=None,
     transform=None,
     branches=None,
+    base: Optional[str] = None,
     name: Optional[str] = "",
 ):
     if name == "":
-        name = reducer.__name__
-        if expand is not None:
-            name += expand.__name__
-        if transform is not None:
-            name += transform.__name__
-        if branches is not None:
-            name += "[" + ",".join(branches) + "]"
+        name = reduce_namefinder(reducer, expand, transform, branches, base)
     fields = None
+    base_fields = None
     for branch, v in fork.branches().items():
         if branches is not None and branch not in branches:
             continue
-        if fields is None:
-            fields = {f: list() for f in v} if isinstance(v, dict) else list()
-        if isinstance(v, dict):
-            for f in v:
-                fields[f].append(
-                    astensor(v[f]) if transform is None else transform(astensor(v[f]))
+        if base is None or base != branch:
+            if fields is None:
+                fields = {f: list() for f in v} if isinstance(v, dict) else list()
+            if isinstance(v, dict):
+                for f in v:
+                    fields[f].append(
+                        astensor(v[f])
+                        if transform is None
+                        else transform(astensor(v[f]))
+                    )
+            else:
+                fields.append(
+                    astensor(v) if transform is None else transform(astensor(v[v]))
                 )
         else:
-            fields.append(
-                astensor(v) if transform is None else transform(astensor(v[v]))
-            )
+            if base_fields is None:
+                base_fields = {f: list() for f in v} if isinstance(v, dict) else list()
+            if isinstance(v, dict):
+                for f in v:
+                    base_fields[f].append(
+                        astensor(v[f])
+                        if transform is None
+                        else transform(astensor(v[f]))
+                    )
+            else:
+                raise Exception(
+                    "The base argument is supported only in the reduction of forks of dicts"
+                )
     if expand is not None:
         fields = (
-            {k: _tryorexplainable(expand, v) for k, v in fields.items()}
+            {
+                k: _tryorexplainable(
+                    expand, v, None if base_fields is None else base_fields[k]
+                )
+                for k, v in fields.items()
+            }
             if isinstance(fields, dict)
             else _tryorexplainable(expand, fields)
         )
     result = (
         {
             k: _tryorexplainable(
                 Explainable,
-                _tryorexplainable(fromtensor, _tryorexplainable(reducer, v), False),
+                _tryorexplainable(asprimitive, _tryorexplainable(reducer, v), False),
                 fork[k],
                 desc=name,
             )
             for k, v in fields.items()
         }
         if isinstance(fields, dict)
         else _tryorexplainable(
             Explainable,
-            _tryorexplainable(fromtensor, _tryorexplainable(reducer, fields), False),
+            _tryorexplainable(asprimitive, _tryorexplainable(reducer, fields), False),
             fork,
             desc=name,
         )
     )
     return result if name is None else Fork({name: result})
```

## Comparing `fairbench-0.2.9.dist-info/METADATA` & `fairbench-0.3.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbench
-Version: 0.2.9
+Version: 0.3.0
 Summary: Fairness model assessment framework
 Home-page: https://github.com/mever-team/FairBench
 Author: Emmanouil (Manios) Krasanakis
 Author-email: maniospas@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,10 +18,11 @@
 Requires-Dist: matplotlib
 Requires-Dist: wget
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: objwrap
 Requires-Dist: bokeh
 Requires-Dist: pyyaml
+Requires-Dist: requests
 
 A comprehensive AI fairness exploration framework.<br>**Homepage:** https://github.com/mever-team/FairBench<br>**Documentation:** https://fairbench.readthedocs.io
```

## Comparing `fairbench-0.2.9.dist-info/RECORD` & `fairbench-0.3.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-fairbench/__init__.py,sha256=Ido_Y_0n5fjUZDnEXn5vFcHTNnSJBJ95PI8sp_Y_Gpo,411
-fairbench/export.py,sha256=_u97-Yi8VArkwof63mcVXgnUD-i9AY1vjxtCnQ_jKcs,1952
-fairbench/stamps.py,sha256=naC2tvM9ihnMyFqlInP57thAgCf5af4000fjY8snNCE,5762
+fairbench/__init__.py,sha256=vx1onc6vHPsAv_M78DUG9Segdq4tJGc8TcRGOrTMBrM,497
+fairbench/verification.py,sha256=hpHtLM17cJ1AnG83wMGX0D8I6UtYPEtWCaPiEm7wZ1Q,6985
 fairbench/bench/__init__.py,sha256=piA_S0SAZ96_-MxdcGO_V7pCKngOFBeAv8KGj9rkGRA,38
-fairbench/bench/demos.py,sha256=ODVbSjCVrl_S1lP7cZOyoaVFPUZmsz75SYbeD3sflFY,2341
-fairbench/bench/loader.py,sha256=P1PiDtR67NFSk_lIQvzQ0Wez2ZvcxprP7zMpsLcsTYo,1660
+fairbench/bench/demos.py,sha256=hLWxupPPaEB-7fF2DlOP3u_h0lfJAmpx1gSHPsnbju8,5853
+fairbench/bench/loader.py,sha256=tg9GvdxhsxUE_7fX-Yj7IprvExmSRRyesAibz6fFyjY,1660
+fairbench/blocks/__init__.py,sha256=DmnOAEuZscW_w_fzywqzDMxB5pnrLWMg5gDOqfEBAmY,179
+fairbench/blocks/framework.py,sha256=-HbNcC9ASWKW8zd2OUqhhr6qVscorrAqxtiZ0teYI_A,3823
+fairbench/blocks/expanders/__init__.py,sha256=voqD22YoinY2UiNnlmPSUDCNqgzI6nyJSbMM-mHJ3Hg,52
+fairbench/blocks/expanders/expanders.py,sha256=Es0blfm-N1fazVPHOTUGspljepK0E-JYyGZizBYl5ys,4309
+fairbench/blocks/metrics/__init__.py,sha256=cwCdbJ1bSSbEJKxb546lLhH-eNtfRth0onev3NYmjPY,274
+fairbench/blocks/metrics/classification.py,sha256=I4Wn52fsdl95-YYngTnSyGXVSfia4kTJC1woGIjY0pk,4016
+fairbench/blocks/metrics/disparate_impact.py,sha256=IU6D_edmcrNv8G4a77GGlEgTcVXn-g6-HCnaRQIfyM8,2769
+fairbench/blocks/metrics/disparate_mistreatment.py,sha256=I6wvfnGQ5ojJv1mgdQMDHQyhhCiClzmU15OK1Ijxni0,1583
+fairbench/blocks/metrics/ranking.py,sha256=0stoNAhI9LSQmG7HWy_pPAgOeY_JOvQ59kpd1DRDzqA,5162
+fairbench/blocks/metrics/regression.py,sha256=7XFu1pwbJAs3plmzkUuvHOmubbQDVxXum0Bax2aQfYw,3006
+fairbench/blocks/reducers/__init__.py,sha256=8Vnpfirx3LzEXotYq816X8NdG-E3o8u7dF_ZgE42afg,50
+fairbench/blocks/reducers/reducers.py,sha256=o-1MrykqK7U889sSQAgjhiYSzwLxac3BFlgeTJbr45w,4283
+fairbench/core/__init__.py,sha256=CwHCbN-2c3-GKF-OwxcOg9jYSmPFtWnQ206AtiCXkyQ,157
+fairbench/core/categorical.py,sha256=3JAYlGGXPLKVJH3djWGgn3YsfEjdd7gl3Rka2ZaPvbs,2463
+fairbench/core/fork.py,sha256=M8sYC_yekygM3HtMp10fh9DT6Q-Dm-yLMctjgzcmjSo,15076
+fairbench/core/compute/__init__.py,sha256=Weh6I7npSLreu6G4Ntk4SfDwEzVsRDtvIbBt3ixar9Q,49
+fairbench/core/compute/backends.py,sha256=4TVEjIlDXHrpTfI1gowUd3wCaywXGVGUyC9USW8AvJs,3935
+fairbench/core/compute/delegation.py,sha256=hkFpCeB6D9Bczx-cB0twaQ3wbK9yM6H-ZS6vwNwMb9w,5563
+fairbench/core/explanation/__init__.py,sha256=fdnZ5GT5oZmriea9k-dVQ4j9bg_JoT1evhnnAj_5J5E,183
+fairbench/core/explanation/base.py,sha256=bBBFc9RLPMuYovo8MhGI4RqcgXMZPbmeSgIYXmvc6ms,1999
+fairbench/core/explanation/curve.py,sha256=daHB7H13USy3Qvj2n-IzVLAT_0BgXZ2yBSJX8UMNzyo,674
+fairbench/core/explanation/error.py,sha256=wYCIFAewcL5bvV1WYfcBY8ks7hA8GwaP3yEyjnPPYeI,388
 fairbench/export/__init__.py,sha256=ZQ3m4piX_o-z5mlmG_H7O26SGuhKo7b38Nc64Bs8pik,134
-fairbench/export/interactive.py,sha256=yoa0Xdp8wrsjYIDU9ps-QVRFIC7M6zsfv2kKYDXdY8Y,16566
-fairbench/export/native.py,sha256=dTgt72i0uTPdD59ruMC7jQKB_qD4qp148_bCmOzqtuE,3022
+fairbench/export/interactive.py,sha256=OWGinEoGgvGL7bjWfxubJYRdLu0F9oZIw3ylDfI7yxw,19106
+fairbench/export/native.py,sha256=gd6LKM9Uo7gTmodg7rGt6E0OhOV9RowKpxXl7ypiyD0,3200
 fairbench/export/modelcards/__init__.py,sha256=B9gsTh-sWzIkY5pIPSPJ8ZdurlBsr2MS4o95n3WXXj0,173
-fairbench/export/modelcards/tohtml.py,sha256=IkVy8NpNBe-OYjc68QPWZeSfAHp5b9rvZ6fl8y5-J0Y,2856
-fairbench/export/modelcards/tomarkdown.py,sha256=Jesxn2AF0lRrDZxCjhj47phKI-PmLIdQ02GNrzoZjKk,2423
-fairbench/export/modelcards/toyaml.py,sha256=-DW4YcICcuWiNGdtECTKam7XlDXliuf4S3UvJzJrp6g,562
-fairbench/forks/__init__.py,sha256=eBRDSxc31Pc1yKCc1VjFBvPMsBVaOzVOfXHpkYQodG0,122
-fairbench/forks/categorical.py,sha256=nfsA1ZjrrywMzOhEoPUF6_9oazIJWcZEI4gvil-1VIs,2130
-fairbench/forks/explanation.py,sha256=x6zqF4b9dc1-XBg_xAQXu43czI4f900mrwEgoo-vR6o,2936
-fairbench/forks/fork.py,sha256=-UCnFFthc9WPBqoaovACVek7xvN12pmerJpy44Y0kDc,26940
-fairbench/metrics/__init__.py,sha256=kqs5vladIyri5R_l4u6fcte-O4j_n-jt9OeiIRA2KPo,239
-fairbench/metrics/classification.py,sha256=aqsbknk20xfIFposX-WpWs3RB59YQ-8JkEp4DB-QoBQ,4016
-fairbench/metrics/disparate_impact.py,sha256=VJw9Q4cA1YqP9fTTE-aMMUzjeuk072L-HRow_vaLkZA,2066
-fairbench/metrics/disparate_mistreatment.py,sha256=ORoUcMU_Dh18Ytz4dgQn8wPyaNJ_w98m_oegxI90vc4,1494
-fairbench/metrics/ranking.py,sha256=bX_ckM7k8syEBgoT7PcKMG5NPu_xuXcqGl4iAecZ7DY,3760
-fairbench/metrics/regression.py,sha256=w7zVO0hfLABovxIzGZ7XkWzYfT9eJOA2ceIME7XPMeQ,2970
-fairbench/mitigation/__init__.py,sha256=f-owl1xAKGweXEuVbFJGYSel3-7kccvTo6SEziKmXRk,100
-fairbench/mitigation/postprocessing.py,sha256=CF2WcAWQKKfNRJ4yvNqIjuNdLaCBrSIpI_XNhmfiUkY,1790
-fairbench/reports/__init__.py,sha256=YQm7A6K3PUB4uNOw3iDu2RUaoWa07Rsn3GJr4wZkn2M,207
-fairbench/reports/accumulate.py,sha256=jDlJFb1bK9nRfumzSWFbCpAGWi8aCOFil4L8Hj44xe0,1491
-fairbench/reports/adhoc.py,sha256=KNrF0CmdQasVVJBYQ2g-x9JqLxjTM_LePtwlUQZipgo,2075
-fairbench/reports/base.py,sha256=KQHdSzzU7c3uH0cmV7CmU1YUlIwKhRviGtAGucNEzk4,2590
-fairbench/reports/surrogate.py,sha256=LnV6kkNPMGL2SYEBSSIFWjkXQ8N5m2k4y5as2zUyDt8,883
-fairbench/reports/reduction/__init__.py,sha256=a3c0w4bKV3f6NXnGMPPGFRxdfg_YIrcccy_mEBSr8zk,155
-fairbench/reports/reduction/expanders.py,sha256=DZvDpfXw8LI3ZquA5c22-25PSuLsOhpp_B_IYo5VeVY,2260
-fairbench/reports/reduction/reduce.py,sha256=H6_rIdw4JZRkhpS2ldpi3kPgBKuHjcQ6OOuXwPyRIUk,2637
-fairbench/reports/reduction/reducers.py,sha256=EQlN9rCKDBJmls0rtoA9vyAlrIyIBzQCCcpRDBMRlMA,2834
+fairbench/export/modelcards/tohtml.py,sha256=Yvex2msBltytQpvoSE4whASH0C6lO5yEgDRMpdTEgnc,2978
+fairbench/export/modelcards/tomarkdown.py,sha256=p62rCtRiIhhIHOyLv4MArD6aoSIUi33YXeZ4fPcT-R0,2569
+fairbench/export/modelcards/toyaml.py,sha256=tfSnr27ECkvF7rMUdTOz3cw0iKQEJSAM92CpYXzP0OQ,1229
+fairbench/reports/__init__.py,sha256=Cq6gbXBY3DfzP66Bt1NojxwIzRRA5hbfWjGI4yW89-E,164
+fairbench/reports/accumulate.py,sha256=iZGNeAvVqbc-FQvXpJGhKhntVMDt18BmehLSrR4_yYY,1437
+fairbench/reports/adhoc.py,sha256=JVxPag5IwUeDSOiw2MSY5T_vQSwnfvt81XTq99W_YP4,3954
+fairbench/reports/base.py,sha256=wNHs-inLNKivoF4zTGDaDifivgErBhGEoSAXAKzBHXg,2969
+fairbench/reports/surrogate.py,sha256=cCyYSk6LJl7RtiFyHiouCXzV6XfA7mAr-sGzS5bUriY,912
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/test_batching.py,sha256=bXewsKXAlDTeyZZ8OlG74-qYQ_hhiwcYJigxy0M_YKY,1394
-tests/test_benchmarks.py,sha256=RZwehxePgR6fwFCh9HWbK3rXsXQNLHomrn7M6BboiMw,1278
-tests/test_demos.py,sha256=VgXBcev7XAnvy2OWiOZf0yBNXzhkjWvf0Bl6of00WzM,1103
-tests/test_forks.py,sha256=Dyu5UPAFG8fxVCfeZ9JwisVwUtZT0NV1WqAMe2GXt3Y,5807
-tests/test_metrics.py,sha256=44ukRpPdweJEIjk5GtsKR1mhBeZzN3dVdAIwVC_ENeo,3391
-tests/test_modelcards.py,sha256=v73DtkMJZGnfnTEymv48ad2qsQCn7XI6nOs7OedTckE,1150
-tests/test_reduction.py,sha256=JMXZeh3Catiboki8TG50A_caMh4zpSt_NKScqGS2Pr0,1624
-tests/test_reports.py,sha256=2nNSZjkrTdZl8P5bvEz8dDdRd_W7CmSvn51GDdHFPvo,6556
-fairbench-0.2.9.dist-info/METADATA,sha256=eF2oXQnrzMhOOyvgkZnK7Jz1oasChqGAAz4POA3EQyY,877
-fairbench-0.2.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-fairbench-0.2.9.dist-info/top_level.txt,sha256=lrkG910bN_2UdVUqCXaR6aeRjjXfOQX2-wSeVjhhFnM,16
-fairbench-0.2.9.dist-info/RECORD,,
+tests/test_batching.py,sha256=vPwN0ZjgIcCh5inIAfxPmzHyCxbATLyt35WTxiIzdfQ,1613
+tests/test_demos.py,sha256=5q5NeAsbsDuz5ymtmi1mMFD-WKtuCGaebcFStRFXhwg,1370
+tests/test_forks.py,sha256=stYpDWDmzyJrqweHU8f1c888HNwzeij7k8FUtEBttQE,7095
+tests/test_metrics.py,sha256=aNLd86E6okgqAD4CEkcFeDGlanl2AlBqL4MzJRq_Vp4,4391
+tests/test_modelcards.py,sha256=5glZjRh8M7fmq20KS16ZB3VfsreI0kqMKjrvULHI8bQ,1101
+tests/test_reduction.py,sha256=t-HOX6m-zJlFVQGyrRQh_NRaguRB2BUdAoCqlg-yVuw,2242
+tests/test_reports.py,sha256=wKSl-bKXqwuraDxauofgNsRQiDuSDdTW4U5kAsI4Mv8,8347
+fairbench-0.3.0.dist-info/METADATA,sha256=M1Xx5sfh3MvMIFhl1gIeWcEgEQOFx64IGZAMcHR1XbE,901
+fairbench-0.3.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+fairbench-0.3.0.dist-info/top_level.txt,sha256=lrkG910bN_2UdVUqCXaR6aeRjjXfOQX2-wSeVjhhFnM,16
+fairbench-0.3.0.dist-info/RECORD,,
```

